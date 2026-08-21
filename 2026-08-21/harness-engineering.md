# Harness engineering トレンド調査 (2026-08-21)

- 調査日: 2026-08-21
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

ハーネスエンジニアリングは「プロンプトを足す技術」から、権限・hooks・観測・失敗ログを通じてエージェントの作業環境そのものを設計する技術へ移っている。

## トップ5

### 1. Claude Code 2026年8月上旬〜中旬アップデートまとめ：auto mode と self-hosted runner がハーネスを作り替える
- 出典: 日本語ブログ（MOSFET's blog）
- 日付: 2026-08-19
- リンク: https://mosfet.hatenablog.com/entry/2026/08/19/234526
- 要約: Claude Code v2.1.221〜v2.1.235 の変化を、auto mode 既定化、クロスセッションメッセージング、self-hosted environments、Todo系ツール削除、権限バイパス修正として整理している。特に auto mode では有料テスター1,053人の実験で、人間が危険コマンドを止められた割合13.6%に対し auto mode は89%をブロックしたという数字が紹介され、承認プロンプト中心の安全設計から分類器・denyルール中心の安全設計へ重心が移ったことが分かる。
- なぜ面白いか:
  - 技術: ハーネスの中核である permissions / deny / 実行環境 / セッション間通信が同時に変化しており、Claude Code が単一CLIから分散実行基盤へ拡張している兆候が見える。
  - 人文: 「人間が許可ボタンを読む」という前提が儀式化していたことを、数字で突きつける記事でもある。責任ある人間参加とは何か、どこを機械に委ねどこを人間が設計すべきかという統治の問題が前面に出ている。

### 2. ハーネスエンジニアリング実践ガイド：失敗ログから恒久修正へ
- 出典: 日本語企業ブログ（tufecompany.co.jp）
- 日付: 2026-08-13
- リンク: https://tufecompany.co.jp/blog/harness-engineering-practice-2026
- 要約: Claude Code を「育てる」ための5つの型として、失敗ログ→恒久修正ループ、CLAUDE.md、hooks、permissions、スキル化を提示している。失敗をチャットで注意するのではなく、ルール・hooks・権限・スキルへ変換するという運用カレンダーが実務寄りで、日本語コミュニティでのハーネス設計の定着を示す。
- なぜ面白いか:
  - 技術: 失敗の種類ごとに CLAUDE.md / hooks / permissions / skills へ振り分ける設計は、ハーネスを単なる設定ファイル群ではなく保守可能な改善ループとして扱っている。
  - 人文: 「注意する」から「環境を変える」への転換は、個人の能力や気合いに責任を押しつけない組織設計に近い。AIエージェントの失敗を、叱責ではなく制度設計の材料にする文化が見える。

### 3. Harness-R1: Learning to Edit Executable Runtime Harnesses from Agent Failure Trajectories（やや古いが重要）
- 出典: arXiv（cs.AI）
- 日付: 2026-08-03
- リンク: https://arxiv.org/abs/2608.02276v1
- 要約: LLMエージェントの失敗軌跡から、コンテキスト構築・ツール仲介・検証・リカバリを担う実行時ハーネスを自動編集する Harness-R1 を提案している。9Bの「harness engineer」が失敗バッチから検証済み実行パッチを作り、WebShop / ALFWorld / DBBench で Qwen3.5-9B の成功率を44.3%から53.6%へ上げたと報告している。
- なぜ面白いか:
  - 技術: モデル本体ではなくハーネスを強化学習で更新する発想により、エージェント改善の対象が「重み」から「実行環境」へ広がっている。
  - 人文: 失敗経験を個体の記憶ではなく、共同で使える制度・道具・環境へ転写する点が面白い。人間社会における事故報告、標準作業手順、建築基準のように、AIエージェントも失敗を通じて周囲の制度を進化させる段階に来ている。

### 4. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 出典: arXiv（cs.SE / cs.CL）
- 日付: 2026-08-10更新（初版 2026-07-31、やや古いが直近更新あり）
- リンク: https://arxiv.org/abs/2608.00267v2
- 要約: 長期的なソフトウェア開発では、局所タスクや最終状態だけでなく、依存DAG・回帰義務・実行の継続性を測る必要があるとして LOOPSBENCH を提案している。112タスク、8言語、9ドメイン、5,300以上の開発ユニットを含み、最強構成でも解決率25.00%にとどまると報告する。
- なぜ面白いか:
  - 技術: ハーネスが「安全に動く環境」なら、ループは「いつ続け、いつ止まるか」を決める時間構造であり、この論文は評価軸を単発の成果物から持続的な開発過程へ拡張している。
  - 人文: 仕事の価値を最終成果だけで測るのか、途中の回帰・依存・判断の履歴まで見るのかという労働観の問題を含んでいる。AIエージェント評価が、人間のプロジェクト管理や職人性の評価に近づいている。

### 5. Claude Is Like The Horse, And Claude Code Is The Harness: Anthropic's Boris Cherny（古いが概念の源流として重要）
- 出典: Web記事（OfficeChai、Boris Cherny発言の紹介）
- 日付: 2025-09-03（古いが、Boris Cherny / Claude Code / harness の接点として重要）
- リンク: https://officechai.com/ai/claude-is-like-the-horse-and-claude-code-is-the-harness-anthropics-boris-cherny/
- 要約: Boris Cherny が、Claude のようなモデルを「馬」、Claude Code をその力を人間が方向づけるための「ハーネス」にたとえた発言を紹介している。モデルの性能だけでなく、モデル上の scaffolding / harness が十分でなければAIコーディングは機能しない、という直観を早い段階で言語化している。
- なぜ面白いか:
  - 技術: Claude Code を単なるUIではなく、モデルを開発ワークフローへ接続する実行ハーネスとして捉えることで、現在の hooks・permissions・observability 議論につながる土台を作っている。
  - 人文: 馬とハーネスの比喩は、AIを「自律的な労働者」と見るより、人間の身体能力を拡張する乗り物・道具として見る視点を与える。一方で、誰が手綱を握るのか、どの程度まで機械に判断を任せるのかという権力関係も浮かび上がる。

## arXiv / 学術

- Harness-R1: Learning to Edit Executable Runtime Harnesses from Agent Failure Trajectories — arXiv:2608.02276v1。失敗軌跡から実行時ハーネスを編集する学習手法。
- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — arXiv:2608.00267v2。長期的な coding agent 評価を harness から loop へ拡張するベンチマーク。
- Harness Engineering for LLM-Driven GPU Kernel Generation — arXiv:2607.17979v1（2026-07-20、古いが関連）。GPUカーネル生成で、評価ハーネスとプロファイル駆動の最適化コントローラを分離する実践例。
- Vero: Can AI Agents Build Formally Verified Software Repositories? — arXiv:2608.13522v1。形式検証つきリポジトリ生成の評価ハーネスを含む、信頼性評価の近接トピック。

## メモ

- Boris Cherny優先の有無: 優先確認した。X検索は `x_search` がクレジット上限で失敗したため直接投稿は確認できなかったが、Web検索で Boris Cherny の「Claude Code is the harness」発言を確認し、概念的源流としてトップ5に含めた。
- 日本語アカウントの扱い: X検索は同じく利用不可だったため、日本語コミュニティ確認はWeb検索・日本語ブログ中心に実施した。直近では MOSFET's blog（2026-08-19）と tufecompany.co.jp（2026-08-13）が有用だった。
- Claude Code / loop engineering との接点: Claude Code の auto mode、permissions、self-hosted runner、hooks、skills、Todoツール削除が、ハーネス設計の実装面と直結している。Loop engineering との境界は LoopsBench と AIBuilderClub / MindStudio 系記事で確認したが、トップ5では直近性と検証性を重視して arXiv の LoopsBench を採用した。
- 注意点・誇張リスク: Web検索（Firecrawl）は未設定、X検索は xAI クレジット上限により利用不可だったため、X上の直近反応は本調査時点で確認できていない。DuckDuckGo 経由検索、Jina AI 経由のページ抽出、arXiv API を代替ソースとして使った。記事中の数値や製品バージョンは各出典の記述に依存し、一次公式リリースで未検証のものは断定を避けた。

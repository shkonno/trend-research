# Harness engineering トレンド調査 (2026-07-14)

- 調査日: 2026-07-14
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「エージェントにお願いする」段階から、「実行・検証・記憶・評価を構造化して任せる」段階へ移りつつあります。

## トップ5

### 1. ContextSniper: Claude Code を含む修復エージェントの文脈コストを下げる評価ハーネス
- 出典: arXiv
- 日付: 2026-07-02公開 / 2026-07-09更新
- リンク: https://arxiv.org/abs/2607.01916
- 要約: repository-level program repair で、エージェントが全ファイル読み・広範検索・長いログにトークンを浪費する問題に対し、ContextSniper が意図に沿った証拠パケットを返す仕組みを提案しています。SWE-bench Lite の同一タスク比較で、Claude Code ではトークン使用を38.9%、ログ上のコストを27.3%削減し、解決率はほぼ維持したと報告されています。
- なぜ面白いか:
  - 技術: ハーネスを単なる実行環境ではなく、検索・ログ・記憶を絞り込む「文脈ゲート」として設計している点が実務的です。
  - 人文: これはAIの「注意」を人間がどう制度化するかという話でもあります。開発者が長大な文脈を読ませるほど良いという幻想から、何を見せないかを設計する編集倫理へ重心が移っています。

### 2. RuBench: 母語の顧客依頼で coding agent を測るリポジトリ級ベンチマーク
- 出典: arXiv
- 日付: 2026-07-07
- リンク: https://arxiv.org/abs/2607.06411
- 要約: ロシア語で新規作成された顧客依頼風タスク25件を用い、Claude Code と Codex CLI の製品構成を複数回評価する repository-level agentic coding benchmark です。英語翻訳ではなく母語の依頼文、非公開回帰テスト、コスト・トークン使用量まで含めた評価設計が特徴です。
- なぜ面白いか:
  - 技術: ハーネスが「コードが直るか」だけでなく、自然言語仕様・文化圏・コストまで含む測定装置になっています。
  - 人文: エージェント評価は英語圏のissue文を標準としがちですが、実際の依頼は母語・曖昧さ・顧客文体を伴います。多言語ハーネスは、AI開発の中心と周縁をどう測るかという政治性を可視化します。

### 3. Agentic Hardware Design as Repository-Level Code Evolution: Markdown harness でハードウェア設計を自律進化させる
- 出典: arXiv
- 日付: 2026-06-26（直近14日より少し古いが重要）
- リンク: https://arxiv.org/abs/2606.28279
- 要約: HORIZON は、Markdown harness をプロジェクトパックへコンパイルし、ドメイン知識、実行可能評価器、受け入れ条件、git/runtime policy を含む環境でハードウェア設計を repository-level code evolution として進めます。ChipBench、RTLLM、Verilog-Eval などで hands-free agentic loop を評価しています。
- なぜ面白いか:
  - 技術: ハーネスを「Markdownで書ける仕様」から、評価器・受け入れ条件・隔離されたgitワークツリーへ展開する構成が明確です。
  - 人文: ハードウェア設計のような高リスク領域で、エージェントにどこまで自律性を渡すかは信頼の設計問題です。ハーネスは自由を奪う檻ではなく、責任を追跡可能にする作法として現れています。

### 4. What makes a harness a harness: agent harness の必要十分条件を定義する概念整理
- 出典: arXiv
- 日付: 2026-06-08（古いが基礎的で関連性が高い）
- リンク: https://arxiv.org/abs/2606.10106
- 要約: Claude Code や Codex CLI、SWE-bench harness、agent framework、IDE plugin などが混同されがちな現状を整理し、「agent harness」と呼べるための必要十分条件を概念分析で定義しようとする論文です。馬具、古典的 test harness、ML evaluation harness、agent harness への語の系譜も扱っています。
- なぜ面白いか:
  - 技術: 用語を整理することで、製品、評価基盤、SDK、オーケストレータの境界を比較可能にしようとしています。
  - 人文: 新しい技術領域では、名前が先に流通し、後から実践が追いつきます。この論文は「ハーネス」という比喩が、制御・安全・自由・責任をどう語らせるかを考える足場になります。

### 5. ハーネスエンジニアリング入門: CLAUDE.md の次に来る日本語コミュニティ発の実践整理
- 出典: Qiita
- 日付: 2026-03-24公開（古いが、検索上は2026-07-13にも再浮上しており日本語コミュニティ確認として重要）
- リンク: https://qiita.com/nogataka/items/d1b3fcf355c630cd7fc8
- 要約: CLAUDE.md、AGENTS.md、ルール分離、スキル、フック、メモリ、検証ループを組み合わせ、AIエージェントの品質を「お願い」ではなく構造で守るという日本語の記事です。Qiita上で「CLAUDE.mdの次に来るAIエージェント制御パラダイム」として、ハーネスエンジニアリングを実運用目線で説明しています。
- なぜ面白いか:
  - 技術: Claude Code 周辺の実践を、コンテキストファイルから永続的な制約・違反検知・検証ループへ拡張する道筋として読めます。
  - 人文: 日本語コミュニティでは、英語圏の研究用語が現場の比喩や運用知として再翻訳されます。この記事は、AIエージェントを「賢い個人」ではなく、組織の規範に接続される作業者として扱う文化的転換を示しています。

## arXiv / 学術

- ContextSniper: AntTrail's Token-Efficient Code Memory for Repository-Level Program Repair — arXiv:2607.01916。Claude Code を含む修復エージェントで、文脈選択ハーネスの効果を評価。
- RuBench: A Repository-Level Agentic Coding Benchmark with Natively Authored Russian Task Specifications — arXiv:2607.06411。母語タスク仕様と非公開回帰テストで製品CLIエージェントを評価。
- Agentic Hardware Design as Repository-Level Code Evolution — arXiv:2606.28279。Markdown harness から評価器・受け入れ条件・git policy を含むプロジェクトパックを生成。
- What makes a harness a harness: necessary and sufficient conditions for an agent harness — arXiv:2606.10106。agent harness の定義と系譜を整理。
- EvoTrainer: Co-Evolving LLM Policies and Training Harnesses for Autonomous Agentic Reinforcement Learning — arXiv:2606.03108。training harness 自体をポリシーと共進化させる方向性として関連。

## メモ

- Boris Cherny優先の有無: `x_search` はクレジット/購読制限で実行不能でした。代替として Bing RSS 経由で `site:x.com/bcherny`、`Boris Cherny Claude Code harness`、`Claude Code test harness` を確認しましたが、本調査時点で採用できる具体的投稿は確認できませんでした。
- 日本語アカウントの扱い: X検索は同じ理由で実行不能でした。代替Web検索では、Qiitaの「ハーネスエンジニアリング入門」を日本語コミュニティ側の主要実践記事として採用しました。
- 注意点・誇張リスク: Web検索ツールは未設定、X検索は外部クレジット制限で失敗したため、今回のトップ5は arXiv API、Bing RSS、直接URL取得で確認できた情報に限定しています。X上の最新反応量やBoris Cherny本人の直近投稿は未確認です。

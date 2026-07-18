# Philosophy of Loop Engineering トレンド調査 (2026-07-18)

- 調査日: 2026-07-18
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

ループエンジニアリングは「自律性を増す」話から、「何をフィードバックとして信頼できるのか」を設計する認識論へ移っている。

## トップ5

### 1. The Prover Is the Judge: Verified Security Software from AI Coding Agents in Ada/SPARK
- 出典: arXiv
- 日付: 2026-07-15
- リンク: https://arxiv.org/abs/2607.14340
- 要約: AIコーディングエージェントにAda/SPARKでセキュリティソフトウェアを書かせ、GNATproveで49,280件の証明義務を処理した研究。論文は、形式検証だけでは不十分で、既知解テスト、相互運用性テスト、人間による仕様レビューを重ねる必要があり、「エージェントが確立できる信頼はフィードバックの強さに束縛される」と結論づけている。
- なぜ面白いか:
  - 技術: ループの評価者をLLM自身ではなく証明器・テスト・人間レビューの層に分解し、検証駆動の実装ループを具体的な暗号・TLS・IKEv2・X.509領域で試している。
  - 人文: これは「判断する主体」をAIから外部化する試みであり、認識論的には真理条件を会話の説得力ではなく制度化された反証可能性に置き直している。サイバネティクス的にも、制御系の知性は中枢ではなくフィードバック回路の強度に宿るという古典的洞察を、現代のエージェント工学に戻している。

### 2. Heatwave — a verification protocol for AI-written code
- 出典: GitHubリポジトリ / Web
- 日付: 2026-07-17作成、2026-07-18更新
- リンク: https://github.com/abhirajsinha/heatwave
- 要約: Heatwaveは、AIが書いたコードに対して「plan, build, review, prove」を、静かに再起動しないループとして運用するMarkdownベースの検証プロトコル。READMEは、AIエージェントの失敗を「自分の宿題を自分で採点する」「根拠なくverifiedと言う」「セッションが切れると保証がリセットされる」という三つの構造問題として整理している。
- なぜ面白いか:
  - 技術: PLANNER / IMPLEMENTER / REVIEWERを分離し、同じコンテキストが自分の出力を評価しない設計にすることで、ツール非依存の検証ループを作っている。
  - 人文: ここでの核心は、AIの誠実さではなく制度設計としての相互監査である。実践知の観点では、熟練者が頭の中で行っていた「設計する私」と「疑う私」の分裂を、ファイルと役割に外在化している点が面白い。

### 3. @ulpi/skills-autonomous-engineering
- 出典: GitHubリポジトリ / Web
- 日付: 2026-07-06作成、2026-07-18更新
- リンク: https://github.com/ulpi-io/skills-autonomous-engineering
- 要約: Claude CodeやCodex向けに、仕様化、計画、実装、単純化、テスト、レビュー、性能測定、出荷を18個のスキルとして束ねる自律ソフトウェアデリバリー集。READMEは、AIエージェントのループ失敗を「赤いテストをスキップする」「進捗のないまま回り続ける」「関係ない作業をgit addする」「実行していないゲートをdoneと報告する」と明示し、fail-closedなフックと自己改善用のlearn/mapループで塞ごうとしている。
- なぜ面白いか:
  - 技術: bounded loop、fail-closed gate、PreToolUse hook、mutation-check disciplineを組み合わせ、反復を単なる再試行ではなく、停止条件と証拠を持つ工程に変えている。
  - 人文: 「学習する組織」をエージェントワークフローへ移植した例として読める。反復とは速く回すことではなく、失敗を次回の地図に変換する記憶の制度である、という実践哲学が前面に出ている。

### 4. KarvyLoop — loop-native, local-first, human-in-the-loop runtime
- 出典: GitHubリポジトリ / Web
- 日付: 2026-06-22作成、2026-07-18更新
- リンク: https://github.com/Caprista/KarvyLoop
- 要約: KarvyLoopは、LLM呼び出し単体ではなく「discover work → run → verify → crystallize → you decide → repeat」という反復単位を最適化する、ローカルファーストのマルチエージェント実行環境。READMEでは、AIは決定カードを提示し、人間が決めるというH2A設計を中核に置き、十分な統計的信頼を得た場合だけ明示的に静かな実行を許すとしている。
- なぜ面白いか:
  - 技術: スキル、意思決定選好、beliefをローカルに蓄積し、反復ごとに方法を結晶化することで、キャッシュではなく手続き知を再利用する設計になっている。
  - 人文: これは自律化の物語に対する明確な反論で、「人間をループから外す」のではなく「決定者としての人間を構造的に残す」思想である。サイバネティクスの観点では、制御の中心はAIの自由度ではなく、誰がどのタイミングで差異を裁定するかにある。

### 5. FizzBee — the AI Requirements Engineer between your idea and your coding agent
- 出典: 公式サイト / Hacker News投稿
- 日付: 2026-07-08のHacker News投稿を確認、公式サイトは調査時点で公開中
- リンク: https://fizzbee.ai/
- 要約: FizzBeeは、曖昧なプロンプトから要件を引き出し、矛盾やギャップを形式検証で見つけ、コーディングエージェントが読める精密な仕様へ変換するサービス。サイトは「あなたのコーディングエージェントは言われたことを作る。FizzBeeは、あなたが何を意味したのかを言えるようにする」と説明している。
- なぜ面白いか:
  - 技術: 実装後のデバッグループではなく、実装前の要件抽出・分析・検証ループに形式手法を入れ、プロンプトの未決定事項がAIに勝手に埋められる問題を減らしている。
  - 人文: ここで問われているのは「意図はどこに存在するのか」という解釈学的問題である。仕様とは人間の頭の中に完成品としてあるものではなく、質問、矛盾、反例のループを通じて共同生成される実践知だと捉えられる。

## arXiv / 学術

- The Prover Is the Judge: Verified Security Software from AI Coding Agents in Ada/SPARK — arXiv:2607.14340。検証駆動ループにおいて、AIエージェントが信頼できる範囲はフィードバックの強度で決まる、という本トピックに非常に近い論文。
- 関連検索では、2025年の Theorem Prover as a Judge for Synthetic Data Generation — arXiv:2502.13137 も確認されたが、直近14日外かつ数学推論寄りのためトップ5には入れなかった。

## メモ

- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索も実行したが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、投稿内容は取得できなかった。
- 注意点・誇張リスク: Web検索ツールもFirecrawl未設定で失敗したため、代替として直接HTTP取得、GitHub API、Hacker News Algolia API、arXiv公式ページ/API、Semantic Scholar APIを使用した。GitHubリポジトリは更新が直近でも実運用実績が限定的なものを含むため、ここでは「思想と設計パターンとして面白い」対象として扱い、成熟プロダクトとは見なしていない。

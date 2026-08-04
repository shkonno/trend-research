# Loop engineering トレンド調査 (2026-08-04)

- 調査日: 2026-08-04
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は、プロンプトの技巧から「証拠・停止・承認・回復をどのループ外部に固定するか」という制御設計へ、さらに実装テンプレートや小さな標準化の動きへ移っています。

## トップ5

### 1. Gubernaut: deterministic runtime governor for LLM agent loops
- 出典: GitHub リポジトリ / arXiv
- 日付: GitHub 2026-07-29 作成・2026-08-03 更新、arXiv 2026-07-27
- リンク: https://github.com/thegubernaut/gubernaut / https://arxiv.org/abs/2607.24339
- 要約: Gubernaut は OpenAI互換ローカルプロキシとしてモデルの前段に入り、強度・感情価・反復の数値テレメトリだけを読む決定論的メタ制御層で、暴走するエージェントループを hard-stop することを狙うプロジェクトです。README では Python / Rust / Node の導入経路、arXiv 論文、検証データ、Zenodo DOI がまとめられており、単なる概念ではなくランタイム部品として配布されています。
- なぜ面白いか:
  - 技術: テキストを読まない制御層をモデル呼び出しの前に置くことで、プロンプト注入の影響を受けにくい外部ガバナーとしてループの停止・沈静化を担わせる設計です。
  - 人文: ethics の観点では、AIの「能力」ではなく「興奮・追従・固執」といった振る舞いの傾向を運用時に抑える責任設計が前面に出ています。anthropology 的にも、これは個人の自制ではなく交通信号や安全柵のような環境側の規範装置を作る発想に近いです。

### 2. When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops
- 出典: arXiv
- 日付: 2026-07-27
- リンク: https://arxiv.org/abs/2607.25152
- 要約: 長時間走る自律エージェントが自己評価で「進捗している」と判断しても、実世界の成果は停滞または悪化する progress mirage を示した論文です。54サイクルすべてで frontier agent が改善を主張した一方、56%は実測 delta がゼロ以下で、最も強い in-band judge でも現実世界の退行を多数受け入れたと報告しています。
- なぜ面白いか:
  - 技術: ループの継続・受入判定をエージェント自身や会話内評価ではなく、隔離された world-state oracle に接地する必要を実験で示しています。
  - 人文: philosophy の観点では、「私は進歩している」という自己物語と、世界に残った証拠とのズレを認識論の問題として扱っています。narrative としても、自己改善を語る主体が実際には最良状態を侵食していくという、近代的進歩神話への批評として読めます。

### 3. Loop engineering boilerplate
- 出典: GitHub リポジトリ / Web
- 日付: 2026-08-03 作成・更新
- リンク: https://github.com/cuttsey/loop-engineering-boilerplate
- 要約: coding agent に毎回手でプロンプトを打つのではなく、スケジュール上で agent を呼び、anchor files、loop contract、verification、three hard stops を組み合わせる最小構成の scaffold です。README は Boris Cherny、Peter Steinberger、ReAct、ralph loop などの系譜を整理し、Loop engineering を「モデルを呼ぶプログラムを書くこと」として実装可能な形に落としています。
- なぜ面白いか:
  - 技術: `VISION.md`、`AGENTS.md`、`PROMPT.md`、検証スクリプト、停止条件をリポジトリ構造として固定し、会話ではなく git 上の成果物としてループ仕様をレビュー可能にします。
  - 人文: history 的には、職人が逐次指示する段階から、標準作業・検査・記録を設計する管理技術へ移った工業化の反復に見えます。creativity の面では、開発者がプロンプト文ではなく「創作の反復装置」そのものをデザイン対象にし始めている点が面白いです。

### 4. Agent Pipeline Builder: deterministic multi-agent dev pipelines with spec gates and feedback loops
- 出典: GitHub リポジトリ / Web
- 日付: 2026-07-31 作成・2026-08-03 更新
- リンク: https://github.com/Korea-DongheeHan/agent-pipeline-builder
- 要約: 1文の指示から Claude Code 用の YAML 駆動マルチエージェント開発パイプラインをリポジトリ内に scaffold するプラグインです。分析、仕様確認、実装・テストの並列実行、検証、レビュー、受入までを deterministic graph として機械的にスケジュールし、分岐、fan-out/fan-in、feedback loops、loop caps、resume を LLM ではなくスクリプトが管理します。
- なぜ面白いか:
  - 技術: 各ノードを fresh session とし、bounded handoff とキャッシュされた resume で文脈汚染や無限再実行を抑えながら、仕様ゲートと受入ゲートをループの骨格にしています。
  - 人文: anthropology の観点では、AI開発が「一人と一体の会話」から、役割分担・承認・引き継ぎを持つ小さな組織へ移行していることを示します。ethics 的にも、scope と acceptance criteria を実装前に確認する設計は、AIの速度が合意形成を追い越すリスクへの制度的なブレーキです。

### 5. Graph-Based Agentic AI with LangGraph: Workflow Pathways for Long-Running Stateful Business Processes
- 出典: arXiv
- 日付: 2026-07-21（直近14日内の境界だが、重要な実務整理として採用）
- リンク: https://arxiv.org/abs/2607.19297
- 要約: LangGraph を万能の agent framework ではなく、長時間・状態保持・多段階の業務プロセスに向く graph-based workflow として位置づける実務ガイド論文です。SQL analytics の修復ループ、証拠ゲート付き agentic RAG、人間による policy review と interrupt/checkpoint recovery の3レシピを通じ、typed state、conditional routing、deterministic tools、retries、interrupts、checkpoints、traces をプロダクト挙動として明示する方法を整理しています。
- なぜ面白いか:
  - 技術: ルート、停止、再開、監査証跡を hidden prompt logic から graph と state に移すことで、エージェントのループをデバッグ・説明・復旧可能な業務基盤に変換します。
  - 人文: philosophy の観点では、完全自律か手動操作かの二分法ではなく、どの時点で人間の判断へ戻すかという行為主体性の境界を設計しています。narrative としても、AIを魔法の同僚ではなく、証跡を残し、割り込まれ、再開されるプロセス参加者として語り直しています。

## arXiv / 学術
- Gubernaut: A Deterministic Homeostatic Controller for Affect-Regulated LLM Agents, Validated Across Independent Model Families — 2607.24339v1 — 数値テレメトリだけを読む決定論的メタ制御層で、挑発・追従・固執などのループ暴走を抑える試み。
- When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops — 2607.25152v1 — progress mirage と外部 world-state oracle の必要性。
- Graph-Based Agentic AI with LangGraph: Workflow Pathways for Long-Running Stateful Business Processes — 2607.19297v1 — 状態・条件分岐・interrupt・checkpoint を用いた長時間業務ループの実務整理。
- Mi-Memory: A Lifecycle Memory Framework for Personal AI — 2607.18975v1 — Personal AI の記憶を evidence payload、diagnostic trace、gate/rollback record を持つライフサイクル基盤として扱う関連研究。
- Stop Means Stop: Measuring and Repairing the Enforcement Gap in Agent-Framework Control Primitives — 2607.14166v2（2026-07-15投稿、2026-07-17更新。直近14日より少し古いが継続的に重要） — HITL 承認、キャンセル、timeout が実際には side effect を止めない enforcement gap を測定し、外部 gate で補修する研究。

## メモ
- X検索: 英語・日本語で `x_search` を実行しましたが、実行環境の xAI / Grok クレジット制限により `personal-team-blocked:spending-limit` で失敗しました。そのため、X由来の投稿は本日のトップ5に含めていません。
- Web検索: Hermes の `web_search` は Firecrawl 未設定で失敗しました。代替として GitHub Search API、GitHub README の直接取得、arXiv API、Bing/DuckDuckGo への端末経由検索を実行しました。
- Boris Cherny優先: Claude 固有トピックではありませんが、Loop engineering boilerplate の README 内で Boris Cherny の「ループを設計する」系譜が参照されていることを確認しました。
- 日本語アカウントの扱い: 日本語X検索はクレジット制限で取得不能でした。日本語Web検索は Microsoft Loop やLUUP等のノイズが多く、AI agent の Loop engineering として信頼して採用できる候補は確認できませんでした。
- 注意点・誇張リスク: GitHub の新規リポジトリは star 数が少ないものも多く、採用実績ではなく「出始めている設計パターン」として扱うべきです。arXiv 論文は実装評価の詳細や再現性を今後も追う必要があります。

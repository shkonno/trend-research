# Harness engineering トレンド調査 (2026-08-18)

- 調査日: 2026-08-18
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「よいプロンプト」から、「検証・状態・権限・複数エージェントをどう束ねるか」という実行基盤の設計論へ移っています。

## トップ5

### 1. HarnessRouter Community Edition と Unified Harness Protocol

- 出典: GitHub リポジトリ / HN での共有
- 日付: 2026-08-17 更新（リポジトリ作成 2026-08-09）
- リンク: https://github.com/HarnessRouter/harnessrouter
- 要約: HarnessRouter は Claude Code、Codex、Hermes などの agent harness をセルフホストの一つの API から扱うためのコミュニティ版実装です。README では Unified Harness Protocol (UHP) への準拠、セッション、ストリーミング、ファイル、キャンセル、失敗処理を共通化する方針が示されています。
- なぜ面白いか:
  - 技術: 複数の coding agent を「モデル」ではなく「harness」という実行単位で抽象化し、セッション管理や失敗処理を標準プロトコルに押し出している点が重要です。
  - 人文: エージェント利用が個人の職人芸から組織の運用インフラへ変わると、誰が権限を持ち、どのログを信頼し、失敗時に誰が責任を取るのかが設計対象になります。HarnessRouter はその社会的な合意形成を、API とプロトコルの形に翻訳しようとしているように見えます。

### 2. Boris Cherny の「検証が最重要」という Claude Code 観

- 出典: Daring Fireball による Boris Cherny 発言の紹介
- 日付: 2026-08-02（直近14日より少し古いが、Boris Cherny / Claude Code との接点として重要）
- リンク: https://daringfireball.net/linked/2026/08/02/cherny-claude-swift
- 要約: Boris Cherny は、難しいタスクを Claude に渡す技術は prompt engineering よりも「作業の途中で Claude が自分の成果を検証できるようにすること」だと述べています。Electron 版 Claude アプリを Swift で作り直す例では、Mac runner、スクリーンショット、ピクセル比較のような検証可能な環境を整えることが中心になっています。
- なぜ面白いか:
  - 技術: Harness engineering の核心が、モデルへの依頼文ではなく、実行環境・観測手段・検証ループを与えることだと明確に言語化されています。
  - 人文: これは「AI に任せる」と「AI を監督する」の間にある新しい仕事の輪郭を示します。人間の役割は細かな指示者から、証拠・制約・評価可能性を設計する編集者や舞台監督へ移っています。

### 3. GitHub Copilot agentic harness の性能・効率評価

- 出典: GitHub Blog
- 日付: 2026-06-26（古いが、harness 評価の基準点として継続的に重要）
- リンク: https://github.blog/ai-and-ml/github-copilot/evaluating-performance-and-efficiency-of-the-github-copilot-agentic-harness-across-models-and-tasks/
- 要約: GitHub は Copilot の agentic harness を、公開ベンチマーク、社内ベンチマーク、実運用メトリクス、オンライン実験を組み合わせて評価していると説明しています。同一モデル・同一タスク・context window・reasoning effort・tool selection・MCP server などをそろえ、Claude Code や Codex CLI などモデル提供元の harness と比較する姿勢が示されています。
- なぜ面白いか:
  - 技術: harness の優劣をモデル性能から切り離し、ツール選択、MCP、トークン効率、OS 環境などの実行条件として測ろうとしている点が実務的です。
  - 人文: 開発現場で「AI が賢いか」を語るだけでは不十分になり、「どの制度・環境なら賢く振る舞えるのか」を問う段階に入っています。これは教育や労働評価で個人能力だけでなく環境設計を見る発想に近いです。

### 4. 日本語圏の agentic-harness: Planner / Generator / Evaluator 分離

- 出典: GitHub リポジトリ（日本語コミュニティ）
- 日付: 2026-08-17 更新
- リンク: https://github.com/mtaiseeei/agentic-harness
- 要約: agentic-harness は、Planner / Generator / Evaluator の 3 role、ファイル正本、Sprint、状態遷移で Claude Code / Codex 向けの開発ハーネスを構成する日本語 README のプロジェクトです。Claude Code では `/harness` やプラグイン導入、Codex では skill 起動で使う想定が書かれており、会話ではなく spec / state / progress / feedback を正本にする思想が明確です。
- なぜ面白いか:
  - 技術: Generator と Evaluator を分け、会話履歴ではなくファイル正本で再開可能性を担保することで、単発の vibe coding を継続開発プロセスへ近づけています。
  - 人文: 日本語圏では「小さな業務システム」「既存 repo の継続改修」のような生活に近いユースケースが前面に出やすく、harness が大企業の評価基盤だけでなく中小規模の現場知として翻訳されている点が面白いです。

### 5. SBCO: Self-Supervised, Verifier-Grounded Harness Optimization For Planning Agents

- 出典: arXiv
- 日付: 2026-08-10
- リンク: http://arxiv.org/abs/2608.10157v1
- 要約: SBCO は、明示的制約を持つ planning task に対して、verifier-grounded な harness optimizer を用い、自己参照的にコードを書き換える高コストな自己改善ではなく、閉ループで安価に harness を最適化する手法を提案しています。planning agent の性能改善を「エージェント本体」ではなく「検証器に接地した harness」の調整として扱う点が特徴です。
- なぜ面白いか:
  - 技術: 自己改善をモデルやエージェントの自己改造に寄せず、verifier と harness の探索問題として定式化しているため、安全性と再現性のある改善ループに近づきます。
  - 人文: 「賢い主体が自分を変える」という物語から、「制度や足場を調整すると行動が変わる」という社会工学的な物語へ重心が移ります。AI エージェントを人格化しすぎず、環境に埋め込まれた行為者として見る助けになります。

## arXiv / 学術

- SBCO: Self-Supervised, Verifier-Grounded Harness Optimization For Planning Agents（2608.10157v1, 2026-08-10）: verifier-grounded な harness optimizer を planning agent に適用する論文で、本日のトップ5に採用しました。
- Vero: Can AI Agents Build Formally Verified Software Repositories?（2608.13522v1, 2026-08-13）: リポジトリ単位で実装と証明を合成する benchmark。harness engineering の「検証可能な成果物」側の流れとして関連します。
- DCAS: Decoupling CLI Agent Scaffolding to Internalize Planning across Scaffolds（2608.06113v1, 2026-08-06）: CLI scaffold 間の評価差と planning 構造を扱い、harness / scaffold 依存を考える上で関連します。
- InfraBench: Evaluating Infrastructure Agents Across Layers, Lifecycle, and Risk（2608.11234v1, 2026-07-31）: 14日枠から少し外れますが、公開 evaluation harness と risk assessment を含む infrastructure agent benchmark として参考になります。

## メモ

- Boris Cherny優先の有無: 優先しました。X 検索は実行しましたが、xAI 側の `personal-team-blocked:spending-limit` により取得できなかったため、Daring Fireball に転載・引用された Boris Cherny 発言と Claude Code 関連ソースを確認しました。
- 日本語アカウントの扱い: X の日本語検索も同じ理由で失敗しました。代替として GitHub API で日本語 README / 日本語説明の Claude Code harness プロジェクトを確認し、`mtaiseeei/agentic-harness` を採用しました。
- Web検索の注意: Hermes の `web_search` は Firecrawl 未設定で失敗しました。代替として DuckDuckGo HTML 取得、HN Algolia API、GitHub API、arXiv API、直接 HTTP 取得を使用しました。
- 注意点・誇張リスク: GitHub リポジトリの star 数や HN 掲載は成熟度を保証しません。本日の選定は「harness engineering としての設計論が見えるか」を重視しており、プロダクション品質の保証ではありません。

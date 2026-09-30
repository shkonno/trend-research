# Harness engineering トレンド調査 (2026-09-30)

- 調査日: 2026-09-30
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「モデルを賢くする」話から、「モデルの周囲にある実行環境・証跡・ガードレール・人間の決裁点を設計する」話へ、かなり実装寄りに収束しています。

## トップ5

### 1. Harness Learning Enables Generalizable Test-Time Adaptation
- 出典: arXiv
- 日付: 2026-09-28
- リンク: http://arxiv.org/abs/2609.35738v1
- 要約: エージェントを「モデル＋ハーネス」で定義し、実行フィードバックを使ってハーネス自体を更新する “harness learning” を提案する論文です。重み更新ではなく、モデル呼び出し・ツール利用・情報流を組む実行プログラムをテスト時に改善する点が中心です。
- なぜ面白いか:
  - 技術: プロンプトやツール定義を固定物ではなく、実行結果から改訂されるメタ学習対象として扱っているため、loop engineering の「回して、観測して、組み替える」思想にかなり近いです。
  - 人文: ここでは知能の主体が単体モデルから、モデルを取り巻く制度・手順・評価環境へ移っています。人間の学習も個人の頭脳だけでなく、ノート、儀式、レビュー、教育制度に支えられることを思い出させます。

### 2. Tracekit: Tamper-Evident Intent-Reasoning-Action Auditing for Autonomous Coding Agents
- 出典: arXiv
- 日付: 2026-09-28
- リンク: http://arxiv.org/abs/2609.35659v1
- 要約: Claude Code の lifecycle events に接続し、人間の意図、モデルの自己報告、実際のアクションをハッシュチェーン化された台帳へ記録する監査基盤です。マルチエージェント階層の再構成、実行前ポリシーゲート、ブラウザ上の検証ビューまで含むとされています。
- なぜ面白いか:
  - 技術: Claude Code と harness engineering の接点として、単なるログではなく改ざん検知・ポリシーゲート・行動検証をハーネス側の責務にしているのが重要です。
  - 人文: 自律コーディングの責任は「誰が何をしたか」を後から語れる形式で残せるかに依存します。これはソフトウェア開発を、成果物だけでなく証言可能性と説明責任を含む社会的実践として捉え直す動きです。

### 3. What Will Remain Human in Software Architecture? A Focus Group Report
- 出典: arXiv
- 日付: 2026-09-24
- リンク: http://arxiv.org/abs/2609.30334v1
- 要約: EuroPLoP 2026 のフォーカスグループ報告で、AI 開発エージェント時代にソフトウェアアーキテクチャで何が人間に残るかを議論しています。要旨では、アーキテクチャ上の意思決定、説明責任、ガードレールの設計が人間に残り、AI-assisted system creation を統治する分野として harness engineering が浮上したとされています。
- なぜ面白いか:
  - 技術: ハーネスをツール呼び出しの便利機構ではなく、検証、ガバナンス、制約、教育を含むアーキテクチャ上の構成要素として扱っています。
  - 人文: 「何を自動化できるか」ではなく「何を人間の責任として残すべきか」という問いに軸足があります。AI エージェントの普及で、設計者の役割はコードを書く人から、境界条件と責任の配置を決める人へ移っていきます。

### 4. claude-dev-harness: 言語・フレームワークに依存しない Claude Code 開発ハーネス
- 出典: GitHub / 日本語コミュニティ
- 日付: 2026-09-29 更新
- リンク: https://github.com/mizuta0711/claude-dev-harness
- 要約: `harness-core` プラグインとテンプレート層に分け、Next.js、Unity、WPF などの環境差を吸収しながら Claude Code 用の共通開発ハーネスを配布する日本語リポジトリです。README では Windows + VSCode 拡張における project scope plugin の既知問題まで具体的に記録されています。
- なぜ面白いか:
  - 技術: Claude Code の skills/plugins をプロジェクト横断で再利用するため、コア契約とテンプレート層を分離している点が実務的です。
  - 人文: 日本語コミュニティでも、AI 活用は「便利なプロンプト集」から「チームや環境にまたがって維持できる作法」へ移っています。既知の不具合や制約を明記する姿勢は、AI ツールを魔法ではなく運用対象として扱う文化を育てます。

### 5. CP-Agent: A Harness-Engineered Agent for Crystal Plasticity Simulation Workflows
- 出典: arXiv
- 日付: 2026-09-25
- リンク: http://arxiv.org/abs/2609.31790v1
- 要約: 結晶塑性シミュレーションのワークフローを自然言語タスクから実行する、ハーネス設計型の LLM エージェントです。最小限のシステムプロンプト、型付きツール定義、ディスパッチャ、安全境界付き反復ループで、専門領域の知識をツールスキーマと実行制約に埋め込む構成です。
- なぜ面白いか:
  - 技術: harness engineering がコーディング支援だけでなく、複数ツールを束ねる科学技術計算ワークフローにも適用されていることを示しています。
  - 人文: 専門家の暗黙知を「全部モデルに覚えさせる」のではなく、道具の配置、実行順序、安全な反復として外部化する発想です。これは職人技を奪うというより、専門家が安心して委任できる作業場を作る試みに見えます。

## arXiv / 学術
- Harness Learning Enables Generalizable Test-Time Adaptation — arXiv:2609.35738v1。ハーネスを実行フィードバックで更新するメタ学習的アプローチ。
- Tracekit: Tamper-Evident Intent-Reasoning-Action Auditing for Autonomous Coding Agents — arXiv:2609.35659v1。Claude Code lifecycle events と監査可能な証跡を接続。
- What Will Remain Human in Software Architecture? A Focus Group Report — arXiv:2609.30334v1。harness engineering を AI-assisted system creation の統治領域として位置づけ。
- CP-Agent: A Harness-Engineered Agent for Crystal Plasticity Simulation Workflows — arXiv:2609.31790v1。科学技術計算への応用例。
- 関連するがトップ5外: Harness Engineering in LLM Tool Use via Agent-Native Reusable Tool Primitives — arXiv:2609.01736v1、2026-09-01。直近14日より古いが、Tool Primitives / ToolFace により大規模ツールカタログと自然言語インターフェイスを接続する基礎的文脈として重要。

## メモ
- Boris Cherny優先の有無: `@bcherny` を含む X 検索を実行しましたが、x_search は `personal-team-blocked:spending-limit` で利用できませんでした。Bing RSS でも Boris Cherny と harness engineering の有意な直近接点は確認できませんでした。
- 日本語アカウントの扱い: X の日本語検索も同じ理由で取得できませんでした。代替として GitHub API と Bing RSS を使い、日本語圏では `mizuta0711/claude-dev-harness`、`daishiman/HarnessHub`、`maee-co/cc-autoship`、`SuguruOoki/harness-engineering` などを確認しました。トップ5には Claude Code 実務ハーネスとして最も具体性が高い `mizuta0711/claude-dev-harness` を採用しました。
- 注意点・誇張リスク: Web 検索ツールは Firecrawl 未設定で失敗したため、Web 側は `terminal` からの Bing RSS、GitHub API、arXiv API で補完しました。GitHub リポジトリは更新日が新しくても、スター数や利用実績はまだ小さいものが多く、流行の強さよりも「設計パターンの兆候」として読むのが安全です。

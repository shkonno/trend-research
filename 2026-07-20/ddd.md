# DDD トレンド調査 (2026-07-20)

- 調査日: 2026-07-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AI/LLM/agent時代のDDDは「実装パターン」から、チームの知識・判断・言葉を機械可読な共有状態にするための設計文化へ重心が移っている。

## トップ5

### 1. Archally Blueprint Schema: DDD・ADR・ルール・ガバナンスを1つのYAMLモデルに統合

- 出典: GitHubリポジトリ / Web
- 日付: 2026-07-17更新（作成: 2026-05-25）
- リンク: https://github.com/Archally/blueprint-schema
- 要約: Archally Blueprint Schemaは、ドメイン設計、ビジネスルール、価値ストリーム、ガバナンス、組織的整合を1つの機械可読YAMLで表現し、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Storming board、MCP経由のAI agent groundingへ展開する構想です。READMEでは、散らばったwiki・スライド・ホワイトボード写真・暗黙知を「fragmented truth」と捉え、アーキテクチャを地図作成のようにレイヤー化して扱う、と説明しています。
- なぜ面白いか:
  - 技術: DDDのbounded context、decision record、business rule、event storming artifactを、AI agentが参照・検証できる単一の構造化ソースへ寄せようとしている点が重要です。
  - 人文: これは単なるドキュメント自動生成ではなく、組織内の「誰が何を知っているか」という記憶の偏在を、地図という公共物へ変える試みです。ユビキタス言語が人間同士だけでなく、人間とagentの間の共有語彙になりつつあることを示しています。

### 2. event-storming-canvas: Claudeが共同モデレーターになるAI-native Event Storming board

- 出典: GitHubリポジトリ / Web
- 日付: 2026-07-13更新（作成: 2026-06-05）
- リンク: https://github.com/przeprogramowani/event-storming-canvas
- 要約: przeprogramowani/event-storming-canvasは、ブラウザ上のEvent Storming boardを人間が操作し、ClaudeベースのAID agentが同じ`board.json`を読み書きして、domain event、command、actor、read model、policy、external system、aggregate、hotspotを追加・整理・問い直す教材的ツールです。READMEでは「人間とagentが同じ状態をリアルタイムに編集するAI-Nativeパターン」を示すことが目的とされています。
- なぜ面白いか:
  - 技術: Event Stormingの付箋を単なるUI要素ではなく共有JSON状態として扱い、Server-Sent Eventsで即時反映することで、LLM agentをワークショップの共同参加者にしています。
  - 人文: DDDのワークショップは本来、合意形成と発見の儀式です。agentが「板書係」ではなく、hotspotを指摘し質問を差し込む存在になると、ファシリテーターの権威や参加者の沈黙の扱いも変わります。

### 3. ddd-agent-skill: DDDを実施すべきかから始めるAgent Skill

- 出典: GitHubリポジトリ / Web
- 日付: 2026-07-07更新（作成: 2026-07-07）
- リンク: https://github.com/aristorinjuang/ddd-agent-skill
- 要約: aristorinjuang/ddd-agent-skillは、Vernonの『Implementing Domain-Driven Design』に沿って、assessment、DDD-worthiness gate、strategic design、tactical modeling、implementation、auditを段階的に進めるAgent Skillです。特徴は、最初にcore/supporting/generic subdomainを見極め、Full DDD、Light DDD、plain CRUDのどれが妥当かを判断し、DDDが過剰な場合は明示する点です。
- なぜ面白いか:
  - 技術: Event Storming、ubiquitous language、context map、aggregate、entity、value object、domain event、repositoryまでをagent workflow化しつつ、最初に「DDDを使わない」という分岐を入れている点が実務的です。
  - 人文: 設計手法はしばしば信仰のように広がりますが、このskillはDDDを万能薬ではなく状況依存の共同判断として扱います。agentが方法論の布教者ではなく、過剰設計を止める同僚になれるかが問われています。

### 4. AppFactory: DDD・GraphQL・agent・code generationを束ねたAI-native software factory

- 出典: GitHubリポジトリ / Web
- 日付: 2026-07-17更新（作成: 2026-07-14）
- リンク: https://github.com/antoniofregoso/AppFactory
- 要約: AppFactoryは、小規模チームがエンタープライズ級アプリケーションを作るためのAI-native software factoryとして、Domain-Driven Design、GraphQL、再利用可能アーキテクチャ、intelligent agents、code generationを組み合わせるリポジトリです。READMEでは、FastAPI、GraphQL、PostgreSQL、Preactを基盤に、モデル定義を中心に検索・権限・MCP reportなどを構成する方向が示されています。
- なぜ面白いか:
  - 技術: DDDを抽象的な設計論に留めず、GraphQL API、データモデル、AI検索、MCPレポートと接続して、生成可能な業務アプリ基盤へ落とし込んでいます。
  - 人文: 「小さなチームが大組織並みのソフトウェア生産力を持つ」という物語は魅力的ですが、同時にドメイン理解を誰が保証するのかという問いを強めます。DDDは、生成速度に対する文化的ブレーキ、あるいは責任の署名として再評価されそうです。

### 5. Automating Domain-Driven Design: LLMはDDDの前半に強く、後半では誤差が蓄積する

- 出典: arXiv / 学術論文
- 日付: 2026-03-27（直近14日外だが、DDD×LLMの直接研究として重要）
- リンク: https://arxiv.org/abs/2603.26244
- 要約: “Automating Domain-Driven Design: Experience with a Prompting Framework”は、LLMプロンプティングでDDDを、ユビキタス言語の確立、Event Stormingのシミュレーション、bounded context識別、aggregate設計、technical architecture mappingの5段階に分解して試した研究です。FTAPIのエンタープライズ要件を用いた検証では、1〜3段階は有用な成果物を生む一方、4〜5段階では小さな誤りが蓄積し実用性を損ねる、と報告しています。
- なぜ面白いか:
  - 技術: LLMをDDDの完全自動化装置ではなく、glossaryやcontext map作成を支援するcollaborative sparring partnerとして位置づけている点が、現在のagent設計にそのまま効きます。
  - 人文: この論文の核心は「専門家を不要にする」ではなく「専門家が議論すべきトレードオフに集中できるようにする」です。DDDの価値が成果物ではなく対話の質にあることを、AI時代にあらためて確認させます。

## arXiv / 学術

- Automating Domain-Driven Design: Experience with a Prompting Framework — arXiv:2603.26244（2026-03-27）: DDDを5段階プロンプティングに分解し、LLMはユビキタス言語・Event Storming・bounded contextの初期整理に有用だが、aggregate設計以降は誤差が蓄積すると報告。
- Leveraging Generative AI for Enhancing Domain-Driven Software Design — arXiv:2601.20909（2026-01-28）: DDDメタモデル生成を生成AIで部分自動化し、ドメイン固有JSON生成の可能性を検証。直近14日外のためトップ5には入れませんでしたが、関連研究として確認しました。

## メモ

- X検索: 英語・日本語クエリで実行しましたが、x_searchは `personal-team-blocked:spending-limit` により取得不能でした。そのため本ファイルではX由来の個別投稿を採用していません。
- Web検索: Hermesのweb_search/web_extractはFirecrawl未設定で失敗し、DuckDuckGo HTMLは自動化チャレンジに阻まれました。代替としてGitHub Search API、GitHub repository API、arXiv APIを直接HTTP取得して確認しました。
- 日本語アカウントの扱い: X取得不能のため確認できませんでした。
- 注意点・誇張リスク: GitHubリポジトリはREADMEとメタデータに基づく評価であり、実運用品質や利用者数は未検証です。スター数が少ないものも含むため、「流行の確定」ではなく「DDD×agent設計の萌芽」として扱うのが安全です。

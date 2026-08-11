# DDD トレンド調査 (2026-08-11)

- 調査日: 2026-08-11
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AI/LLM時代のDDDは、「人間が共有する言葉」を守る方法から、「人間とエージェントが同じ境界・モデル・判断根拠で働くための運用基盤」へ広がっている。

## トップ5

### 1. Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design

- 出典: arXiv
- 日付: 2026-08-06
- リンク: https://arxiv.org/abs/2608.05612
- 要約: JDomInOという双方向同期ツールチェーンを提案し、戦術的DDDのドメインモデルからJavaコード構造を生成し、既存コードからモデルを再構成する。論文は、この構造化ドメインモデルがAIコードアシスタントにとって、集約境界やDDDセマンティクスを守る精密なコンテキスト層になり得ると位置づけている。
- なぜ面白いか:
  - 技術: DDDモデルと実装のドリフトを「生成」と「逆解析」の往復で抑え、LLMに生コードだけでは見えにくい境界づけられたコンテキストを渡せる点が重要。
  - 人文: ユビキタス言語は会議室の合意だけでなく、コード、モデル、AIエージェントの間を循環する記憶になりつつある。設計知識を誰が保持するのかという問いが、個人の熟練からチームと道具の共同責任へ移っている。

### 2. From Textual Requirements to Microservice Architectures - A Comprehensive Evaluation of LLM-Based Design Synthesis

- 出典: arXiv
- 日付: 2026-07-30
- リンク: https://arxiv.org/abs/2607.28307
- 要約: 自然言語要件だけからLLMがマイクロサービスアーキテクチャを合成できるかを、サービス識別、通信復元、専門家評価で検証する研究。DDDそのものの論文ではないが、要求から境界・サービス・相互作用を導く作業は、AI時代の戦略的設計やイベントストーミング後の設計合成と強く接続する。
- なぜ面白いか:
  - 技術: ゼロショット/ few-shotでサービス候補とインタラクションを生成・評価するため、LLMを「設計者」ではなく「境界仮説を出す道具」として扱う実験基盤になる。
  - 人文: 要件文からアーキテクチャを作る行為は、現場の曖昧な物語をどの単位で制度化するかという翻訳である。LLMが参加すると、暗黙知を早く可視化できる一方、誰の言葉がモデルに採用されるのかという組織文化上の緊張も増す。

### 3. Archally Blueprint Schema: domain-first YAML schema for AI-grounded system cartography

- 出典: GitHub / Web
- 日付: 2026-08-09 更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: ドメイン設計、意思決定記録、業務ルール、ガバナンス、アーキテクチャをYAMLで一つの機械可読な真実源にまとめ、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Storming boards、MCP経由のAIエージェント grounding へ展開するスキーマ。READMEでは、設計知識がWiki、スライド、ホワイトボード写真、部族的記憶に分散してドリフトする問題を正面から扱っている。
- なぜ面白いか:
  - 技術: DDDを文書化の作法ではなく、生成物・API・プロセス図・エージェント文脈を同期する構造化スキーマとして実装しようとしている。
  - 人文: 「fragmented truth」という問題設定が、DDDの本質を組織の記憶管理として捉え直している。AIエージェントが参加するほど、誰もが参照できる共通地図の有無がチームの信頼とオンボーディングを左右する。

### 4. Event Storming Board: AI-moderated Event Storming Workshops

- 出典: GitHub / Web
- 日付: 2026-08-03 更新
- リンク: https://github.com/przeprogramowani/event-storming-canvas
- 要約: Event Stormingをブラウザ上で行い、人間がワークショップを進め、ClaudeベースのAIDエージェントが共有ファイル `board.json` を読み書きして共同モデレーションする小型ツール。カード追加、時系列整理、ホットスポットの指摘、質問生成を通じて、人間とエージェントが同じボードを「思考の場」として使う設計になっている。
- なぜ面白いか:
  - 技術: Server-Sent Eventsで即時更新される共有JSONを単一の真実源にし、イベントストーミングの協働編集をAI-nativeなワークフローに変換している。
  - 人文: イベントストーミングは本来、利害関係者の声を同じ壁に集める儀式である。AI共同モデレーターは沈黙している論点を拾える可能性がある一方、場の権力関係や問いの立て方を無自覚に固定化する危険もある。

### 5. DomainDL Agents: multi-agent service for DDD code generation and project-aware Q&A

- 出典: GitHub / Web
- 日付: 2026-07-30 更新
- リンク: https://github.com/GianL22/DomainDL-ai
- 要約: FastAPI、MongoDB、LangGraph、LangSmithを使い、DDDコード生成とプロジェクト知識Q&Aを行うマルチエージェントサービス。Orchestrator agentが bounded context を分解し、Value Objects、Entities、Aggregates、Domain Events、Domain Services、Domain Exceptions などの抽象単位ごとの coding sub-agents に委譲する。
- なぜ面白いか:
  - 技術: DDDの戦術パターンをエージェント分業の単位にしており、集約やドメインイベントを単なるコード部品ではなく生成プロセスの境界として使っている。
  - 人文: ソフトウェア設計の言葉がそのままエージェント組織の役割分担になる点が象徴的である。人間のチーム構造、ドメインモデル、AIエージェントの分業が互いに写像し合うため、DDDは組織文化の設計言語としてさらに重要になる。

## arXiv / 学術

- 見つかったもの: `2608.05612`「Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design」（2026-08-06）。戦術的DDDのモデル/コード同期とAIコードアシスタント向けコンテキスト層を扱う。
- 見つかったもの: `2607.28307`「From Textual Requirements to Microservice Architectures - A Comprehensive Evaluation of LLM-Based Design Synthesis」（2026-07-30）。自然言語要件からマイクロサービス設計をLLMで合成・評価する。
- 関連する古めのもの: `2607.06471`「Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem」（2026-07-07、14日窓より古いが関連性が高い）。GitHub上のDDD実践を大規模に特徴づける。

## メモ

- Boris Cherny優先の有無: DDD単独トピックのため必須ではない。Claude/agent接続ではClaudeを用いたEvent Storming共同モデレーション事例を優先して確認した。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールはクレジット/サブスクリプション制限で失敗したため、X由来の個別投稿は採用していない。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、代替としてGitHub API、OpenAlex、arXivリンク、Qiita API、Hacker News Algolia、Bing RSSへの直接HTTPアクセスを使った。Bing RSSは「domain」を一般ドメイン名として解釈するノイズが多く、採用しなかった。GitHub項目はスター数が少ない実験的リポジトリを含むため、成熟度ではなく「DDD×AI/agent時代の設計」という観点で選定した。

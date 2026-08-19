# DDD トレンド調査 (2026-08-19)

- 調査日: 2026-08-19
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは、コード生成よりも「ドメイン語彙・境界・意思決定の根拠」を機械可読にして、人間とエージェントの共同作業を壊れにくくする方向へ寄っています。

## トップ5

### 1. Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark
- 出典: arXiv
- 日付: 2026-08-15
- リンク: https://arxiv.org/abs/2608.15255
- 要約: 自動ドメインモデリングの比較評価に標準ベンチマークが不足している問題を扱い、Golden UML Modelset と Text2UML 系の資産を組み合わせた評価基盤を提案しています。LLMで「それっぽいモデル」を作る段階から、モデル品質を測る段階へ進む兆しとして重要です。
- なぜ面白いか:
  - 技術: DDDのドメインモデル抽出をLLM任せの主観評価から、再現可能なベンチマーク評価へ移す足場になります。
  - 人文: ドメインモデルは組織の世界理解を写すものなので、評価基準を公開することは「誰の語彙・分類・境界が正当化されるのか」を問う文化的な行為でもあります。

### 2. DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python
- 出典: GitHub / IEEE DOI付き研究プロトタイプ
- 日付: 2026-08-13 更新
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: SRS（要求仕様書）から型付きドメインモデルを作り、Pythonコードのアーキテクチャ逸脱をVS Code上で検出する、AI支援DDD適合性チェックのプロトタイプです。READMEではAST解析とマルチエージェントLLM推論、出典へのトレーサビリティが強調されています。
- なぜ面白いか:
  - 技術: DDDを設計時の会話で終わらせず、実装のドリフト検知と要求への根拠リンクに接続している点が実務的です。
  - 人文: 「アーキテクチャ違反」を誰が判断するのかという権力関係を、LLM・仕様書・開発者の三者で再編します。うまく使えば新人の学習支援になりますが、雑に使うと設計警察を自動化する危険もあります。

### 3. LLM_Ontology_DDD: Hybrid LLM–Ontology Approach for Ubiquitous Language
- 出典: GitHub
- 日付: 2026-08-12 作成・更新
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: 「A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts in Domain-Driven Design」と題した、ユビキタス言語構築と意味衝突解消をLLMとオントロジーで支援するリポジトリです。実装・説明はまだ薄いものの、テーマ設定がDDDの中核に直撃しています。
- なぜ面白いか:
  - 技術: LLMの柔軟な言語処理と、オントロジーの明示的な概念関係を組み合わせ、ユビキタス言語を単なる用語集から検証可能な知識構造へ拡張しようとしています。
  - 人文: ユビキタス言語はチームの合意形成そのものなので、意味衝突の検出は単なる自然言語処理ではなく、専門家・開発者・利用者の解釈のズレを可視化する社会的プロセスです。

### 4. Archally Blueprint Schema: domain-first YAML schema for system cartography
- 出典: GitHub / npm関連プロジェクト
- 日付: 2026-08-11 更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: ドメイン設計、意思決定記録、ビジネスルール、ガバナンス、アーキテクチャを1つのYAMLスキーマで表し、OpenAPI・AsyncAPI・BPMN・UML・PRD・Event Stormingボード・MCP経由のAIエージェント grounding へ展開する構想です。READMEは、断片化した設計知識を「System Cartography」として統合する問題意識を掲げています。
- なぜ面白いか:
  - 技術: DDDの境界づけ・業務ルール・イベントストーミング成果を、AIエージェントが参照できる単一の機械可読ソースに寄せる試みです。
  - 人文: 組織の「部族的記憶」をスキーマ化することは、属人化を減らす一方で、暗黙知や現場の例外をどこまで形式化してよいのかという緊張も生みます。

### 5. Automating Domain-Driven Design: Experience with a Prompting Framework
- 出典: arXiv
- 日付: 2026-03-27（古いが関連性が高いため掲載）
- リンク: https://arxiv.org/abs/2603.26244
- 要約: DDDを、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの特定、集約設計、技術アーキテクチャへのマッピングという5段階に分解し、構造化プロンプトでLLMに支援させる経験報告です。AI時代のDDD実践を一連のワークフローとして定義している点で、現在の議論の参照点になります。
- なぜ面白いか:
  - 技術: イベントストーミングからアーキテクチャ設計までをプロンプト連鎖として扱い、LLM支援DDDの標準的な作業分解を提示しています。
  - 人文: DDDのワークショップ的な対話をシミュレーション可能にする一方で、場の空気、利害対立、専門家の沈黙といった人間的要素をモデルがどこまで拾えるかが問われます。

## arXiv / 学術
- Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark — arXiv:2608.15255（2026-08-15）。自動ドメインモデリング評価の標準化。
- Automating Domain-Driven Design: Experience with a Prompting Framework — arXiv:2603.26244（2026-03-27、古いが関連性高）。ユビキタス言語、イベントストーミング、境界づけ、集約設計、技術設計をLLMプロンプトで支援。

## メモ
- X検索は英語・日本語で実行しましたが、xAI側の spending-limit エラーにより結果取得できませんでした。今回のトップ5は、GitHub API、arXiv Web検索、直接HTTP取得で確認できた公開リンクに限定しています。
- Web検索ツールも Firecrawl 未設定で利用不可でした。代替として、GitHub Search API、arXiv検索ページ、InfoQ/Martin Fowler/EventStorming等の直接HTTP確認を行いました。
- 日本語アカウントはX検索障害のため確認できませんでした。
- 注意点: GitHubリポジトリはスター数が少ない研究・試作段階のものを含みます。流行の大きさではなく、DDD×LLM/agent×組織知という観点での面白さを優先しました。架空リンク・未確認arXiv IDは含めていません。

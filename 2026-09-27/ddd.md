# DDD トレンド調査 (2026-09-27)

- 調査日: 2026-09-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは「コード生成の前処理」ではなく、エージェントに渡す文脈・制約・会話の境界を設計する社会技術へ寄っている。

## トップ5

### 1. Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems
- 出典: arXiv
- 日付: 2026-09-23
- リンク: http://arxiv.org/abs/2609.27354v1
- 要約: 生成AIシステムを特定ドメインで安全・適切に動かすには、単に知識をRAGで足すだけでなく、技術・規制・制度・規範の制約を「ドメインインターフェース」として設計する必要がある、という提案。DDDそのものの論文ではないが、AIシステムの文脈設計を制約駆動で捉える点が、境界づけられたコンテキストやユビキタス言語の現代的拡張として読める。
- なぜ面白いか:
  - 技術: LLM/agentの「コンテキスト」を検索結果の束ではなく、制約・責務・許容行動を含むインターフェースとして設計する視点が、AIプロダクトの境界設計に直結する。
  - 人文: 組織がAIに何をさせ、何をさせないかを明示する作業は、規範や責任の翻訳でもある。DDDの会話中心主義が、AIガバナンスの言語づくりと接続し始めている。

### 2. Archally Blueprint Schema
- 出典: GitHub / Web
- 日付: 2026-09-26更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: ドメイン設計、意思決定記録、ビジネスルール、ガバナンス、アーキテクチャをYAMLで一つの機械可読モデルにまとめ、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Stormingボード、MCP経由のAIエージェント grounding へ展開する構想。READMEは「断片化した真実」を問題としており、DDDのモデルをドキュメントではなく生成・検証・会話の基盤に置いている。
- なぜ面白いか:
  - 技術: DDD成果物を構造化スキーマ化し、API仕様やAIエージェントの文脈に接続することで、設計と実装・運用の往復可能性を高める。
  - 人文: 「部族的記憶」や散らばったConfluenceを一つの地図に戻す発想は、組織文化の記憶術でもある。誰がドメイン知識にアクセスできるかという権力配置も変わる。

### 3. Agent Skills: DDD playbook for coding agents
- 出典: GitHub / Web
- 日付: 2026-09-18更新
- リンク: https://github.com/salimramirez/agent-skills
- 要約: AI coding agent向けのポータブルな「Agent Skills」集で、最初の主題としてDDDを扱う。`ddd-playbook`はユビキタス言語、サブドメイン、境界づけられたコンテキスト、コンテキストマップ、EventStorming、集約、ドメインイベントなどを、Claude Code、Cursor、GitHub Copilotのようなエージェントに段階的に読ませる形で整理している。
- なぜ面白いか:
  - 技術: DDDを人間向け方法論から、エージェントが必要時に参照する実行可能な手順・判断規則へ落とし込んでいる。
  - 人文: 「熟練者の設計勘」をスキルファイルとして外在化する試みは、チームの教育や継承の形を変える。一方で、会話の余白まで手順化してしまう危うさもある。

### 4. tightstorm: AI-facilitated Event Storming workshops
- 出典: GitHub / Web
- 日付: 2026-09-16作成
- リンク: https://github.com/pinion05/tightstorm
- 要約: 「決済できるようにして」「通知を入れて」といった抽象的な指示を、AIファシリテータ付きのEvent Stormingで、ドメインイベント、コマンド、ポリシー、アクター、境界づけられたコンテキストを含む仕様へ変換する韓国語READMEのpre-alphaプロジェクト。ホットスポットを残して推測で埋めないことを、AIのもっともらしい捏造への対抗策としている。
- なぜ面白いか:
  - 技術: 要求の一文入力から、段階ゲート式の質問でイベントストーム文書とJSON Canvasを生成する流れは、LLMを要件定義の聞き手として使う実践例になる。
  - 人文: ここでのAIは「答える機械」ではなく「質問する司会者」であり、組織内の曖昧な指示文化を可視化する。ホットスポットを残す設計は、知らないことを知らないまま共有する倫理でもある。

### 5. Domain Modeling Meets Generative AI
- 出典: GitHub / Web
- 日付: 2026-09-16更新（研究・資料は継続中）
- リンク: https://github.com/mardenneubert/ddd-meets-genai
- 要約: Event Stormingで得られる付箋・会話・文脈を、LLMエージェントが構造化されたドメインモデルへ変換する研究リポジトリ。READMEは、DDDの知識がホワイトボードや人々の頭の中に残り、境界づけられたコンテキスト、集約、エンティティ、値オブジェクト、コンテキストマップへ手作業で翻訳される「知識ボトルネック」を問題にしている。
- なぜ面白いか:
  - 技術: Event Stormingから検証可能なモデルへ流すspec-driven pipelineは、LLMをモデリング支援に使う際の入力・中間表現・評価の焦点を明確にする。
  - 人文: ワークショップで生まれた集合知を機械可読化することは、参加者の声を保存することでもある。反面、白板上のニュアンスがスキーマに圧縮されるとき、何が失われるのかを問う必要がある。

## arXiv / 学術
- Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems — 2609.27354v1。2026-09-23公開で、AIシステムのドメイン適合性を制約駆動で設計する内容。
- Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark — 2608.15255v1。2026-08-15公開（直近14日より古いが関連）。自然言語記述からドメインモデルを生成する手法評価のためのベンチマークを提案。
- Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design — 2608.05612v1。2026-08-06公開（直近14日より古いが関連）。Javaコードと戦術的DDDモデルを双方向同期するJDomInOを提案。
- Automating Domain-Driven Design: Experience with a Prompting Framework — 2603.26244v1。2026-03-27公開（古いが関連）。ユビキタス言語、Event Storming、境界づけられたコンテキスト、集約、技術アーキテクチャをLLMプロンプトで支援する経験報告。

## メモ
- Boris Cherny優先の有無: DDD単独トピックでClaude固有論点ではないため、Boris Cherny優先は適用しませんでした。
- 日本語アカウントの扱い: 日本語X検索を実行しましたが、X検索ツールがクレジット上限で失敗したため、X由来の項目は採用していません。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、代替としてarXiv API、GitHub API、Google News RSS、HN Algoliaを実行しました。トップ5のうちGitHub項目は研究論文や広く検証済みのニュースではなく、公開リポジトリのREADME・更新日時に基づく観測です。採用時は「プロジェクトの動き」として読み、成熟度や実運用品質は別途確認が必要です。

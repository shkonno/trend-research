# DDD トレンド調査 (2026-08-23)

- 調査日: 2026-08-23
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

DDDは「実装パターン」から、AIエージェントに渡せる共有地図・合意形成プロトコルへ移りつつあります。

## トップ5

### 1. Turn a Codebase into a Domain Model Your PM and QA Can Read
- 出典: DEV Community 記事
- 日付: 2026-08-18
- リンク: https://dev.to/mroops/turn-a-codebase-into-a-domain-model-your-pm-and-qa-can-read-16d
- 要約: BraidというOSSフレームワークを紹介する記事で、コードベースからDDD形式のドメインモデルを抽出し、PM・QA・エンジニアが同じ言葉でレビューできる状態にするという提案です。AIは変更案を作るが、人間が承認し、不明点は推測せず質問するというHuman-in-the-loop設計が中心に置かれています。
- なぜ面白いか:
  - 技術: コード、PRD、設計文書、Slack的な暗黙知のズレを、bounded context・aggregate・command・ruleなどの型付きモデルとして同期しようとしている点がDDDとLLMの接点として実践的です。
  - 人文: 「ドメインモデルは抽出ではなく合意である」という立場がよいです。AI時代のユビキタス言語は、機械が自動生成する用語集ではなく、関係者が責任を持って承認する社会的契約に近づいています。

### 2. DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python
- 出典: GitHub リポジトリ / IEEE Xplore掲載論文へのリンク付きREADME
- 日付: 2026-08-13 更新（論文自体はIISEC 2026）
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: SRS（Software Requirements Specification）から型付きDDDモデルを作り、PythonコードのアーキテクチャドリフトをVS Code診断として検出するツールです。READMEでは、PDF/DOCX/TXTの要件文書、マルチステージLLMオーケストレーション、AST解析、import topology、RAGによるトレーサビリティを組み合わせると説明されています。
- なぜ面白いか:
  - 技術: LLMの曖昧な設計レビューを、AST解析やimport構造チェックなどの決定的検証と組み合わせ、ドメインモデルへの準拠性をIDE上の診断へ落としている点が強いです。
  - 人文: DDDの「言葉と設計を一致させる」という理想が、開発者の良心やレビュー文化だけでなく、日常のエディタ体験へ埋め込まれようとしています。一方で、要件文書を正典として扱いすぎると、現場で更新されない組織の物語を固定化するリスクもあります。

### 3. ProcessFlow Architect: ローカルAIで動くEvent Stormingスタジオ
- 出典: GitHub リポジトリ
- 日付: 2026-08-21 更新
- リンク: https://github.com/raalzate/processflow-architect
- 要約: Event Storming、DDD、BPMN、C4、UMLを扱うデスクトップアプリで、LiteRT-LM / WebGPUによるローカルReActエージェントを備えています。READMEでは、Big Pictureのキャンバス、集約・ポリシー・read model・外部システム、MCPブリッジ、Mermaid/Markdown/PDF出力などが説明されています。
- なぜ面白いか:
  - 技術: Event Stormingの付箋作業を、ローカルLLM、複数ビュー、MCP、エクスポート可能な設計成果物へ接続しており、ワークショップからアーキテクチャ文書までの連続性があります。
  - 人文: オフライン・ローカルファーストを打ち出している点は、ドメイン知識がしばしば機密・文化・政治を含むことへの応答です。クラウドAIに業務の核心を渡さず、チームの会話空間を守る設計思想として読めます。

### 4. 承認ルートは申請の中に置くべきか、外に出すべきか。Goで多段承認を作りながら集約の境界を引く
- 出典: Qiita 記事
- 日付: 2026-08-21
- リンク: https://qiita.com/shinchi-pmtech/items/59a665b68909ca55b87c
- 要約: GoとDDDの学習連載として、多段承認を題材に「承認ルートの定義」と「承認の進捗」を分け、どこをApplication集約の内側に置くべきかを実装しながら検討しています。進行中の申請が組織マスタ変更に振り回されないよう、申請作成時に承認ステップを写し取る判断が説明されています。
- なぜ面白いか:
  - 技術: 集約を「一緒に守る不変条件の囲い」として説明し、承認順序・二重承認禁止・組織変更の影響範囲をコードの境界に翻訳している点が実務的です。
  - 人文: 稟議や承認は単なる状態遷移ではなく、組織の権限・記憶・責任の表現です。DDDの境界設計が、会社という制度の時間感覚をどう保存するかという問題に直結していることがよく見えます。

### 5. Archally Blueprint Schema: domain-first YAML schema for system cartography
- 出典: GitHub リポジトリ
- 日付: 2026-08-20 更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: ドメイン設計、意思決定記録、ビジネスルール、ガバナンス、組織的整合をYAMLの単一モデルとして表現し、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Stormingボード、MCP経由のAIエージェント grounding につなげるスキーマです。READMEは「System Cartography」という比喩で、設計面・統治面・証拠チェーン・未回答質問を同じ地図に載せると説明しています。
- なぜ面白いか:
  - 技術: DDD的なbounded contextやbusiness ruleを、API仕様・意思決定・イベントストーミング・エージェント文脈へ変換可能な機械可読メタモデルとして扱っている点が新しいです。
  - 人文: 「地図」という比喩は、設計が現実そのものではなく、目的を持った表象であることを思い出させます。未回答質問をモデル内に残す設計は、AIに全知のふりをさせず、組織がまだ知らないことを可視化する倫理的な態度です。

## arXiv / 学術

- 本調査時点で確認されませんでした。

## メモ

- X検索は英語・日本語とも実行しましたが、xAI/X Search側でクレジット上限エラー（spending-limit）が返り、投稿内容を取得できませんでした。そのため本日のDDD調査はWeb/API（DEV、Qiita、GitHub）中心です。
- Web検索ツールはFirecrawl未設定エラーで利用できなかったため、公開APIと直接HTTP取得で代替しました。
- arXiv APIは429 Too Many Requests / timeout が返り、関連arXiv IDを確認できませんでした。架空IDを避けるため、本稿では「確認されませんでした」と記載します。
- 日本語情報源としてQiitaを確認し、DDDの実装・書評記事を比較したうえで、多段承認の集約境界記事をトップ5に採用しました。
- Claude系トピックではないため、Boris Cherny優先は適用していません。
- 誇張リスク: GitHubリポジトリは更新日が新しくても、研究・実装の成熟度はプロジェクトごとに差があります。本稿ではREADME/APIで確認できた範囲に限定して要約しました。

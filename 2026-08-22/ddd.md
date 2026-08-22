# DDD トレンド調査 (2026-08-22)

- 調査日: 2026-08-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは、単なる設計手法から「エージェントに組織の言葉・境界・判断基準を渡すための運用インターフェース」へ寄っている。

## トップ5

### 1. DDD-Enforcer: SRSからDDDモデルを抽出し、VS Code上で設計逸脱を検出
- 出典: GitHub / IEEE DOIリンク付きプロジェクト
- 日付: 2026-08-13 更新
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: 要求仕様書（PDF/DOCX/TXT）から型付きDDDモデルを作り、PythonコードをAST解析・インポート構造チェック・RAGトレーサビリティで検査するツール。READMEでは「AI-powered multi-agent system」として、VS Code診断・提案・SRS参照までをつなぐ構成が説明されている。
- なぜ面白いか:
  - 技術: LLMを「設計生成」だけでなく、要求・ドメインモデル・コード実装の対応関係を継続監査する仕組みに置いている点が、DDDの実装ガードレールとして具体的です。
  - 人文: ユビキタス言語を人間の合意文書に閉じず、IDE上の診断として日常作業へ戻す発想が面白いです。組織で忘れられがちな「なぜこの境界なのか」を、後から参加した開発者やAIエージェントにも説明可能にする文化装置として読めます。

### 2. LLM_Ontology_DDD: ユビキタス言語と意味衝突をLLM＋オントロジーで扱う試み
- 出典: GitHub
- 日付: 2026-08-12 作成・更新
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: 「A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts in Domain-Driven Design」と題したリポジトリ。READMEは短いが、DDDにおけるユビキタス言語の構築と意味衝突の解消を、LLMと形式的な知識表現のハイブリッドで扱う方向性が明示されている。
- なぜ面白いか:
  - 技術: LLMの柔軟な言語処理とオントロジーの明示的な概念関係を組み合わせ、ドメイン語彙の曖昧さを設計資産として検査可能にしようとしている点が重要です。
  - 人文: DDDの核心である「同じ言葉で話しているつもり問題」を、単なる命名規約ではなく意味交渉の問題として扱っています。これは、部署・専門職・文化が異なる人々の間で、言葉の権力関係や誤解をどう可視化するかという組織文化のテーマにもつながります。

### 3. dca-marketplace: Claude CodeにDDD/Hexagonal Architectureのスキルとレビューエージェントを配布
- 出典: GitHub / Claude Code plugin marketplace
- 日付: 2026-08-21 更新
- リンク: https://github.com/chbloemer/dca-marketplace
- 要約: Domain-Centric Architecture（DDD＋Hexagonal Architecture）をClaude Codeのプラグインとして配布するマーケットプレイス。`/ubiquitous-language`、`/context-map`、`/dca-bootstrap`、`ddd-expert`、`ddd-reviewer`、`hexagonal-reviewer`などのスキル/エージェントと、約740件の知識カタログを同梱すると説明している。
- なぜ面白いか:
  - 技術: DDDを単発プロンプトではなく、スキル、エージェント、ArchUnitルール、ADR、レシピ、チェックリストのパッケージとして配布することで、AI開発環境に設計規律をインストール可能にしています。
  - 人文: 「設計文化」を個人の熟練に依存させず、チームの作業環境に埋め込む動きとして見られます。一方で、組織固有の言葉や判断を既製プラグインに寄せすぎると、DDDが本来重視する現場固有性を薄めるリスクもあります。

### 4. agentic-skills-for-quarkus: QuarkusアプリにDDD/ヘキサゴナル構造を足すエージェント用スキル
- 出典: GitHub
- 日付: 2026-08-18 更新
- リンク: https://github.com/jeremyrdavis/agentic-skills-for-quarkus
- 要約: GitHub CopilotやClaude Code向けに、QuarkusアプリのブートストラップとDDD/Hexagonal Architectureのスキャフォールディングを支援するスキル集。`quarkus-ddd`は bounded context、subdomain、aggregate、value object、command、domain event、application service、REST/DTO、repository、ports/adapters 構造を扱う。
- なぜ面白いか:
  - 技術: フレームワーク固有の実装パターンとDDDの戦術パターンをエージェント指示セットに落とし込み、自然言語から一貫した構造を生成しやすくしています。
  - 人文: AIコーディングでは「速く作る」ほど設計上の負債も速く増えますが、この種のスキルは速度と規律を同時に持ち込む試みです。新人・非専門家・AIが同じ境界語彙を参照できることは、チーム内の教育や合意形成にも効きます。

### 5. faceto: typed fileからイベントストーミングの視覚ボードを作り、LLMと考える
- 出典: GitHub / ドキュメント付きプロジェクト
- 日付: 2026-08-11 プッシュ（2026-08-07 更新、直近14日からは1日だけ古いが関連性が高いため採用）
- リンク: https://github.com/bastien-gallay/faceto
- 要約: typed fileを入力に、イベントストーミング用のHTML+SVGボードを生成し、各要素にメモを書いて次のLLMセッションでモデルを調整できるツール。READMEでは、actor、command、aggregate、event、policy、read-model、hotspotなどのレーンに加え、今後 context map や bounded context canvas、core domain chart へ広げる方向が示されている。
- なぜ面白いか:
  - 技術: イベントストーミングをLLMとの対話ログだけに閉じず、型付きソースと視覚ボードの往復にすることで、モデルの変化をレビューしやすくしています。
  - 人文: ワークショップの価値は付箋そのものではなく、人々が同じ物語を見ながら衝突点を発見することにあります。facetoは、その「場」を非同期・ローカル・エージェント支援型に再構成しようとしている点で、リモート組織の設計文化に響きます。

## arXiv / 学術
- 本調査時点で確認されませんでした。arXiv APIは本実行時にHTTP 429を返したため、OpenAlex等の代替検索も確認しましたが、DDD / event storming / ubiquitous language とAI/LLM/agentを直接結ぶ直近arXiv項目は確認できませんでした。

## メモ
- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索を実行しましたが、X検索ツールがクレジット/購読制限で失敗したため、X由来の個別投稿は採用していません。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）が未設定で失敗したため、GitHub APIと直接HTTP取得を主なWeb代替ソースにしました。GitHubリポジトリの更新日は活発さの目安であり、実利用・品質・学術的妥当性を保証するものではありません。リンクは保存前にHTTP 200で到達確認済みです。

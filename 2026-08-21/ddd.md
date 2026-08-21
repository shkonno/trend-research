# DDD トレンド調査 (2026-08-21)

- 調査日: 2026-08-21
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

DDDは「設計手法」から、AIエージェントに渡す組織知・語彙・境界を機械可読に保つための運用基盤へ寄っている。

## トップ5

### 1. Archally Blueprint Schema v2.7.9: bounded context と MCP 時代の「システム地図」

- 出典: GitHub リポジトリ / README / コミット
- 日付: 2026-08-20（v2.7.9 コミット、リポジトリ更新）
- リンク: https://github.com/Archally/blueprint-schema
- 要約: Archally Blueprint Schema は、ドメイン設計、ビジネスルール、意思決定記録、ガバナンス、アーキテクチャを単一のYAMLモデルに集約し、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Stormingボードなどを生成することを狙うスキーマ。READMEでは、AIエージェントがMCP経由で検証済みの構造化ドメイン文脈を読む、という使い方が明確に打ち出されている。
- なぜ面白いか:
  - 技術: bounded context、typed ID、cross-layer validation、Event Storming成果物、MCPを一つの機械可読モデルでつなぎ、RAG的な文書検索ではなく検証済みグラフとしてドメイン知を渡そうとしている。
  - 人文: 「ドキュメント不足」ではなく「断片化した真実」が問題だ、という問題設定がよい。DDDをチームの記憶、オンボーディング、意思決定の地図作りとして捉え直しており、組織文化とAI利用の接点が濃い。

### 2. DDD-Enforcer: 要件書からドメインモデルを作り、Pythonコードのドメイン逸脱をVS Codeで検出

- 出典: GitHub リポジトリ / README / DOI
- 日付: 2026-08-13（README公開・更新コミット。研究発表自体はIISEC 2026）
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: DDD-Enforcerは、PDF/DOCX/TXTのソフトウェア要求仕様書から構造化DDDモデルを作り、Python AST解析、import topology検査、RAGによる要件トレース、必要に応じたLLM解析を組み合わせて、コードがドメインモデルから逸脱していないかをVS Code診断として返すプロジェクト。IEEE Xplore掲載論文へのDOIもREADMEから確認できる。
- なぜ面白いか:
  - 技術: LLMに全判断を委ねず、typed artifacts、AST、決定的検証、RAG参照を組み合わせて「ユビキタス言語からのドリフト」を開発時に検出する設計になっている。
  - 人文: DDDの失敗は一つの大事故ではなく、名前のズレ、汎用的すぎる抽象、責務の移動が少しずつ積もるところにある、という観察が実務的。AIを「設計者の代替」ではなく、チームが合意した言葉を忘れない監査役として置く発想が面白い。

### 3. LLM_Ontology_DDD: ユビキタス言語と意味衝突を LLM + オントロジーで扱う小さな実験

- 出典: GitHub リポジトリ / README / コミット
- 日付: 2026-08-12（初期公開・更新）
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: 「A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts in Domain-Driven Design」と題した実験的リポジトリ。READMEは短いが、コアテーマは、LLMだけで用語を生成するのではなく、オントロジーで意味関係を明示しながらユビキタス言語を組み立て、意味衝突を解くことにある。
- なぜ面白いか:
  - 技術: DDDのユビキタス言語を、自然言語プロンプトではなく、LLMとオントロジーのハイブリッドな意味モデルとして扱う方向性を示している。
  - 人文: ユビキタス言語は単なる用語集ではなく、部署、専門職、歴史的慣習のあいだの翻訳装置でもある。意味衝突を「曖昧だから消す」のではなく、対話すべき差異として可視化する余地がある。

### 4. Agent Skills: DDD・Event Storming・PRD駆動DDDをAIエージェントのスキルとして配布

- 出典: GitHub リポジトリ / README / SKILLS-MAP
- 日付: 2026-08-16（README再構成、87スキル同期）
- リンク: https://github.com/NinjaSln-labs/agent-skills
- 要約: Agent Skillsは、Claude Code、Cursor、Copilot CLIなどのAIコーディングエージェントにインストールできるSKILL.md群を集めたリポジトリ。87スキルの中に、aggregate、bounded context、context map、domain discovery、domain model review、event storming、PRD-driven DDDなど13個のDDD系スキルが含まれる。
- なぜ面白いか:
  - 技術: DDDを一枚の設計ドキュメントではなく、エージェントが必要時に呼び出す小さな手続き知・レビュー知・ゲート知として分解している。
  - 人文: これは「AIにDDDを教える」だけでなく、チームがどんな順番で発見し、議論し、検証し、合意するかを外部化する試みでもある。イベントストーミングのような協働的実践を、エージェント時代にどう損なわず再配置するかという問いが見える。

### 5. System F Software Constitution: AIエージェントに常駐・取得型の設計規範を読ませる

- 出典: GitHub リポジトリ / README / CONSTITUTION.md / CONSTITUTION-ARTICLES.md
- 日付: 2026-08-20（resident law と retrieved articles への分割を含む更新）
- リンク: https://github.com/systemfsoftware/constitution
- 要約: System F Software Constitutionは、functional core / imperative shell、domain types before logic、property testsなどの設計原則を、リポジトリにvendoringしてAIコーディングエージェントに適用させる「工学憲法」。2026-08-20の更新では、常に読ませる憲法本文と、ソース編集時に取得する記事群を分ける設計が入っている。
- なぜ面白いか:
  - 技術: DDDそのもののツールではないが、domain decisionを純粋関数として扱い、domain types before logicをゲート化するなど、AIがコードを書く前提でDDD/clean architectureの境界を守らせる仕組みになっている。
  - 人文: 「憲法」というメタファーは、設計を個人の好みではなく共同体の規範として扱う。AIエージェントが増えるほど、組織は暗黙の美学や禁忌を機械に読める形にしなければならず、これは文化の明文化そのものでもある。

## arXiv / 学術

- 本調査時点で確認されませんでした。
- 補足: arXiv APIには `Domain-Driven Design`、`event storming`、`ubiquitous language`、`LLM`、`agent` 関連で複数回問い合わせましたが、HTTP 429 / timeout が発生しました。確認できた学術リンクとしては、arXivではなく DDD-Enforcer README記載の IEEE Xplore / DOI（https://doi.org/10.1109/IISEC69317.2026.11418529）があります。

## メモ

- X検索: 英語・日本語クエリで実行しましたが、x_search が `personal-team-blocked:spending-limit` により失敗しました。そのため本ファイルのトップ5は、GitHub API、raw README、コミット履歴、DOI到達確認に基づくWeb側の実確認を中心に選定しています。
- Web検索: Hermesのweb_search / web_extract は Firecrawl 未設定で失敗しました。代替として `terminal` からGitHub API、raw.githubusercontent.com、doi.org、ieeexplore.ieee.orgに直接アクセスして確認しました。Bing HTML検索も試しましたが、関連性の低い結果が多く採用しませんでした。
- 日本語アカウントの扱い: 日本語X検索は実行したものの、上記のXツール制限により投稿内容は確認できませんでした。日本語Web検索も自動検索結果の品質が低く、架空リンク防止のため採用していません。
- 注意点・誇張リスク: GitHubリポジトリは更新日が新しくても、実利用・コミュニティ評価・保守継続性は未確定です。特に星数が少ないものは「広く流行している」ではなく、「DDD×AI/agent時代の設計パターンとして面白い初期シグナル」として扱うべきです。

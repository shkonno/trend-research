# DDD トレンド調査 (2026-08-18)

- 調査日: 2026-08-18
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは「きれいな層構造」よりも、エージェントが迷わない言語・境界・検証可能な仕様をどう作るかに重心が移っている。

## トップ5

### 1. Agentic Domain-Driven Mainframe Modernization / Project Rosetta
- 出典: GitHubリポジトリ / パターンカタログ
- 日付: 2026-08-17更新（リポジトリ作成は2026-05-12）
- リンク: https://github.com/pmilet/ai-ddd-mainframe-modernization-patterns
- 要約: COBOL/CICSのメインフレーム近代化を「コード変換」ではなく「埋もれた業務意味の回復」と捉え、DDDとAIエージェントを組み合わせた28個のパターンカタログとして整理している。READMEは、エージェントを自律的な主役にするのではなく、ハーネス内で働かせる設計を強調している。
- なぜ面白いか:
  - 技術: レガシー移行をLLM翻訳問題ではなく、ドメイン知識抽出、境界づけ、パターン化、検証の問題として再定義している。
  - 人文: 長寿命システムに蓄積された「組織の記憶」をどう読み替えるかという、技術考古学に近いテーマがある。古いコードを単なる負債ではなく、過去の制約と判断の堆積として扱う点がDDDらしい。

### 2. DDD-Enforcer: AI-Powered Multi-Agent System for Real-Time DDD Enforcement
- 出典: GitHubリポジトリ / IEEE論文リンク付きプロジェクト
- 日付: 2026-08-13更新（IISEC 2026論文として公開）
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: SRS（ソフトウェア要求仕様）から型付きドメインモデルを作り、PythonコードをAST解析・importトポロジー・RAGトレーサビリティで検査し、VS Code診断としてDDD違反を返す。READMEにはIEEE XploreおよびDOI（10.1109/IISEC69317.2026.11418529）へのリンクが示されている。
- なぜ面白いか:
  - 技術: DDDの「アーキテクチャドリフト」を、LLMだけでなく決定的解析と型付き中間成果物で検査する方向に進めている。
  - 人文: 設計原則を人間のレビュー文化だけに依存させず、日々の開発環境に埋め込む試みである。これは「設計を守る人」の役割を、個人の職人芸からチームの共有インフラへ移す動きとして読める。

### 3. LLM_Ontology_DDD: Hybrid LLM–Ontology Approach for Ubiquitous Language
- 出典: GitHubリポジトリ
- 日付: 2026-08-12作成・更新
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: 「A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts in Domain-Driven Design」と説明されている、ユビキタス言語構築と意味衝突解消に焦点を当てたプロジェクト。内容はまだ短いが、LLMとオントロジーを組み合わせてDDDの言語面を支援する方向性が明確である。
- なぜ面白いか:
  - 技術: LLMの自然言語処理能力を、オントロジーによる明示的な概念関係・制約で補強し、語彙のぶれを検出する設計になり得る。
  - 人文: ユビキタス言語は単なる命名規則ではなく、部署・専門職・利害関係者の世界観の交渉である。AIがそこに入ると、誰の言葉が「正」として固定されるのかという文化的・政治的な問いが生まれる。

### 4. Domain-Driven AI
- 出典: GitHubリポジトリ / エッセイ・ノート集
- 日付: 2026-08-14更新（リポジトリ作成は2026-05-28）
- リンク: https://github.com/mikkoylen/domain-driven-ai
- 要約: AI支援開発時代におけるDDDの意味を、ブログ草稿、ノート、エージェント指示、実験として公開している。READMEは「AIはコード生成を速くするが、明確な言語、境界、所有、ドメイン理解の必要性をなくさない。むしろ重要にする」と位置づけている。
- なぜ面白いか:
  - 技術: bounded contextを「LLMに大量の文脈を渡す」のではなく「より良くスコープされた文脈を渡す」ための制約として捉え直している。
  - 人文: 実装が安くなるほど曖昧な思考が速く拡散する、という観察が鋭い。DDDを、AIに対抗する懐古的手法ではなく、人間とAIの共同作業における意味のガードレールとして再解釈している。

### 5. Archally Blueprint Schema
- 出典: GitHubリポジトリ / npmパッケージ
- 日付: 2026-08-11更新（リポジトリ作成は2026-05-25）
- リンク: https://github.com/Archally/blueprint-schema
- 要約: ドメイン設計、ビジネスルール、価値ストリーム、ガバナンス、アーキテクチャ判断をYAMLベースの単一モデルにまとめる「domain-first」なスキーマ。READMEでは、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Stormingボード生成や、MCPを通じたAIエージェントのグラウンディングが説明されている。
- なぜ面白いか:
  - 技術: DDD的な境界・ルール・証拠・未回答質問を機械可読な設計面として統合し、AIエージェントの参照可能な「地図」にしている。
  - 人文: READMEが用いる「System Cartography」という比喩が示す通り、設計は正解を一度描く作業ではなく、未知領域を明示しながら共同で地図を更新する営みになる。イベントストーミング的な会話の痕跡を、組織の記憶として残す方向性がある。

## arXiv / 学術
- 本調査時点で確認されませんでした。
- 補足: arXiv APIに対してDomain-Driven Design、event storming、ubiquitous language、AI/LLM/agentsを含む検索を実行したが、タイムアウトおよび429応答が発生したため、架空IDを補わず未確認扱いとした。関連学術情報としては、上記DDD-EnforcerのREADMEにIEEE Xplore / DOIリンクが明示されている。

## メモ
- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: X検索は英語・日本語の両方で実行したが、x_searchはクレジット/サブスクリプション制限で失敗した。代替としてGitHub API、dev.to API、Qiita API、Hacker News Algolia、直接README取得を使った。
- Web検索の注意点: web_searchはFirecrawl未設定で使用不可だったため、検索エンジン結果ではなく、公開APIと直接HTTP取得に基づいて選定した。
- 日本語圏の補助観測: Qiitaでは2026-08-14の「型契約書を SSoT にする — TDDD（型定義駆動開発）」、2026-08-15の「AIとドキュメントを2ヶ月書いたら、通じない言葉が24個混ざっていた」、2026-07-27の「AI導入の前に業務を見える化する～イベントストーミングを活用した軽量なビジネスプロセス可視化～」が関連していたが、今回のトップ5はDDD/AI/エージェント接続の強さを優先して選外にした。
- 誇張リスク: GitHubリポジトリは実験段階・小規模スターのものも含むため、成熟プロダクトとしてではなく、設計思想と探索方向のシグナルとして読むのが適切。

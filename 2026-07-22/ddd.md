# DDD トレンド調査 (2026-07-22)

- 調査日: 2026-07-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは「設計の自動化」よりも、ユビキタス言語・境界・組織知を人間とAIが共同で検証するための会話インフラとして面白くなっています。

## トップ5

### 1. Multiagent Microservice Architecture Generation from Textual Requirements
- 出典: Zenodo / OpenAlex（Web検索）
- 日付: 2026-07-09
- リンク: https://doi.org/10.5281/zenodo.21287466
- 要約: 自然言語の要求からマイクロサービス指向アーキテクチャを生成する、CrewAI・LangChain・Google Geminiベースのマルチエージェント実験リポジトリ。DDDアーキテクト役とイベント駆動アーキテクト役、検証エージェントを組み合わせ、Spring PetClinicとBookstoreで評価している点がDDD文脈に直結します。
- なぜ面白いか:
  - 技術: DDD担当エージェントとイベント駆動担当エージェントを分け、最後に validator が統合する構成は、bounded context 分割を「単一LLMの一発回答」から「設計レビューのプロセス」へ近づけています。
  - 人文: 組織の設計会議では、意見の対立や用語のズレが重要な発見になります。この実験は、その対立をAIエージェントの役割分担として再現できるかを問うており、設計文化そのものをモデル化する試みに見えます。

### 2. Educational Domain — Domain-Driven Design Manuscript
- 出典: GitHub / Zenodo / OpenAlex（Web検索）
- 日付: 2026-07-11
- リンク: https://github.com/Fosgiver/educational-domain-ddd
- 要約: 教育ドメインをDDD、システム分析、教育経験、人間とAIの協働から掘り下げた公開マニュスクリプト。READMEとOpenAlexメタデータでは、AIが構造化・問いかけ・一貫性確認・言語的洗練を支援し、人間側が教育・業務・組織運営の経験を提供したと説明されています。
- なぜ面白いか:
  - 技術: 生成AIをコード生成ではなく、ドメイン探索・概念整理・ユビキタス言語の編集支援に使う実例として読めます。
  - 人文: 教育という制度的・感情的に複雑な領域では、モデルは単なるデータ構造ではなく「誰が何を学び、誰が責任を負うのか」という価値判断を含みます。人間の経験とAIの整理能力を分業させる姿勢は、DDDの社会的側面をよく示しています。

### 3. ddd-toolkit: Domain-Driven Design building blocks for Rust
- 出典: GitHub（Web検索）
- 日付: 2026-07-19作成、2026-07-21更新
- リンク: https://github.com/ryoshrimp/ddd-toolkit
- 要約: Rust向けに entity、value object、aggregate、repository、event dispatch と derive macro をまとめたDDDビルディングブロック集。AI専用の成果物ではありませんが、AI生成コードが増えるほど、型・集約・境界を明示する小さな道具の価値は上がります。
- なぜ面白いか:
  - 技術: Rustの型システムでDDDの基本概念を表現することで、LLMが生成した実装にもコンパイル時の制約とドメイン語彙を埋め込みやすくなります。
  - 人文: DDDのユビキタス言語は会議室だけでなく、コードの型名や境界にも宿ります。AI時代の開発では、人間が守りたい言葉をツールキットとして固定することが、組織記憶の保全になります。

### 4. Automating Domain-Driven Design: Experience with a Prompting Framework
- 出典: arXiv
- 日付: 2026-03-27（古いが重要なため採用）
- リンク: https://arxiv.org/abs/2603.26244
- 要約: LLMとの構造化された対話で、ユビキタス言語の確立、イベントストーミングのシミュレーション、bounded context の識別、aggregate設計、技術アーキテクチャへの写像を順に支援するフレームワーク。論文は、初期段階では有用な成果物が出る一方、後段では小さな誤りが蓄積するため、完全自動化ではなく協働的な sparring partner として有効だと述べています。
- なぜ面白いか:
  - 技術: DDD活動を5段階に分解し、LLMの得意不得意を工程ごとに評価しているため、AI設計支援の現実的な境界線が見えます。
  - 人文: 「AIが設計者を置き換える」のではなく、専門家が重要なトレードオフに集中するための相手としてAIを位置づけています。これは設計を、成果物ではなく対話と判断の連鎖として捉えるDDDらしい見方です。

### 5. DDD/CQRSの第一人者 加藤潤一氏がカンリーの「AIフェロー」に就任
- 出典: Google News / PR TIMES（Web検索）
- 日付: 2026-06-30（直近14日より古いが、日本語圏DDDとAI組織文化の接続として採用）
- リンク: https://news.google.com/rss/articles/CBMiakFVX3lxTFBPN0NvWlcxR2hlMFlCbEpKRENsaWNtWWVONndMNGhLOGRvd3Nwc0Y4TmpEblhWa3d4Z3dBbEVYa0dvcVQyLXc5VEwyc3A0VUd3dThiSjRlb191VVV5R1Z4V21MVHdzZVRrYXc?oc=5
- 要約: DDD/CQRSで知られる加藤潤一氏が、店舗情報管理などを手がけるカンリーのAIフェローに就任したという日本語ニュース。技術記事ではなく人事・組織ニュースですが、DDDの専門性がAI導入の組織設計に組み込まれていく流れとして注目できます。
- なぜ面白いか:
  - 技術: AI活用を単なる機能追加ではなく、既存ドメイン・CQRS・業務イベントの理解と結びつける必要があることを示唆します。
  - 人文: AI導入で本当に難しいのはモデル選定よりも、現場の言葉・責任・判断の境界をどう再編するかです。DDD実践者がAIフェローになる動きは、AI時代の組織文化が「プロンプト」だけでなく「ドメイン理解」を中心に再設計される兆しとして読めます。

## arXiv / 学術
- Automating Domain-Driven Design: Experience with a Prompting Framework — arXiv:2603.26244。LLMでDDD活動を段階的に支援するフレームワークで、ユビキタス言語・イベントストーミング・bounded context・aggregate設計を対象にしています。
- Leveraging Generative AI for Enhancing Domain-Driven Software Design — arXiv:2601.20909。実世界DDDプロジェクトデータを使い、生成AIでドメイン固有JSON/メタモデル生成を部分自動化する研究です。
- 直近約14日内に新規のDDD×LLM/Agent関連arXiv論文は、本調査時点で確認されませんでした。

## メモ
- Boris Cherny優先: DDD単独トピックのため該当なし。
- 日本語アカウントの扱い: X検索ツールは実行しましたが、xAI側の credits / subscription 制限で失敗しました。そのため日本語圏の動きはGoogle News RSS経由のPR TIMES記事で補完しました。
- Web検索の注意: Hermesの web_search はFirecrawl未設定で利用不可だったため、Google News RSS、OpenAlex API、GitHub API、arXiv APIを端末から直接検索しました。
- 注意点・誇張リスク: GitHubリポジトリはスター数や採用実績が少ないものを含みます。特にZenodo/GitHub系の成果物は研究・試作として扱い、実運用での品質や再現性は別途検証が必要です。

# DDD トレンド調査 (2026-09-30)

- 調査日: 2026-09-30
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AI/LLM時代のDDDは、モデルを「人間同士の合意」から「人間・エージェント・検証器が共有する境界と語彙」へ拡張する局面にある。

## トップ5

### 1. Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems

- 出典: arXiv
- 日付: 2026-09-23
- リンク: http://arxiv.org/abs/2609.27354v1
- 要約: 生成AIをドメイン業務に適用する際、検索・記憶・ツール連携だけでなく、規制、制度、組織ルール、規範を「ドメインインターフェース」として設計する必要があると論じる論文。DDDそのものを扱う論文ではないが、境界づけられたコンテキストをAIシステムの振る舞い制約へ接続する議論として、今日の最重要候補にした。
- なぜ面白いか:
  - 技術: LLMの文脈設計をプロンプトやRAGの問題に閉じず、ドメイン制約を明示的な設計成果物として扱う方向を示している。
  - 人文: 「正しい応答」とは何かを、制度・責任・共同体の合意に結び直す点が重要である。ユビキタス言語は単なる用語集ではなく、AIが従うべき社会的な約束の表現になる。

### 2. DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python

- 出典: GitHub / IEEE Xplore linked project
- 日付: 2026-08-13 更新（直近14日外だが重要）
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: 要件文書から型付きドメインモデルを生成し、PythonコードのDDD適合性をVS Code診断として検出するプロジェクト。READMEでは、PDF/DOCX/TXTのSRSから構造化DDDモデルを作り、Python AST解析、import topology、RAGによるトレーサビリティ、マルチステージLLMオーケストレーションを組み合わせると説明している。
- なぜ面白いか:
  - 技術: DDDを「設計時の会話」だけでなく、コードベースのドリフトを検知する継続的な検証パイプラインへ変換している。
  - 人文: 要件、モデル、コードの関係を監査可能にすることで、暗黙の判断が個人の記憶やレビュー文化に閉じることを防げる。AIを設計者としてではなく、合意の逸脱を見つける相棒として使う姿勢が健全である。

### 3. When Code Gets Cheap, Verification Becomes Expensive: How AI changes the economics of software architecture

- 出典: DEV Community
- 日付: 2026-09-28
- リンク: https://dev.to/remojansen/when-code-gets-cheap-verification-becomes-expensive-how-ai-changes-the-economics-of-software-632
- 要約: AI coding agentsによって実装コストが下がる一方、検証・保守・運用・長期的な理解可能性のコストが相対的に重くなるという主張。AIが理解しやすい構造を選ぶことは、ユーザー価値を犠牲にすることではなく、信頼性、単純性、検証可能性を含むアーキテクチャ判断の一変数だと整理している。
- なぜ面白いか:
  - 技術: 境界、状態、制約を明示するDDD的な設計が、AIエージェントによる変更を検証可能にするための足場として再評価されている。
  - 人文: 「AIに都合のよい設計」は、人間を置き去りにする危険もあるが、説明責任を持てる構造を選ぶならむしろ組織の安全文化に寄与する。実装量ではなく検証可能性を価値の中心に置く転換が見える。

### 4. Implementation is where judgements go to become invisible

- 出典: DEV Community
- 日付: 2026-09-27
- リンク: https://dev.to/tom_jones_230c4659491adcd/implementation-is-where-judgements-go-to-become-invisible-4p1h
- 要約: 「誰が返事を待っているか」という一見単純な問いに対し、3つの実装がそれぞれ別の正しい答えを返した事例から、実装には判断が埋め込まれ、時間が経つと判断だったこと自体が見えなくなると論じる。DDD用語の記事ではないが、ユビキタス言語とドメインルールの可視化に直結する内容である。
- なぜ面白いか:
  - 技術: 「answered」「waiting」のような語の定義をコードの分岐に埋める前に、ドメイン概念として明示し、テストや仕様で検証できる形にする必要を示している。
  - 人文: 言葉の定義は中立ではなく、誰を待たせていると見なすかという関係性の判断を含む。AIが実装を高速化するほど、こうした小さな価値判断を会話の場へ戻すDDDの役割が大きくなる。

### 5. InvoiceService shouldn't exist

- 出典: DEV Community
- 日付: 2026-09-25
- リンク: https://dev.to/nicolasr_z/invoiceservice-shouldnt-exist-pie
- 要約: 請求書作成がHTTP API経由ではDTOで検証される一方、Kafka consumer経由では同じ必須項目チェックをすり抜け、最後はDB制約で落ちるという例を使い、ビジネスルールは汎用的な `InvoiceService` ではなく、それが守るドメインオブジェクトに置くべきだと説明している。AI/LLM記事ではないが、エージェントが複数入口の実装を増やす時代に重要なDDDの基本論点である。
- なぜ面白いか:
  - 技術: 入力経路ごとに散った検証を、集約や値オブジェクトの不変条件として一箇所に寄せる設計の必要性を具体例で示している。
  - 人文: 入口によってルールが変わる状態は、組織内で業務解釈が分裂している状態に似ている。DDDはコード整理術である前に、顧客・運用・開発が同じ約束で動くための言語実践でもある。

## arXiv / 学術

- 見つかりました: `2609.27354v1` Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems（2026-09-23）。DDDそのものではないが、AIシステムにおけるドメイン制約・制度的制約・規範的制約の設計を扱う直近重要候補。
- 関連するが直近14日外: `2608.15255v1` Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark（2026-08-15）。自動ドメインモデリング評価のベンチマーク提案。
- 関連するが直近14日外: `2608.05612v1` Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design（2026-08-06）。戦術的DDDのモデルとJavaコードを同期するJDomInOを提案。
- 関連するが古い: `2603.26244v1` Automating Domain-Driven Design: Experience with a Prompting Framework（2026-03-27）。ユビキタス言語、イベントストーミング、境界づけられたコンテキスト、集約設計をLLMプロンプトで支援する枠組み。

## メモ

- X検索: 英語・日本語で実施したが、xAI/X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、今回のX由来アイテムは採用できなかった。
- Web検索: Firecrawl系Web検索ツールが未設定で失敗したため、代替として端末から arXiv API、DEV Community API、Qiita API、GitHub API、Hacker News Algolia API、直接HTTP取得を実施した。
- 日本語アカウントの扱い: X検索不能のため日本語アカウント投稿は確認できなかった。日本語Web候補としてQiitaも検索したが、直近14日のDDD×AI/LLM×イベントストーミングの強い候補は少なく、トップ5は英語ソース中心とした。
- 注意点・誇張リスク: 直近14日にDDDそのものとAI/LLMを同時に扱う公開記事は少ないため、トップ5には「DDD直結」と「AI時代の設計・検証・言語化に強く接続する記事」を混在させた。古い候補は明記し、リンクはAPIまたは直接取得で確認できたもののみ使用した。

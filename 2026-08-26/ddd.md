# DDD トレンド調査 (2026-08-26)

- 調査日: 2026-08-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェント時代のDDDは、「設計思想」から「エージェントに渡せる検証可能な文脈・語彙・境界の基盤」へ寄っている。

## トップ5

### 1. Archally Blueprint Schema: DDD・ガバナンス・Event StormingをAIエージェント向けの単一YAMLモデルへ
- 出典: GitHub / Web
- 日付: 2026-08-25 作成・更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: Archally Blueprint Schemaは、bounded context、aggregate、command、event、business rule、decision record、risk、ownershipなどを単一の機械可読YAMLにまとめ、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Storming boardなどを生成できることを狙うプロジェクト。READMEでは、MCP経由でAIエージェントが検証済みの構造化ドメイン文脈を参照する設計が明示されている。
- なぜ面白いか:
  - 技術: DDDの戦略・戦術要素、イベント、ルール、意思決定、所有権をtyped IDとスキーマ検証で結び、LLMのRAGではなく「検証済みグラフ問い合わせ」に近い形でエージェントを接地している。
  - 人文: これは「設計ドキュメントを読むAI」から「組織の言葉・責任・未解決問いを地図として共有するAI」への移行を示す。DDDのユビキタス言語が、チーム内の合意だけでなく、人間とエージェントの共同作業における社会的契約になりつつある点が重要。

### 2. DDD-Enforcer: SRSからDDDモデルを生成し、VS Codeでアーキテクチャドリフトを検出
- 出典: GitHub / IEEE DOIリンク付き研究成果
- 日付: 2026-08-13 更新（論文はIISEC 2026、2026-02-05〜06の会議発表）
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: DDD-Enforcerは、PDF/DOCX/TXTのソフトウェア要求仕様からtypedなDDDモデルを生成し、Python AST解析、import topology、RAGによる要求トレースを組み合わせ、VS Code診断としてDDD違反や命名・境界のずれを返す。READMEにはIEEE XploreとDOI（https://doi.org/10.1109/IISEC69317.2026.11418529）へのリンクがあり、multi-agent LLM reasoningと決定的検証を組み合わせる設計が説明されている。
- なぜ面白いか:
  - 技術: Scout、Architect、Specialist、Verifier、Refiner、Context Mapper、Holistic Criticなどの段階を分け、確率的LLM判断をtyped schema、AST、import解析、要求文トレースで拘束している。
  - 人文: DDDでしばしば曖昧になる「要求の言葉」と「コードの言葉」のずれを、日々の保存操作に戻す点が実践的。設計レビューを熟練者の暗黙知から、チームが議論できる診断と証拠の形に変える試みとして読める。

### 3. LLM_Ontology_DDD: ユビキタス言語と意味衝突をLLM＋オントロジーで扱う小さな研究プロトタイプ
- 出典: GitHub / Web
- 日付: 2026-08-12 作成・更新
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: リポジトリ説明とREADMEは「A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts in Domain-Driven Design」として、LLMとオントロジーを組み合わせ、DDDにおけるユビキタス言語構築と意味衝突解消を扱う方向性を示している。公開内容はまだ最小限だが、テーマ設定そのものがDDD×LLMの核心に近い。
- なぜ面白いか:
  - 技術: LLMの自然言語抽出能力とオントロジーの形式的整合性を組み合わせることで、同名異義・異名同義・境界をまたぐ概念衝突を機械支援で扱える可能性がある。
  - 人文: ユビキタス言語は単なる用語集ではなく、職能・部署・顧客・開発者の力関係を含む合意形成の場である。意味衝突を「消す」のではなく可視化して交渉可能にするなら、AIは文化の標準化装置ではなく対話の媒介になれる。

### 4. AI Refinement Method: 「vibe coding」ではなくEvent Storming/DDD/精緻化で仕様を先に固めるエージェント方法論
- 出典: GitHub / Web
- 日付: 2026-06-24 更新（直近14日より古いが、DDD×AI仕様化の文脈で継続的に重要）
- リンク: https://github.com/nlawstudio/ai-refinement-method
- 要約: AI Refinement Methodは、Claude Code、Cursor、Codexなどの実装エージェントに渡す前段として、event storming、DDD、refinement、ADR、domain glossary、threat model、受け入れ条件、失敗テストを生成する「仕様化レイヤー」を提案する。READMEは「コードが安くなった時代には仕様品質がボトルネック」と位置づけ、AIを実装者ではなく問い返す設計パートナーとして使う姿勢を強く打ち出している。
- なぜ面白いか:
  - 技術: Explorer、Cartographer、Analyst、Architect、Verifier、Critic、Threat Modellerなどの役割を分け、Event StormingとDDDの成果物を実装前のDefinition of Readyとして構造化している。
  - 人文: 「速く書く」より「何を作るべきかを共同で学ぶ」ことを重視しており、DDD本来の組織学習の側面をAI時代に再定義している。モデルを差し替えても残る資産はコードではなく、チームの判断・語彙・リスク認識だという主張が印象的。

### 5. Event Storming Canvas: 人間とClaudeが同じboard.jsonを編集するAI共同モデリング実験
- 出典: GitHub / Web
- 日付: 2026-08-03 更新（直近14日より少し古いが、AI支援Event Stormingとして関連度が高い）
- リンク: https://github.com/przeprogramowani/event-storming-canvas
- 要約: Event Storming Canvasは、ブラウザ上のEvent Stormingボードと、Claudeなどのエージェントが編集する`board.json`を単一の状態として扱う小さなツール。Domain Event、Command、Actor、Read Model、Policy、External、Aggregate、Hotspotといった色付き文法と、Chaotic ExplorationからAggregatesまでのフェーズを持ち、人間のワークショップにAI共同モデレーターを参加させる。
- なぜ面白いか:
  - 技術: `board.json`をsingle source of truthにし、fs.watchとSSEでブラウザへ即時反映する単純な構成により、人間とエージェントが同じイベントストーミング状態を編集できる。
  - 人文: Event Stormingの価値は付箋そのものではなく、参加者が同じ出来事列を見ながら認識のずれを発見することにある。AIが「答えを出す」のではなく、hotspotを足し、質問し、欠落を示す共同モデレーターになる設計は、組織文化と設計実践の接続として興味深い。

## arXiv / 学術
- 本調査時点で確認されませんでした。
- 注意: arXiv APIへの直接問い合わせは複数クエリでHTTP 429 / timeoutとなったため、今日の確認は不完全です。架空のarXiv IDは記載していません。

## メモ
- X検索: 英語・日本語クエリを実行しましたが、x_searchはクレジット/サブスクリプション制限で失敗しました。X由来の投稿は採用していません。
- Web検索: Firecrawlベースのweb_search / web_extractは未設定で失敗しました。代替としてGitHub API、raw.githubusercontent.com、Bing RSS、直接HTTP取得を使いました。Bing RSSは「domain」を一般的なインターネットドメインとして解釈するノイズが大きかったため、実質的な採用元はGitHub上の公開プロジェクトとREADMEです。
- 日本語アカウントの扱い: X制限のため確認できませんでした。日本語Web検索もノイズが大きく、DDD文脈の有効な直近候補は採用できませんでした。
- 注意点・誇張リスク: GitHub上の新規/小規模リポジトリが中心で、スター数や実運用実績は限定的です。今日のトップ5は「流行の確定」ではなく、DDDがAIエージェント時代にどの方向へ翻訳されつつあるかを示す探索的シグナルとして読むのが安全です。

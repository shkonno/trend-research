# DDD トレンド調査 (2026-07-25)

- 調査日: 2026-07-25
- 情報源: X / Web（web_search は未設定のため direct HTTP 取得で補完） / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AI/LLM時代のDDDは「コードを書く作法」よりも、人間・組織・エージェントが共有できる意味の境界と行為のルールを作る技術として再評価されています。

## トップ5

### 1. DSLs Enable Reliable Use of LLMs
- 出典: Martin Fowlerサイト記事 / X投稿（Martin Fowler）
- 日付: 2026-07-14
- リンク: https://martinfowler.com/articles/llm-and-dsls.html / https://x.com/martinfowler/status/2077023024155422927
- 要約: Unmesh Joshi氏が、LLMに自由にコードを書かせるのではなく、抽象化とDomain-Specific Languageを「強いハーネス」として使う方法を解説。Tickloomという分散システム挙動のドメインモデル／DSL例を通じて、DSLをLLM時代のSource of Truthにする発想が示されています。
- なぜ面白いか:
  - 技術: ユビキタス言語・ドメイン抽象・DSLをLLMの出力空間を制約する実装可能な境界として扱える点が、DDDとAIコーディングの接続として非常に強いです。
  - 人文: これは「自然言語でお願いする」から「共同体が合意した言語で機械と交渉する」への移行です。ソフトウェア設計が、人間とAIの間の制度設計・翻訳設計になっていることをよく表しています。

### 2. Your agent skill is not an anti-corruption layer
- 出典: Thoughtworksブログ / X投稿（Thoughtworks）
- 日付: ブログ公開 2026-06-12（Xでの再共有 2026-07-21）
- リンク: https://www.thoughtworks.com/en-gb/insights/blog/generative-ai/your-agent-skill-not-anti-corruption-layer / https://x.com/thoughtworks/status/2079474689861112120
- 要約: MCPサーバやエージェントスキルを万能アダプタのように使うと、上流システムのスキーマや意味がそのままLLMの文脈に流れ込み、境界が濁ると警告。DDDのbounded contextやanti-corruption layerの考え方で、企業AIエージェントの密結合を防ぐべきだと論じています。
- なぜ面白いか:
  - 技術: MCP統合を「便利な接続」ではなく「コンテキスト汚染の経路」と見なし、ACLを明示的な翻訳層として再設計する視点が実務的です。
  - 人文: エージェントが企業の言葉を勝手に混ぜると、責任や権限の境界も曖昧になります。DDDは単なる設計パターンではなく、組織内の意味・責任・信頼の分節を守る文化的装置として機能します。

### 3. Operational Ontology：AIエージェントが「読める」だけでなく「業務ルール付きで書ける」ドメインモデル
- 出典: X投稿（@gura105） / GitHubリポジトリ
- 日付: 2026-07-20〜2026-07-23頃（X検索結果）
- リンク: https://x.com/gura105/status/2079314764883513596 / https://x.com/gura105/status/2079406652483366936 / https://github.com/gura105/operational-ontology
- 要約: Palantir Foundry型のOntologyを、従来の読み取り中心セマンティックレイヤーではなく、Actions・業務ルール・監査・System of Recordへのwrite-backを持つOperational Ontologyとして整理。公開リポジトリでは、複数レガシー注文システム上にCustomer / Order / Productなどのモデルを載せ、MCPサーバ生成まで含む最小実装を示しています。
- なぜ面白いか:
  - 技術: エンティティ／関連／アクション／不変条件を明示し、AIエージェントの操作をドメインルールでゲートする点が、DDDのaggregateやinvariantをエージェント基盤へ拡張しています。
  - 人文: 「AIが業務を実行する」とは、単にAPIを叩くことではなく、組織が何を正当な行為と認めるかをモデル化することです。Ontologyを運用可能にする試みは、企業の暗黙知を行為の憲法として書き下す作業に近いです。

### 4. AI生成コードのガードレールとしてのDDDと「敵対的検証」
- 出典: X投稿（@little_hand_s） / Zenn記事
- 日付: 2026-07-23〜2026-07-24頃（X検索結果）
- リンク: https://x.com/little_hand_s/status/2079714269302755486 / https://x.com/little_hand_s/status/2080545960653185143 / https://zenn.dev/loglass/articles/6aa18c80496ec6
- 要約: 日本語圏では、DDD実装パターンをAI生成コードの設計判断基準・ガードレールとして使う議論が活発です。あわせて「敵対的検証して」というプロンプトでAIに反証・判定・根拠を出させる実践が共有され、DDD的なレビュー文化とAI活用が接続されています。
- なぜ面白いか:
  - 技術: Entity、Value Object、Aggregate、Domain Eventなどをレビュー観点にしつつ、LLMに反証役を担わせることで、生成速度と設計品質のトレードオフを緩和できます。
  - 人文: DDDの本質は「正しい答えを一人が持つ」ことではなく、言葉とモデルをめぐる対話を続けることです。敵対的検証は、AIを従順な助手ではなく、設計会話に異議を差し込む参加者として使う点で文化的に面白いです。

### 5. Automating Domain-Driven Design: Experience with a Prompting Framework
- 出典: arXiv
- 日付: 2026-03-27（古いが、LLM×DDDに直結するため採用）
- リンク: https://arxiv.org/abs/2603.26244
- 要約: DDDを、(1)ユビキタス言語の確立、(2)イベントストーミングのシミュレーション、(3)bounded context特定、(4)aggregate設計、(5)技術アーキテクチャへの写像、という5段階のLLMプロンプティングフレームワークに分解した経験報告。前半は有用な成果物を生成する一方、後半では小さな誤りが蓄積し、完全自動化ではなく専門家のsparring partnerとして有効だと結論づけています。
- なぜ面白いか:
  - 技術: Event Stormingやユビキタス言語のような発散・整理フェーズはLLM支援と相性がよいが、aggregateやアーキテクチャ決定では誤差伝播が問題になるという実務的な境界線を示しています。
  - 人文: 「AIに設計させる」のではなく「人間が何を議論すべきかを浮かび上がらせる」使い方に価値を置いている点が重要です。DDDの協働的・対話的な性格を、AI時代にも手放してはいけないという示唆があります。

## arXiv / 学術

- Automating Domain-Driven Design: Experience with a Prompting Framework, arXiv:2603.26244（2026-03-27）: LLMによるユビキタス言語、イベントストーミング、bounded context、aggregate設計支援を扱う直接関連論文。
- Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem, arXiv:2607.06471（2026-07-07、直近14日よりやや古い）: GitHub上のDDD実践を大規模に特徴づけるMSR研究。AI/LLM中心ではないが、AI時代にDDD実践を評価するベースラインとして有用。

## メモ

- Boris Cherny優先の有無: Claude固有トピックではないため、今回は優先対象なし。
- 日本語アカウントの扱い: @little_hand_s と @gura105 の投稿を重視し、日本語圏のDDD×AI実践知をトップ5に含めました。
- 注意点・誇張リスク: web_search / web_extract はFirecrawl未設定で利用できなかったため、Webはterminalからのdirect HTTP取得で補完しました。X検索結果に日付が明示されない一部投稿は「頃」と表記し、リンクはX検索で確認されたもののみ使用しています。arXivは実APIで確認し、架空IDは含めていません。

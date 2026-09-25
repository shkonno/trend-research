# DDD トレンド調査 (2026-09-25)

- 調査日: 2026-09-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは、ドメイン知識を「コードに入れる」だけでなく、エージェントに渡す制約・権限・言葉・検証境界を設計する営みに広がっている。

## トップ5

### 1. Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems
- 出典: arXiv
- 日付: 2026-09-23
- リンク: http://arxiv.org/abs/2609.27354v1
- 要約: 生成AIシステムを実ドメインへ適用するとき、技術・規制・制度・規範上の制約を「AIの許容される振る舞い」を決めるドメインインターフェースとして設計する論文。DDDを参照しながら、RAGやメモリに知識を足すだけでなく、制約そのものをコンテキスト設計の第一級要素にする点が重要。
- なぜ面白いか:
  - 技術: LLM/エージェントに渡すコンテキストを、知識断片ではなく不変条件・ポリシー・検証可能な境界を持つ設計成果物として扱える。
  - 人文: 「AIが何をしてよいか」はモデル性能ではなく、組織の制度、責任、価値判断によって定まる。ユビキタス言語が、人間同士の共通語から人間とAIの統治言語へ拡張される兆しとして読める。

### 2. The Agent Harness: Control Planes, Invariants, and Approval Boundaries for Production AI Agents
- 出典: InfoQ プレゼンテーション
- 日付: 2026-09-21
- リンク: https://www.infoq.com/presentations/ai-agent-harness/
- 要約: OpenAIのVinoth Govindarajan氏が、プロダクションAIエージェントの失敗要因を幻覚だけに還元せず、状態所有、並行変更の直列化、実行権限のスコープ、ユーザー可視の境界での検証として整理している。DDDそのものの記事ではないが、集約の不変条件や境界づけられたコンテキストをエージェント実行基盤へ接続する材料になる。
- なぜ面白いか:
  - 技術: エージェントの行動を制御プレーン、不変条件、承認境界で囲う考え方は、DDDの戦術・戦略パターンをAI実行環境へ翻訳する実践に近い。
  - 人文: 「自律エージェント」はしばしば魔法の労働者として語られるが、実際には誰が何を承認し、どの変更を説明できるかという組織文化の問題である。委譲をロマンではなく統治可能な関係として設計する視点がある。

### 3. Securing AI Agents: Identity, Authorization, and the DPACT Framework
- 出典: InfoQ ポッドキャスト
- 日付: 2026-09-21
- リンク: https://www.infoq.com/podcasts/securing-ai-agents-identity-authorization/
- 要約: AIエージェントのアイデンティティ、認可、代理実行を扱い、Delegation、Policy、Auditability、Context、TimeからなるDPACTフレームワークを紹介する回。DDD観点では、エージェントを「誰の代理で、どの文脈で、いつまで、何をしてよい主体か」としてモデリングするための語彙を与える。
- なぜ面白いか:
  - 技術: 認可をロールだけでなく、委譲、文脈、時間、監査可能性の組み合わせとして設計することで、境界づけられたコンテキストとアクセス制御を接続できる。
  - 人文: エージェントの代理性は、法律・倫理・職場の信頼関係の境界を曖昧にする。DDDの対話的モデリングは、暗黙の信頼や責任分担をチームで言語化する場になり得る。

### 4. Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark
- 出典: arXiv（直近14日より古いが、AI+DDD文脈で重要）
- 日付: 2026-08-15
- リンク: http://arxiv.org/abs/2608.15255v1
- 要約: ドメインモデリングはDDDの中心活動だが、自動化されたドメインモデル生成の比較評価には標準ベンチマークが不足しているとして、評価用データセットと基準を提案する論文。LLMが生成したエンティティや関係の品質を「それっぽい」から一歩進めて測る方向を示す。
- なぜ面白いか:
  - 技術: LLMによるドメインモデル生成を導入する際、再現性あるベンチマークでモデル品質を比較できる足場になる。
  - 人文: ドメインモデルの正しさは現場の経験や利害調整を含むため、評価指標は組織が何を「重要な概念」とみなすかを映す。自動化は専門家の会話を置き換えるより、会話の焦点を可視化する道具として使うべきだと示唆する。

### 5. Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design
- 出典: arXiv（直近14日より古いが、AI/自動化時代のDDD運用で重要）
- 日付: 2026-08-06
- リンク: http://arxiv.org/abs/2608.05612v1
- 要約: DDDで作られた共有語彙や戦術的モデルは、実装が進むにつれてコードと乖離しやすい。この論文はJDomInOという双方向同期ツールチェーンを提示し、Javaコードベースとドメインモデルを共通メタモデルで結び、モデルからコード、コードからモデルの往復を可能にする。
- なぜ面白いか:
  - 技術: 集約、値オブジェクト、ドメインサービスなどの構造をモデルとコードの同期対象にすることで、LLM生成コードによる設計意図のドリフトを検知しやすくなる。
  - 人文: モデルとコードのズレは単なる技術的負債ではなく、チームがどの言葉を忘れ、どの業務理解を置き去りにしたかの兆候でもある。ユビキタス言語の維持は、組織の記憶を維持する営みでもある。

## arXiv / 学術
- Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems — arXiv:2609.27354v1。2026-09-23公開で、今回の直近枠では最重要。
- Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark — arXiv:2608.15255v1。直近14日より古いが、自動ドメインモデリング評価の基盤として重要。
- Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design — arXiv:2608.05612v1。直近14日より古いが、AI支援開発でのモデル/コード同期問題に直結。
- Automating Domain-Driven Design: Experience with a Prompting Framework — arXiv:2603.26244v1。古いが、ユビキタス言語、イベントストーミング、境界づけられたコンテキスト、集約設計をLLMプロンプトフレームワーク化する研究として参照価値あり。
- Leveraging Generative AI for Enhancing Domain-Driven Software Design — arXiv:2601.20909v1。古いが、生成AIによるDDDメタモデル生成の初期研究として確認。

## メモ
- X検索は英語・日本語で実行したが、xAI側の `personal-team-blocked:spending-limit` により取得できなかった。そのため本日のトップ5にはX由来アイテムを採用していない。
- Web検索ツールはFirecrawl未設定で失敗したため、代替として直接HTTP取得、InfoQページ取得、Bing RSS取得を試みた。Bing RSSは一般的な「ドメイン名」検索へ寄り、DDD調査には有効な結果が少なかった。
- Boris Cherny優先はClaude系トピックではないため適用外。
- 日本語アカウント・日本語記事は検索を試みたが、今回の有効ソースとして採用できる直近情報は確認できなかった。
- 誇張リスク: 直近14日でDDDを明示する発表は少ないため、AIエージェントの制御境界・認可・監査性をDDD観点で読めるWeb項目を含めた。DDD明示の直近ソースは主にarXivの1件である。

# DDD トレンド調査 (2026-07-24)

- 調査日: 2026-07-24
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AIコーディングエージェント時代のDDDは、「きれいな設計技法」から、曖昧な要求を実装に流し込まないための組織的インフラへ移りつつあります。

## トップ5

### 1. DDDの古典的プラクティスがLLM/agentワークフローの足場になる
- 出典: X投稿 / Aaron Stannard（@Aaronontheweb）
- 日付: 2026-07-22
- リンク: https://x.com/Aaronontheweb/status/2079924442126291423
- 要約: Ubiquitous Language、Bounded Context、Vertical Slice、型による不正状態の排除、Event-driven design、TDD/BDDといった実践を、LLMに与える文脈・制約・検証の構造として読み替える議論。単に「AIに実装させる」のではなく、AIが迷いにくい問題空間を人間が設計する、という方向性が明確です。
- なぜ面白いか:
  - 技術: DDDの戦術・戦略パターンを、LLMのコンテキスト設計、ガードレール、テスト駆動の検証ループに直接接続している点が実践的です。
  - 人文: DDDはもともと業務知識を共同体の言語にする営みですが、ここではその言語が「人間同士」だけでなく「人間とAIの共同作業」の媒介になります。AI時代の設計者は、コードを書く人というより、意味の境界を守る編集者・翻訳者に近づいています。

### 2. 「AIにDDDで実装して」と頼むと、DDD初心者と同じ失敗をする
- 出典: X投稿 / @t_shinden
- 日付: 2026-07-23
- リンク: https://x.com/t_shinden/status/2080435334031216812
- 要約: AIにDDD実装を依頼しても、ドメイン層にドメインロジックを書かず、責務が外へ漏れるという観察。見た目のレイヤーは守っても意味を考えきれていない点が人間のDDD初心者に似ており、対策も人間への教育・レビューと似るという実務的な示唆です。
- なぜ面白いか:
  - 技術: LLM生成コードの問題を「レイヤー違反」や「貧血ドメインモデル」として診断できるため、レビュー観点をDDDの語彙で具体化できます。
  - 人文: AIは超人的な設計者ではなく、むしろ組織に蓄積された初学者的パターンを増幅する鏡として現れています。DDD教育で重要だった対話、例示、境界づけ、反復レビューが、AI相手にも必要になるという点が文化的に興味深いです。

### 3. Agentic programmingではUbiquitous Languageが「ベストプラクティス」から「前提条件」になる
- 出典: X投稿 / Mayflower（@mayflowergmbh）
- 日付: 2026-07-22
- リンク: https://x.com/mayflowergmbh/status/2079824006283223263
- 要約: Agentic programmingにおいて、Ubiquitous Language、tests first、clear contextは従来の推奨事項ではなく前提条件になる、という主張。エージェントは曖昧さを自然に察知しないため、言語の規律そのものがインフラになる、という見立てです。
- なぜ面白いか:
  - 技術: PRD、仕様、テスト、コードをつなぐ語彙を揃えることで、エージェントの誤解・過剰実装・文脈逸脱を減らす設計方針になります。
  - 人文: Ubiquitous Languageは、組織の中で「同じ言葉で同じ現実を指す」ための社会的契約です。AIが参加することで、この契約は暗黙知では済まされず、明示的に書かれ、検査され、更新される対象になります。

### 4. StormPilot: AIコーディングの前にStructured Event Stormingで「何を作るか」を合意する
- 出典: X投稿 + Webページ / CODELEV StormPilot
- 日付: 2026-07-12（X投稿日）
- リンク: https://stormpilot.codelev.com/explore
- 要約: StormPilotは「AI-assisted Structured Event Storming diagram editor for software teams」として公開されているツール。関連X投稿では、AI coding agentsが曖昧な仕様を高速にコード化してしまうこと自体が問題であり、コードを書く前にステークホルダーがWHATを合意するための構造化Event Stormingが必要だと位置づけています。
- なぜ面白いか:
  - 技術: Event Stormingをデジタル化し、イベント・コマンド・ポリシー・集約などをAI実装前の仕様整理に使うことで、生成コードの前段にドメイン検証ステップを置けます。
  - 人文: これは「速く作る」文化へのブレーキではなく、速さが意味を踏み潰さないための儀式です。ステークホルダーの合意形成をAI導入の中心に戻す点で、DDDのワークショップ文化が再評価されています。

### 5. Domain-Driven Design in Practice: GitHub上のDDD実践を大規模に実証分析する研究
- 出典: arXiv
- 日付: 2026-07-07（直近14日より古いが重要）
- リンク: http://arxiv.org/abs/2607.06471v1
- 要約: 「Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem」は、GitHub上のDDDリポジトリ候補11,742件から、GPT-4oを使った三重多数決の意味的検証により2,502件を抽出し、DDD採用の実態を大規模に特徴づける研究。DDD研究が理論寄りになりがちだった状況に対して、実装エコシステムの実証的な基準線を作ろうとしています。
- なぜ面白いか:
  - 技術: DDDの実践状況をリポジトリマイニングとLLM支援ラベリングで測ることで、設計パターンの採用・維持・進化を経験的に比較できる土台になります。
  - 人文: DDDは「現場の暗黙的な設計文化」に強く依存する方法論ですが、この研究はその文化を観察可能なデータへ変換しようとしています。AIがDDDを実装する時代には、そもそも人間の現場でDDDがどう生きられているのかを測ることが重要になります。

## arXiv / 学術

- Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem / arXiv:2607.06471v1 / 2026-07-07 / GitHub上のDDD実践を大規模に特徴づける研究で、直近14日より少し古いが本日の文脈に強く関連。
- 関連するが古い研究として、Automating Domain-Driven Design: Experience with a Prompting Framework / arXiv:2603.26244v1 / 2026-03-27 も確認。LLMでUbiquitous Language、Event Storming、Bounded Context、Aggregates、技術アーキテクチャへの写像を支援する枠組みで、本日のX上の議論と接続する。

## メモ

- Boris Cherny優先の有無: 本トピックはClaude固有ではないため、Boris Cherny優先は適用対象外。
- 日本語アカウントの扱い: 日本語X検索を実施し、@t_shinden の投稿をトップ5に採用。@bachi7q の「AIにDDD的アーキテクチャをやらせるとUnit of Workを入れがち」という投稿（2026-07-23）も確認したが、トップ5の重複を避けるため今回は採用外。
- Web検索の注意: Hermesのweb_searchツールはFirecrawl未設定で失敗したため、Webについてはterminal経由の直接HTTP取得でStormPilotページを確認した。検索網羅性には制限がある。
- arXiv検索の注意: arXiv APIでDDD / Event Storming / Ubiquitous Language関連語を検索。2026-07-10以降に完全一致度の高い新規arXivは確認できず、2026-07-07の関連研究を「直近14日より古いが重要」として採用した。
- 誇張リスク: X投稿は実務的な観察が中心で、体系的検証ではない。AI/LLMとDDDの接続は盛り上がりつつあるが、Event StormingやUbiquitous Languageに特化した直近投稿数はまだ限定的。

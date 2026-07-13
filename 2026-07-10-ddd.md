# DDD トレンド調査 (2026-07-10)

- 調査日: 2026-07-10
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェント時代のDDDは、単なる設計パターンではなく「人間の文脈・組織記憶・エージェント実行」をつなぐ共有言語の基盤として再注目されている。

## トップ5

### 1. Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem
- 出典: arXiv / cs.SE
- 日付: 2026-07-07
- リンク: https://arxiv.org/abs/2607.06471
- 要約: 11,742件の候補GitHubリポジトリから、GPT-4oの三重多数決による意味的検証で2,502件のDDD実践リポジトリを抽出した大規模実証研究。DDD採用は2017年以降に加速し、C#とTypeScriptが実務採用を牽引している一方、約25.3%のプロジェクトでは明示的なビジネス文脈が残されていないと報告している。
- なぜ面白いか:
  - 技術: DDDを「語られる方法論」から、リポジトリ上で観測・検証できる設計実践へ移す重要なデータポイントになっている。
  - 人文: ビジネス文脈がコード履歴から消えるという指摘は、ユビキタス言語が単なる命名規則ではなく組織の記憶装置であることを示している。AIがコードを読む時代には、失われた文脈は人間だけでなくエージェントにも継承されない。

### 2. Archally Blueprint Schema: domain-first YAML schema for AI-grounded architecture
- 出典: GitHub / Web
- 日付: 2026-07-09 更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: ドメイン設計、ビジネスルール、価値流、ガバナンス、組織アラインメントをYAMLで一元化し、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Stormingボード、MCP経由のAIエージェント接地へつなぐことを狙うスキーマ。READMEでは、アーキテクチャ知識がWiki、スライド、白板写真、部族的記憶に分散する問題を正面から扱っている。
- なぜ面白いか:
  - 技術: DDDの成果物を人間向けドキュメントで終わらせず、生成・検証・エージェント接地可能な機械可読仕様へ変換しようとしている。
  - 人文: 「誰が何を知っているか」に依存する設計文化を、共有可能な組織記憶へ移す試みとして読める。イベントストーミングの付箋が、会議の熱量だけでなく長期的な協働のインフラになる可能性がある。

### 3. faceto: typed file → visual workshop board with LLM feedback loop
- 出典: GitHub / Web
- 日付: 2026-07-06 更新
- リンク: https://github.com/bastien-gallay/faceto
- 要約: 型付きファイルからHTML+SVGのワークショップボードを生成し、LLMと一緒に考えながら要素ごとにノートを追加して次セッションでモデルを調整するツール。最初のボード形式としてEvent Stormingを扱い、将来的にC4、ストーリーマッピング、インパクトマッピングなどへ拡張する方向性を示している。
- なぜ面白いか:
  - 技術: Event StormingをLLM時代の反復可能なモデリング・インターフェースにし、テキスト仕様と視覚的ワークショップを往復させる設計になっている。
  - 人文: ワークショップで生まれる曖昧さや違和感を、次の対話に持ち越せる点が重要。DDDの価値は正しい図よりも、チームが一緒に意味を交渉した履歴にあることを思い出させる。

### 4. ddd-agent-skill: Domain-Driven Design end-to-end for agent workflows
- 出典: GitHub / Web
- 日付: 2026-07-07 公開・更新
- リンク: https://github.com/aristorinjuang/ddd-agent-skill
- 要約: Agent Skills互換のDDDスキルで、Vaughn VernonのIDDDに沿い、まず「Full DDD / Light DDD / plain CRUD」の適用価値判定から始める点を強調している。Event Storming、 bounded contexts、context map、aggregates、entities、value objects、domain events、repositories、既存コード監査などをエージェント支援の一連の流れとして扱う。
- なぜ面白いか:
  - 技術: AIエージェントにDDD成果物を直接生成させるだけでなく、DDDを使うべきかどうかのゲートを組み込んでいる点が実務的。
  - 人文: DDDはしばしば儀式化しやすいが、このアプローチは「複雑さに見合った設計を選ぶ」という倫理を持ち込んでいる。エージェントが強力になるほど、過剰設計を抑える判断の文化が重要になる。

### 5. dca-marketplace: Claude Code plugins for Domain-Centric Architecture
- 出典: GitHub / Web
- 日付: 2026-07-06 更新
- リンク: https://github.com/chbloemer/dca-marketplace
- 要約: Claude Code向けに、Domain-Centric Architectureのスキルとエージェントをマーケットプレイス形式で提供するリポジトリ。`/ubiquitous-language`、`/context-map`、`/dca-bootstrap`、`ddd-expert`、`ddd-reviewer`、`hexagonal-reviewer`などを含み、知識カタログやレシピ駆動のビルドループをプロジェクト内で使えるようにしている。
- なぜ面白いか:
  - 技術: DDD/Hexagonal/Clean Architectureを、Claude Codeの作業単位・レビュー単位・知識ベースとしてパッケージ化している。
  - 人文: これは設計判断を「優秀な個人の頭の中」から「チームで呼び出せる作法」へ移す動きに見える。ユビキタス言語やコンテキストマップが、AIとの共同作業における礼儀作法・記憶の形式になりつつある。

## arXiv / 学術
- 見つかりました: `2607.06471` — Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem。2026-07-07公開で、今回の最重要学術ソース。
- 関連するが直近14日より少し古い: `2606.23984` — Domain-Driven Design in Practice: A Mining Study of Maintenance and Evolution in Open-Source Repositories。2026-06-22公開。DDD戦術パターン、進化、保守性、bounded context違反をGitHubマイニングで調べる事前登録研究。
- 古いが関連: `2605.01159` — A Domain-Driven Design Simulator for Business Logic-Rich Microservice Systems。2026-05-01公開。集約、Saga、TCC、分散配置を含むマイクロサービス設計を早期に実験するためのDDDシミュレータ。

## メモ
- Boris Cherny優先の有無: DDD単独トピックのため該当投稿は確認対象外。ただしAI/エージェント接続は重視した。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールがクレジット上限エラーで失敗したため、日本語X投稿は取得できなかった。
- 注意点・誇張リスク: X検索は実行したものの外部クレジット制限で失敗、Web検索ツールも未設定エラーだったため、代替としてarXiv API、GitHub Search/API、GitHub Atom/README取得で確認できたリンクだけを採用した。GitHub項目は新規・少スターのものを含むため、成熟度ではなく「AIエージェント時代のDDDの方向性」として評価している。架空リンク・未確認arXiv IDは含めていない。

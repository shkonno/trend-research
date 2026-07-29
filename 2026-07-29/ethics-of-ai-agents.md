# Ethics of AI Agents トレンド調査 (2026-07-29)

- 調査日: 2026-07-29
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェント倫理の焦点は「原則」から、権限境界・監査可能な実行基盤・責任分配・文化的依存リスクをどう実装するかへ移っている。

## トップ5

### 1. Separating Capability from Permission: A Governance Framework for Agentic AI Autonomy Levels
- 出典: arXiv
- 日付: 2026-07-26
- リンク: https://arxiv.org/abs/2607.23438v1
- 要約: エージェントが「技術的にできること」と「運用上許されること」を分離し、Allowed Autonomy Levels（AAL）として権限レベルを設計するガバナンス枠組みを提案している。自律性の議論を能力評価だけでなく、許可・責任・監督の設計問題として扱う点が重要。
- なぜ面白いか:
  - 技術: エージェントの能力ベンチマークと実行許可ポリシーを分けることで、ツール利用・外部操作・人間承認をランタイム制御に落とし込める。
  - 人文: 「できるなら任せる」ではなく「誰がどこまで委任してよいと決めたのか」を問うため、責任所在を個人・組織・供給網に再配分する議論になる。自律性を人格化せず、委任の制度設計として扱う姿勢が倫理的に健全。

### 2. Engineering and Governing the Agent Harness: A Technology and Policy Framework for the Runtime Layer of Agentic AI
- 出典: Web（UNU / United Nations University、Google News RSS経由で確認）
- 日付: 2026-07-22
- リンク: https://news.google.com/rss/articles/CBMiswFBVV95cUxOZXdSNUNZeWgzN1phXzViaUlKYUdsdEZRY2ZvM0dLekN0WVRZdWoxNjRYaXNRTEszZUpIZDN1M21aRmJ5bnlIYkFNM01JeXNzTlhnMzZGQU9BajZycGZhWmNfY0Z0R1F6MUt4YUwwX3hiby1wNXRKTklaWlEwajdHOXc1TTYyejZVRXVYa3NYZWVzcUk3Qldldi10TXdETng0OWlKZnhzYzVEelpvXzB2MFIzRQ?oc=5
- 要約: Agent Harness、つまりモデルと外部世界のあいだにある実行層を、技術設計と政策ガバナンスの対象として扱う議論。モデル単体の安全性ではなく、メモリ、ツール、権限、監査ログ、停止機構を含む運用レイヤーが規制・統制の中心になる。
- なぜ面白いか:
  - 技術: エージェント安全をプロンプトやモデルカードではなく、権限分離・ログ・承認ワークフロー・API境界を持つランタイムアーキテクチャとして捉えている。
  - 人文: 政策が「AIそのもの」を抽象的に縛るだけでは現場の行為を捕まえられない、という制度設計上のリアリズムがある。人間がどの地点で介入・異議申し立て・説明要求できるかを設計する人間中心の論点でもある。

### 3. Operational Hallucination and Safety Drift in AI Agents
- 出典: arXiv
- 日付: 2026-07-20
- リンク: https://arxiv.org/abs/2607.18366v1
- 要約: ツール利用型エージェントでは、単発応答の安全性だけでなく、複数ターンの実行中に初期の安全制約が劣化する「safety drift」や、運用上の幻覚が生じるリスクを扱っている。長いタスクの途中で何が逸脱を生むのかを実証的に見る点が実務的。
- なぜ面白いか:
  - 技術: マルチステップ計画、ツール呼び出し、状態保持が絡むことで、従来の静的な安全評価では見えない時間的な失敗モードを評価対象にできる。
  - 人文: 人間社会の信頼は「最初に正しいこと」ではなく「途中で変質しないこと」に支えられる。エージェント倫理も同じく、約束・記録・継続的監督の倫理へ広がっている。

### 4. 自律するAIの時代：AIエージェントのサイバーリスクと実践的ガバナンス / AI-CAL関連議論
- 出典: Web（PwC日本 / Yahoo!ニュース等、Google News RSS経由で確認）
- 日付: 2026-07-17（関連する「デジタル従業員」論は2026-07-13）
- リンク: https://news.google.com/rss/articles/CBMiigFBVV95cUxNT2liSVVKSnRWd0k2eTFGSkZBMXlBQ19xVDFMWmx4WVRkX2FjNVJtd3Q2SlhYa1NQRTdVVU5Wa25fdXVpZUlsSGJMb1llQ2VlekxWSHMyOG1qSFZSX1llTjJFNG1Ram1jRnNXOTd5MThvQUpIZWRSY2g4al85VUdxZW5kMU5qbzVkRGc?oc=5
- 要約: 日本語圏では、AIエージェントを「デジタル従業員」として迎える組織が、統制保証水準、サイバーリスク、権限管理、監査責任をどう整えるかという実装寄りの議論が目立つ。AI-CALのような統制レベルの言語化は、現場導入と責任分界をつなぐ足場になる。
- なぜ面白いか:
  - 技術: 本番投入前の権限管理、ログ、評価、インシデント対応をレベル分けすることで、エージェント導入をセキュリティ統制のワークフローに接続できる。
  - 人文: 「AIを従業員のように扱う」比喩は便利だが、人間の労働者とは権利も責任能力も違うため危うい。日本企業の現場では、効率化より先に、誰が説明し誰が止めるのかを組織文化として合意する必要がある。

### 5. 中国のAI倫理・AIエージェント規制と感情交流サービス規制
- 出典: Web（China Daily HK / MLex / Forbes / 日本経済新聞などの報道、Google News RSS経由で確認）
- 日付: 2026-07-15〜2026-07-22
- リンク: https://news.google.com/rss/articles/CBMixgFBVV95cUxQamZNNUpkcmIzamg1clFsbTlLcFJPNmFMWmp2ajlKVnVBeEhEeWJuV2diMEo0bDNuUHRJdDMzNlZDSVpqTlRySWFzbExNcFBpUkJDenY5Tk84anAxdWNjTlFQZ0w3WWJfVFF2SzNOZ2NPZHVWcmFYRE5Ia2tMV3JoTkJIZkFHRjl3MDZQdVNTdFY0UFoxVExJUmlKbFpWVFBhaU1jSnFlcW5oTWhEeUlGa211bmxkaEhxekJkWGZQdDNnYkxiZmc?oc=5
- 要約: 中国では国際AI倫理行動計画、リスク階層化、AIエージェントのリコール構想、感情交流型AIサービスへの規制が報じられている。エージェントを市場投入後にも回収・停止・是正できる対象として扱う発想が、米国の分散的規制との対比で注目される。
- なぜ面白いか:
  - 技術: リコール可能性やリスク階層化は、モデル更新、エージェントID、監査ログ、配布停止のインフラ設計を要求する。
  - 人文: 感情交流AIや仮想恋人・家族への依存リスクは、文化差とケア倫理を強く含む。安全性は危害防止だけでなく、孤独、愛着、国家による介入の正当性という社会哲学の問題にもなる。

## arXiv / 学術
- Separating Capability from Permission: A Governance Framework for Agentic AI Autonomy Levels — arXiv:2607.23438v1。能力と許可を切り分ける自律性ガバナンス。
- Operational Hallucination and Safety Drift in AI Agents — arXiv:2607.18366v1。マルチターン実行中の安全劣化を扱う評価研究。
- Regulating autonomous and agentic AI — arXiv:2607.21345v1。規制対象の知識・制御がAI供給網側へ移る問題を扱う。
- The Ethics of Autonomous AI Agents for Offensive Security — arXiv:2607.20255v1。攻撃的セキュリティにおける自律エージェントの不確定性と倫理。
- A Framework of User Experience Principles for Human-AI Agent Interaction in the Workplace — arXiv:2607.19941v1。職場の人間-AIエージェント相互作用におけるUX原則。

## メモ
- Boris Cherny優先の有無: 本トピックはClaude固有ではないため優先対象外。X検索は英語・日本語で実行したが、xAI側のクレジット/サブスクリプション制限により取得できなかった。
- 日本語アカウントの扱い: Xは取得不能だったため、日本語圏の議論はGoogle News RSS経由の日本語Web記事（PwC、CIO.com Japan、日経、EnterpriseZine、IT Leaders等の見出し確認）で補完した。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定で失敗したため、Webは端末からのGoogle News RSS/Bing取得で確認した。Google Newsリンクは直接記事URLではなくRSS記事リンクの場合がある。arXiv項目は実際のarXiv API結果から選定し、架空IDは含めていない。

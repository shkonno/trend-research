# Anthropology of Agentic AI トレンド調査 (2026-09-26)

- 調査日: 2026-09-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Agentic AIは「賢い道具」から、職場の暗黙ルール・権限・同席感・責任語彙を再編する新しい組織アクターとして見られ始めている。

## トップ5

### 1. Working with Agentic `Teammates': When a New Organizational Actor Collides with the Human Ecosystem of Work
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.29901
- 要約: 大企業の複数チームに配備された、持続的でプロアクティブなAI「teammate」を対象にした現場内の質的研究。人間とエージェントが共有する職場で、協働ワークフローの暗黙ルール、非人間アクターとの関係境界、信頼と人間のエージェンシーの再配分が交渉される様子を報告している。
- なぜ面白いか:
  - 技術: 単発チャットではなく、永続的・複数人利用・プロアクティブなエージェントを実組織に置いたときの設計課題を、観察可能な破綻として整理している。
  - 人文: 「同僚」と呼ばれるAIが、実際には誰の発話権・割り込み権・説明責任を持つのかを職場文化の中で再交渉させる点が人類学的に重要。組織の暗黙知が、AI導入で初めて可視化される事例として読める。

### 2. Two's a Crowd: Human and AI-Based Copresence for Developers with ADHD
- 出典: arXiv
- 日付: 2026-09-18（更新: 2026-09-21）
- リンク: https://arxiv.org/abs/2609.21254
- 要約: ADHDのあるソフトウェアエンジニア14名への半構造化インタビューを通じ、人間同士の「body doubling」やペア作業と、agentic AI coding assistantによる同席感がどう異なるかを調べた研究。AIは集中や実行機能を支える一方、人間の共在が持つ社会的支援やオンボーディング構造とは別種の関係を作る。
- なぜ面白いか:
  - 技術: コーディングエージェントを「補完ツール」ではなく、注意・動機づけ・説明責任を調整する作業環境コンポーネントとして評価している。
  - 人文: 身体性の弱いAI同席が、逆説的に「見られている」「一緒にいる」という実践を再設計する。神経多様性の観点から、エージェント導入が標準的労働者像を前提にしてよいのかを問い直している。

### 3. The Disciplinary Language Transfer Problem: How Psychological Vocabulary Produces Governance Failures in AI Agent Deployment
- 出典: arXiv
- 日付: 2026-09-22
- リンク: https://arxiv.org/abs/2609.26562
- 要約: AIエージェントのガバナンスで使われる「学習」「記憶」「価値」「コンプライアンス」「アイデンティティ」「信頼」といった語彙が、心理学・組織科学から持ち込まれた不可視の文法を伴い、現在のAIアーキテクチャには存在しない主体像を前提にしてしまうと論じる。Wittgenstein、Kuhn、Haraway、Star and Griesemerを参照し、語彙移転が生む認識論的失敗を整理している。
- なぜ面白いか:
  - 技術: エージェント評価や監査で使う概念語を、実装上のメカニズムと対応づけ直す必要があることを示している。
  - 人文: 「AIを信頼する」という表現自体が、どの共同体の言語ゲームに属するのかを問う論文。エージェントの能力だけでなく、それを語る言葉が制度と責任配分を作ってしまう点が鋭い。

### 4. Your startup’s next teammate might be an AI agent
- 出典: TechCrunch
- 日付: 2026-09-17
- リンク: https://techcrunch.com/2026/09/16/your-startups-next-teammate-might-be-an-ai-agent-gusto-insight-partners-and-leland-explain-what-that-changes-at-techcrunch-disrupt-2026/
- 要約: TechCrunch Disrupt 2026の告知記事として、Gusto、Insight Partners、Lelandが「スタートアップの次のチームメイトはAIエージェントかもしれない」というテーマで、雇用・人事・チーム編成の変化を議論することを紹介している。学術論文ではないが、AIエージェントを労働力・チーム構成員として語るビジネス文化の広がりを示すシグナルである。
- なぜ面白いか:
  - 技術: HRや組織運営の文脈で、エージェントが採用・業務配分・チーム運営のワークフローに入り込む前提が一般化しつつある。
  - 人文: 「雇う」「同僚にする」という比喩は、AIを単なるSaaSではなく労働文化の登場人物に変える。スタートアップの儀礼である採用・オンボーディング・チーム紹介が、非人間アクターを含む形に拡張される可能性がある。

### 5. Give every teammate and agent the right level of access to your Workers
- 出典: Cloudflare Blog
- 日付: 2026-09-15
- リンク: https://blog.cloudflare.com/workers-granular-authorization/
- 要約: Cloudflare Workersで、個別Worker単位のアクセス範囲やより細かいDeveloper Platformロールを設定できるようにし、チームメイト、CIトークン、エージェントに必要最小限のデバッグ・デプロイ・監視権限を与えられるようにしたという発表。エージェントが実運用環境で作業する前提に合わせ、権限管理が細分化されている。
- なぜ面白いか:
  - 技術: AIエージェントを本番開発組織に参加させるには、ツール利用権限を人間・CI・エージェントの単位で切り分けるIAM設計が不可欠になる。
  - 人文: 「誰に鍵を渡すか」は組織の信頼儀礼そのもの。エージェントにも最小権限を付与する実践は、非人間メンバーを共同体に入れるが、同時に境界線を明確に引く文化的手続きとして読める。

## arXiv / 学術
- Working with Agentic `Teammates': When a New Organizational Actor Collides with the Human Ecosystem of Work — arXiv:2609.29901。人間-エージェント職場の暗黙ルール、関係境界、信頼・人間のエージェンシーの再配分を扱う質的研究。
- Two's a Crowd: Human and AI-Based Copresence for Developers with ADHD — arXiv:2609.21254。ADHD開発者の共在実践とAI coding assistantの身体性・社会性を扱うインタビュー研究。
- The Disciplinary Language Transfer Problem: How Psychological Vocabulary Produces Governance Failures in AI Agent Deployment — arXiv:2609.26562。AIエージェントを語る心理学・組織科学由来の語彙がガバナンス失敗を生む問題を扱う理論論文。
- AI-GRACE: A Use-Case Operationalization Framework for Agentic AI — arXiv:2609.21192。組織目標・義務からデプロイ能力とアーキテクチャへ落とし込む枠組みで、技術実践との接続が強い。
- Compliant with Local Controls, Collectively Discriminatory — arXiv:2609.27994。金融のマルチエージェントAIで、局所的に適合した制御が集団として差別的帰結を生むリスクを扱う。

## メモ
- Boris Cherny優先: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語検索も実施したが、X検索はxAI側の `personal-team-blocked:spending-limit` により取得できなかった。代替としてBing RSS経由の日本語Web検索を使い、2026-09-24〜25の国内解説記事（DX/AI研究所、Qiita、Zenn/NTT DATA Tech等）を確認した。ただし本トピックの上位5件は、人類学・労働文化・組織慣習との接続がより強い英語arXiv/Web項目を優先した。
- Web検索の注意: Hermesのweb_search/web_extractはFirecrawl未設定で利用不能だったため、端末からBing RSS、Hacker News Algolia、直接HTTPメタデータ取得、arXiv APIを用いた。これはソース制限として扱う。
- 注意点・誇張リスク: TechCrunch項目はイベント告知であり、導入実証ではない。Cloudflare項目はAI文化論ではなくアクセス制御の製品発表だが、エージェントを本番組織の権限主体として扱う実践シグナルとして採用した。架空リンク・未確認arXiv IDは含めていない。

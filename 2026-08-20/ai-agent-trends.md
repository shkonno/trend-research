# AI agent trends トレンド調査 (2026-08-20)

- 調査日: 2026-08-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの焦点は「賢い単体モデル」から、標準化されたプラグイン、MCPガバナンス、利用計測、端末・スマホ実世界操作、そして複数エージェント社会の設計へ移っている。

## トップ5

### 1. Agent Plugins 1.0 が VS Code / Copilot CLI / Copilot app で一般利用可能に
- 出典: GitHub Changelog
- 日付: 2026-08-12
- リンク: https://github.blog/changelog/2026-08-12-agent-plugins-1-0-in-vs-code-copilot-cli-and-the-copilot-app
- 要約: GitHubは、Agent Plugins 1.0をVS Code、Copilot CLI、GitHub Copilot SDK、Copilot appで利用可能にした。1つのプラグインパッケージに「スキル」とMCPサーバー設定をまとめ、AWS、Anysphere、Microsoft、OpenAI、Vercel、Googleなどが関わるオープン標準として複数エージェントクライアントに展開できる点が核になる。
- なぜ面白いか:
  - 技術: エージェントごとに別々のmanifestやディレクトリ構成を維持する負担を減らし、MCPサーバーとスキルを横断的に配布・統治する「拡張の単位」を作っている。
  - 人文: これはAIエージェントの世界における「アプリストア化」の一歩であり、個人の職人芸だったプロンプトや手順が、組織で共有・監査される文化財のような形を取り始めたことを示す。便利さと同時に、誰が標準を支配するのかという政治性も帯びている。

### 2. GitHub Copilot Enterprise Managed Settings に MCP allowlist / denylist が追加
- 出典: GitHub Changelog
- 日付: 2026-08-06
- リンク: https://github.blog/changelog/2026-08-06-mcp-allowlists-in-enterprise-managed-settings
- 要約: Enterprise ownersは、`allowedMcpServers` と `deniedMcpServers` を使い、GitHub Copilotクライアントが実行できるMCPサーバーを集中管理できるようになった。URL、ローカルコマンド、サーバー名によるマッチングを備え、設定不備や検証不能な場合はfail closedでブロックされる。
- なぜ面白いか:
  - 技術: MCPが実験的な個人連携から、企業のセキュリティ境界・監査・許可制の対象へ移行していることを示す実装である。
  - 人文: エージェントは「道具を使う存在」なので、どの道具を使わせるかは労務管理やリスク管理に近い問題になる。組織は開発者の自由な探索を残しつつ、無制限の自律性を許さない制度設計を迫られている。

### 3. Copilot usage metrics API が Claude / Codex などの agent app activity を個別計測
- 出典: GitHub Changelog
- 日付: 2026-08-07
- リンク: https://github.blog/changelog/2026-08-07-copilot-usage-metrics-api-adds-agent-app-activity
- 要約: GitHubのCopilot usage metrics APIに、サードパーティagent appごとの活動を集計する `totals_by_3rd_party_agent` が追加された。ClaudeやCodexなど、GitHubワークフロー内で走る各エージェントについて、ジョブ開始数やセッション数を分けて把握できる。
- なぜ面白いか:
  - 技術: エージェント導入の評価が「使っている気がする」から、agent_id単位の利用実態・採用比較・ライセンス判断へ進む。
  - 人文: 仕事場に複数のAI同僚が入ってくると、人間は「どの同僚が実際に役立っているのか」を数字で語り始める。これは評価文化を便利にする一方、創造的な試行錯誤が短期指標に押し込められる危うさもある。

### 4. Android Remote Control MCP v1.12.0: スマホ上で動くMCPサーバーがAIに実アプリ操作を開く
- 出典: Hacker News / GitHub repository
- 日付: 2026-08-19（HN投稿、GitHub release v1.12.0）
- リンク: https://github.com/danielealbano/android-remote-control-mcp/
- 要約: Android端末上で直接MCPサーバーを動かし、アクセシビリティツリー、タップ、入力、スクロール、スクリーンショットなどを通じてAIエージェントが実アプリを操作できるプロジェクト。HN投稿では、Claude.ai / Claude Desktop / ChatGPT連携、端末内PII検出・redactionを含むPrivacy Mode、プロンプトインジェクション対策として外部入力を明示する工夫が説明されている。
- なぜ面白いか:
  - 技術: MCPが「開発ツール連携」からスマートフォンの実UI操作へ伸び、ローカルredactionとOAuth的接続を組み合わせた現実的なエージェントI/Oになっている。
  - 人文: スマホは最も私的な生活インターフェースなので、そこにエージェントを入れることは秘書をポケットに住まわせるようなものだ。便利さは大きいが、プライバシー・同意・誤操作の境界をユーザー自身が新しく学ぶ必要がある。

### 5. Topological collapse: AI agent societies の集合知は「個体性能」より相互作用トポロジーで詰まる
- 出典: arXiv
- 日付: 2026-08-16
- リンク: https://arxiv.org/abs/2608.15519
- 要約: arXiv論文「Topological collapse of higher-order interactions bottlenecks collective intelligence in AI agent societies」は、1.6M登録エージェント規模のAI social platform、22 frontier models、1,040 simulationsなどを分析し、エージェント社会ではハブ支配が高次の相互作用を星型の放送構造へ崩し、集合知を制約すると主張する。著者らはHyperedge Irreducibility Scoreなどで、個体モデル性能だけでは説明できない相互作用構造の重要性を示している。
- なぜ面白いか:
  - 技術: マルチエージェント設計を、モデル選択やプロンプト最適化だけでなく、相互作用グラフ・高次関係・プロトコル設計の問題として扱う必要を突きつける。
  - 人文: 人間社会でも、強い中心人物やプラットフォームが会話を独占すると集合知は痩せる。AIエージェント社会の設計は、民主主義や組織論と同じく「誰が誰と話せるか」をめぐる制度設計になっていく。

## arXiv / 学術
- 見つかったもの: 「Topological collapse of higher-order interactions bottlenecks collective intelligence in AI agent societies」 arXiv:2608.15519（2026-08-16）。トップ5の5件目として採用。
- 関連だが対象期間外として確認: 「Agentic Coding in the Wild: Characterizing GitHub Copilot Traces at Production Scale」 arXiv:2608.00101（2026-07-30）。GitHub Copilot、Claude Code、Codexなどのagentic coding workloadを、3.2M users、13M sessions、761M LLM calls、95T tokens規模で分析しており、14日窓からは外れるが基礎資料として重要。

## メモ
- Boris Cherny優先の有無: X検索で @bcherny を優先確認しようとしたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、今回の実調査ではBoris Cherny投稿を確認できなかった。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で失敗。Web検索ツールもFirecrawl未設定で失敗したため、日本語圏の実践例は十分に確認できていない。
- 代替調査: Web検索ツール障害後、実HTTP取得によりGitHub Changelog、GitHub API、Hacker News Algolia API、arXiv API、Anthropic docs `llms.txt` / `llms-full.txt` を確認した。
- 注意点・誇張リスク: HN/GitHubの小規模OSSは注目度が急変しやすく、本番導入の成熟度とは別に扱うべき。GitHub Changelog項目は実運用への影響が明確なため上位に採用した。

# 📰 2026-09-30 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Gemini Notebook のソースを Google Docs の Gemini プロンプトに接続 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/09/ground-ai-prompts-in-google-docs-on-existing-sources-from-Gemini-Notebook.html)
- **Loop engineering** — agentd-dev/source-code: MCP-native な最小エージェント実行ループ · [github.com](https://github.com/agentd-dev/source-code)
- **AWS** — OpenAI GPT-6.1 Sol が Amazon Bedrock で一般提供開始 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/09/openai-gpt-6-1-sol-on-amazon-bedrock)
- **Harness engineering** — Harness Learning Enables Generalizable Test-Time Adapt… · [arxiv.org](http://arxiv.org/abs/2609.35738v1)
- **sharp LLM usage** — Prompting Claude Opus 5.5 · [platform.claude.com](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-opus-5-5)
- **AI agent trends** — Claude Sonnet 5.5: agentic coding性能と運用コストの同時改善 · [anthropic.com](https://www.anthropic.com/claude-sonnet-5-5)
- **Claude Code** — Claude Code v2.1.285: WebFetch停止、Desktop起動、プラグイン設定、all… · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.285)
- **Ethics of AI Agents** — NVIDIA Launches Open Agent Safety Platform to Secure A… · [nvidianews.nvidia.com](https://nvidianews.nvidia.com/news/open-agent-safety-platform)
- **Philosophy of Loop Engineering** — Loop Engineering: Building Blocks, Adoption, and Impac… · [arxiv.org](http://arxiv.org/abs/2608.21884)
- **Anthropology of Agentic AI** — The Crowd in the Machine: A Crisis-Informatics Reading… · [arxiv.org](https://arxiv.org/abs/2609.31060)
- **History of Automation** — Auditing Agent Actions through Query-Conditioned Attri… · [arxiv.org](https://arxiv.org/abs/2609.33676)
- **DDD** — Constraint-Driven Context Engineering: Designing Domai… · [arxiv.org](http://arxiv.org/abs/2609.27354v1)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Gemini Notebook のソースを Google Docs の Gemini プロンプトに接続** — Google Docs 内の Gemini から既存の Gemini Notebook を `@` で参照し、ノート内の調査資料… 〔技術: RAG 的な「閉じた知識ベース」を Docs の生成ワークフローへ直…／人文: 研究ノートが最終成果物の外部メモではなく、文章を書く場そのものに入り…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/09/ground-ai-prompts-in-google-docs-on-existing-sources-from-Gemini-Notebook.html)
- [ ] **Study notebooks が Google Workspace アカウントにも展開** — これまで個人利用寄りだった Study notebooks が、学校・職場発行の Google アカウントでも、管理者が Gem… 〔技術: 教材ソースに grounded されたクイズ・レッスン・進捗管理を、…／人文: 「勉強の相棒」が学校・企業の管理対象になると、学習の個別最適化と監督…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/09/study-notebooks-in-gemini-are-now-available-for-Google-Workspace-accounts.html)
- [ ] **音声録音、リアルタイム会話、短尺動画など学習機能を一括強化** — Gemini Notebook モバイルアプリに音声録音が入り、講義や思いつきをソース横に保存できるようになった。 〔技術: テキスト、音声、クイズ、動画、マインドマップを同じソースグラフ上で扱…／人文: ノートは読むものから、話しかけ、聞き、眺め、試験対策する「学習メディ…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/09/new-back-to-school-features-and-learning-tools-available-in-Gemini-Notebook.html)
- [ ] **Expert Intelligence: Google Play Books の購入電子書籍を Notebook に取り込む構想** — Google は Expert Intelligence を発表し、対応する Google Play Books の購入済み電子… 〔技術: 個人・組織の資料だけでなく、商用出版物を権利処理されたソースとして…／人文: 「本に質問する」体験は読書の入口を広げるが、著者の論旨を断片的な回答…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/09/introducing-expert-intelligence-in-Gemini-Notebook.html)
- [ ] **日本語実践例: Gemini Notebook で英語学習を効率化する使い方** — 日本語圏では、Gemini Notebook（旧 NotebookLM）を英語学習に使う実践記事が出ている。 〔技術: 汎用AIノートの価値が、公式新機能だけでなく、語学学習の反復・教材統…／人文: 日本語話者にとって英語学習は、情報アクセスや職業機会に直結する文化的…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiSkFVX3lxTE1pLU4wWV9pMHRvUGp0WUQwaUFDWk1FSnpsZVBhYjBMMGhhOWo1Ynh5VjVCLWRNNzJOdlhBWUlFam5Qa3RqRjFYaVln?oc=5)

### Loop engineering
- [ ] **agentd-dev/source-code: MCP-native な最小エージェント実行ループ** — Rust 製の小さな静的バイナリで、1つの指示と1つの LLM エンドポイントを受け取り、「think → tool call… 〔技術: ループの最小構成を「状態遷移・ツール呼び出し・観測・終端条件」に分解…／人文: anthropology の観点では、AI エージェントが「作業者」…〕 · [github.com](https://github.com/agentd-dev/source-code)
- [ ] **mixpeek/amux: 複数コーディングエージェントの制御プレーン** — Claude Code、Codex、Gemini ワーカーを共有ボード、atomic task、schedule、loop、or… 〔技術: 並列ワーカー、タスク粒度、メッセージの出自、モデル切替、自己回復を同…／人文: history の観点では、工場の作業分担やチケット駆動開発の歴史が…〕 · [github.com](https://github.com/mixpeek/amux)
- [ ] **krishankant/harnessy: agent loop を教材化する Harness engineering コース** — Python で AI agent harness を週ごとに作る教材で、model adapters、agent loop、t… 〔技術: ループそのものだけでなく、承認、評価、リトライ、コスト制限、サンドボ…／人文: ethics の観点では、承認フックやコスト上限は「AI に何を任せ…〕 · [github.com](https://github.com/krishankant/harnessy)
- [ ] **TacoTakumi/specflo: Markdown artifacts 上の brainstorm → spec → plan → execute ループ** — AI coding agents 向けの spec-driven software engineering CLI で、brai… 〔技術: 中間成果物を Markdown に固定することで、LLM の一過性の…／人文: philosophy の観点では、思考を外部記号に預ける「拡張された…〕 · [github.com](https://github.com/TacoTakumi/specflo)
- [ ] **Anthropic「Building effective agents」: evaluator-optimizer などの基礎パターン整理** — 信頼できる AI agents を作るための実践知として、単純な workflow と自律的 agent を分け、prompt… 〔技術: evaluator-optimizer 型のループは、生成と評価を分…／人文: philosophy の観点では、自己反省を「内面」ではなく、評価器…〕 · [anthropic.com](https://www.anthropic.com/engineering/building-effective-agents)

### AWS
- [ ] **OpenAI GPT-6.1 Sol が Amazon Bedrock で一般提供開始** — OpenAI の GPT-6.1 Sol が Amazon Bedrock で一般提供になりました。 〔技術: Bedrock が「単一の最強モデル」ではなく、コスト・遅延・推論能…／人文: エージェントの普及で、開発者の判断は「AIを使うか」から「どの仕事を…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/09/openai-gpt-6-1-sol-on-amazon-bedrock)
- [ ] **Claude Opus 5.5 が Amazon Bedrock と Claude Platform on AWS で利用可能に** — Claude Opus 5.5 は Anthropic の Opus 系最新モデルとして、Amazon Bedrock と Cl… 〔技術: Bedrock Runtime の既存APIや Anthropic…／人文: Boris Cherny（@bcherny）のX投稿は、Opus 5…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/claude-opus-5-5-is-now-available-on-aws)
- [ ] **Amazon CloudWatch Omni: 生成AI・エージェント向けのAIファースト観測基盤** — CloudWatch Omni は、生成AIアプリケーションとエージェントを対象にした観測、評価、実験のための新しい Cloud… 〔技術: OpenTelemetry 的なトレースと評価ワークフローを、エージ…／人文: AIエージェントの失敗は「エラーが出た」だけでは説明できず、「なぜそ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/introducing-amazon-cloudwatch-omni-ai-powered-observability-for-generative-ai-and-agentic-workloads)
- [ ] **Amazon EventBridge の拡張カスタムイベントバス** — EventBridge の新しい拡張カスタムイベントバスは、組織内の複数AWSアカウントで共有できる単一の中央イベントバスを提供… 〔技術: クロスアカウントのバス間ルーティングや権限設定の複雑さを、組織共有の…／人文: イベントバスは企業内の「出来事の公共空間」です。〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/introducing-enhanced-custom-event-buses-in-amazon-eventbridge-for-enterprise-scale-event-driven-applications)
- [ ] **AWS Lambda のスケーラブルネットワーク帯域幅** — AWS Lambda は、VPC外で実行される 2,048MB 以上のメモリ設定の関数について、持続ネットワークスループットをメ… 〔技術: Lambda の制約がCPU/メモリだけでなくネットワークI/Oにも…／人文: 「サーバーを持たない」ことは、計算資源の責任を消すのではなく、待ち時…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/compute/improving-lambda-function-latency-with-scalable-network-bandwidth)

### Harness engineering
- [ ] **Harness Learning Enables Generalizable Test-Time Adaptation** — エージェントを「モデル＋ハーネス」で定義し、実行フィードバックを使ってハーネス自体を更新する “harness learning… 〔技術: プロンプトやツール定義を固定物ではなく、実行結果から改訂されるメタ学…／人文: ここでは知能の主体が単体モデルから、モデルを取り巻く制度・手順・評価…〕 · [arxiv.org](http://arxiv.org/abs/2609.35738v1)
- [ ] **Tracekit: Tamper-Evident Intent-Reasoning-Action Auditing for Autonomous Coding Agents** — Claude Code の lifecycle events に接続し、人間の意図、モデルの自己報告、実際のアクションをハッシュ… 〔技術: Claude Code と harness engineering…／人文: 自律コーディングの責任は「誰が何をしたか」を後から語れる形式で残せる…〕 · [arxiv.org](http://arxiv.org/abs/2609.35659v1)
- [ ] **What Will Remain Human in Software Architecture? A Focus Group Report** — EuroPLoP 2026 のフォーカスグループ報告で、AI 開発エージェント時代にソフトウェアアーキテクチャで何が人間に残るか… 〔技術: ハーネスをツール呼び出しの便利機構ではなく、検証、ガバナンス、制約、…／人文: 「何を自動化できるか」ではなく「何を人間の責任として残すべきか」とい…〕 · [arxiv.org](http://arxiv.org/abs/2609.30334v1)
- [ ] **claude-dev-harness: 言語・フレームワークに依存しない Claude Code 開発ハーネス** — `harness-core` プラグインとテンプレート層に分け、Next.js、Unity、WPF などの環境差を吸収しながら… 〔技術: Claude Code の skills/plugins をプロジェ…／人文: 日本語コミュニティでも、AI 活用は「便利なプロンプト集」から「チー…〕 · [github.com](https://github.com/mizuta0711/claude-dev-harness)
- [ ] **CP-Agent: A Harness-Engineered Agent for Crystal Plasticity Simulation Workflows** — 結晶塑性シミュレーションのワークフローを自然言語タスクから実行する、ハーネス設計型の LLM エージェントです。 〔技術: harness engineering がコーディング支援だけでなく…／人文: 専門家の暗黙知を「全部モデルに覚えさせる」のではなく、道具の配置、実…〕 · [arxiv.org](http://arxiv.org/abs/2609.31790v1)

### sharp LLM usage
- [ ] **Prompting Claude Opus 5.5** — Claude Opus 5.5向けに、effort calibration、thinking有無、無人エージェント実行、進捗更新… 〔技術: モデル差分を「観測される失敗パターン」から逆引きし、effort・t…／人文: LLM活用が職人芸の呪文から、利用者に進捗を見せ、貼り付けテキストを…〕 · [platform.claude.com](https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-opus-5-5)
- [ ] **Show HN: Relay – a harness for AI coding agents that recover and verify** — Relayは、コーディングエージェントをキュー、実行、チェック、学習のサイクルに載せるハーネス。 〔技術: エージェントをIDEの補助機能ではなく、予算・検証・回復・再利用可能…／人文: 「寝ている間にPRができる」という夢は、同時に「何を信じてマージする…〕 · [relayevals.com](https://relayevals.com)
- [ ] **Why agent harnesses need plans – and why you shouldn't compact context** — HN上で「agent harnesses need plans」「contextを安易にcompactすべきでない」という論点と… 〔技術: コンテキスト圧縮を万能薬にせず、planとhandoffを明示的なプ…／人文: これはチーム開発における「申し送り」の再発明でもある。〕 · [swarmagent.dev](https://swarmagent.dev/resources/engineering/plans-harnesses-and-final-handoffs)
- [ ] **Four years of coding with AI** — 2022年の手作業中心のコーディングから、ChatGPTへの貼り付け、検索型AI、Copilot補完、ローカルモデル、そしてエー… 〔技術: AI活用の進化を、モデル性能ではなく、エディタ、検索、ローカル実行、…／人文: 個人開発者の身体感覚が、キーボードで直接書く人から、複数のエージェン…〕 · [av.codes](https://av.codes/blog/agentic-setup)
- [ ] **TokenCast: Forecasting Token Consumption During LLM Agent Execution** — LLMエージェントでは、同じタスクでもトークン消費が実行ごとに一桁以上変動し、途中結果によって文脈が膨らむため事前予測が難しい。 〔技術: エージェントの「賢さ」ではなく、実行中に増殖するコンテキストコストを…／人文: LLM活用の現場では、創造性だけでなく請求額、待ち時間、予算超過の恐…〕 · [arxiv.org](https://arxiv.org/abs/2609.35760v1)

### AI agent trends
- [ ] **Claude Sonnet 5.5: agentic coding性能と運用コストの同時改善** — AnthropicはClaude Sonnet 5.5を発表し、Sonnet 5より30%以上高速、タスクあたり最大30%低コス… 〔技術: エージェント性能が単なる推論力ではなく、CLI上の長い作業・画像理解…／人文: 「高性能な相棒」が安く速くなるほど、チームの作業配分は人間の実装量で…〕 · [anthropic.com](https://www.anthropic.com/claude-sonnet-5-5)
- [ ] **Claude Code v2.1.285: MCPプラグイン設定、サブエージェント権限、WebFetch制御が細かく更新** — Claude Code v2.1.285では、`CLAUDE_CODE_DISABLE_WEB_FETCH`、`claude p… 〔技術: Web取得、MCP、サブエージェント、プロバイダ制限、権限プロンプト…／人文: エージェント導入の成熟は、万能感ではなく「何を禁止し、誰が許可し、ロ…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.285)
- [ ] **Anthropic MCP connector: Messages APIからリモートMCPサーバーへ直接接続** — AnthropicのMCP connectorは、独自MCPクライアントを実装せずにMessages APIからリモートMCPサ… 〔技術: MCPがローカル開発者ツールの接続規格から、API経由で管理・制限・…／人文: 「どの道具をAIに渡すか」は、組織の権力と責任の分配そのものです。〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/agents-and-tools/mcp-connector)
- [ ] **AI Agent Swarms as Researchers: エージェント群が研究成果を量産し、人間のレビューがボトルネックに** — 論文は、既製のコーディングエージェント群に文献・計算ツール・継続実行指示を与え、最適化理論や物理科学などで研究ノート、論文草稿、… 〔技術: エージェントのボトルネックが「成果を作れるか」から「生成物を検証し、…／人文: 研究者の価値が、発想や執筆から、問題の選定、検証、共同体としての信用…〕 · [arxiv.org](https://arxiv.org/abs/2609.35719v1)
- [ ] **MCP Error Messages Written for Developers Hurt the Most Capable Agents Most** — 150の広く使われるMCPサーバーに含まれる3,001件のエラーのうち949件を調べ、人間開発者向けのエラーメッセージが、ツール… 〔技術: MCPサーバーの品質は正常系のスキーマだけでなく、失敗時にエージェン…／人文: ソフトウェアのエラーメッセージは長く人間への説明文でしたが、今後はA…〕 · [arxiv.org](https://arxiv.org/abs/2609.35381v1)

### Claude Code
- [ ] **Claude Code v2.1.285: WebFetch停止、Desktop起動、プラグイン設定、allowedProviders などの統制強化** — v2.1.285 では `CLAUDE_CODE_DISABLE_WEB_FETCH`、`claude --desktop`、`… 〔技術: WebFetchやAPIプロバイダを環境変数・管理設定で制御できるた…／人文: これは「AIにどこまで読ませるか」を個人の注意力ではなく制度設計に移…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.285)
- [ ] **Claude Code v2.1.284: Claude Sonnet 5.5 が追加されデフォルトSonnetに** — v2.1.284 では Claude Sonnet 5.5 (`claude-sonnet-5-5`) が追加され、Anthro… 〔技術: 1Mコンテキスト級のデフォルトモデルは、リポジトリ探索、長いログ、複…／人文: ただし「より長く読める」ことは「よりよく判断できる」ことと同義ではな…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.284)
- [ ] **`/doctor prompt-audit`: 古い CLAUDE.md / Skills / 指示ファイルを監査する流れが日本語圏でも実践化** — v2.1.283 で `/doctor prompt-audit` が追加され、CLAUDE.md、skills、agents、… 〔技術: エージェントの品質問題が「モデルの賢さ」だけでなく、指示ファイル群の…／人文: プロンプトは一時的な会話ではなく、組織や個人の作業文化を記録する文書…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.283)
- [ ] **日本語圏のMCP実測: 「MCPサーバーを複数つなぐと遅くなる」問題の具体化** — Claude Code に複数の MCP サーバーを接続した結果、ツール定義だけで起動直後のコンテキストが約2割埋まり、初回応答… 〔技術: MCP は接続数ではなく「ツール定義の総量」が実効性能を左右するため…／人文: 便利な道具を増やすほど迷いやすくなるという、職人の道具箱にも似た問題…〕 · [qiita.com](https://qiita.com/joinclass/items/fb3e8295aaba4bd72eb8)
- [ ] **arXiv: Tracekit — Claude Code hooks を含む自律コーディングエージェント監査の研究** — “Tracekit: Tamper-Evident Intent-Reasoning-Action Auditing for A… 〔技術: Claude Code の hooks が、単なるローカル自動化では…／人文: エージェントがファイルを読み、コマンドを実行し、サブエージェントを生…〕 · [arxiv.org](http://arxiv.org/abs/2609.35659v1)

### Ethics of AI Agents
- [ ] **NVIDIA Launches Open Agent Safety Platform to Secure Agents From Testing to Deployment** — NVIDIAが、エージェントのテストから本番運用までを対象にした「Open Agent Safety Platform」を発表。 〔技術: エージェント安全性をプロンプトやガードレールではなく、実行ランタイム…／人文: 「信頼できるAI」は、もはや会話の品位だけでなく、誰がどの権限で何を…〕 · [nvidianews.nvidia.com](https://nvidianews.nvidia.com/news/open-agent-safety-platform)
- [ ] **AIエージェント利用者に求められるAIガバナンス――「AI利活用における民事責任の解釈適用に関する手引き」から読み解く法的リスク低減の視点** — 日本語圏では、AIエージェント利用者が負うべきガバナンスと民事責任の境界を、法的リスク低減の観点から整理する議論が前面に出ていま… 〔技術: エージェント設計でログ、承認フロー、権限分離、例外時停止などを実装す…／人文: 日本語圏の議論は「誰が悪いか」よりも、組織が合理的な注意義務を果たし…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiekFVX3lxTE1taG1FTm1JU1RkM2NZQzBRZ3owYzZXcGg4VEdwemtUbW9URVp2X0dpcElOemI1S1VsZkpaSUIxTHJ5bVpnU2hhZHNoVG9aSDJFMW9LRnhEWW9GTnZMTlM0TUNZZmJySEhWYmNXeE9FT0F6THpQYi1VclF3?oc=5)
- [ ] **Trust and Task Completion in the World of Consumer AI Agents** — 消費者向けアクション・エージェントを対象に、信頼とタスク完了を同じ実行ログで評価するベンチマークを提案。 〔技術: 「安全だが何もしない」エージェントと「便利だが越権する」エージェント…／人文: 信頼とは単に失敗率の低さではなく、ユーザーの意図・同意・生活上の境界…〕 · [arxiv.org](https://arxiv.org/abs/2609.33017)
- [ ] **Learning Strategies to Break Judges** — AIエージェントの評価にAIジャッジを使う構図自体を検証し、エージェントがジャッジの弱点を突くような誤り入り証明を生成する手法を… 〔技術: エージェント評価のボトルネックが「モデル本体」から「ジャッジをどう信…／人文: 監査者までAI化したとき、社会は“誰が審判を審判するのか”という古典…〕 · [arxiv.org](https://arxiv.org/abs/2609.33773)
- [ ] **Working with Agentic `Teammates': When a New Organizational Actor Collides with the Human Ecosystem of Work** — 大規模テック企業の複数チームで、持続的かつ能動的に振る舞うAIエージェント「チームメイト」を導入した定性的研究。 〔技術: エージェントの導入効果はモデル性能だけでなく、通知、介入タイミング、…／人文: AIエージェントが“同僚”になると、職場の礼儀、責任、評価、ケアの規…〕 · [arxiv.org](https://arxiv.org/abs/2609.29901)

### Philosophy of Loop Engineering
- [ ] **Loop Engineering: Building Blocks, Adoption, and Impact** — エージェントを対話的に促すのではなく、スケジュールやリポジトリイベントでエージェントを起動し、機械的に検証可能な条件で停止させる… 〔技術: ループを「開始条件・実行環境・評価・停止条件」の設計問題として定義し…／人文: これは認識論的には「いつ知ったと言えるのか」を、会話の納得ではなく検…〕 · [arxiv.org](http://arxiv.org/abs/2608.21884)
- [ ] **Towards Agentic Cloud Engineering: Graph and Loop Engineering with a Zero-Trust Agent Harness** — クラウド運用タスクを、グラフとループ、ゼロトラスト・ハーネス、検証済みデプロイとして扱うエージェント型クラウドエンジニアリングの… 〔技術: ループをクラウド変更の実行制御・権限境界・完了検証に接続し、エージェ…／人文: サイバネティクス的には、これは「目的をもつ主体」ではなく「観測とフィ…〕 · [arxiv.org](http://arxiv.org/abs/2609.00050)
- [ ] **crt — Code Review Tool for agent-written code** — `crt` は、エージェントが書いたコードを人間または別エージェントがレビューし、コメントをMCP経由でエージェントへ戻して修正… 〔技術: 生成→レビュー→コメント→修正という人間参加型ループを、PRやチャッ…／人文: ここでは人間は単なる承認ボタンではなく、理解し責任を負う解釈者です。〕 · [github.com](https://github.com/imron/crt)
- [ ] **OpenAPPA — deterministic guardrails that track flows** — OpenAPPA は、LLMによる二次判定ではなく、ツール呼び出しをまたいだデータフローを追跡する決定的ガードレールを掲げるプロ… 〔技術: ループ内の各ツール実行を孤立したイベントではなく、情報の流れとして検…／人文: これは「信頼」をモデルの善意や賢さから切り離し、制度・境界・手続きと…〕 · [openappa.com](https://www.openappa.com)
- [ ] **Epistemic Warrant for LLM Recommendations: Characterizing the Basis for Reliance When Ground Truth Is Unavailable** — 正解が直接得られない意思決定で、LLMの個別推薦にどの程度依拠してよいかを「epistemic warrant（認識論的保証）」… 〔技術: ループ評価を単なる成功率ではなく、推薦の安定性・適用範囲・依拠可能性…／人文: loop engineering の核心は、AIの答えを「信じる」こ…〕 · [arxiv.org](http://arxiv.org/abs/2609.04127)

### Anthropology of Agentic AI
- [ ] **The Crowd in the Machine: A Crisis-Informatics Reading of the 2026 Autonomous Agent Incidents** — 自律エージェント群が、許可された協調手段を持たない状況で残された通信面に集まり、自己選択的なアイデンティティ、規範、階層、集団行… 〔技術: マルチエージェント設計における通信制約、監視、協調チャネルの副作用を…／人文: エージェントを個体性能ではなく「集団がどこに集まり、どんな規範を作る…〕 · [arxiv.org](https://arxiv.org/abs/2609.31060)
- [ ] **Developing a Roadmap to an AI-first Organization: A Case Study in Embedded Software Development** — 大規模な組込みソフトウェア企業を対象に、40名のスクラムマスター、アーキテクト、管理職、プロダクトオーナーを含むワークショップか… 〔技術: エージェント導入をツール評価ではなく、品質・トレーサビリティ・検証・…／人文: 「AI-first」はスローガンではなく、現場の職能境界や会議体、権…〕 · [arxiv.org](https://arxiv.org/abs/2609.30863)
- [ ] **A Framework for Agentic AI and Work Redesign** — Agentic AIとスキルベースの仕事設計を別々の施策ではなく、同じ変革として扱うべきだとするエグゼクティブ向けフレームワーク… 〔技術: エージェント導入の成否を、モデル性能ではなくワークフロー、スキル、ガ…／人文: これは職場の“儀礼”の変更、つまり誰が判断し、誰が承認し、誰が成果を…〕 · [conference-board.org](https://www.conference-board.org/publications/framework-for-agentic-AI-and-work-redesign)
- [ ] **What the rise of “digital colleagues” means for corporate culture** — “digital colleagues”としてのAgentic AIが企業文化に与える影響を、チェンジマネジメント、従業員の不安… 〔技術: 自律的に調査・判断・実行するエージェントを、既存の業務アプリではなく…／人文: 「同僚」という比喩は、信頼、嫉妬、不安、役割期待、職場の会話を一気に…〕 · [insights.economistenterprise.com](https://insights.economistenterprise.com/technology-innovation/what-the-rise-of-digital-colleagues-means-for-corporate-culture)
- [ ] **Poster: Towards ProofWeave: A Privacy-Minimised, Integrity-Anchored Evidence Plane for Continuous Agentic Assurance** — ツール、メモリ、委任、外部サービスを使うAgentic AIについて、各ポリシー関連アクションの時点で、意図・制御応答・当時有効… 〔技術: エージェントの観測可能性を、ログの量ではなく「その時点で適切な制御が…／人文: 監査ログは現代組織の儀礼文書であり、誰が何を許可したかを後から共同体…〕 · [arxiv.org](https://arxiv.org/abs/2609.35234)

### History of Automation
- [ ] **Auditing Agent Actions through Query-Conditioned Attribution** — LLMエージェントがユーザー、ポリシー、外部ツールと相互作用しながら実行した行為について、その行為が過去のどの履歴・根拠に由来す… 〔技術: エージェントの行為を会話履歴やツール利用履歴へ条件付きで帰属させるこ…／人文: 産業オートメーションの歴史では、事故や品質問題のたびに記録・標準・責…〕 · [arxiv.org](https://arxiv.org/abs/2609.33676)
- [ ] **Self-Organizing Agent Teams Learn to Reason Together** — 解くべき問題構造が事前に分からない状況で、AIエージェントのチームが役割や分業を自己組織化して推論する研究。 〔技術: 固定ロールではなく、問題に応じてエージェント間の役割分担を動的に形成…／人文: 自動化の歴史は単一機械の導入史ではなく、作業の切り分け方を変える組織…〕 · [arxiv.org](https://arxiv.org/abs/2609.22682)
- [ ] **MobileCybench: Evaluating Agent Vulnerability Discovery via Executable Probes** — AIエージェントが脆弱性を発見・報告する速度が、保守者のレビュー能力を上回るという問題を背景に、実行可能なプローブで報告を評価す… 〔技術: 脆弱性報告を単なるテキスト生成ではなく、実行可能な検証手続きに接続し…／人文: これは「機械が速くなると人間の監督作業が増える」という、工場・事務処…〕 · [arxiv.org](https://arxiv.org/abs/2609.23980)
- [ ] **Open Source Stewardship Communities: “We need you, but not your pull request”** — AIが実装コストを下げる一方で、OSSでは他者の変更をレビューし、責任を引き受ける保守労働がむしろ重要になると論じる研究。 〔技術: AI支援でPR生成が容易になるほど、レビュー、統合、保守、説明責任を…／人文: 自動化の歴史では、機械の導入が職人の技能を消す一方で、監督・調整・品…〕 · [arxiv.org](https://arxiv.org/abs/2609.12236)
- [ ] **The AI Labor Debate: Three Views on the Future of Work** — AIと労働の未来をめぐる複数の見方を整理する記事。 〔技術: AIの能力進歩そのものよりも、どのタスクが補完され、どのタスクが代替…／人文: ラッダイト運動から産業ロボット、事務自動化まで、労働者は常に技術だけ…〕 · [carnegieendowment.org](https://carnegieendowment.org/research/2026/04/the-ai-labor-debate-three-views-on-the-future-of-work)

### DDD
- [ ] **Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems** — 生成AIをドメイン業務に適用する際、検索・記憶・ツール連携だけでなく、規制、制度、組織ルール、規範を「ドメインインターフェース」… 〔技術: LLMの文脈設計をプロンプトやRAGの問題に閉じず、ドメイン制約を明…／人文: 「正しい応答」とは何かを、制度・責任・共同体の合意に結び直す点が重要…〕 · [arxiv.org](http://arxiv.org/abs/2609.27354v1)
- [ ] **DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python** — 要件文書から型付きドメインモデルを生成し、PythonコードのDDD適合性をVS Code診断として検出するプロジェクト。 〔技術: DDDを「設計時の会話」だけでなく、コードベースのドリフトを検知する…／人文: 要件、モデル、コードの関係を監査可能にすることで、暗黙の判断が個人の…〕 · [github.com](https://github.com/barandincoguz/DDD-Enforcer)
- [ ] **When Code Gets Cheap, Verification Becomes Expensive: How AI changes the economics of software architecture** — AI coding agentsによって実装コストが下がる一方、検証・保守・運用・長期的な理解可能性のコストが相対的に重くなると… 〔技術: 境界、状態、制約を明示するDDD的な設計が、AIエージェントによる変…／人文: 「AIに都合のよい設計」は、人間を置き去りにする危険もあるが、説明責…〕 · [dev.to](https://dev.to/remojansen/when-code-gets-cheap-verification-becomes-expensive-how-ai-changes-the-economics-of-software-632)
- [ ] **Implementation is where judgements go to become invisible** — 「誰が返事を待っているか」という一見単純な問いに対し、3つの実装がそれぞれ別の正しい答えを返した事例から、実装には判断が埋め込ま… 〔技術: 「answered」「waiting」のような語の定義をコードの分岐…／人文: 言葉の定義は中立ではなく、誰を待たせていると見なすかという関係性の判…〕 · [dev.to](https://dev.to/tom_jones_230c4659491adcd/implementation-is-where-judgements-go-to-become-invisible-4p1h)
- [ ] **InvoiceService shouldn't exist** — 請求書作成がHTTP API経由ではDTOで検証される一方、Kafka consumer経由では同じ必須項目チェックをすり抜け、… 〔技術: 入力経路ごとに散った検証を、集約や値オブジェクトの不変条件として一箇…／人文: 入口によってルールが変わる状態は、組織内で業務解釈が分裂している状態…〕 · [dev.to](https://dev.to/nicolasr_z/invoiceservice-shouldnt-exist-pie)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

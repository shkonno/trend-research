# 📰 2026-08-06 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMがGemini Notebookへ改称、既存ノートは継続利用可能 · [notebooklm.google](https://notebooklm.google/?hl=ja)
- **Loop engineering** — LoopsBench: From Harness Engineering to Loop Engineeri… · [arxiv.org](https://arxiv.org/abs/2608.00267)
- **AWS** — Amazon DynamoDB now supports real-time vector search a… · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale)
- **Harness engineering** — numbat: AIエージェント活動を端末側で監視・ブロック・フォレンジック化 · [github.com](https://github.com/perplexityai/numbat)
- **sharp LLM usage** — Context Engineering for Agents: A Practical Guide · [blog.malt.engineering](https://blog.malt.engineering/dont-take-this-out-of-context-feeding-your-llm-exactly-what-it-needs-0db8a86d2151)
- **AI agent trends** — agentacct: コーディングエージェントの作業・費用・トークンをローカルで可視化 · [github.com](https://github.com/mikehasa/agentacct)
- **Claude Code** — Claude Code 2.1.222: worktree 隔離と auto mode 安全性の修正 · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- **Ethics of AI Agents** — Accountability Asymmetry and Structural Trust in Auton… · [arxiv.org](https://arxiv.org/abs/2608.03670)
- **Philosophy of Loop Engineering** — Reframing AI Loss of Control: What Control Is, How to… · [arxiv.org](http://arxiv.org/abs/2606.12442)
- **Anthropology of Agentic AI** — An Exploratory Study of Agent Plans for Agentic AI Cod… · [arxiv.org](https://arxiv.org/abs/2608.04661)
- **History of Automation** — Navigating the skill diversity frontier: How skill com… · [arxiv.org](https://arxiv.org/abs/2608.02102)
- **DDD** — faceto: typed fileからLLMと議論できるEvent Stormingボードへ · [github.com](https://github.com/bastien-gallay/faceto)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMがGemini Notebookへ改称、既存ノートは継続利用可能** — Google公式ページでは、2026年7月よりNotebookLMがGemini Notebookになったこと、既存ノートブック… 〔技術: プロダクト名の変更は、RAG的なソース読解ツールをGemini全体の…／人文: 「ノートブック」という比喩が残りつつGeminiブランドへ吸収される…〕 · [notebooklm.google](https://notebooklm.google/?hl=ja)
- [ ] **Geminiアプリからノートブックを表示・編集・チャット可能に** — Gemini Notebookで作成したノートブックがGeminiのナビゲーションに自動表示され、Gemini Notebook… 〔技術: ノート、ソース、カスタム指示、会話履歴をアプリ横断で同期することで、…／人文: これは「会話」が単なる一時的なやり取りではなく、あとから参照される研…〕 · [support.google.com](https://support.google.com/gemininotebook/answer/17003757?hl=ja)
- [ ] **動画解説・スライド・インフォグラフィック・クイズなど、Studio系アウトプットが拡張** — 公式ヘルプには、動画解説、フラッシュカードやクイズ、インフォグラフィック、スライド資料、マインドマップなどの生成機能がまとまって… 〔技術: 同じソース集合から、対話・音声・動画・図解・スライド・テストを生成す…／人文: 読む、聴く、見る、発表する、試験するという学習行為が、一つのAIノー…〕 · [support.google.com](https://support.google.com/notebooklm/?hl=ja)
- [ ] **日本語圏で「Gemini Notebook」完全入門・企業活用・コード実行の解説が増加** — 日本語記事では、NotebookLMからGemini Notebookへの改称、新機能、Geminiアプリ統合、無料/Pro/U… 〔技術: 日本語実務層の関心が「便利な要約ツール」から、コード実行・ファイル生…／人文: 日本語での入門記事が増えることは、ツールの普及が英語圏の先端ユーザー…〕 · [ai-revolution.co.jp](https://ai-revolution.co.jp/media/what-is-gemini-notebook)
- [ ] **PHITS向けAI支援ワークフローでNotebookLMを知識ベースとして利用** — 論文「Toward AI-Agent-Driven Particle Transport Simulations」では、粒子輸送… 〔技術: ドメイン固有ソフトウェアの周辺資料をRAG知識ベース化し、実行系エー…／人文: これは専門知が「人に弟子入りして覚えるもの」から「資料パッケージとし…〕 · [arxiv.org](https://arxiv.org/abs/2607.11309v1)

### Loop engineering
- [ ] **LoopsBench: From Harness Engineering to Loop Engineering in Benchmarking Coding Agent** — 長期のソフトウェア開発タスクを、依存関係DAGと段階的に解放されるテストで評価するベンチマーク。 〔技術: coding agent 評価を「最終成果物」ではなく、ready…／人文: ethics の観点では、エージェントの成功宣言を鵜呑みにせず、長期…〕 · [arxiv.org](https://arxiv.org/abs/2608.00267)
- [ ] **Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control** — 「reviewed」「tested」「DONE」「ready-to-merge」といったライフサイクル状態を、エージェントの自己… 〔技術: lifecycle transition を evidence ga…／人文: philosophy の観点では「信頼」と「証明」を区別し、AIの発…〕 · [arxiv.org](https://arxiv.org/abs/2607.14890)
- [ ] **108 PRs in eight days: Accidentally discovering loop engineering** — 8日で108件のPRを作ったという実践報告がHacker Newsで議論を呼んだ。 〔技術: 大量PR生成は agentic coding loop のスループッ…／人文: anthropology の観点では、開発者コミュニティが「速さ」を…〕 · [brittany-ellich.offprint.app](https://brittany-ellich.offprint.app/a/3mrjj34puva23-108-prs-in-eight-days-accidentally-discovering-loop-engineering)
- [ ] **Stop Prompting, Start Looping** — HNで共有された「プロンプトを重ねるのではなく、ループを設計する」という実践記事。 〔技術: prompt engineering を一回の入力最適化から、検証・…／人文: history の観点では、手作業の指示書から標準作業手順書へ移った…〕 · [lanes.sh](https://lanes.sh/blog/loop-engineering-with-lanes)
- [ ] **cobusgreyling/loop-engineering** — AI coding agent 向けの loop engineering パターン、スターター、CLI群をまとめたリポジトリ。 〔技術: ループを抽象論ではなく、監査・初期化・コスト計測という開発者が実行で…／人文: ethics の観点では、コストや停止条件を見える化することは、自律…〕 · [github.com](https://github.com/cobusgreyling/loop-engineering)

### AWS
- [ ] **Amazon DynamoDB now supports real-time vector search at any scale** — DynamoDBがネイティブなリアルタイム・ベクトル検索を一般提供し、単一桁ミリ秒レイテンシ、99%以上のリコール、最大で兆単位… 〔技術: 低レイテンシのキー・バリュー/ドキュメントDBにベクトル索引が入るこ…／人文: 「記憶」を専用の実験的ストアではなく、既存の業務台帳に隣接させる動き…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale)
- [ ] **Introducing Web Search on Amazon Bedrock for foundation model grounding** — Amazon BedrockでWeb Searchが一般提供され、サーバーサイドの組み込みツールとしてモデル応答を最新Web情報… 〔技術: 検索・取得・引用の接地をアプリ側で寄せ集めるのではなく、Bedroc…／人文: AIの「知っているふり」を減らすには、能力そのものよりも情報源との関…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-web-search-on-amazon-bedrock-for-foundation-model-grounding)
- [ ] **How we built an MCP bridge to give our AgentCore-hosted AI agent access to local MCP tools** — Amazon Bedrock AgentCore上のクラウドホスト型AIエージェントから、ユーザーのローカルMCPツールやファイ… 〔技術: AgentCore、MCP、署名付き接続を組み合わせることで、クラウ…／人文: エージェントが「どこで働くのか」という問題は、単なるネットワーク設計…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/how-we-built-an-mcp-bridge-to-give-our-agentcore-hosted-ai-agent-access-to-local-mcp-tools)
- [ ] **AWS Lambda announces scalable network bandwidth up to 3,000 Mbps for functions outside a VPC** — VPC外のLambda関数で、実行環境あたり最大3,000 Mbpsまでスケールするネットワーク帯域が告知されました。 〔技術: サーバーレスが軽量イベント処理だけでなく、データ転送量の多いAI/E…／人文: インフラの制約が見えなくなるほど、開発者は「関数」という小さな抽象で…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/aws-lambda-network-bandwidth)
- [ ] **1つのエージェントで、あらゆるクライアントに: Kiro エージェントハーネスをどう構築したか** — Kiro IDE、CLI、Webに分かれていたエージェントを、単一のKiroエージェントハーネスへ統合した設計が日本語で解説され… 〔技術: IDE/CLI/Webをまたぐ同一エージェント実行基盤と権限モデルは…／人文: 日本語コミュニティ向けにこのレベルの内部設計が共有されている点が重要…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/one-agent)

### Harness engineering
- [ ] **numbat: AIエージェント活動を端末側で監視・ブロック・フォレンジック化** — Perplexity の `numbat` は、Claude Code / Codex などのエージェント活動をローカルフック、… 〔技術: エージェントの「発話」ではなく、フック・ログ・ファイル痕跡を観測対象…／人文: これはAIを共同作業者として信頼するための監視社会化ではなく、責任の…〕 · [github.com](https://github.com/perplexityai/numbat)
- [ ] **Claude Code Safety Harness: bypassPermissionsを“YOLO”ではなくサンドボックス付きで使う** — `claude-safety-harness` は Claude Code の `--dangerously-skip-perm… 〔技術: hook だけでは防げない任意サブプロセスをOSサンドボックスで、O…／人文: 自律エージェント利用の心理は、便利さが増すほど境界を緩めたくなる方向…〕 · [github.com](https://github.com/jonnyeclectic/claude-safety-harness)
- [ ] **Agent Arena: Claude Code / Codex / Gemini CLIを同じタスクで戦わせる評価ハーネス** — `agentarena` は2つの coding agent に同じリポジトリ課題を解かせ、パッチ検証、実行可能な攻撃テスト、修… 〔技術: 単なるLLM-as-judgeではなく、攻撃テストと再現確認を含む「…／人文: AI開発は「どのモデルを信じるか」から「どの提案を採用する儀式を設計…〕 · [github.com](https://github.com/JDKrasnick/agentarena)
- [ ] **日本語圏の Claude Code test gate: Stop hookで“テスト未実行の完了報告”を止める** — `claude-code-test-gate` は、Claude Code の `PostToolUse(Edit|Write)… 〔技術: 編集ファイルから対象ラベルとテストコマンドを対応付け、Stop時に未…／人文: 日本語圏でも、AIへのお願い文ではなく作業規範をコード化する流れがは…〕 · [github.com](https://github.com/Shotaro-Yoshinaga-sti/claude-code-test-gate)
- [ ] **PRWeaver: 長期・分割された悪意あるPRに対するLLMコード監査ベンチマーク** — `PRWeaver` は、実リポジトリ10件から208件の実行検証済み攻撃を作り、4種類のレビュー表現で計832レンダリングを評… 〔技術: ハーネスが「正解パッチを通す」だけでなく、履歴・文脈・PR単位の見せ…／人文: 悪意は単発の黒い差分ではなく、もっともらしい物語の中に埋め込まれる。〕 · [arxiv.org](https://arxiv.org/abs/2608.02693)

### sharp LLM usage
- [ ] **Context Engineering for Agents: A Practical Guide** — 「LLMに全部渡す」のではなく、エージェントがその時点で必要とする情報だけを供給する実践としてのコンテキスト設計が前面に出ている… 〔技術: 長いプロンプトの巧拙より、検索・要約・状態管理・不要情報の排除を含む…／人文: 人間の仕事でも「何を伝えないか」は熟練の一部であり、AIとの協働でも…〕 · [blog.malt.engineering](https://blog.malt.engineering/dont-take-this-out-of-context-feeding-your-llm-exactly-what-it-needs-0db8a86d2151)
- [ ] **Rudder: Measure your own input on AI generated code** — RudderはClaude CodeやCodex向けのローカルプラグインで、セッション履歴中のプロンプトに直接ひもづく単体テスト… 〔技術: 「AIが書いたコードを眺める」から「自分のプロンプトが満たすべきテス…／人文: これは作者性の測定でもある。〕 · [github.com](https://github.com/RudderCode/Rudder)
- [ ] **Armature: Analytics and evals for your MCP** — ArmatureはClaude Connector、ChatGPT App、MCPなどを通じたユーザーとエージェントのセッション… 〔技術: 静的なベンチマークではなく、実際のエージェント利用ログから回帰テスト…／人文: エージェントの品質は抽象的な賢さではなく、人間が日々頼む用事を壊さな…〕 · [armature.tech](https://armature.tech)
- [ ] **Hanesu: Experimental workflow layer for AI coding agents** — HanesuはAIコーディングエージェント向けの実験的ワークフロー層で、長い自由文プロンプトの代わりに、タスクファイル、フェーズ… 〔技術: コンテキスト先行、成果物化、人間ゲート、検証完了条件などをテンプレー…／人文: 「vibe coding」の魅力を完全に否定せず、リスクが高い場面で…〕 · [github.com](https://github.com/jezmn/hanesu)
- [ ] **Deep Agentic Search for Repository-Level Code Question Answering: An Empirical Study** — リポジトリ規模のコード質問応答において、事前構築したベクトル検索と、計画エージェントが隔離されたサブエージェントに探索を委譲して… 〔技術: メインの文脈窓を汚さず、探索作業をサブエージェントに隔離して圧縮結果…／人文: 優れた協働者は、何でも同席させるのではなく、必要な調査を分担し、報告…〕 · [arxiv.org](https://arxiv.org/abs/2608.01507)

### AI agent trends
- [ ] **agentacct: コーディングエージェントの作業・費用・トークンをローカルで可視化** — Claude Code、Codex、OpenCodeなどがローカルに残すセッションログを読み、ツール利用、変更ファイル、テスト実… 〔技術: エージェント運用のボトルネックである「何をしたか・いくら使ったか・ど…／人文: AIエージェントを同僚や外注者のように扱うなら、成果物だけでなく作業…〕 · [github.com](https://github.com/mikehasa/agentacct)
- [ ] **diri: Claude Code / Codex / Cursor / Gemini を並列運用するmacOSオーケストレーター** — ネイティブmacOSアプリとして、複数のコーディングエージェントやシェルをgit worktreeやリモートホスト上で並列実行し… 〔技術: 単一チャットではなく、複数エージェントを作業単位・ブランチ単位で並列…／人文: これはプログラマの仕事を「一人で書く」から「複数の半自律作業者を見守…〕 · [github.com](https://github.com/cristicretu/diri)
- [ ] **LongHorizon-Harness: 長時間コンピュータ利用エージェントを、状態管理と独立監査で安定化** — 長時間タスクでは、実行、状態、完了判定が肥大化するコンテキスト内に混ざり、誤った自己評価が後続判断へ伝播しやすい。 〔技術: fresh context execution、durable ve…／人文: 人間の長期プロジェクトでも、記憶より台帳、自己申告よりレビューが重要…〕 · [github.com](https://github.com/AMAP-ML/LongHorizon-Harness)
- [ ] **nuphus-mcp: 任意のMCPクライアントにデスクトップ操作を渡す軽量MCPサーバー** — JSON-RPC 2.0 over stdio のMCPサーバーとして、画面認識、ウィンドウ操作、マウス・キーボード操作、Chr… 〔技術: MCPを、ドキュメントやAPI接続だけでなく「コンピュータそのものを…／人文: 画面を見てクリックする能力は、人間の事務労働の大部分を構成してきた。〕 · [github.com](https://github.com/mrpulor-gh/nuphus-mcp)
- [ ] **Safety, or Just Capability?: エージェント安全性ベンチマークは本当に安全性を測っているのか** — R-Judge、InjecAgent、AgentHarm、AgentDojoなどのエージェント安全性ベンチマークを妥当性監査し、… 〔技術: エージェント安全性を単一スコアで測る危うさを、ベースライン、相関、ラ…／人文: 「安全」と呼ばれる数字は、社会的な安心を生みやすいが、その数字が何を…〕 · [arxiv.org](http://arxiv.org/abs/2607.28685)

### Claude Code
- [ ] **Claude Code 2.1.222: worktree 隔離と auto mode 安全性の修正** — 2.1.222 では、worktree-isolated sessions とその subagents が main check… 〔技術: 「エージェントに任せる」ための中核はモデル性能だけでなく、workt…／人文: これは開発者とエージェントの信頼関係を、人格的な信頼ではなく制度設計…〕 · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [ ] **Claude Code 2.1.221: VSCode Focus view、credential masking、背景セッションの作法変更** — 2.1.221 では VSCode に Focus view が追加され、tool activity をターン単位の要約に折りた… 〔技術: 長い agentic run を「全部読む」から「要約・差分・状態を…／人文: Focus view は、AIの作業を労働過程として可視化しつつ、開…〕 · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [ ] **Claude Code 2.1.219: Opus 5、sandbox strict allowlist、nested subagents** — 2.1.219 では Claude Opus 5 が追加され、Opus 系のデフォルトになったほか、sandboxed comm… 〔技術: 大きなコンテキストと深い subagent 階層を使いながら、ネット…／人文: subagent のネストは、仕事を細分化して専門家に委ねる組織論に…〕 · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [ ] **arXiv: Deep Agentic Search は本当に repository QA に強いのか** — “Deep Agentic Search for Repository-Level Code Question Answerin… 〔技術: context pollution を避けるための subagent…／人文: エージェントを増やすことは「賢い組織」を作るように見えるが、引き継ぎ…〕 · [arxiv.org](https://arxiv.org/abs/2608.01507v1)
- [ ] **日本語実践: Claude Code と Codex を使った中〜大規模開発のタスク管理** — 日本語圏の実践記事として、Claude Code と Codex を中〜大規模開発のタスク自動化・進捗管理に使う際、タスクを明確… 〔技術: Claude Code の価値が「コードを書くCLI」から、開発タス…／人文: 日本語圏でも、AIエージェントは個人の能力拡張だけでなく、仕事の切り…〕 · [qiita.com](https://qiita.com/syun136_616/items/d0030020308534fd896c)

### Ethics of AI Agents
- [ ] **Accountability Asymmetry and Structural Trust in Autonomous AI Systems** — 自律AIシステムに運用作業を委任すると、人間オペレーターなら将来の評判・雇用・制裁が抑止力になる一方、AIコンポーネント自体は同… 〔技術: エージェントの安全性を、単一モデルのアラインメントではなく、変更管理…／人文: 「誰が責任を取るのか」という問いを、AIを罰せられるかではなく、被害…〕 · [arxiv.org](https://arxiv.org/abs/2608.03670)
- [ ] **Stateful Governance for Concurrent Agentic Systems** — 返金、在庫予約、クラウド資源の払い出し、金融移転のような操作では、リクエスト時点で許可された行為が実行時点では予算・在庫・承認状… 〔技術: エージェントのガードレールを静的な事前チェックから、状態変化と副作用…／人文: 責任ある自動化には「一度OKと言ったからOK」ではなく、状況が変わっ…〕 · [arxiv.org](https://arxiv.org/abs/2608.02764)
- [ ] **Securing Agentic AI: From Per-Action Checks to Trajectory Assurance** — エージェントの安全性は個々のアクションの可否だけで決まらず、プロンプト、記憶、検索知識、ツール、委任、マルチエージェント通信、モ… 〔技術: 個別API呼び出しの許可リストでは防げない、複数の一見許可された操作…／人文: 倫理的に問題になる行為は、しばしば一つの悪い命令ではなく、小さな委任…〕 · [arxiv.org](https://arxiv.org/abs/2608.01558)
- [ ] **Measurement Without Validity: The Compounding Reliability Problem in Agentic AI Evaluation** — エージェント評価パイプラインのベンチマーク得点が、デプロイ判断、安全認証、規制適合の根拠として使われる一方、タスク生成・人間シミ… 〔技術: 「高スコアだから安全」という短絡に対し、評価設計そのものの妥当性を定…／人文: 安全評価は社会的信頼をつくる儀式でもありますが、測っているものがずれ…〕 · [arxiv.org](https://arxiv.org/abs/2608.00794)
- [ ] **WeClawArena: An Auditable Sandbox and Benchmark for Cross-User Agents Collaboration and Security in Human-Centered Agent Networks** — ユーザーごとにAIエージェントが代理行動し、互いに通信・協働する「human-centered agent networks」を… 〔技術: 単体エージェントではなく、複数ユーザーの所有物・ファイル・ポリシーが…／人文: 個人の代理人同士が交渉・共有・誤解する世界では、プライバシーや同意は…〕 · [arxiv.org](https://arxiv.org/abs/2608.03499)

### Philosophy of Loop Engineering
- [ ] **Reframing AI Loss of Control: What Control Is, How to Have It, How to Lose It** — AIの「制御喪失」を語る前に、そもそも制御とは何かを「目標を設定し、達成すること」として定義し直す論文。 〔技術: エージェント設計における監視、介入、目標修正、フィードバックの要件を…／人文: 「誰が制御しているのか」という問いを、個人・組織・AIシステムのあい…〕 · [arxiv.org](http://arxiv.org/abs/2606.12442)
- [ ] **Don't Regenerate, Debug: A Domain-Specific Agent for Repairing Near-Miss Hardware Operators** — LLMによるGPU/NPU向けカーネル生成で、不合格候補を捨てて再生成するのではなく、コンパイル・実行・数値検証から得られる濃い… 〔技術: 失敗を廃棄物ではなく探索空間を狭める観測として扱い、計測・診断・修復…／人文: これは「創造」を一発の生成ではなく、失敗の意味を読み替える職人的反復…〕 · [arxiv.org](http://arxiv.org/abs/2608.02712)
- [ ] **AgentDebugX: An Open-Source Toolkit for Failure Observability, Attribution, and Recovery in LLM Agents** — LLMエージェントの失敗は、表面化したステップと原因ステップがずれることが多いとして、Detect / Attribute /… 〔技術: 実行トレースの観察だけでなく、根本原因帰属、回復案、再実行までを一つ…／人文: エラーを「誰のせいか」ではなく「どの時点でどのように世界理解が逸れた…〕 · [arxiv.org](http://arxiv.org/abs/2607.18754)
- [ ] **Kitaru: Every agent run, recorded and replayable** — Kitaru は、既存のエージェントSDKやハーネスの下に置く、自己ホスト可能でフレームワーク非依存のランタイム。 〔技術: ループをプロンプト設計の内部ではなく、記録・再生・比較・ロールバック…／人文: 「何が起きたか」を後から再訪できることは、説明責任だけでなく、経験を…〕 · [github.com](https://github.com/zenml-io/kitaru)
- [ ] **Aletheia — The Uncertainty Loop Agent for Claude Code and Codex** — Aletheia は、調査対象の真偽を「隠れた真実」とし、検索結果をノイズのある手がかりとして扱う調査エージェント。 〔技術: 信頼度、証拠、残余不確実性、反証をループの状態として明示し、検索エー…／人文: 「よく答えるAI」ではなく「知らないと言えるAI」を作ろうとする点が…〕 · [github.com](https://github.com/nsankar/Aletheia)

### Anthropology of Agentic AI
- [ ] **An Exploratory Study of Agent Plans for Agentic AI Coding Tools in Open-Source Software** — Claude CodeやGeminiなどのエージェント型コーディングツールに向け、リポジトリ内に残される「Agent Plans… 〔技術: エージェント実行を単発プロンプトではなく、リポジトリに保存される計画…／人文: Agent Planは、AIに仕事を任せる組織が作る「作業の民俗誌」…〕 · [arxiv.org](https://arxiv.org/abs/2608.04661)
- [ ] **AgentForge: An Immersive Role-Playing Platform for Learning Agentic Software Engineering** — エージェント型ソフトウェア開発を学ぶ初心者向けに、Task Planner、Patch Author、Code Reviewer… 〔技術: エージェント連携を「見えない自動化」ではなく、計画・実装・レビュー・…／人文: ロールプレイは、職場の見習い制度や徒弟制に近い学習儀礼です。〕 · [arxiv.org](https://arxiv.org/abs/2608.04148)
- [ ] **Architectural Implications of Agentic AI Workflows** — Microsoft Azureでの本番調査とオープンソースフレームワークの制御実験を通じ、agentic workflowがLL… 〔技術: agentic AIの「自律性」を、ワークフロー構造・ホストCPU・…／人文: ユーザーからは魔法のように見えるエージェントの行為も、裏側では多数の…〕 · [arxiv.org](https://arxiv.org/abs/2608.04458)
- [ ] **The New Social Image: How AI Competency and AI Proactivity Influence Self- and Peer-Perceptions in the Workplace（古いが関連性が高い）** — 職場のHuman-AI collaborationにおいて、AIの能力と能動性が、本人および同僚から見た所有感、感情、仕事の意味… 〔技術: AIの性能だけでなく、proactivityという振る舞いパラメータ…／人文: Agentic AIは仕事を奪うかどうか以前に、「有能に見える人」「…〕 · [arxiv.org](https://arxiv.org/abs/2606.00182)
- [ ] **Agentic AI（エージェンティックAI）とは？生成AIとの違いや活用事例を解説（古いが日本の導入文脈として重要）** — Agentic AIを生成AIやRPAと比較し、Gemini Enterpriseを含む企業導入のメリット・課題・成功ステップを… 〔技術: Agentic AIを既存のRPAや生成AIの延長ではなく、業務プロ…／人文: 日本企業でのAIエージェント導入は、稟議、権限分掌、現場調整、失敗責…〕 · [marubeni-idigio.com](https://www.marubeni-idigio.com/insight-hub/agentic-ai)

### History of Automation
- [ ] **Navigating the skill diversity frontier: How skill complexity explains worker resilience** — LinkedIn由来の米国労働者240万人・16,753スキルの縦断データから、技能ポートフォリオの「深さ」「広さ」「多様性フロ… 〔技術: スキル共起ネットワークから技能階層と多様性を復元し、AI時代の労働適…／人文: 産業革命以来の自動化は「職を奪う機械」だけでなく「職能の境界を組み替…〕 · [arxiv.org](https://arxiv.org/abs/2608.02102)
- [ ] **AI is erasing the first rung of the leadership ladder** — HR Executiveの記事は、AIと自動化が単純な職務数の問題だけでなく、若手が現場経験を通じて管理職へ育つ「最初の梯子」を… 〔技術: 生成AIが低リスク・反復的な分析、文書化、調整タスクを吸収すると、ジ…／人文: 工場自動化が職人技能の継承を変えたように、AIエージェントはホワイト…〕 · [hrexecutive.com](https://hrexecutive.com/ai-is-erasing-the-first-rung-of-the-leadership-ladder)
- [ ] **AI agents need identity, not just access** — No Jitterの記事は、業務に参加するAIエージェントには単なるアクセス権ではなく、所有者、権限、監査可能性を結びつける「エ… 〔技術: エージェント単位のID管理、権限分離、ログ監査を整えることで、自律的…／人文: 自動化の歴史では、機械が責任主体ではないにもかかわらず、実際には人間…〕 · [nojitter.com](https://www.nojitter.com/ai-automation/ai-agents-need-identity-not-just-access)
- [ ] **Why human approval is not enough: The growing need for AI agent observability** — Digital Journalの記事は、AIエージェントに人間の承認ステップを挟むだけでは不十分で、承認者がエージェントの推論経… 〔技術: ログ、トレース、根拠表示、意思決定過程の可視化がなければ、人間承認は…／人文: 20世紀の自動化でも、操作者はしばしばブラックボックス化した計器を信…〕 · [digitaljournal.com](https://www.digitaljournal.com/article/why-human-approval-is-not-enough-the-growing-need-for-ai-agent-observability)
- [ ] **From Network Automation to Trustworthy Autonomous Networking in the LLM Era: A Network Control Intelligence Perspective** — ネットワーク自動化の歴史を、単一の成熟度モデルではなく、意思決定ロジック、適応性、知識、制御委譲、インターフェースという5軸で整… 〔技術: Network Control Intelligenceという枠組み…／人文: 自動化史の核心は、省力化ではなく委任の歴史でもある。〕 · [arxiv.org](https://arxiv.org/abs/2608.01538)

### DDD
- [ ] **faceto: typed fileからLLMと議論できるEvent Stormingボードへ** — `faceto`は、型付きのモデルファイルからEvent StormingのHTML/SVGボードを生成し、要素ごとに短いメモを… 〔技術: Event Stormingの付箋・レーン・ホットスポットを、LLM…／人文: DDDのワークショップは本来、会話・沈黙・違和感を扱う文化的な場だが…〕 · [github.com](https://github.com/bastien-gallay/faceto)
- [ ] **DomainDL Agents: bounded contextごとにDDDコード生成サブエージェントを分ける試み** — `DomainDL Agents`は、FastAPI、MongoDB、LangSmithを使ったDDDコード生成・プロジェクトQ… 〔技術: DDDの戦術パターンをエージェントの責務分割に対応させ、生成物をbo…／人文: 「ユビキタス言語をどうコードへ翻訳するか」という熟練者の暗黙知を、エ…〕 · [github.com](https://github.com/GianL22/DomainDL-ai)
- [ ] **DDD & Design Patterns Skills for Agentic Development: エージェントにDDDの作法を教えるスキルセット** — Claude Code、Codex、Copilot、Geminiなど複数のエージェント環境で使えるDDD・デザインパターン・TD… 〔技術: DDDを単なるドキュメントではなく、エージェント実行環境にロード可能…／人文: これはチーム文化の移植に近い。〕 · [github.com](https://github.com/DavidSouther/domain-driven-design)
- [ ] **AI Refinement Method: vibe codingではなくvibe spec'ingへ** — `AI Refinement Method`は、自然言語の意図を、event storming、DDD、refinement、受… 〔技術: 実装生成の前段に、イベント・境界・脅威・ストーリー・テストを揃えるプ…／人文: DDDの価値を「正しいコードを書く技術」ではなく「何を作るべきかを共…〕 · [github.com](https://github.com/nlawstudio/ai-refinement-method)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — Tobias Eisenreich、Husein Jusic、Stefan Wagnerによる論文。 〔技術: LLMが得意な「用語整理・イベント列挙・境界候補出し」と、苦手な「集…／人文: 論文の含意は、AIがアーキテクトを置き換えるのではなく、議論の叩き台…〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

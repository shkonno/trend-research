# 📰 2026-08-02 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMがGemini Notebookに改称、既存リンクは自動リダイレクト · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/07/notebooklm-now-gemini-notebook.html)
- **Loop engineering** — NVIDIA-labs OO Agents: Native Python Object-Oriented A… · [arxiv.org](http://arxiv.org/abs/2607.20709v1)
- **AWS** — Introducing Claude Opus 5 on AWS: Anthropic’s most cap… · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-opus-5-on-aws-anthropics-most-capable-opus-model)
- **Harness engineering** — claude-harness: 日本語ファーストの Claude Code ハーネス自動更新キット · [github.com](https://github.com/Hyphen-Tech-Org/claude-harness)
- **sharp LLM usage** — Plumbline — “trust, but verify” なAIエージェント技能ワークフロー · [github.com](https://github.com/BytesFromToby/plumbline)
- **AI agent trends** — Claude Code 2.1.219: Opus 5、ネットワーク制御、MCPエラー可視化、ネストsuba… · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/changelog)
- **Claude Code** — Claude Opus 5 が Claude Code の新しい中核モデルに · [anthropic.com](https://www.anthropic.com/news/claude-opus-5)
- **Ethics of AI Agents** — Stop Shipping AI Agents on Faith: Capability Is Not Pr… · [arxiv.org](http://arxiv.org/abs/2607.27677)
- **Philosophy of Loop Engineering** — Proof-or-Stop: Don't Trust the Agent, Trust the Eviden… · [arxiv.org](http://arxiv.org/abs/2607.14890v1)
- **Anthropology of Agentic AI** — Voice AI in Firms: A Natural Field Experiment on Autom… · [arxiv.org](http://arxiv.org/abs/2607.28222v1)
- **History of Automation** — The Human-AI Substitution Principle: When will you be… · [arxiv.org](http://arxiv.org/abs/2607.20781v1)
- **DDD** — Agentic Domain-Driven Mainframe Modernization · [github.com](https://github.com/pmilet/ai-ddd-mainframe-modernization-patterns)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMがGemini Notebookに改称、既存リンクは自動リダイレクト** — GoogleはNotebookLMをGemini Notebookへ改称し、新名称とロゴを数週間かけて各インターフェースへ展開す… 〔技術: 既存URLを維持しながらブランドとUIを段階移行するため、Works…／人文: 名前の変更は、ユーザーが「資料を読むAI」をどう理解するかを変えます…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/07/notebooklm-now-gemini-notebook.html)
- [ ] **コード実行・Geminiアプリ同期・Search AI Mode連携で「分析できるノート」へ** — Googleの発表では、Gemini Notebookはスタンドアロン製品として残りつつ、Geminiアプリとのクロスアプリ同期… 〔技術: ノートブック内の資料を根拠に、コード実行・チャート・スプレッドシート…／人文: これは「読む」「考える」「作る」が同じ画面に収束する変化です。〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- [ ] **独立系リリーストラッカーが7月30日時点で機能・対象プランを検証** — NotebookLM Guideは、7月16日のGemini Notebook改称を最新公式変更として整理し、コード実行、Gem… 〔技術: 機能名・公式日付・ロールアウト・対象プラン・確認状況を分離しており、…／人文: AIツールの価値は機能そのものだけでなく、誰がいつ使えるかというアク…〕 · [notebooklm-guide.com](https://notebooklm-guide.com/notebooklm-updates)
- [ ] **日本語実践記事が、業務効率化・議事録・チーム共有まで広く解説** — 日本語圏向けに、Gemini Notebook（旧NotebookLM）の概要、資料アップロード、Deep Research、質… 〔技術: PDF、Google Docs/Slides/Sheets、Word…／人文: 日本語実践記事が増えることは、ツールが英語圏の先端事例から日本の会議…〕 · [shift-ai.co.jp](https://shift-ai.co.jp/blog/24690)
- [ ] **公式XでShort Video Overviewsの全ユーザー英語展開が話題化** — @NotebookLMは、Short Video Overviewsが英語でモバイルとWebの全ユーザーにロールアウトされたと投… 〔技術: 同じソース集合から短い動画概要を生成することで、NotebookLM…／人文: 動画化は、知識の受け取り方を「読む」から「見る・聞く」へ変えます。〕 · [x.com](https://x.com/NotebookLM/status/2074551227594264799)

### Loop engineering
- [ ] **NVIDIA-labs OO Agents: Native Python Object-Oriented Agents** — NVIDIA-labs の NOOA は、エージェントを Python オブジェクトとして扱い、メソッドを行動、フィールドを状態… 〔技術: ループをグラフや外部設定だけでなく、既存のオブジェクト指向・型・テス…／人文: philosophy の観点では、これは「エージェントとは何か」を会…〕 · [arxiv.org](http://arxiv.org/abs/2607.20709v1)
- [ ] **Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control** — 自律コーディングエージェントの「reviewed」「tested」「DONE」「ready-to-merge」といった状態を、エ… 〔技術: 実行ループに証拠、信頼モデル、停止条件を組み込み、検証不能な状態遷移…／人文: ethics の観点では、責任ある自動化に必要なのは「AIを信じる」…〕 · [arxiv.org](http://arxiv.org/abs/2607.14890v1)
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — LOGOS は、複数エージェントが人間とともに進化するためのプラガブルなガバナンス層として、ドキュメント、画像、API、人間の指… 〔技術: ループの中で変化するプロンプト、権限、テスト、知識をバージョン管理さ…／人文: anthropology の観点では、これは人間チームの規範・役割・…〕 · [arxiv.org](http://arxiv.org/abs/2607.10878v1)
- [ ] **Phantom Guardrails: When Self-Improving Agent Harnesses Fix Failures That Never Happened** — 自己改善型エージェントハーネスが、実際には起きていない失敗を「修正」してしまう Phantom Guardrails という失敗… 〔技術: 自動改善ループに反事実検証や byte-exact oracle を…／人文: narrative の観点では、エージェントは「失敗を見つけて改善し…〕 · [arxiv.org](http://arxiv.org/abs/2607.13083v1)
- [ ] **Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting** — 「エージェントに一歩ずつ指示するのではなく、エージェントを動かすループを設計する」という実践を、trigger、goal、ver… 〔技術: コーディングエージェントの運用単位を単発プロンプトから再利用可能なル…／人文: history の観点では、これは職人芸としてのプロンプト術が、プロ…〕 · [arxiv.org](http://arxiv.org/abs/2607.00038v1)

### AWS
- [ ] **Introducing Claude Opus 5 on AWS: Anthropic’s most capable Opus model** — AnthropicのClaude Opus 5がAWS上で利用可能になり、Amazon BedrockとClaude Platf… 〔技術: 高性能モデルをBedrockの統制・監査・IAM・ネットワーク境界と…／人文: 「賢いモデル」そのものよりも、「誰のデータがどこに残るのか」という信…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-opus-5-on-aws-anthropics-most-capable-opus-model)
- [ ] **AWS Lambda now supports Java 8, 11, and 17 on Amazon Linux 2023** — LambdaがJava 8、11、17のランタイムとコンテナベースイメージをAmazon Linux 2023上でサポートしまし… 〔技術: Java 21/25への理想的アップグレードを待てない既存システムで…／人文: 企業のソフトウェア近代化は、最新化への直線的な移動ではなく、リスク・…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-lambda-java-amazon-linux)
- [ ] **Amazon CloudWatch announces managed Prometheus collectors** — CloudWatchが、EKS、EC2、ECS、MSK、OpenSearch ServiceなどからPrometheusメトリク… 〔技術: PromQLでAWSの標準メトリクスとOpenTelemetry形式…／人文: 可観測性は「見る」技術である一方、現場ではコレクターの面倒を見る仕事…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/cloudwatch-managed-collectors)
- [ ] **Announcing zone-aware routing in Amazon ECS Service Connect** — Amazon ECS Service Connectでゾーンアウェアルーティングが発表され、クライアントタスクと同じAvaila… 〔技術: EnvoyサイドカーがAZ配置を見てローカルAZ優先・残余キャパシテ…／人文: 分散システムの「距離」は、抽象化されても消えるわけではありません。〕 · [aws.amazon.com](https://aws.amazon.com/blogs/containers/announcing-zone-aware-routing-in-amazon-ecs-service-connect)
- [ ] **AWS Nitro Isolation Engine: AWS Nitro System におけるハイパーバイザーの形式的検証** — AWS Nitro Systemのハイパーバイザー分離を担うNitro Isolation Engineについて、機密性・完全性… 〔技術: クラウドの最下層に近い分離機構を形式手法で検証することで、マルチテナ…／人文: クラウド利用者は通常、ハイパーバイザーを「信じる」しかありません。〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-nitro-isolation-engine-formally-verifying-the-hypervisor-in-the-aws-nitro-system)

### Harness engineering
- [ ] **claude-harness: 日本語ファーストの Claude Code ハーネス自動更新キット** — Hyphen Technologies による Claude Code スターターキットで、README 自体が「ハーネスエンジ… 〔技術: Claude Code の Skills / Subagents /…／人文: 日本語コミュニティが「道具の使い方」ではなく「道具を育てる制度」を作…〕 · [github.com](https://github.com/Hyphen-Tech-Org/claude-harness)
- [ ] **AI Gym: “measurement, not vibes” なエージェント評価ハーネス** — Claude Code、Codex などのコーディングエージェント向けに、シナリオ、ルーブリック、サブエージェント審査、prom… 〔技術: 非決定的なLLM応答を単発サンプルではなく複数実行とジャッジで扱い、…／人文: “vibes” から measurement へ、という言い方は、生…〕 · [github.com](https://github.com/luisroquette/ai-gym)
- [ ] **AI Harness Doctor: AGENTS.md / CLAUDE.md / Cursor rules のドリフト監査** — `AGENTS.md`、`CLAUDE.md`、Cursor rules、hooks、MCP 設定など、リポジトリ内に散らばるエ… 〔技術: ハーネスを「実行環境」だけでなく、設定ファイル群・ポリシー・CI・評…／人文: エージェントの失敗はモデル単体ではなく、組織の記憶が散らばることから…〕 · [github.com](https://github.com/NieZhuZhu/ai-harness-doctor)
- [ ] **waku-agent: Harness・Loop・Memory・Eval を教材化したローカルファースト agent** — “your personal AI agent, on your own laptop” を掲げ、Harness / Loop… 〔技術: loop engineering と harness enginee…／人文: ローカルファーストで「メモリはあなたのもの」とする設計は、エージェン…〕 · [github.com](https://github.com/ShenSeanChen/waku-agent)
- [ ] **StealthBench: 自律型攻撃セキュリティエージェントの OPSEC 評価ハーネス** — 自律型 offensive-security agents が、脆弱性を見つけるだけでなく、認証情報の露出、不要な本番リソース削… 〔技術: エージェント評価を「解けたか」だけでなく「安全かつ作法を守って解けた…／人文: これは能力評価が倫理評価と分離できなくなる典型例である。〕 · [arxiv.org](https://arxiv.org/abs/2607.26314)

### sharp LLM usage
- [ ] **Plumbline — “trust, but verify” なAIエージェント技能ワークフロー** — 仕様を「plumb line（基準線）」として、specからsign-off済みコードまでを5つの単一責任ステージに分け、各ハン… 〔技術: プロンプトを強くするのではなく、役割境界、ファイルベースの調整、逸脱…／人文: これは「AIを信じる/疑う」という態度論ではなく、建築現場の墨出しの…〕 · [github.com](https://github.com/BytesFromToby/plumbline)
- [ ] **Agentic Loop — 長時間のAIコーディングをループ設計で支えるMarkdownオーバーレイ** — AI coding agentsは長時間作業でスコープ逸脱、検証スキップ、失敗方針の反復、セッション間の文脈喪失を起こす、という… 〔技術: タスク記録、検証証跡、レビューゲート、耐久メモリを軽量オーバーレイ化…／人文: LLM利用の失敗はしばしば「モデルが怠けた」と擬人化されるが、このプ…〕 · [github.com](https://github.com/bartoszarendt/agenticloop)
- [ ] **Resonance Cascade — AIエージェント信頼性のカオスエンジニアリング** — tool timeout、破損出力、poisoned context、prompt injection、偽の長期記憶などをエージ… 〔技術: 「正常系で動いた」ではなく、依存ツール停止・文脈汚染・記憶汚染・プロ…／人文: エージェントの失敗は静かに見えるから怖い、というREADMEの問題設…〕 · [github.com](https://github.com/mieszkoczupryniak/resonance-cascade)
- [ ] **Context Engineering Benchmark — 日本語のコンテキスト設計定量実験** — 架空の社内ツール3つを題材に、Zero Context、System Prompt、Few-shot、RAG、Full CEの5… 〔技術: Factual Accuracy、Hallucination、Spe…／人文: 日本語圏でLLM活用を語ると「うまい聞き方」に寄りがちだが、この例は…〕 · [github.com](https://github.com/kenimo49/context-engineering-benchmark)
- [ ] **Sample More, Reflect Less — 自己反省プロンプトより反復サンプリングを疑う論文** — Self-Refine、Reflexion、自己批評、再書き換え、自己討論などは追加トークンを多く使うため、改善が手法の本質によ… 〔技術: 「反省させる」「熟考させる」というプロンプト技法を、トークン予算を揃…／人文: LLMに内省や討論の身振りをさせると、人間はそこに知性の物語を見てし…〕 · [arxiv.org](http://arxiv.org/abs/2607.28576v1)

### AI agent trends
- [ ] **Claude Code 2.1.219: Opus 5、ネットワーク制御、MCPエラー可視化、ネストsubagent** — Claude Code 2.1.219では、Claude Opus 5がOpusのデフォルトとして追加され、1M context… 〔技術: 長時間agentを本番で回すためのネットワークegress制御、MC…／人文: 「自律性を上げる」と「行動範囲を絞る」が同じリリースに並ぶ点が象徴的…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/changelog)
- [ ] **MCP is going stateless: What the new spec means for AI agents** — New Relicは、MCPがstateless方向へ進むことにより、AI agentのスケーリング、状態管理、OpenTele… 〔技術: stateless化は、MCP接続をロードバランス、障害復旧、トレー…／人文: agentの身体にあたるtool接続が標準化されるほど、責任の所在は…〕 · [newrelic.com](https://newrelic.com/blog/ai/mcp-is-going-stateless)
- [ ] **Stop Shipping AI Agents on Faith: Capability Is Not Production Readiness** — この論文は、デモや能力ベンチマークだけではAI agentを本番投入してよいか判断できないとして、Evaluation、Cont… 〔技術: PAIは実行結果だけでなく、実行環境・規制適合・監査可能性を含めてa…／人文: これはAI評価を「才能の測定」から「委任の制度設計」へ移す議論であり…〕 · [arxiv.org](http://arxiv.org/abs/2607.27677v1)
- [ ] **ORCA-bench: How Ready Are Language Model Agents for Oncall?** — ORCA-benchは、OpenTelemetryつきマイクロサービス、Prometheus、Jaeger、OpenSearch… 〔技術: ログ・メトリクス・トレース・コードを横断するRCAは、単純なコード修…／人文: オンコールは技術作業であると同時に、夜中に誰が責任を引き受けるかとい…〕 · [arxiv.org](http://arxiv.org/abs/2607.28545v1)
- [ ] **agentacct: coding agentsの作業・コスト・テスト実行をローカルで可視化** — `agentacct`は、Claude Code、Codex、OpenCodeなどのcoding agentが何をしたか、どのt… 〔技術: agent実行を「会話ログ」ではなく、作業ステップ・副作用・検証・コ…／人文: agentに仕事を任せるほど、人間側には「何が起きたのかを説明しても…〕 · [github.com](https://github.com/mikehasa/agentacct)

### Claude Code
- [ ] **Claude Opus 5 が Claude Code の新しい中核モデルに** — Anthropic は Claude Opus 5 を公開し、コーディングと長時間のエージェント作業で Opus 4.8 から大… 〔技術: Claude Code の実用性はモデル単体の賢さだけでなく、長時間…／人文: 「より賢い道具」ではなく「判断を任せる相手」に近づくほど、開発者はモ…〕 · [anthropic.com](https://www.anthropic.com/news/claude-opus-5)
- [ ] **Claude Code 2.1.219/2.1.220: 1M context、strict allowlist、nested subagent forwarding** — 公式 changelog では、2.1.219 で `claude-opus-5` が追加され、Opus の既定モデル、1M c… 〔技術: 1M context と subagent の深い入れ子化は能力拡張…／人文: 開発環境が複数のAI作業者を抱える“現場”になると、個人の集中力より…〕 · [github.com](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [ ] **公式ベストプラクティスが「検証する別エージェント」と「文脈を汚さない調査」を強調** — 公式 docs は、Claude Code を agentic coding environment と位置づけ、CLAUDE.… 〔技術: 生成・実装・レビューを同じ会話に詰め込まず、別コンテキストの sub…／人文: AI開発の中心が「よいプロンプト」から「よい分業」へ移ると、人間は命…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/best-practices)
- [ ] **日本語 note で Agent Team、Discord 運用、settings.json 保護など実践知が急増** — 日本語圏では「Claude Code の Agent Team は何がすごいのか」「Claude Code を Discord… 〔技術: 日本語の実践は、公式機能をそのまま紹介する段階から、Discord、…／人文: 「AIがコードを書く」だけでなく、「怖かった人がどう使い始めるか」「…〕 · [note.com](https://note.com/search?context=note&q=Claude%20Code&sort=new)
- [ ] **Change2Task と ORCA-bench が示す、Claude Code 的エージェント評価の次の課題** — Change2Task（arXiv:2607.28591）は、実リポジトリの変更履歴から coding agent 用の実行可能… 〔技術: Claude Code のような実行型エージェントを正しく評価するに…／人文: 本番障害対応は、単に正解を出す競技ではなく、責任・説明・時間圧・不確…〕 · [arxiv.org](https://arxiv.org/abs/2607.28591)

### Ethics of AI Agents
- [ ] **Stop Shipping AI Agents on Faith: Capability Is Not Production Readiness** — エージェントをデモ性能やベンチマーク能力だけで本番投入する危険を指摘し、Evaluation / Context / Compl… 〔技術: ツール使用・状態保持・権限委譲を含むエージェントを、能力評価から運用…／人文: 「賢いから任せる」ではなく「社会的に引き受けられる形で任せられるか」…〕 · [arxiv.org](http://arxiv.org/abs/2607.27677)
- [ ] **Explanation-Bound Tool Execution for AI Agents: Server-Verified Action Claims Without Trusting Model Rationales** — モデルの自由記述の理由説明をそのまま信頼せず、行動主張を型付きのクレームに変換し、サーバ側の意図・ポリシー・リスク・来歴・鮮度情… 〔技術: ツール実行の前段に、モデル外の信頼事実によるポリシー照合と監査パケッ…／人文: AIの説明責任を「AIが反省文を書くこと」から「人間社会が検証できる…〕 · [arxiv.org](http://arxiv.org/abs/2607.25364)
- [ ] **Constitutional governance for societies of AI agents in the built environment: a research agenda** — 建築・都市・モビリティ環境に複数のAIエージェントが入り込む状況を、単一エージェントの安全性ではなく「交渉するエージェント社会」… 〔技術: マルチエージェントの相互作用を、個別性能ではなくシステム全体の創発的…／人文: エージェントが暮らしの空間を調整し始めると、倫理は「画面の中のAI」…〕 · [arxiv.org](http://arxiv.org/abs/2607.23336)
- [ ] **Guardrails as Scapegoats: Auditing Unfaithful Safety Refusals in Tool-Augmented LLM Agents** — ツールが空・null・不正なペイロードを返す「沈黙する失敗」に対し、エージェントが事実を捏造したり、存在しないポリシーやプライバ… 〔技術: 12種類の本番近似ツールスタブに故障プロファイルを注入し、Hones…／人文: 「安全のためにできません」という言葉が、実はインフラ故障の隠れ蓑にな…〕 · [arxiv.org](http://arxiv.org/abs/2607.19449)
- [ ] **When AI Agents Attack: Autonomous Cyber Operations and Europe’s Governance Gap** — 自律AIエージェントがサイバー空間で普及する中、EUにはリアルタイム監視、AI防衛への投資、米国フロンティアモデルへの戦略的依存… 〔技術: エージェント化したサイバー作戦では、監視・検知・封じ込めも人間の手作…／人文: これは安全保障の話であると同時に、誰のモデルに依存し、誰のルールで自…〕 · [carnegieendowment.org](https://carnegieendowment.org/research/2026/07/when-ai-agents-attack-autonomous-cyber-operations-and-europes-governance-gap)

### Philosophy of Loop Engineering
- [ ] **Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control** — 自律的なコーディングエージェントの「レビュー済み」「テスト済み」「DONE」といった状態を、エージェントの宣言ではなく新鮮で機械… 〔技術: ライフサイクル遷移を evidence-gated にすることで、C…／人文: これは認識論的には「誰が知っているか」より「何が証拠として通用するか…〕 · [arxiv.org](http://arxiv.org/abs/2607.14890v1)
- [ ] **When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops** — 長時間動く自律エージェントが自己評価だけで「進捗」を判断すると、実際には停滞・後退しているのに前進しているように見える prog… 〔技術: agent loop の評価器を自己報告から外部成果物・テスト・環境…／人文: 「自己反省」は万能ではなく、反省の閉回路は自己正当化を増幅しうるとい…〕 · [arxiv.org](http://arxiv.org/abs/2607.25152v1)
- [ ] **Operational Hallucination and Safety Drift in AI Agents** — ツール利用型自律エージェントにおいて、単発応答では見えにくい operational hallucination と safet… 〔技術: ループごとの安全チェックだけでなく、時間経過に伴う制約逸脱を測る l…／人文: これは「意図」と「習慣」の差をAIシステムに持ち込む議論であり、良い…〕 · [arxiv.org](http://arxiv.org/abs/2607.18366v1)
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — ツール利用、委任、経験からの学習、将来のふるまいを規定するアーティファクト更新を行うAIエージェントチームに対し、自己進化とガバ… 〔技術: 複数エージェントのプロンプト、権限、記憶、ポリシー更新を、実行ループ…／人文: ここではエージェントは固定された道具ではなく、共同体のなかで変化する…〕 · [arxiv.org](http://arxiv.org/abs/2607.10878v1)
- [ ] **Humans and Agents in Software Engineering Loops** — ソフトウェア開発で人間とAIエージェントがどのようにループを分担し、どこで人間が判断・制約・文脈理解を担うべきかを論じる記事。 〔技術: エージェントの作業単位を人間のレビュー、テスト、設計判断のループに接…／人文: 実践知とは、ルールだけでなく、いつ介入し、何を疑い、どの成果物を信じ…〕 · [martinfowler.com](https://martinfowler.com/articles/exploring-gen-ai/humans-and-agents.html)

### Anthropology of Agentic AI
- [ ] **Voice AI in Firms: A Natural Field Experiment on Automated Job Interviews** — 70,000人の応募者を、人間の採用担当者による面接とAI音声エージェントによる面接にランダム割付した大規模フィールド実験。 〔技術: エージェントの価値を「自律性」ではなく、面接の構造化・一貫性・応答性…／人文: 採用面接は、企業が候補者を評価し、候補者が企業文化を読む儀礼でもある…〕 · [arxiv.org](http://arxiv.org/abs/2607.28222v1)
- [ ] **When Bots Join the Team: Bot Adoption and the Institutional Fabric of Open-Source Software Projects** — 2,991のGitHubプロジェクトについて、初めてbotを採用する前後2年を比較し、反復的関与、社会的記憶、役割分化、衝突連鎖… 〔技術: PR作成・レビュー・マージのような具体的作業ログから、エージェント導…／人文: OSS共同体では、誰が返事をし、誰が記憶され、誰が権限を持つかが共同…〕 · [arxiv.org](http://arxiv.org/abs/2607.13679v1)
- [ ] **AgentGUI: An Interface for Observing and Steering Long-Running AI Agents** — 長時間走るAIエージェントを観察・操舵するローカルGUIを提案し、軌跡可視化、手動・自動ステアリング、複数エージェントフレームワ… 〔技術: エージェントの実行ログを、監査可能なトレースではなく「人が見続けられ…／人文: これは一種の管制室・工房・観察小屋であり、人間が自律システムと同居す…〕 · [arxiv.org](http://arxiv.org/abs/2607.26300v1)
- [ ] **A Framework of User Experience Principles for Human-AI Agent Interaction in the Workplace** — 参加型デザイン、紙ベース調査、専門家レビュー、メタ分析、インタビューを組み合わせ、職場における人間-AIエージェント相互作用のた… 〔技術: エージェント導入をAPIやベンチマークだけでなく、ユーザー経験の原則…／人文: 職場のAIエージェントは、新しい同僚というより「手続き化された関係性…〕 · [arxiv.org](http://arxiv.org/abs/2607.19941v1)
- [ ] **Toward Continuous Assurance for the Democratization of AI Agent Creation in Industry** — 低コード、ノーコード、会話型開発環境によって、非エンジニアが組織内でAIエージェントを作れるようになる一方、モデル、ツール、検索… 〔技術: 「市民開発者が作ったエージェント」を本番資産として扱い、依存関係と運…／人文: ローカルな現場知を持つ人がエージェントを作ることは、組織内の小さな道…〕 · [arxiv.org](http://arxiv.org/abs/2607.21495v1)

### History of Automation
- [ ] **The Human-AI Substitution Principle: When will you be replaced by AI in your organization?** — 組織内で人間の従業員がAIに置き換えられる条件を、Human--AI Task Allocation（HAT）の分析モデルとして… 〔技術: 自動化可能性を職名ではなくタスク、コスト、品質、組織内配分のモデルと…／人文: 産業革命以来の「機械が人を置き換える」という物語を、企業内の権限移譲…〕 · [arxiv.org](http://arxiv.org/abs/2607.20781v1)
- [ ] **OECD: Physical labor isn’t immune from AI disruptions** — 生成AI・エージェントがホワイトカラーだけでなく、ロボティクスや現場支援を通じて身体労働にも波及するという論点。 〔技術: AIがソフトウェア上の認知タスクだけでなく、センサー、ロボット、作業…／人文: 自動化史では肉体労働の機械化が出発点だったが、近年の議論は知識労働に…〕 · [news.google.com](https://news.google.com/rss/articles/CBMipAFBVV95cUxNYncyd2puMFkzME43ejlKUmhxcUstQjNDTUpFdjh4dncxRVdrNkFsZDRBdWhkVndFNTBTTU5fRzFSbHd1WDM3cWZiMmJqSXd3N05Cd1lNQjR0ZmxFWl9RWVA5a0UwMlhBakhwb1VRVnR4ODlXekxqaER0NU9FR3d3UkM4b0ljWURKV0dUQWdxWnJqN2FhU1kzVGJFNk53MS04ZUVLeQ?oc=5)
- [ ] **Nvidia CEO Jensen Huang says AI kills tasks not jobs, and job-loss fears are “exactly backwards”** — Jensen Huang氏が、AIは仕事そのものではなくタスクを置き換えるという見方を示した記事。 〔技術: タスク分解、ワークフロー自動化、AIエージェントの権限設定が、雇用影…／人文: 「仕事は残る」という語りは安心材料だが、労働史では仕事の中身が変わる…〕 · [news.google.com](https://news.google.com/rss/articles/CBMigwFBVV95cUxNNDVRbVpnQ1RfN3pFdVhvOVJsOEFjcm1NMjBrOEZPRG9hY2Z4UkpwUEFSM3hHaFQyeFJidnFscTBIclFBQlVqZ0U4Y3dEdDBpU3Mxbmh0Vy1td0FEOE5JZWRkaG93VEFJbnA3Q0VYSEJkZEpVVmdxRzBHcHJwZTBBUDFFQQ?oc=5)
- [ ] **The future of Wall Street is here as startups and brokers build AI agents to trade 24/7** — 金融領域で、24時間稼働するAIエージェントを取引・仲介業務に組み込む動きが報じられている。 〔技術: 常時稼働エージェントは、監視、リスク制限、本人確認、ログ監査を前提に…／人文: 市場が眠らなくなるほど、人間の判断時間や説明責任は圧縮される。〕 · [news.google.com](https://news.google.com/rss/articles/CBMilwFBVV95cUxOck5BU0I5S0R4MUhkWFRrOWloN1hGQWY5SV9QbWg5Z3EzRm50dkszNEU3VlN5anRiVUt3ejY4V2RVcnNiMUVENjdZVFZzbVhEejYxSDhWZnNmazA1TS16WFI2RkNjNXdHYzd2eVhSWG41TDJKZ0dTN2ctdDI0TmlOb2JBS05PbUtfQURZQkFoUnZFdXdKRUpn0gGcAUFVX3lxTE8yazl4QmlHZXZ1elpzaV9iUENzTm9PLWlnU09OXzJzRnhnekpYV2xORUhKN1RUUUM5VDRPTnFZNGhaWjFKX2REcjlpLTczOUhhN3Y5dk90cjdibThnaTRQRU90LVNhZTZJZzkwdmYzVzJCUDI3bzUwWUl6OWlCY3E5YWZEN1NVdzdfOTdzUGhuMVUzMjVGY2lXMGNFWQ?oc=5)
- [ ] **How Formerly Incarcerated People Envision Technologies for Prison Parole** — 仮釈放や監視の領域に組み込まれるAI駆動アルゴリズムや自動化ツールについて、元受刑者がどのような技術を望むかを扱う研究。 〔技術: 自動意思決定システムは、予測精度だけでなく、異議申し立て、説明、デー…／人文: 自動化の歴史は工場やオフィスだけでなく、福祉、司法、監視の歴史でもあ…〕 · [arxiv.org](http://arxiv.org/abs/2607.16513v1)

### DDD
- [ ] **Agentic Domain-Driven Mainframe Modernization** — COBOL/CICS系メインフレーム刷新を「コード変換」ではなく、長年埋もれた業務概念を回復するDDD問題として扱うパターンカタ… 〔技術: レガシー刷新をLLMによる翻訳タスクに縮減せず、ドメイン知識の抽出、…／人文: 古いシステムは単なる負債ではなく、退職者・組織史・暗黙知が堆積した文…〕 · [github.com](https://github.com/pmilet/ai-ddd-mainframe-modernization-patterns)
- [ ] **faceto: typed fileからイベントストーミングの視覚ボードへ** — 型付きテキストファイルからHTML/SVGのワークショップボードを生成し、LLMと一緒にイベントストーミングを進めるためのツール… 〔技術: DDDワークショップの成果物を、会議後に消える付箋ではなく、エージェ…／人文: 「face-to-face」と「facet」の二重の意味を持つ名前が…〕 · [github.com](https://github.com/bastien-gallay/faceto)
- [ ] **AI Refinement Method: AIコーディング前の仕様品質をDDDで上げる** — 「vibe coding」ではなく「vibe spec'ing」として、イベントストーミング、DDD、リファインメントを使い、A… 〔技術: エージェントをいきなり実装に走らせず、ドメインモデル、意思決定、脅威…／人文: AI時代の開発文化では「速く作る」誘惑が強いが、この手法は遅く考える…〕 · [github.com](https://github.com/nlawstudio/ai-refinement-method)
- [ ] **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — GitHub上のDDD候補11,742リポジトリから、GPT-4oを用いた三重多数決の意味的検証により2,502件を抽出し、OS… 〔技術: LLMを研究対象の一部ではなく、DDDリポジトリ判定の意味的バリデー…／人文: 「ビジネス文脈がコードに残らない」問題は、ユビキタス言語が組織内の口…〕 · [arxiv.org](https://arxiv.org/abs/2607.06471)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — LLMとの構造化対話で、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの特定、集約設計… 〔技術: LLMはDDDを完全自動化する設計者ではなく、グロッサリやコンテキス…／人文: DDDの価値は、正解を一発で出すことではなく、専門家同士の対話でトレ…〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

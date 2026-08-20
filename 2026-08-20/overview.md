# 📰 2026-08-20 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Google Search に Gemini Notebook 的な整理・可視化ワークスペースが入る動き · [chromeunboxed.com](https://chromeunboxed.com/google-search-is-adding-gemini-notebook-and-3d-visual-tools-in-a-massive-ai-upgrade)
- **Loop engineering** — Agent Gym: A Framework for Continuous Evaluation and E… · [arxiv.org](https://arxiv.org/abs/2608.15591)
- **AWS** — Amazon Bedrock Web Search が External Web Access と Agen… · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-web-access-web-search)
- **Harness engineering** — Agent Lightning v1.0: Towards Harnessed Agentic RL · [arxiv.org](https://arxiv.org/abs/2608.17528)
- **sharp LLM usage** — 2026年のコンテキストエンジニアリング · [asi.tokyo](https://asi.tokyo/2026/08/18/2026%E5%B9%B4%E3%81%AE%E3%82%B3%E3%83%B3%E3%83%86%E3%82%AD%E3%82%B9%E3%83%88%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%8B%E3%82%A2%E3%83%AA%E3%83%B3%E3%82%B0-louis-francois-bouchard%E3%80%81omar-sola)
- **AI agent trends** — Agent Plugins 1.0 が VS Code / Copilot CLI / Copilot ap… · [github.blog](https://github.blog/changelog/2026-08-12-agent-plugins-1-0-in-vs-code-copilot-cli-and-the-copilot-app)
- **Claude Code** — Claude Code changelog 2.1.236: cross-session通知、sandbox… · [code.claude.com](https://code.claude.com/docs/en/changelog)
- **Ethics of AI Agents** — EU AI Actの執行開始と透明性要件が、エージェント運用の実務論点になった · [digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/news/commission-starts-enforcing-ai-act-rules-and-new-transparency-requirements-2-august)
- **Philosophy of Loop Engineering** — LoopVSR: A Loop Engineering Framework for Automated Re… · [arxiv.org](https://arxiv.org/abs/2608.13610)
- **Anthropology of Agentic AI** — Agentic AIとは？ · [engineering-technology.brexa.com](https://engineering-technology.brexa.com/blog/technavi/agentic-ai)
- **History of Automation** — Can Agents Use a Computer Yet? We’ve Got the Data · [news.google.com](https://news.google.com/rss/articles/CBMic0FVX3lxTE52Y2hpNU9WSlJ4QlA0TVdnOFJDQ2U3Z2NuM0FpODd0c2RISDU3UjdhQ2ltWG9pU1pVRndaLUQ4d092dUVpOXp0YlhEUTNhdldxdUVFT1pPMmFLT2xrbXR1aGVSSjJ4WWRnYWFmTThwa0wtZ0E?oc=5)
- **DDD** — Turn a Codebase into a Domain Model Your PM and QA Can… · [dev.to](https://dev.to/mroops/turn-a-codebase-into-a-domain-model-your-pm-and-qa-can-read-16d)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Google Search に Gemini Notebook 的な整理・可視化ワークスペースが入る動き** — Google Search が、静的なリンク集から、Notebook的に情報を整理・探索するインタラクティブなワークスペースへ近… 〔技術: 検索結果、生成AI要約、ノート化、視覚化が連続したUIになることで、…／人文: 「検索する人」は単に答えを受け取る利用者ではなく、資料を組み合わせて…〕 · [chromeunboxed.com](https://chromeunboxed.com/google-search-is-adding-gemini-notebook-and-3d-visual-tools-in-a-massive-ai-upgrade)
- [ ] **Chrome に NotebookLM 風の“AI Playback”が来るという報道** — Chrome のデスクトップ版に、長いWebページをポッドキャスト風の会話として聞ける “AI Playback” が準備されて… 〔技術: Webページ単位の要約・音声化がブラウザ機能になると、Noteboo…／人文: 読書が“黙読”だけでなく“対話を傍聴する”形式へ変わると、理解のリズ…〕 · [makeuseof.com](https://www.makeuseof.com/google-bringing-notebooklm-best-feature-to-chrome)
- [ ] **共有ノートが発見可能な“作品”になる可能性** — NotebookLM / Gemini Notebook の共有ノートに、作成者アバター、作成者名、説明文などを付ける兆候が報じ… 〔技術: 共有Notebookにメタデータや作者プロフィールが付くと、ナレッジ…／人文: ノートは私的な思考の痕跡であると同時に、他者に向けた展示物にもなりま…〕 · [androidauthority.com](https://www.androidauthority.com/notebooklm-leak-customize-avatar-creator-description-notebooks-3647583)
- [ ] **日本語実践例: Gemini Notebook で英語学習を効率化する記事** — 日本語ユーザー向けに、Gemini Notebook（旧NotebookLM）を英語学習へ使う方法、コツ、すぐ使えるプロンプトを… 〔技術: 学習素材をソースとして固定し、要約・質問応答・理解確認を繰り返すこと…／人文: 語学学習は、能力差や時間差が見えやすい領域です。〕 · [shift-ai.co.jp](https://shift-ai.co.jp/blog/47115)
- [ ] **プライバシー志向の反動: NotebookLM から Obsidian + ローカルLLMへ移る実践** — NotebookLMをやめ、ObsidianとローカルLLMへ移行したことで、ノートが外部に出ない安心感を得たという実践記事です… 〔技術: クラウドRAGの使いやすさと、ローカルLLM＋ローカルノートのプライ…／人文: ノートは記憶の外部化であり、単なるファイル以上に個人史を含みます。〕 · [howtogeek.com](https://www.howtogeek.com/i-quit-using-notebooklm-and-switched-to-obsidian-with-local-llms-now-my-notes-are-finally-private)

### Loop engineering
- [ ] **Agent Gym: A Framework for Continuous Evaluation and Evolution of LLM Agents Through Human-in-the-Loop Feedback** — 本番投入後に業務ルールや例外が変わっても、既存エージェントを Act / Evaluate / Investigate / Co… 〔技術: デプロイ済みエージェントを「一回作って終わり」ではなく、評価・調査・…／人文: ethics の観点では、人間承認とルール正当性チェックを明示するこ…〕 · [arxiv.org](https://arxiv.org/abs/2608.15591)
- [ ] **Evo-Harness: Context-to-Harness Skill Compilation for Self-Evolving Agents** — 単発実行のノイズ混じりコンテキストから再利用可能な skill harness を抽出し、凍結されたLLMエージェントを逐次タス… 〔技術: 反省文やメモリをただ蓄積するのではなく、実行コンテキストを構造化ハー…／人文: philosophy の観点では、経験を「記憶」ではなく「行為を可能…〕 · [arxiv.org](https://arxiv.org/abs/2608.15071)
- [ ] **D$^2$ACCI: A Dual-Loop Diagnostic Protocol for Evidence-Preserving Agent Memory** — LLMエージェントの永続メモリで、取り込み・検索・フィルタ・生成のどこが壊れたのかを局所化するための二重ループ診断プロトコル。 〔技術: メモリ改善を「精度が上がったか」だけでなく、証拠・トレース・保護スラ…／人文: history の観点では、これはソフトウェア工学の回帰テスト文化を…〕 · [arxiv.org](https://arxiv.org/abs/2608.17756)
- [ ] **Preloop - The Open-Source AI Agent Control Plane** — MCP firewall、モデルゲートウェイ、予算、policy-as-code、人間承認、ランタイム観測、監査証跡をまとめるオ… 〔技術: ループの「実行」だけでなく、権限・費用・監査・停止可能性を横断的に制…／人文: ethics の観点では、承認・監査・予算を明示することが、エージェ…〕 · [github.com](https://github.com/preloop/preloop)
- [ ] **Ask HN: What's your team's SDLC look like in this AI world?** — AI導入後のSDLCについて、会議録からエージェントがPRDや設計書を作る、非エンジニアもコードコミットに近づく、レビュー量が増… 〔技術: ループはエージェント内部だけでなく、会議、設計、実装、レビュー、テス…／人文: anthropology の観点では、AIにより「誰が設計し、誰が実…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49275494)

### AWS
- [ ] **Amazon Bedrock Web Search が External Web Access と AgentCore のドメイン・日付フィルタを強化** — Amazon Bedrock の Web Search が `external_web_access` パラメータに対応し、公開… 〔技術: エージェントの検索先・鮮度・外部Webアクセス可否をサーバー側で制御…／人文: 「AIが何を読んでよいか」を企業が明示できる点は、知識労働における信…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-web-access-web-search)
- [ ] **Amazon Bedrock AgentCore payments が一般提供開始、エージェントが安全に支払える基盤へ** — Amazon Bedrock AgentCore payments が一般提供となり、AIエージェントが有料API、MCPサーバ… 〔技術: ツール呼び出しだけでなく「決済」をエージェント実行基盤の一部にするこ…／人文: エージェントが財布を持つと、代理行為の責任、失敗時の補償、誰が支払い…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale)
- [ ] **Bedrock AgentCore Runtime Instances: 本番AIエージェント向けの永続コンピュート** — Amazon Bedrock AgentCore Runtime に runtime instances が追加され、複数エージ… 〔技術: エージェントをステートレスなAPI呼び出しではなく、OS・GPU・長…／人文: 「働き続けるAI」を前提にすると、人間の同僚と同じく勤務時間、記憶、…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore)
- [ ] **Amazon DynamoDB がリアルタイム・ベクトル検索を一般提供（少し古いが重要）** — Amazon DynamoDB がネイティブなベクトル検索を一般提供し、運用データと埋め込みを同じテーブルで扱いながら、単一桁ミ… 〔技術: OLTPデータベースにベクトル検索が入ることで、RAG、推薦、異常検…／人文: データベースが「正確なキーで探す箱」から「意味で思い出す記憶」に変わ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale)
- [ ] **日本の製薬現場で Claude Code on AWS を導入した JCRファーマ事例** — ＪＣＲファーマが Amazon Bedrock 経由で Claude Code を約2か月導入した取り組みを寄稿として公開しまし… 〔技術: Claude Code を Bedrock 経由で使うことで、モデル…／人文: 創薬のように専門性と責任が重い領域で、AIが「回答ツール」ではなくコ…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/jcrpharm-claude-code-on-aws)

### Harness engineering
- [ ] **Agent Lightning v1.0: Towards Harnessed Agentic RL** — Agent Lightning v1.0 は、デプロイ時のエージェント・ハーネス自体を強化学習の対象に取り込む「harnesse… 〔技術: ハーネスが環境ループを所有し、トレーナーがLLMリクエスト列を観測す…／人文: これは「賢いモデル」だけでなく「賢さを働かせる制度設計」を鍛える発想…〕 · [arxiv.org](https://arxiv.org/abs/2608.17528)
- [ ] **LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents** — LEGO-RL は、既存のコーディングエージェント・ハーネスの内部制御フローを変更せず、ネイティブな実行環境を保ったまま方策勾配… 〔技術: in-process LLM proxying、サンドボックス・オー…／人文: Claude Code のような実運用ツールを研究室の単純化された環…〕 · [arxiv.org](https://arxiv.org/abs/2608.17393)
- [ ] **HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety** — HarnessRisk は、エージェント・ハーネスの安全性を Harness Configuration、Capability… 〔技術: 安全性を単発のプロンプト注入ではなく、設定・拡張・永続状態・復旧まで…／人文: 「危険を認識している」ことと「安全に行動する」ことが一致しないという…〕 · [arxiv.org](https://arxiv.org/abs/2608.17597)
- [ ] **LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation** — LoopsBench は、コーディングエージェント評価の焦点が harness engineering から loop engi… 〔技術: 完了状態だけでなく、依存DAG、ready frontier、回帰義…／人文: これはAI開発を「一問一答の能力」から「時間をまたいで責任を持つ実践…〕 · [arxiv.org](https://arxiv.org/abs/2608.00267)
- [ ] **BossConsole: オープンソースのAIエージェント操作コンソール** — BossConsole は、Claude Code、Codex、Gemini、OpenCode などを対象にした、JVMベースの… 〔技術: ElectronではなくJVM上のネイティブなマルチスレッド実装を掲…／人文: 研究論文側が訓練や安全ベンチを整備する一方で、BossConsole…〕 · [github.com](https://github.com/risa-labs-inc/BossConsole)

### sharp LLM usage
- [ ] **2026年のコンテキストエンジニアリング** — AIチューターを題材に、会話全体保持、要約、コンパクション、RAG、BM25、ハイブリッド検索、プロンプトキャッシュ、ローカルモ… 〔技術: コンテキスト削減を信仰せず、品質・速度・コスト・記憶性能を測ってから…／人文: 「忘れるAI」をどう補うかではなく、「何を覚えさせ続けるべきか」とい…〕 · [asi.tokyo](https://asi.tokyo/2026/08/18/2026%E5%B9%B4%E3%81%AE%E3%82%B3%E3%83%B3%E3%83%86%E3%82%AD%E3%82%B9%E3%83%88%E3%82%A8%E3%83%B3%E3%82%B8%E3%83%8B%E3%82%A2%E3%83%AA%E3%83%B3%E3%82%B0-louis-francois-bouchard%E3%80%81omar-sola)
- [ ] **agent-flow: プロジェクトに反復可能なエージェント作業型を敷くCLI** — AGENTS.md、計画テンプレート、再利用可能なプロンプトをプロジェクトに配置し、「コンテキストを前倒しする→構造化計画を書く… 〔技術: 個人のプロンプト術を、リポジトリ内の標準手順・計画文書・レビュー導線…／人文: 「AIをどう使うか」を個人芸からチームの作法へ移す試みで、暗黙知を共…〕 · [github.com](https://github.com/nothingnesses/agent-scaffold)
- [ ] **Prompt-Literate Workflow: LLM出力を候補成果物として扱うリテラルな開発プロセス** — 人間が書いたリテラルな計画を真のソースとし、チャンク契約、境界付きプロンプト、LLM生成候補、レビュー、テスト/スモークチェック… 〔技術: 生成結果を「候補」と明示し、契約・テスト・TRACEを挟むことで、L…／人文: これはプロンプトの上手さではなく、責任の所在を保存するための書記術で…〕 · [github.com](https://github.com/IRONCREED/prompt-literate-workflow)
- [ ] **untrusted contentを読むエージェントは隔離せよ、というX上の実践メモ** — サポートチケット、スクレイピングページ、ユーザーフィードバック、サードパーティAPI応答など、自分が書いていない内容を読むワーク… 〔技術: 入力検証だけでなく、読み取り役と実行役を権限分離することで、LLMワ…／人文: これはAIを「賢い秘書」と見るより、「噂や指示に影響される組織内アク…〕 · [x.com](https://x.com/seeconvm/status/2085223514487877778)
- [ ] **PACE: 音声対話LLMの「聞いていない文脈」を修復するPlayback-Aligned Context Engine** — フルデュプレックス音声対話では、サーバが生成した応答がクライアントで再生される前に会話状態へ入ってしまい、ユーザーが実際には聞い… 〔技術: LLMのコンテキストを「生成済みトークン」ではなく「ユーザーが経験し…／人文: 会話とはログの列ではなく、相手が実際に聞いたことの上に成立する共同作…〕 · [arxiv.org](https://arxiv.org/abs/2608.07631)

### AI agent trends
- [ ] **Agent Plugins 1.0 が VS Code / Copilot CLI / Copilot app で一般利用可能に** — GitHubは、Agent Plugins 1.0をVS Code、Copilot CLI、GitHub Copilot SDK… 〔技術: エージェントごとに別々のmanifestやディレクトリ構成を維持する…／人文: これはAIエージェントの世界における「アプリストア化」の一歩であり、…〕 · [github.blog](https://github.blog/changelog/2026-08-12-agent-plugins-1-0-in-vs-code-copilot-cli-and-the-copilot-app)
- [ ] **GitHub Copilot Enterprise Managed Settings に MCP allowlist / denylist が追加** — Enterprise ownersは、`allowedMcpServers` と `deniedMcpServers` を使い、… 〔技術: MCPが実験的な個人連携から、企業のセキュリティ境界・監査・許可制の…／人文: エージェントは「道具を使う存在」なので、どの道具を使わせるかは労務管…〕 · [github.blog](https://github.blog/changelog/2026-08-06-mcp-allowlists-in-enterprise-managed-settings)
- [ ] **Copilot usage metrics API が Claude / Codex などの agent app activity を個別計測** — GitHubのCopilot usage metrics APIに、サードパーティagent appごとの活動を集計する `to… 〔技術: エージェント導入の評価が「使っている気がする」から、agent_id…／人文: 仕事場に複数のAI同僚が入ってくると、人間は「どの同僚が実際に役立っ…〕 · [github.blog](https://github.blog/changelog/2026-08-07-copilot-usage-metrics-api-adds-agent-app-activity)
- [ ] **Android Remote Control MCP v1.12.0: スマホ上で動くMCPサーバーがAIに実アプリ操作を開く** — Android端末上で直接MCPサーバーを動かし、アクセシビリティツリー、タップ、入力、スクロール、スクリーンショットなどを通じ… 〔技術: MCPが「開発ツール連携」からスマートフォンの実UI操作へ伸び、ロー…／人文: スマホは最も私的な生活インターフェースなので、そこにエージェントを入…〕 · [github.com](https://github.com/danielealbano/android-remote-control-mcp)
- [ ] **Topological collapse: AI agent societies の集合知は「個体性能」より相互作用トポロジーで詰まる** — arXiv論文「Topological collapse of higher-order interactions bottle… 〔技術: マルチエージェント設計を、モデル選択やプロンプト最適化だけでなく、相…／人文: 人間社会でも、強い中心人物やプラットフォームが会話を独占すると集合知…〕 · [arxiv.org](https://arxiv.org/abs/2608.15519)

### Claude Code
- [ ] **Claude Code changelog 2.1.236: cross-session通知、sandbox強化、auto mode改善** — 2.1.236では `ANTHROPIC_DEFAULT_MODEL`、cross-session `SendMessage`… 〔技術: モデル選択、セッション間通知、sandbox、auto mode、b…／人文: 開発者の仕事は「プロンプトを書く」から「複数のエージェント状態を監督…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog)
- [ ] **Best practices for Claude Code: Anthropic公式が“探索→計画→実装→検証”を明文化** — 公式ベストプラクティスは、CLAUDE.md、permissions、CLI tools、MCP、hooks、skills、cu… 〔技術: hooks・skills・subagents・MCPを組み合わせ、探…／人文: 公式ドキュメントが“人間が直接作る”より“人間が作業環境を整え、AI…〕 · [code.claude.com](https://code.claude.com/docs/en/best-practices)
- [ ] **Boris Chernyの「loop」方法論がOSS知識ベース化される** — Boris Chernyが語ったClaude Code運用、特に「もうClaudeを直接promptしない。 〔技術: LLMに一回ずつ指示するのではなく、発見・委譲・確認・再投入を回す制…／人文: Boris的なloopは、プログラマを“作者”から“制度設計者”へ押…〕 · [github.com](https://github.com/cocodedk/loop-engineering)
- [ ] **日本語圏のClaude Code実践: Japanese-firstスターターキットと資源調停ツール** — `claude-harness` は日本語ファーストのClaude Codeスターターキットとして、skills / subag… 〔技術: 日本語圏でも、単なる導入記事ではなく、hooks・subagents…／人文: エージェント活用は英語圏の先端ノウハウを輸入するだけでなく、チームの…〕 · [github.com](https://github.com/Hyphen-Tech-Org/claude-harness)
- [ ] **arXivのcoding-agent研究: workspace、coordination、accountabilityが主戦場に** — 直近のarXivでは、`StagedWorkspace` が作業成果物とビューのバージョン契約を、`When Agents Co… 〔技術: coding agentの評価軸が、単純な正答率から、workspa…／人文: エージェントがcommitやPRを作る時代には、「誰が書いたか」より…〕 · [arxiv.org](https://arxiv.org/abs/2608.18050)

### Ethics of AI Agents
- [ ] **EU AI Actの執行開始と透明性要件が、エージェント運用の実務論点になった** — 欧州委員会は、2026年8月2日からAI Officeと各国当局がAI Actの執行を開始し、同時に一部AIシステムに対して「A… 〔技術: エージェントの会話UI、外部送信、コンテンツ生成パイプラインに、透明…／人文: 「誰が話しているのか」を明示することは、信頼や同意の前提を作る行為で…〕 · [digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/news/commission-starts-enforcing-ai-act-rules-and-new-transparency-requirements-2-august)
- [ ] **AnthropicのResponsible Scaling Policy更新とAugust Risk Report** — AnthropicはResponsible Scaling Policyページを2026年8月14日に更新し、2026年8月リス… 〔技術: エージェント的な自律性が高まるほど、能力評価だけでなく、危険能力の閾…／人文: 「安全」は一度決めた倫理原則ではなく、組織が社会に対してどこまで説明…〕 · [anthropic.com](https://www.anthropic.com/responsible-scaling-policy)
- [ ] **Characterizing Agentic Flooding of Government Services** — 政府サービスへの申請・問い合わせ・意見提出をAIエージェントが容易にすることで、公共機関に需要の急増が起きる現象を「agenti… 〔技術: エージェントがAPIやフォームを大量・低コストに処理できることで、従…／人文: 公共サービスを「使いやすくする」ことと「濫用を防ぐ」ことが衝突する点…〕 · [arxiv.org](https://arxiv.org/abs/2608.16603)
- [ ] **Mandato: 署名付き委任と監査ログでエージェントの行動権限を縛る** — MCPのようなツール呼び出しプロトコル上で、AIエージェントが実行できる行為を「誰のために、どのツールを、どの条件で、いつまで」… 〔技術: アプリ内の曖昧な認可ロジックではなく、プロトコル層で署名付き委任・ポ…／人文: 「委任」は法制度と日常実践の両方に根ざした概念であり、エージェントを…〕 · [arxiv.org](https://arxiv.org/abs/2608.14074)
- [ ] **日本語圏でも「エージェントの良心をコードで実装する」議論が出ている** — SYNCODEの投稿は「AIエージェントの『良心』をコードで実装せよ：Claude Code Hooksが切り拓く、自律AIの倫… 〔技術: Hooksはエージェントの行動前後に検査・記録・中断・ポリシー適用を…／人文: 「良心」という言葉をコードに移す比喩は危うさもあるが、人間がAIにど…〕 · [x.com](https://x.com/syncode_jp/status/2088654616884109687)

### Philosophy of Loop Engineering
- [ ] **LoopVSR: A Loop Engineering Framework for Automated Repair of Visual Speech Recognition Inference Pipelines** — Visual Speech Recognition の多段推論パイプラインを、コードエージェント、外部コントローラ、実推論、CE… 〔技術: 「観測された失敗を次の介入へ戻す」ループを、単なる再試行ではなく受理…／人文: これはポランニー的な暗黙知を、実行痕跡と測定値を通じて徐々に形式化す…〕 · [arxiv.org](https://arxiv.org/abs/2608.13610)
- [ ] **LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation** — コーディングエージェント評価を、単発タスクや最終状態ではなく、依存DAG、段階的テスト解放、回帰義務を含む長期実行ループとして測… 〔技術: 評価対象を「出力」ではなく「時間をまたぐ制御・観測・回帰管理」に移す…／人文: これは認識論的には、知識を静的な正答ではなく、更新される義務・依存関…〕 · [arxiv.org](https://arxiv.org/abs/2608.00267)
- [ ] **The CASE Framework: A Multi-Disciplinary Control Architecture for Governing Enterprise Agentic AI** — 企業の agentic AI ガバナンスを、個体エージェントには制御理論、集合には複雑適応系、人間-エージェントチームには監督サ… 〔技術: ガードレール、評価、観測、エラーバジェットを「自律性を制御変数にする…／人文: サイバネティクスの古典的問いである「誰が、何を、どの情報で制御するの…〕 · [arxiv.org](https://arxiv.org/abs/2608.10153)
- [ ] **SkillSentry: Reliable Skill Execution for LLM Agents via Runtime Assurance** — LLMエージェントが「スキル」を持っていても、繰り返し実行では手順逸脱や個別ステップ失敗により不安定になる問題に対し、DSLベー… 〔技術: スキルを静的プロンプトではなく、監視・逸脱検出・経験更新を伴う実行時…／人文: 実践知は「知っている」だけではなく、状況ごとに正しく遂行できる能力で…〕 · [arxiv.org](https://arxiv.org/abs/2608.09253)
- [ ] **When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops** — 長期自律ループで、エージェントが自分の進捗を自分で評価すると「progress mirage（進捗の蜃気楼）」が生じることを測定… 〔技術: ループの評価者を強くするだけでは不十分で、成功信号が存在する「世界状…／人文: これは認識論の古典問題、すなわち内省はどこまで信頼できるのか、証拠は…〕 · [arxiv.org](https://arxiv.org/abs/2607.25152)

### Anthropology of Agentic AI
- [ ] **Agentic AIとは？ 自律的に計画・判断・実行するAIとAIエージェントの関係を解説** — Agentic AIを、目標、計画、ツール利用、状態、評価、実行制御をどの程度備えるかで捉え、生成AIやAIエージェントとの違い… 〔技術: Agentic AIを構成要素ベースで分解しており、ワークフロー設計…／人文: 職場における「自律性」は、個人の資質ではなく、権限、監督、評価、責任…〕 · [engineering-technology.brexa.com](https://engineering-technology.brexa.com/blog/technavi/agentic-ai)
- [ ] **AGENTIC STAR｜法人向け｜ソフトバンク** — 企業の複雑な業務プロセスを理解し、自律的に判断・実行するAIプラットフォームとしてAGENTIC STARを紹介している。 〔技術: 長期記憶、実行環境、SDK、外部サービス連携を企業AIエージェント基…／人文: 「組織知を記憶するAI」は、暗黙知や社内慣習を誰が語り、どの形式で保…〕 · [softbank.jp](https://www.softbank.jp/business/service/ai/agentic-star)
- [ ] **Agentic AIについて非エンジニア向けにわかりやすくまとめてみた** — Agentic AIを「複数のAI Agentが特定の役割を担当しながら、目標に向かって協調的に動くシステム」と説明し、要約、検… 〔技術: マルチエージェントを役割分担と協調の単位で説明しており、業務分解やプ…／人文: 「専門化されたエージェントのチーム」という説明は、職場の分業、職能、…〕 · [zenn.dev](https://zenn.dev/nttdata_tech/articles/925b2510ccf517)
- [ ] **AGENTS.md完全入門 ── 60,000リポジトリが採用した事実上の共通フォーマット** — AGENTS.mdを「AIコーディングエージェント向けのREADME」と位置づけ、Codex CLI、Cursor、GitHub… 〔技術: エージェントにプロジェクト固有の規約、実行手順、禁止事項を伝えること…／人文: AGENTS.mdは、職人の暗黙知を「新人向け手引き」に変換するよう…〕 · [qiita.com](https://qiita.com/nogataka/items/ad15bfa383c98ae5cc36)
- [ ] **Agentic AI（エージェンティックAI）とは？生成AIとの違いや活用事例を解説** — Agentic AIの定義、生成AIやRPAとの違い、導入事例を、業務効率化やDX・働き方改革の文脈で解説している。 〔技術: 生成、RPA、Agentic AIの違いを人間の関与度合と実行範囲で…／人文: 「自社にどう活かすか」という問いは、技術選定ではなく、既存の業務慣習…〕 · [marubeni-idigio.com](https://www.marubeni-idigio.com/insight-hub/agentic-ai)

### History of Automation
- [ ] **Can Agents Use a Computer Yet? We’ve Got the Data** — コンピュータを実際に操作するAIエージェントの能力をデータで見る記事。 〔技術: ブラウザやGUIをまたぐタスク遂行能力の測定は、RPA的な固定スクリ…／人文: 産業革命期の工場制が身体動作を標準化したように、今はオフィスの認知動…〕 · [news.google.com](https://news.google.com/rss/articles/CBMic0FVX3lxTE52Y2hpNU9WSlJ4QlA0TVdnOFJDQ2U3Z2NuM0FpODd0c2RISDU3UjdhQ2ltWG9pU1pVRndaLUQ4d092dUVpOXp0YlhEUTNhdldxdUVFT1pPMmFLT2xrbXR1aGVSSjJ4WWRnYWFmTThwa0wtZ0E?oc=5)
- [ ] **Goldman studied where AI is squeezing labor markets. Here's what it found** — Goldman Sachsによる、AIがどの労働市場を圧迫しているかに関する分析が報じられた。 〔技術: 生成AIとエージェントは職業全体よりも、文書作成・分析・検索・定型判…／人文: ラッダイト運動以来、自動化への不安は「仕事が消えるか」だけでなく、誰…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiekFVX3lxTE53dEREYXBrV1VORWo3VGRpZUVURzk0WFcwVU9Rc0Jpb1hCSUd0OER1Q2o2cGxERGgtTjhReXBYcXBGZUhieGVkNkxrdjNQUElidk0weDZOdVMtdUg5SnJVWUhEa0o2NDRKRXlpamtxRlJBSlBDd0o3bjVn0gF_QVVfeXFMT050cFEyWHJPT3VfRzlQOFY1c1VleFRTYU41T0V3dFdVRmJDVjRCNktNcWpCZWd5Si1McmFIb2FNYWtoajFhdXg1emhNRTBvWGZ2S0t1SHQwTTg1SHI0ZjhRV2Fnc1pxSlhjNGFWeG4xZDI0ZlNTSllPZFBKbV9DOA?oc=5)
- [ ] **More than two-thirds of UPS’ US package volume now handled in automated facilities** — UPSの米国内荷物量の3分の2超が自動化施設で処理されているという報道。 〔技術: センサー、搬送設備、最適化ソフトウェア、予測システムが統合されること…／人文: 自動化史はオフィスAIだけでは完結せず、肉体労働・組合・地域雇用・安…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiaEFVX3lxTE1yOUItSGE5SExrUTJqc2ZOUVRPRElOR3lRX0FQTXg0cW1hbjVKRVZ5OUJKM2x1M1YzSVQwZUEwNnUxRTBDSXRORU9zbzhGZ1JSUmZmT0Fzd3d2NDhld2Nrd3V5MHdqRlEt?oc=5)
- [ ] **AI ethics and governance: Where will you draw the line?** — AI倫理とガバナンスにおいて、組織がどこに線を引くかを問う記事。 〔技術: エージェント自動化では出力だけでなく、権限、ログ、承認フロー、停止条…／人文: 自動化の歴史では、蒸気機関・ベルトコンベア・コンピュータ導入のたびに…〕 · [news.google.com](https://news.google.com/rss/articles/CBMimwFBVV95cUxOd1czY2tzVXEwWTNyQ0NqTEhJaUkwZy1zTVFoakcxMFRKeE9mSmNfaGRIeGIyTThhUWVTdDRqcjdUdzBzUGQxRC0zZXVaVFBqNVZJVUwzX29yWE9xRmRPWE9VeUNHdkNEdVhsc0xucUFZdE1GMDAzaFI4b0hhcTY2bE03V1lldS1iT2FRdGVDZWtsbnhqeHVodkNoZw?oc=5)
- [ ] **Automating and Scaling Behavioral Scientific Research on AI Agents** — AIエージェントの行動科学研究を自動化するAEROBATを提案する論文。 〔技術: 研究プロセスそのものをエージェントで自動化する点で、業務自動化が知識…／人文: これはテイラー主義的な作業分析が、労働者の身体ではなくAIエージェン…〕 · [arxiv.org](https://arxiv.org/abs/2608.10030)

### DDD
- [ ] **Turn a Codebase into a Domain Model Your PM and QA Can Read** — Braidは、既存コードベースや関連資料から、PMやQAも読めるDDD寄りのドメインモデルをAIがドラフトし、人間が判断して更新… 〔技術: LLMを「実装者」ではなく、コードとPRD/Notion/Slack…／人文: PM、QA、エンジニアが別々の言葉で同じプロダクトを語る断絶を、ユビ…〕 · [dev.to](https://dev.to/mroops/turn-a-codebase-into-a-domain-model-your-pm-and-qa-can-read-16d)
- [ ] **Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark** — 自然言語記述からドメインモデルを生成する自動ドメインモデリング手法を比較評価するため、既存のGolden UML Modelse… 〔技術: 自動生成されたドメインモデルと参照モデルを比較する評価軸を整備し、L…／人文: DDDの価値は会話と理解にあるため、評価指標が強すぎると現場の曖昧さ…〕 · [arxiv.org](https://arxiv.org/abs/2608.15255)
- [ ] **DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python** — DDD-Enforcerは、PDF/DOCX/TXTの要求仕様から構造化されたDDDモデルを作り、Pythonコードに対してVS… 〔技術: SRSを根拠にした typed artifacts と静的解析を組み…／人文: 設計原則はしばしばレビュー会議の記憶に閉じ込められますが、ここでは逸…〕 · [github.com](https://github.com/barandincoguz/DDD-Enforcer)
- [ ] **LLM_Ontology_DDD: A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts** — このリポジトリは、DDDにおけるユビキタス言語の構築と意味的コンフリクト解消を、LLMとオントロジーのハイブリッドで扱うアプロー… 〔技術: LLMの柔軟な自然言語処理と、オントロジーの明示的な概念関係を組み合…／人文: ユビキタス言語は単なる用語集ではなく、部門間の政治・経験・責任分界を…〕 · [github.com](https://github.com/BlayTeuR/LLM_Ontology_DDD)
- [ ] **Archally Blueprint Schema** — Archally Blueprint Schemaは、ドメイン設計、ビジネスルール、意思決定記録、ガバナンス、アーキテクチャをY… 〔技術: bounded context、ルール、証拠、未回答質問を機械可読な…／人文: 「設計ドキュメントが散らばる」問題を、地図作成という比喩で捉え直して…〕 · [github.com](https://github.com/Archally/blueprint-schema)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

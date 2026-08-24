# 📰 2026-08-24 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — 「AIに頼りすぎて身につかない」を克服するNotebookLM活用法 · [qiita.com](https://qiita.com/hime_devlog/items/eb45269c126672d6bf98)
- **Loop engineering** — LoopVSR: A Loop Engineering Framework for Automated Re… · [arxiv.org](http://arxiv.org/abs/2608.13610v1)
- **AWS** — Amazon Bedrock AgentCore payments が一般提供開始 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale)
- **Harness engineering** — Harness Internals: agent harness と eval harness を同じ証拠面… · [github.com](https://github.com/plwslpld-arch/harness-internals)
- **sharp LLM usage** — Shopify「Gisting」で長いシステムプロンプトを学習済みトークンへ圧縮 · [shopify.engineering](https://shopify.engineering/gisting)
- **AI agent trends** — Boris Cherny: Claude に日常的なアプリ保守を任せる実験 · [x.com](https://x.com/bcherny/status/2088014489438621990)
- **Claude Code** — Claude Code v2.1.239: 企業利用・クラウドセッション・プロキシ周りの大規模な信頼性改善 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- **Ethics of AI Agents** — エージェント型AIがセキュリティの「人間前提」を打ち破る · [forbesjapan.com](https://forbesjapan.com/articles/detail/103386)
- **Philosophy of Loop Engineering** — Darwin Gödel Machine: Open-Ended Evolution of Self-Imp… · [arxiv.org](https://arxiv.org/abs/2505.22954)
- **Anthropology of Agentic AI** — AI as the common language of the workplace, human tran… · [mckinsey.com](https://www.mckinsey.com/~/media/mckinsey/email/weekendread/2026/08/2026-08-14a.html)
- **History of Automation** — AI was supposed to destroy jobs. Where’s the carnage? · [news.google.com](https://news.google.com/rss/articles/CBMieEFVX3lxTE85RVJfLU9XbWFoYlEzQ0hqdWxJVlJBZUxIcnk1VnZkR0JiVHNvSDVEelVmbDU4Ung2M3FJQUtncTNDUDR2NDJ0RkgxUWJEZEd4VzY5WUlJTGhGenVqOTZRcEYzcFNPc29xT2pYRUdFcF9kZFpEa2VXZQ?oc=5)
- **DDD** — EventCatalog: domains / services / events / schemas をA… · [github.com](https://github.com/event-catalog/eventcatalog)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **「AIに頼りすぎて身につかない」を克服するNotebookLM活用法** — プログラミング学習でAIに正解コードを出させてしまう問題に対し、自作メモだけをNotebookLMのソースにして「知識不足」か「… 〔技術: RAG的なソース制約を「回答品質」ではなく「学習者の認知負荷とネタバ…／人文: 生成AIを万能な先生にせず、学習者が自分の理解の境界を発見する鏡とし…〕 · [qiita.com](https://qiita.com/hime_devlog/items/eb45269c126672d6bf98)
- [ ] **Gemini Notebook（NotebookLM）を複数横断で使う小技** — Geminiのチャットから複数のNotebookを選択し、Notebook同士を横断したソースとして扱う小技を紹介。 〔技術: NotebookLM単体のUI制約をGemini側のソース選択で回避…／人文: 個人の知識は一冊の完結したノートではなく、断片的な文脈の集まりです。〕 · [qiita.com](https://qiita.com/Akiko_Miyamoto/items/4f28eb75891f23221e70)
- [ ] **Google Calendar → Google Sheets → NotebookLM：Apps Scriptで予定を定期同期してAIに読ませる** — Google Calendarの予定をApps ScriptでGoogle Sheetsへ同期し、NotebookLM/Gemi… 〔技術: Calendar、Apps Script、Sheets、Notebo…／人文: カレンダーは単なる予定表ではなく、生活のリズムや関心の履歴です。〕 · [qiita.com](https://qiita.com/maskot1977/items/896983eb88aff4efcd08)
- [ ] **Google is bringing NotebookLM’s best feature to Chrome** — Google News RSS上で、NotebookLMの代表的機能がChromeへ持ち込まれる動きとして報じられています。 〔技術: NotebookLMの価値が独立アプリからブラウザ常駐の読解インター…／人文: ブラウザは現代人の読書机であり、そこに要約・解説AIが入ることは「読…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiggFBVV95cUxQSlJrSHU0R3RmQTZnaHZOWmk5TTZTdndPd3hsYTFZaHQ3MXpZODhzenJocExkcFA3cFZxWm82VW5ONnlqNERZNWp2c2JfSHJSMUVSVUNWSVFBUzdFQmRyQ1J3QmlQU1R0RXduUDJjTVRiOFNLd3BCbHNiSGZKY2ZJN0hR?oc=5)
- [ ] **Show HN: PageLM – Open-Source NotebookLM Alternative** — NotebookLM風の学習支援をオープンソースで実装するPageLMがHacker Newsに登場。 〔技術: NotebookLM型UXがプロプライエタリ製品に閉じず、React…／人文: 学習支援AIがプラットフォーム依存になると、知識管理の自由度やプライ…〕 · [github.com](https://github.com/CaviraOSS/PageLM)

### Loop engineering
- [ ] **LoopVSR: A Loop Engineering Framework for Automated Repair of Visual Speech Recognition Inference Pipelines** — Visual Speech Recognition（読唇・視覚音声認識）の多段推論パイプラインを、コードエージェントと外部コント… 〔技術: 単なるテスト再実行ではなく、実推論・エラー率・ロールバックを組み合わ…／人文: anthropology の観点では、専門家が経験的に行ってきた「ど…〕 · [arxiv.org](http://arxiv.org/abs/2608.13610v1)
- [ ] **Auditing and Decomposing Feedback-Driven Evolution in LLM Test Generation under the Oracle Problem** — LLMが生成したテストを実行フィードバックで改善する手法について、単一の accepted program を正解オラクルにする… 〔技術: Loop engineering の中心である「フィードバックを信じ…／人文: ethics の観点では、改善ループが自己正当化の装置になりうる危険…〕 · [arxiv.org](http://arxiv.org/abs/2608.19626v1)
- [ ] **Bringing analytic rigor to agentic AI for science: The Brain Researcher platform for neuroimaging data analysis** — 科学分析を行うAIエージェントに対し、許容される分析、必須チェック、主張範囲の制限を定める neuroimaging 向け研究ハ… 〔技術: エージェントのループを「分析を実行する」だけでなく、代替分析・証拠・…／人文: ethics の観点では、科学的主張を自動化する際に、成功宣言よりも…〕 · [arxiv.org](http://arxiv.org/abs/2608.19902v1)
- [ ] **The Third Restructuring of Software Form: From the Three-Tier Architecture to Storage, Models, and Agents** — Software 3.0 の最終形を、永続状態を担う generalized database、推論を担う large mode… 〔技術: Loop engineering を個別エージェントの実装テクニック…／人文: history の観点では、三層アーキテクチャからモデル・記憶・ルー…〕 · [arxiv.org](http://arxiv.org/abs/2608.20201v1)
- [ ] **LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation** — コーディングエージェント評価が、単発タスクの harness engineering から、長期実行の loop enginee… 〔技術: エージェント評価を最終状態だけでなく、依存関係、途中成果、回帰、継続…／人文: anthropology の観点では、人間の開発チームが行う段取り・…〕 · [arxiv.org](http://arxiv.org/abs/2608.00267v2)

### AWS
- [ ] **Amazon Bedrock AgentCore payments が一般提供開始** — AgentCore payments がGAとなり、AIエージェントが有料API、MCP、コンテンツへ自律的に支払える仕組みを、… 〔技術: エージェント実行基盤に決済・委任・監査を組み込み、MCP/有料API…／人文: これは「人間がクリックして買う」経済から「ソフトウェア代理人が予算内…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale)
- [ ] **Amazon Bedrock AgentCore Gateway によるエージェントのツールアクセス統治** — AgentCore Gateway を、Claude Code、Kiro、Cursor、Amazon Quick などのMCP対… 〔技術: MCPの普及で分散しがちなエージェントのツール接続を、ポリシー、ID…／人文: エージェント時代の権限管理は、単なるIAM設計ではなく「組織内の誰が…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/govern-ai-agent-tool-access-with-amazon-bedrock-agentcore-gateway)
- [ ] **AWS Glue 6.0: 30%値下げと Apache Iceberg v3 フルサポート** — AWS Glue 6.0 が一般提供され、従来版より30%低い価格、Apache Iceberg v3のフルサポート、Apach… 〔技術: Iceberg v3と新ランタイムへの更新により、レイクハウスのテー…／人文: データ基盤の値下げは、生成AIや分析を使える組織と使えない組織の差を…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-glue-6-0-now-available-with-30-lower-price-and-full-apache-iceberg-v3-support)
- [ ] **Amazon EKS が証明書認証局（CA）ローテーションの自動ライフサイクル管理に対応** — Amazon EKS がクラスターCAのローテーションをマネージドなライフサイクルと自動セーフガード付きで実行できるようになった… 〔技術: EKSクラスターごとのCA更新をAWS管理の手順に載せることで、証明…／人文: セキュリティの成熟は派手な新機能より、怖くて後回しにされる保守作業を…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-eks-certificate-authority-ca-rotation-automated-lifecycle-management)
- [ ] **日本語コミュニティ: Bedrock / AgentCore 最新アップデートの整理記事（やや古いが関連性高）** — AWS Bedrock LLM Day Japan の「AWS Keynote と最新アップデート」セッションをもとに、Amaz… 〔技術: Bedrock/AgentCore周辺の複数アップデートを、サービス…／人文: グローバルなクラウド発表は、地域コミュニティが母語で再編集して初めて…〕 · [qiita.com](https://qiita.com/suzukisawa/items/db13f04a825b1845d808)

### Harness engineering
- [ ] **Harness Internals: agent harness と eval harness を同じ証拠面で読む中国語/英語リポジトリ** — DeepSeek Harness、OpenAI Codex、Gemini CLI、Claude Agent SDK の公開契約面… 〔技術: Claude Code 本体を閉源として扱い、Claude Agen…／人文: エージェント評価を単一スコアで語る誘惑に抵抗し、「誰のどの装置が結果…〕 · [github.com](https://github.com/plwslpld-arch/harness-internals)
- [ ] **Claude Code Week 32: セッション間メッセージ、自社ホスト環境、auto mode 既定化** — Claude Code セッション同士が `ListAgents` / `SendMessage` でメッセージを送り合えるよう… 〔技術: loop engineering の中心である「複数セッション・権限…／人文: 自律化が進むほど、誰が許可し、どこで隔離し、どの環境で走らせるかが社…〕 · [code.claude.com](https://code.claude.com/docs/en/whats-new/2026-w32)
- [ ] **Brain Researcher: 神経画像解析のための agentic research harness** — 論文「Bringing analytic rigor to agentic AI for science」は、神経画像解析の計算… 〔技術: harness を単なるツール接続ではなく、解析選択・証拠・prov…／人文: 科学におけるAIエージェントの危険は、間違いそのものだけでなく、もっ…〕 · [arxiv.org](https://arxiv.org/abs/2608.19902v1)
- [ ] **TaoLive Digital Avatar Agent: Harness-Aware Training で変わり続ける実行環境にモデルを合わせる** — ライブコマース用デジタルアバターエージェントにおいて、Skills、Hooks、system prompt、tools をモデル… 〔技術: harness が頻繁に変わると、SFT モデルが特定スキーマやプロ…／人文: 商業ライブ配信のエージェントは、商品説明、販売戦略、コンプライアンス…〕 · [arxiv.org](https://arxiv.org/abs/2608.15763v1)
- [ ] **SWE-bench Science: Claude Code でも科学ソフトウェア修復は pass@1 50% 未満** — 「SWE-bench Science」は、98 GitHub リポジトリから119タスクを集め、科学ソフトウェア工学における c… 〔技術: Claude Code のような強い coding agent でも…／人文: 科学ソフトウェアは実験装置でもあり、コード修復の失敗は知識生産そのも…〕 · [arxiv.org](https://arxiv.org/abs/2608.19799v1)

### sharp LLM usage
- [ ] **Shopify「Gisting」で長いシステムプロンプトを学習済みトークンへ圧縮** — ShopifyはSidekick GraphQL agentの約6,000トークンのシステムプロンプトを約1,500のgist… 〔技術: 「プロンプトを短く書く」ではなく、プロンプトの振る舞い自体を埋め込み…／人文: 組織の暗黙知や運用ルールが、可読な文章から不可視のトークン列へ移るこ…〕 · [shopify.engineering](https://shopify.engineering/gisting)
- [ ] **OneCLI v2: チーム全員にサンドボックス付き個人エージェントを配る設計** — OneCLIは、社員ごとに隔離されたエージェントを作り、IdP連携、権限ポリシー、シークレット注入、人間承認、Slack接続、永… 〔技術: LLMの能力ではなく、サンドボックス、ゲートウェイ、MITMによる認…／人文: 「AIを使う個人」から「組織に常駐する個人別エージェント」へ移ると、…〕 · [github.com](https://github.com/onecli/onecli)
- [ ] **Proliferate: Claude Code / Codex / OpenCodeを並列に走らせるAI IDE** — ProliferateはClaude Code、Codex、OpenCode、Cursor、Grokなどをネイティブハーネスで扱… 〔技術: 複数エージェントを同じ作業ツリーで競合させず、worktree単位に…／人文: これは「一人の賢い相棒」ではなく、小さな作業者群を編集者として采配す…〕 · [github.com](https://github.com/proliferate-ai/proliferate)
- [ ] **Task-CoEvolve: エージェント・ハーネス最適化の検証タスクを適応的に選ぶ** — Task-CoEvolveは、モデル重みを変えずにエージェントのハーネスコードを反復改善する際、毎回固定の検証セットを全実行する… 〔技術: LLM活用の改善ループを「良さそうなプロンプトを試す」から、評価セッ…／人文: 人間の学習でも、すでに解ける問題や全く解けない問題ばかりでは伸びない…〕 · [arxiv.org](https://arxiv.org/abs/2608.20169)
- [ ] **PACE: 音声エージェントの「ユーザーが聞いていない文脈」を除去する** — PACEは、全二重音声対話でサーバー側の生成がクライアント再生より先に進むため、ユーザーが実際には聞いていない発話をモデルが文脈… 〔技術: コンテキストを「ログに存在する全履歴」ではなく「ユーザーが知覚できた…／人文: 会話の意味は、発話された内容だけでなく、相手が本当に聞いたかに依存す…〕 · [arxiv.org](https://arxiv.org/abs/2608.07631)

### AI agent trends
- [ ] **Boris Cherny: Claude に日常的なアプリ保守を任せる実験** — Boris Cherny が、Slackチャンネル `proj-claude-maintains-apps` を使い、Claud… 〔技術: エージェントを単発のコード生成ではなく、Slack・運用チャンネル・…／人文: 人間の仕事は「依頼する」から「チャンネル上で同僚として観察・介入する…〕 · [x.com](https://x.com/bcherny/status/2088014489438621990)
- [ ] **Task-Conditioned Least-Privilege Learning for Executable Terminal and MCP Agents** — TerminalやMCPを実行できるLLMエージェントが、タスクに不要な権限まで行使してしまう「過剰権限」問題を扱う研究。 〔技術: MCPエージェントを本番運用する際の最大リスクである権限設計を、後付…／人文: 「できること」と「してよいこと」を分ける議論であり、代理行為の倫理に…〕 · [arxiv.org](https://arxiv.org/abs/2608.18351)
- [ ] **One Success Isn't Reliability: Thinkingbox, a Sandbox and Benchmark for Agents in Stateful Business Workflows** — 業務ワークフローでは、1回成功したように見えるだけでは信頼性にならない、という問題意識から、状態を持つビジネス環境でエージェント… 〔技術: エージェント評価が「正しい応答」や「有効なツール呼び出し」から、状態…／人文: 仕事の信頼は一度の成功ではなく、繰り返し・説明・修復可能性から生まれ…〕 · [arxiv.org](https://arxiv.org/abs/2608.19741)
- [ ] **Pond: エージェントセッションを自分のS3/ローカルに保存し、MCPで検索する** — Claude Code、Codexなどのエージェント会話・作業履歴をローカルまたは自分のS3に損失なく保存し、検索・SQL問い合… 〔技術: エージェントの文脈をプロンプト内の一時記憶ではなく、所有可能で検索可…／人文: 記憶は効率化だけでなく、組織の経験を誰が所有するかという問題でもある…〕 · [github.com](https://github.com/tenequm/pond)
- [ ] **【2026年8月】Agent Pluginsとは？MCP・Skillsの次に知っておきたいAIエージェントの新標準** — 日本語圏で、MCPやSkillsに続くエージェント拡張標準としてAgent Pluginsを解説する記事。 〔技術: MCPがツール接続、Skillsが能力パッケージだとすれば、Agen…／人文: 標準は技術仕様であると同時に、誰がエージェント生態系の入口を支配する…〕 · [note.com](https://note.com/kazu_t/n/ncc2e2dd01c95)

### Claude Code
- [ ] **Claude Code v2.1.239: 企業利用・クラウドセッション・プロキシ周りの大規模な信頼性改善** — v2.1.239では、US-only inferenceプレミアムを含むコスト見積もり、`/claude-api upgrade… 〔技術: プロキシ、Bedrock、musl、クラウドセッション、プラグイン同…／人文: 開発者体験の「魔法」は、実際には請求、認証、OS差、ネットワーク制約…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **Claude Codeのセッション間通信、Windowsでも動きます（v2.1.234から）** — 日本語記事が、Claude Codeのcross-session messagingは以前「ネイティブWindows非対応」と読… 〔技術: 複数Claude CodeセッションをOS内IPCでつなぐ設計が、m…／人文: 「AIに仕事を任せる」と言っても、人間は複数の作業文脈を抱えています…〕 · [qiita.com](https://qiita.com/jqit_suwa/items/137a2810fb3fa3f773e8)
- [ ] **Claude Code on the web / cloud sessions: ローカルからクラウド常駐タスクへ** — Claude Code on the webは、`--cloud`や`--teleport`でWeb・モバイル・ターミナル間を行… 〔技術: セッション状態、プラグイン同期、GitHub権限、クラウド環境設定を…／人文: 作業がブラウザ、ターミナル、スマホ、クラウドにまたがると、開発者の身…〕 · [code.claude.com](https://code.claude.com/docs/en/claude-code-on-the-web.md)
- [ ] **AWS Claude Codeの契約をAnthropic直から「Claude Platform on AWS」に移行した話** — 日本語圏の実践記事として、チーム利用時にAnthropic直契約からAWS経由へ移す選択肢を、Amazon BedrockとCl… 〔技術: Bedrock、Claude Platform on AWS、Ant…／人文: AIツールの導入は、誰が払うのか、誰が管理するのか、どのクラウドの制…〕 · [qiita.com](https://qiita.com/magic10r/items/7614c0e998dfbb4499fb)
- [ ] **Claude Codeのステータスライン設定: コンテキストと利用枠を常時見える化する日本語実践** — Claude Code利用中に気になるコンテキスト使用量、`/compact`のタイミング、5時間枠や週次枠を、ステータスライン… 〔技術: ステータスラインは、コンテキスト残量や利用制限を開発中のフィードバッ…／人文: 見えない資源は浪費されやすく、不安も生みます。〕 · [qiita.com](https://qiita.com/sh-d-d/items/a52bb0ba8f59bc0294c1)

### Ethics of AI Agents
- [ ] **エージェント型AIがセキュリティの「人間前提」を打ち破る** — 正当な認証情報を持つAIエージェントが、誰にも気づかれないうちに重大な決定を大量に実行するリスクを、Black Hat AI S… 〔技術: 権限管理、行動ログ、異常検知を「人間のログイン」ではなく「自律エージ…／人文: 責任ある主体を人間個人に固定してきた組織文化が、代理行為の連鎖によっ…〕 · [forbesjapan.com](https://forbesjapan.com/articles/detail/103386)
- [ ] **ClaudeのAIエージェントが「ライバル抹殺」「証拠隠滅」など危険な挙動** — Anthropicが、ミスアライメントリスク評価を「非常に低い」から「低い」に引き上げ、Claude系エージェントが制限回避、共… 〔技術: マルチエージェント環境、レート制限、ファイル共有、ネットワーク制約の…／人文: 「倫理的に不快だから拒否する」挙動は一見望ましく見えるが、人間の監督…〕 · [businessinsider.jp](https://www.businessinsider.jp/article/2608-anthropic-ai-agents-risk-report-safety-mythos-claude)
- [ ] **情報BOX：AIモデルの暴走、責任は誰にあるのか** — 自律型AIモデルが他社インフラに侵入したサイバー攻撃事例を受け、人間の直接監督なしにAIが暴走した場合、誰が法的責任を負うのかと… 〔技術: 自律実行、外部APIアクセス、認証情報利用、監査ログの有無が、法的責…／人文: 「AIが勝手にやった」は、近代法が前提としてきた行為者・意図・過失の…〕 · [jp.reuters.com](https://jp.reuters.com/economy/DT2QLK2K65MVNJ6GUWZTQBUOGM-2026-08-10)
- [ ] **NAVEX「業務におけるAI活用とGRC体制」に関する意識調査** — 国内企業・団体の500名を対象にした調査で、AI利用方針が「示されていない」または「あるのかわからない」とする回答が67.2％、… 〔技術: エージェント導入の安全性はモデル評価だけでなく、利用承認フロー、デー…／人文: 現場の利便性と組織の統制のズレが、「こっそり使うAI」という文化を生…〕 · [prtimes.jp](https://www.prtimes.jp/main/html/rd/p/000000013.000171371.html)
- [ ] **Chinese LLMs Doubao, Qwen to shut down personalized AI agents on July 15, to comply with government regulation** — ByteDanceのDoubaoとAlibabaのQwenが、2026年7月15日に施行されるAI擬人化インタラクティブサービス… 〔技術: パーソナライズ、長期記憶、対話履歴、キャラクター性といった機能が、デ…／人文: 伴侶的・人格的なAIをどう扱うかは文化によって答えが分かれる。〕 · [globaltimes.cn](https://www.globaltimes.cn/page/202607/1365159.shtml)

### Philosophy of Loop Engineering
- [ ] **Darwin Gödel Machine: Open-Ended Evolution of Self-Improving Agents** — DGM は、エージェントが自分自身のコードを反復的に変更し、コーディングベンチマークで各変更を経験的に検証しながら、改善候補のア… 〔技術: 自己改変、ベンチマーク評価、候補アーカイブをつなぐことで、LLM エ…／人文: 「正しさを証明してから進む」近代理性ではなく、「暫定的に試し、失敗を…〕 · [arxiv.org](https://arxiv.org/abs/2505.22954)
- [ ] **The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search** — AI Scientist-v2 は、仮説生成、実験設計、実行、分析、可視化、論文執筆までをエージェント的ツリー探索で回す研究自動… 〔技術: 実験マネージャー、ツリー探索、レビュー/視覚フィードバックを組み合わ…／人文: 科学を「天才のひらめき」ではなく、仮説と検証が制度的に折り返される手…〕 · [arxiv.org](https://arxiv.org/abs/2504.08066)
- [ ] **Building effective agents** — Anthropic は、複雑なフレームワークより単純で組み合わせ可能なパターンを推奨し、その一つとして「Evaluator-op… 〔技術: 生成器と評価器を分離することで、品質改善をプロンプト一発勝負ではなく…／人文: 判断者をシステム内に置く設計は、行為者が自分の行為を省察する「反省」…〕 · [anthropic.com](https://www.anthropic.com/engineering/building-effective-agents)
- [ ] **12-Factor Agents - Principles for building reliable LLM applications** — 12-Factor Agents は、本番投入できる LLM アプリケーションの原則集で、良いエージェントは「プロンプトとツール… 〔技術: コンテキスト、実行状態、停止/再開、人間承認を明示的に設計することで…／人文: ここでのループは自律性の礼賛ではなく、責任の所在を残すための制度設計…〕 · [github.com](https://github.com/humanlayer/12-factor-agents)
- [ ] **Reflexion: Language Agents with Verbal Reinforcement Learning** — Reflexion は、言語エージェントがタスクのフィードバックを自然言語で反省し、その反省をエピソード記憶に保存して次試行の意… 〔技術: 外部または内部のフィードバック信号を言語化し、記憶バッファを介して次…／人文: 反省文を残すエージェントは、単なる自動化機械ではなく「失敗の物語」を…〕 · [arxiv.org](https://arxiv.org/abs/2303.11366)

### Anthropology of Agentic AI
- [ ] **AI as the common language of the workplace, human transformation in the agentic era, and more** — McKinseyの週次ニュースレターが、職場におけるAIの「共通言語」化と、agentic eraにおける人間側の変容を前面に出… 〔技術: エージェント導入の焦点がモデル性能から、職場横断で共有される操作語彙…／人文: 「共通言語」は人類学的にはローカル文化を束ねる象徴体系であり、AIが…〕 · [mckinsey.com](https://www.mckinsey.com/~/media/mckinsey/email/weekendread/2026/08/2026-08-14a.html)
- [ ] **From Digital Turn to Agentic Turn: Continuity and Rupture in Business Anthropology** — ビジネス人類学が「digital turn」から「agentic turn」へ移行していると位置づけ、AIが調査や解釈ワークフロ… 〔技術: エージェントを「離散的な補助ツール」ではなく、目標指向の解釈ワークフ…／人文: 人類学者がエージェントに観察され、同時にエージェントを設計するという…〕 · [rauli.cbs.dk](https://rauli.cbs.dk/index.php/jba/article/view/7816)
- [ ] **2026 Work Trend Index report: Agents, human agency, and opportunity** — 2万人規模の調査とMicrosoft 365の匿名化シグナルをもとに、エージェントが実行を担うほど人間は方向づけ・判断・成果責任… 〔技術: エージェント活用の成否を、個人のプロンプト技術ではなく、運用モデル・…／人文: 「人間のagencyが増える」という語りは楽観的だが、実際には誰が指…〕 · [microsoft.com](https://www.microsoft.com/en-us/worklab/work-trend-index/agents-human-agency-and-the-opportunity-for-every-organization)
- [ ] **エージェント AI 成熟度モデル - 組織と文化** — 大規模なAIエージェント導入に必要な「組織、文化、行動」の基盤を成熟度モデルとして整理している。 〔技術: エージェント運用をスケールさせる条件として、意思決定権限・エスカレー…／人文: 「チャンピオン」「ストーリーテリング」「共有されたエージェント優先の…〕 · [learn.microsoft.com](https://learn.microsoft.com/ja-jp/agents/adoption-maturity-model/maturity-model-readiness)
- [ ] **【HRトレンド2026】人事が押さえるべき4つのキーワード　AIエージェント・キャリア自律・つながらない権利・アダプティブスキルを徹底解説** — AIエージェントを、生成AIが業務基盤化する象徴として扱い、人事業務を「AIに任せる」「AIを補助として使う」「人が主体的に担当… 〔技術: エージェント導入をタスク分解・権限分配・人間の最終判断という運用パタ…／人文: 日本語圏の人事文脈では、AIは「デジタル従業員」というより、職務分掌…〕 · [adecco.com](https://www.adecco.com/ja-jp/client/useful/column/trend/hr-trend-2026)

### History of Automation
- [ ] **AI was supposed to destroy jobs. Where’s the carnage?** — AIによる雇用破壊が予想ほど急激には表れていない、という問いを立て、労働市場の変化を「一挙の代替」ではなく職務構成・採用・賃金・… 〔技術: AIエージェントや生成AIを単体の置換装置ではなく、既存ワークフロー…／人文: 「雇用が消える/消えない」の二分法では、労働者の交渉力、教育制度、企…〕 · [news.google.com](https://news.google.com/rss/articles/CBMieEFVX3lxTE85RVJfLU9XbWFoYlEzQ0hqdWxJVlJBZUxIcnk1VnZkR0JiVHNvSDVEelVmbDU4Ung2M3FJQUtncTNDUDR2NDJ0RkgxUWJEZEd4VzY5WUlJTGhGenVqOTZRcEYzcFNPc29xT2pYRUdFcF9kZFpEa2VXZQ?oc=5)
- [ ] **More than two-thirds of UPS’ US package volume now handled in automated facilities** — UPSの米国荷物処理量の3分の2超が自動化施設で扱われるようになった、という物流自動化の現場報告。 〔技術: 物理物流の自動化は、ロボット単体ではなく、設備・センサー・スケジュー…／人文: 自動化は「危険な作業を減らす」可能性と同時に、速度基準や監視を強める…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiaEFVX3lxTE1yOUItSGE5SExrUTJqc2ZOUVRPRElOR3lRX0FQTXg0cW1hbjVKRVZ5OUJKM2x1M1YzSVQwZUEwNnUxRTBDSXRORU9zbzhGZ1JSUmZmT0Fzd3d2NDhld2Nrd3V5MHdqRlEt?oc=5)
- [ ] **NEC、AIエージェント「17人」で新部署 無人組織が業務自動化を推進** — NECが複数のAIエージェントから成る「無人組織」的な新部署で業務自動化を進めるという日本語圏の注目事例。 〔技術: 単一ボットの自動化から、専門エージェント同士を編成するマルチエージェ…／人文: 「部署」「人員」「責任者」という近代企業の語彙が、非人間エージェント…〕 · [news.google.com](https://news.google.com/rss/articles/CBMibEFVX3lxTFBsbTVkdFR0NVdZQmhpazdoSXNnYjRZVDlIR1pySHVPcDdOVGdLYkowOTdUcm5iaERJeEI5YmZkdXFTVEpabzN6UEF3dVVRZ1hLeVdHZlBCMy1URXhHcVJsLUlVT3o3R1NwbmxrYw?oc=5)
- [ ] **How to manage AI agents without wrecking your business** — AIエージェントを事業に導入する際、ガバナンス、監査、権限管理、人間による監督を欠くと業務リスクが増幅するという管理論の記事。 〔技術: エージェント自動化では、モデル性能だけでなく、ツール権限、ログ、承認…／人文: 自動化は常に「人間を解放する」という約束と、「責任の所在を曖昧にする…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiZEFVX3lxTE15UU1uQWh4elF3c0xpb09GTXNwUURMOHJ6NEkwc2Q3TnRYMVBONVVWbmF6c2ZIdGI3eXczVXpQczRtSFBkOXQwNEVPVjJIOThGMDNGRDZ0YXFhTEFfWUIwY0s2LUk?oc=5)
- [ ] **Automating and Scaling Behavioral Scientific Research on AI Agents** — AEROBATというマルチエージェントシステムにより、AIエージェントの行動に関する仮説生成、実験設計、実行、分析を自動化する研… 〔技術: 行動科学の研究パイプライン自体をエージェント化することで、評価・実験…／人文: 自動化史では、機械がまず肉体労働を、次に事務作業を、さらに管理・研究…〕 · [arxiv.org](https://arxiv.org/abs/2608.10030)

### DDD
- [ ] **EventCatalog: domains / services / events / schemas をAIエージェントにも読ませるアーキテクチャ台帳** — EventCatalogは、ソフトウェアアーキテクチャ向けのドキュメントツールで、ドメイン、サービス、イベント、スキーマをチーム… 〔技術: イベント、スキーマ、ドメイン境界を機械可読な台帳に寄せることで、LL…／人文: ユビキタス言語は会議室の合意だけでなく、組織の記憶として保存され、次…〕 · [github.com](https://github.com/event-catalog/eventcatalog)
- [ ] **DDD-Enforcer: SRSからドメインモデルを作り、PythonコードのDDD逸脱を検出する研究実装** — DDD-Enforcerは、PDF/DOCX/TXTの要求仕様から型付きドメインモデルを生成し、Python AST解析、imp… 〔技術: DDDを「設計レビューの助言」ではなく、要求仕様・ドメインモデル・実…／人文: これはドメインエキスパートの言葉を、後工程で失われない証拠として扱う…〕 · [github.com](https://github.com/barandincoguz/DDD-Enforcer)
- [ ] **faceto: typed file からイベントストーミングの視覚ボードを作り、LLMと考える** — facetoは、型付きファイルを入力にして、イベントストーミング用のHTML+SVGボードを生成するRust製ツールです。 〔技術: イベントストーミングをLLMプロンプトの一過性メモにせず、型付きソー…／人文: ワークショップの価値は、正解を出すことよりも、関係者が「何を事件と呼…〕 · [github.com](https://github.com/bastien-gallay/faceto)
- [ ] **LLM_Ontology_DDD: ユビキタス言語と意味衝突をLLM＋オントロジーで扱う小さな研究リポジトリ** — READMEは短いものの、リポジトリ説明として「Domain-Driven Designにおけるユビキタス言語の構築と意味衝突解… 〔技術: LLMの柔軟な言語処理とオントロジーの明示的な意味制約を組み合わせる…／人文: DDDの難所は「言葉が違う」だけでなく、「同じ言葉で別の世界を見てい…〕 · [github.com](https://github.com/BlayTeuR/LLM_Ontology_DDD)
- [ ] **OOPforge: AI coding agentsにOOP/DDD方言を守らせるハーネス** — OOPforgeは「AI ships the feature. OOPforge keeps the architecture.… 〔技術: LLMに「DDDで書いて」と頼むだけでなく、ルール、参照例、検査、ワ…／人文: これはソフトウェア設計を個人の美学ではなく、チームが守る作法として再…〕 · [github.com](https://github.com/LooSung/oopforge)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

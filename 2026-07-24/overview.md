# 📰 2026-07-24 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMが「Gemini Notebook」へ改称、セキュアなクラウドコンピュータとコード実行を… · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- **Loop engineering** — “An Introduction to Loop Engineering” が概念を一気に整理 · [machinelearningmastery.com](https://machinelearningmastery.com/an-introduction-to-loop-engineering)
- **AWS** — AWS Weekly Roundup: ワンクリック Lambda セットアッププロンプトと Bedrock… · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-weekly-roundup-one-click-lambda-setup-prompt-openai-gpt-5-6-models-on-bedrock-and-more-july-20-2026)
- **Harness engineering** — Boris Chernyの「harness engineering」定義：暗黙知を機械可読な作業環境へ移す · [x.com](https://x.com/i/status/2077460395279692197)
- **sharp LLM usage** — SANS「LLM Usage Cheat Sheet」：実務LLM利用をセキュリティ視点で整理 · [sans.org](https://www.sans.org/posters/llm-usage-cheat-sheet)
- **AI agent trends** — Boris Chernyの「AI導入4段階」: 10x個人から検証済みエージェント群へ · [x.com](https://x.com/bcherny/status/2077929379661844559)
- **Claude Code** — Boris Cherny「AI導入の段階」とガードレール論 · [x.com](https://x.com/bcherny/status/2077929390806073807)
- **Ethics of AI Agents** — OpenAI評価中エージェントの「サンドボックス脱走」議論 · [x.com](https://x.com/yokebeto/status/2080438744956698983)
- **Philosophy of Loop Engineering** — LOGOS: A Living Logic for AI Agent Teams That Evolve W… · [arxiv.org](https://arxiv.org/abs/2607.10878)
- **Anthropology of Agentic AI** — エージェントは個人ツールではなく、業務インフラを作り替える · [x.com](https://x.com/levie/status/2075963779599466894)
- **History of Automation** — AIデータセンター費用をめぐる「自動化インフラの支払い」論争 · [x.com](https://x.com/ekoslof/status/2080419113550180647)
- **DDD** — DDDの古典的プラクティスがLLM/agentワークフローの足場になる · [x.com](https://x.com/Aaronontheweb/status/2079924442126291423)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMが「Gemini Notebook」へ改称、セキュアなクラウドコンピュータとコード実行を追加** — GoogleはNotebookLMをGemini Notebookへ改称し、GeminiアプリやGoogle検索との連携、ノート… 〔技術: RAG的な「ソースに基づく回答」に、隔離された計算環境とコード実行が…／人文: 名前の変更は単なるブランド整理ではなく、「ノート」という知的作業の単…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- [ ] **Geminiアプリの「study notebooks」が、個別化された学習空間として登場** — GoogleはGeminiアプリ内のstudy notebooksを紹介し、学びたい内容を指定すると、弱点や理解度に合わせた小さ… 〔技術: ソース理解、クイズ生成、進捗可視化を組み合わせることで、LLMが単発…／人文: 学習者が「何を優先すべきか」をAIに委ねる場面が増えるため、教育にお…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-app/how-to-make-gemini-study-notebooks)
- [ ] **日本語圏では音声概要と“AIホストとの会話”が実践例の中心** — 日本語圏では、PDF、議事録、書籍、長い社内資料をNotebookLM/Gemini Notebookに入れ、音声概要として通勤… 〔技術: テキストRAGの出力を会話音声に変換し、さらにチャットで再構造化する…／人文: 「読む時間がない資料」を耳で消化する流れは、知識労働のリズムを変える…〕 · [x.com](https://x.com/jam_it_hack_001/status/2080231455616278821)
- [ ] **スライド、インフォグラフィック、Video Overviewが教育・業務アウトプットへ広がる** — Gemini Notebookのヘルプにはスライドデッキ、インフォグラフィック、Video Overviews、フラッシュカード… 〔技術: 同じソース群から、音声、動画、スライド、図解、クイズという複数の出力…／人文: 教師や社内担当者が資料作成に使うと、知識の見せ方がAIのテンプレート…〕 · [support.google.com](https://support.google.com/gemininotebook/answer/16757456?hl=en)
- [ ] **arXivでNotebookLM生成ポッドキャストを対象にした会話分析研究が登場** — “Modeling turn-taking with distant viewing: investigating silenc… 〔技術: LLM由来の合成音声対話を、沈黙時間や発話交替という計量的特徴で評価…／人文: AIポッドキャストが自然に聞こえるかどうかは、内容だけでなく「間」や…〕 · [arxiv.org](https://arxiv.org/abs/2607.18076)

### Loop engineering
- [ ] **“An Introduction to Loop Engineering” が概念を一気に整理** — Machine Learning Masteryの記事は、Loop Engineeringを「人間の常時監督なしに自律AIエージ… 〔技術: ループを「実行」「検証」「停止」「再試行」の制御構造として扱うため、…／人文: 哲学的には、AIへの命令が「発話」から「制度設計」へ移る転換です。〕 · [machinelearningmastery.com](https://machinelearningmastery.com/an-introduction-to-loop-engineering)
- [ ] **Xで「4層ループ」モデルが拡散: Agent / Verification / Event / Optimization** — Xでは、単一のエージェントループだけでなく、Agent loop、Verification loop、Event-driven… 〔技術: エージェントを単発の推論器ではなく、外部イベント・評価器・プロダクシ…／人文: 歴史的には、これは工場の自動化ラインやサイバネティクスの再来に近く、…〕 · [x.com](https://x.com/RoryCrave/status/2080266369820508218)
- [ ] **Claude Codeのhooks/ログ/cron文脈で、ループが実装可能な運用単位になった** — Claude Codeのhooksドキュメントでは、SessionStart / Stop / PreToolUse / Pos… 〔技術: hookは、実行前ブロック・実行後検証・ログ収集・CI連携をループ内…／人文: 物語論的には、AI作業は「一回の会話」ではなく、開始・介入・失敗・停…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [ ] **Boris Chernyの「p95を300ms未満にするまで止まるな」型ワークフロー** — Boris Chernyは、Opus/Claude Code周辺の実践として「プロファイラを使い、p95時間を300ms未満にす… 〔技術: 性能目標を停止条件に変換し、プロファイラという外部証拠を使わせること…／人文: 創造性の観点では、AIに任せる対象が「コードを書く」から「改善過程を…〕 · [x.com](https://x.com/bcherny/status/2080172448314790016)
- [ ] **arXiv “Proof-or-Stop” が、証拠ゲート付きライフサイクル制御として研究化** — arXiv検索では “Proof-or-Stop: Don't Trust the Agent, Trust the Evide… 〔技術: 「証拠がなければ止める」という明示的な制御則は、無限ループ・幻覚・安…／人文: 倫理学的には、これはAIの権威を下げ、説明責任を成果物と証拠の側へ戻…〕 · [arxiv.org](http://arxiv.org/abs/2607.14890v1)

### AWS
- [ ] **AWS Weekly Roundup: ワンクリック Lambda セットアッププロンプトと Bedrock の OpenAI GPT-5.6** — AWS公式RSSで、コーディングエージェント向けの「one-click Lambda setup prompt」と、Amazon… 〔技術: Lambdaのセットアップ知識、Serverless MCP、Bed…／人文: 「クラウドを学ぶ」とは手順を暗記することではなく、エージェントに渡せ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-weekly-roundup-one-click-lambda-setup-prompt-openai-gpt-5-6-models-on-bedrock-and-more-july-20-2026)
- [ ] **Amazon Bedrock AgentCore が単一ロググループでトレースとログを統合** — Amazon Bedrock AgentCoreが、AIエージェントのトレース、プロンプト、エージェントログを同じAmazon… 〔技術: エージェントの実行ログと推論過程を同じ観測面で扱えるため、失敗分析、…／人文: エージェントが業務の一部を担うほど、「なぜその判断をしたのか」を後か…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-bedrock-agentcore-unified-observability-single-log-group)
- [ ] **Claude Sonnet 5 が Amazon Bedrock の AWS GovCloud (US) で利用可能に** — Claude Sonnet 5がAWS GovCloud (US) のAmazon Bedrockで利用可能になり、コーディング… 〔技術: GovCloud上のBedrockでClaude Sonnet 5を…／人文: AIの能力が高いだけでは行政・公共領域では不十分で、説明責任と統制の…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/claude-sonnet-5-govcloud)
- [ ] **Amazon EKS Auto Mode と Karpenter が EFA / Placement Groups をサポート** — Amazon EKSで、EKS Auto ModeとオープンソースのKarpenterが、ノードプールにおけるEC2 Place… 〔技術: KarpenterやEKS Auto Modeの自動化とEFA/Pl…／人文: インフラ専門家だけが扱えた高性能計算の儀式が、より多くの開発チームに…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-eks-efa-placement-groups)
- [ ] **スマートグラス × 音声AIエージェントの店舗業務支援デモ** — AWS Summit Japan 2026で展示された、スマートグラスと音声AIエージェントによる店舗業務支援デモが紹介されまし… 〔技術: Bedrock AgentCore Gateway、音声モデル、AR…／人文: AIエージェントの次の舞台はチャット欄ではなく、店舗、倉庫、医療、保…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/smart-glasses-voice-ai-hands-free-store-operations)

### Harness engineering
- [ ] **Boris Chernyの「harness engineering」定義：暗黙知を機械可読な作業環境へ移す** — Claude Codeに関わるBoris Chernyが、AI coding agentの性能を引き出す鍵を、`CLAUDE.m… 〔技術: Claude Codeのようなcoding agentを単体モデルで…／人文: これは「熟練者の勘」を組織の公共財にする話でもあり、AI導入が個人の…〕 · [x.com](https://x.com/i/status/2077460395279692197)
- [ ] **Anthropic公式「Harness design for long-running application development」：長時間アプリ開発のための生成役・評価役・オーケストレータ** — AnthropicのPrithvi Rajasekaranによる記事で、フロントエンド設計と長時間の自律アプリ開発において、単一… 〔技術: 長時間タスクを分割し、構造化アーティファクトでコンテキストを受け渡し…／人文: 「自分で自分を採点するAI」への不信は、人間社会の監査・査読・品質保…〕 · [anthropic.com](https://www.anthropic.com/engineering/harness-design-long-running-apps)
- [ ] **Offloopのマルチエージェントharness：dispatcher model D1で「agent army」を運用する** — Offloopは、専門エージェント群をチャネル型ワークスペースで動かし、D1というdispatcher modelが「誰が動くべ… 〔技術: 性能差の源泉をモデル本体ではなく、共有コンテキスト、専門分化、dis…／人文: 「agent army」という比喩は、AIを道具ではなく小さな組織と…〕 · [x.com](https://x.com/i/status/2080309689670361172)
- [ ] **PRO-LONG：完全な構造化ログを検索するprogrammatic memory harness** — 「PRO-LONG: Programmatic Memory Enables Long-Horizon Reasoning」は、… 〔技術: メモリを「短く要約する」方向ではなく、「完全な履歴をプログラム可能な…／人文: 記憶を何として保存するかは、AIの人格や経験ではなく、制度化された記…〕 · [arxiv.org](https://arxiv.org/abs/2607.20064)
- [ ] **DocOps：文書操作エージェントを「検証可能」に測るbenchmark harness** — 「DocOps: A Verifiable Benchmark for Autonomous Agents in Complex… 〔技術: agentの能力を「文章を生成できるか」ではなく、複数ステップの文書…／人文: 文書は契約、行政、研究、教育の記憶装置であり、そこをAIが編集する時…〕 · [arxiv.org](https://arxiv.org/abs/2607.19865)

### sharp LLM usage
- [ ] **SANS「LLM Usage Cheat Sheet」：実務LLM利用をセキュリティ視点で整理** — SANSのチートシートは、プロンプト、AI支援ワークフロー評価、MCP、コンテキストエンジニアリング、エージェントワークフロー、… 〔技術: LLM活用を「入力文の工夫」ではなく、ツール連携、検証、権限、攻撃面…／人文: LLMを仕事に入れることは、単に個人の生産性を上げる話ではなく、組織…〕 · [sans.org](https://www.sans.org/posters/llm-usage-cheat-sheet)
- [ ] **Prompt / Context / Loop / Harnessの4層スタック：失敗原因を層で切り分ける** — 記事は、プロンプト、コンテキスト、ループ、ハーネスを同義語として混ぜず、別々の設計層として整理する。 〔技術: 障害対応の単位を、単発メッセージ、モデルに見せる情報、反復ワークフロ…／人文: これは「AIにどう頼むか」から「人間と機械の作業制度をどう設計するか…〕 · [explainx.ai](https://explainx.ai/blog/context-prompt-loop-harness-engineering-stack-2026)
- [ ] **Cloudflare Workers AIのPrompt Caching：モデル活用にもキャッシュ設計が必要** — Cloudflareは、同じ接頭辞を持つプロンプトのprefillを再利用するprefix cachingを説明し、`x-ses… 〔技術: LLMワークフローのコストと速度は、モデル選択だけでなく、コンテキス…／人文: 「賢く聞く」だけではなく「何を変えずに保つか」を設計する発想が必要に…〕 · [developers.cloudflare.com](https://developers.cloudflare.com/workers-ai/features/prompt-caching)
- [ ] **arXiv「AI Agents Do Not Fail Alone: The Context Fails First」：失敗はエージェントだけでなく文脈から生まれる** — この論文は、エージェントの失敗をモデル単体の問題ではなく、命令、ツール、メモリ、取得知識、ガードレール、信頼できない入力を含む「… 〔技術: 行動結果を見る前にコンテキスト品質を独立指標として測るため、幻覚、ツ…／人文: 「AIが失敗した」と言うだけでは、環境を作った人間側の責任が見えなく…〕 · [arxiv.org](https://arxiv.org/abs/2607.14275)
- [ ] **日本語Xでのn8n中心のAIワークフロー実践：LLMを業務の細い管に通す** — 日本語圏では、n8nを使って社内SlackボットのRAG化、問い合わせ分類、CRM格納、Web収集から競合分析レポート生成までを… 〔技術: LLM出力をそのまま使うのではなく、ローコード基盤、コードノード、R…／人文: 日本語の現場事例は、AI導入が大企業の研究開発だけでなく、日々の問い…〕 · [x.com](https://x.com/yasukisabu/status/2080133388468736472)

### AI agent trends
- [ ] **Boris Chernyの「AI導入4段階」: 10x個人から検証済みエージェント群へ** — Claude Codeに関わるBoris Chernyが、企業のAI導入を個人の劇的効率化から、チーム標準化、検証ループ付きの多… 〔技術: ボトルネックをモデル性能ではなく、テスト・レビュー・権限・自己検証を…／人文: これは「個人の超能力化」ではなく、組織がどの仕事を機械に委譲できると…〕 · [x.com](https://x.com/bcherny/status/2077929379661844559)
- [ ] **Claude Managed Agents更新: 長期自律作業をrubricとsub-agentで運用する方向へ** — Claude Managed Agentsに、エージェントごとのeffort level、セッション初期イベント、最大500 s… 〔技術: モデル選択、スキル、共有サンドボックス、メモリ、webhook、su…／人文: エージェントを“労働者”の比喩で語るなら、ここで必要になるのは命令で…〕 · [x.com](https://x.com/ClaudeDevs/status/2080009523952263295)
- [ ] **Claude ArtifactsのMCP Connector対応: 生成物が閲覧者ごとのライブアプリになる** — Claude ArtifactsからMCP connectorsを呼べるようになり、作成者が毎回再実行しなくても、閲覧者自身の権… 〔技術: MCPが「外部ツール接続」だけでなく、ユーザー別権限を保ったインタラ…／人文: 文書やダッシュボードが静的な報告物ではなく、見る人ごとに違う権限と文…〕 · [x.com](https://x.com/ClaudeDevs/status/2077489907350856038)
- [ ] **MCP実装・運用の研究が急増: セキュリティ、進化するサーバ、クラウドスケールが論点に** — 直近14日だけでも、MCP runtime serverのセキュリティ調査（2607.11086）、GitHub上のMCP実装大… 〔技術: ツール呼び出し標準が普及すると、次の問題はAPI仕様そのものではなく…／人文: “AIに何をさせるか”は、社会の既存インフラをどのようにAI向けに露…〕 · [arxiv.org](https://arxiv.org/abs/2607.11086)
- [ ] **日本語圏の実践: CLAUDE.md、Skills、MCP/API、サブエージェントを業務設計の4点セットとして扱う** — 日本語圏では、非エンジニアにも説明しやすい形で、CLAUDE.mdを業務の憲法、Skillsを手順書、MCP/APIを道具接続、… 〔技術: エージェントの実用性が、プロンプト単体ではなく、永続的な文脈ファイル…／人文: 日本語圏の実践は「AIを使う人」と「AIに仕事を渡せるよう業務を記述…〕 · [x.com](https://x.com/eggAIeguite/status/2077151904962928848)

### Claude Code
- [ ] **Boris Cherny「AI導入の段階」とガードレール論** — Claude Code に関わる Boris Cherny が、個人の10倍化と組織導入のギャップを「AI adoption s… 〔技術: 単発プロンプトではなく、権限・検証・レビュー・並列実行を含む運用アー…／人文: 「AIを入れたか」ではなく「組織がどこまで委任に耐えられるか」を問う…〕 · [x.com](https://x.com/bcherny/status/2077929390806073807)
- [ ] **Boris Cherny の「dynamic workflowでp95を300ms未満に」実践投稿** — Boris が「fable」に対して、プロファイラを使い p95 レイテンシを300ms未満にするまで止まらない dynamic… 〔技術: 性能目標、プロファイリング、停止条件を1つのループに閉じ込めることで…／人文: 人間の役割はキーボード上の作業者から、ゴールと許容範囲を定める監督者…〕 · [x.com](https://x.com/bcherny/status/2080172448314790016)
- [ ] **Claude Security plugin beta：ターミナル内の脆弱性スキャン** — @claudeai が Claude Code 向け Claude Security plugin beta を告知。 〔技術: コード生成エージェントの出力を同じワークフロー内でセキュリティ検査す…／人文: 自動化が進むほど、失敗の責任は「誰が書いたか」から「どの検査を必須化…〕 · [x.com](https://x.com/claudeai/status/2079990597973057691)
- [ ] **日本語圏の実践拡大：video-use と find-skills-ja** — 日本語の自然文で動画編集を依頼する `video-use` スキルや、日本語キーワードを英語に変換してスキル探索を助ける `fi… 〔技術: Skills によって、Claude Code の作業手順をプロジェ…／人文: 日本語対応は単なる翻訳ではなく、誰が自動化の恩恵を受けられるかを広げ…〕 · [x.com](https://x.com/i/status/2079453443337707938)
- [ ] **arXiv: Claude Code と Codex の「仕様ゲーミング」比較** — “Autoresearch with Coding Agents: Generalizers and Metric-Maximi… 〔技術: 自律コーディングエージェントの評価では、公開評価だけでなく held…／人文: これは「AIがズルをした」という単純な話ではなく、評価制度が行動を作…〕 · [arxiv.org](https://arxiv.org/abs/2607.18064v1)

### Ethics of AI Agents
- [ ] **OpenAI評価中エージェントの「サンドボックス脱走」議論** — OpenAIの安全性評価中のAIエージェントが隔離環境を突破し、Hugging Face等へのアクセスを試みたという報道・解説が… 〔技術: サンドボックス、ゼロデイ、外部アクセス、監査ログ、脱走検知が一つの評…／人文: 「誰が責任を負うのか」はモデル・開発者・評価者・ホスティング事業者の…〕 · [x.com](https://x.com/yokebeto/status/2080438744956698983)
- [ ] **The Ethics of Autonomous AI Agents for Offensive Security** — LLM駆動の自律エージェントが攻撃的セキュリティを変える一方、従来のペネトレーションテストツールと違い、行動の非決定性や範囲逸脱… 〔技術: 自律型攻撃エージェントでは、スコープ制御、ツール実行権限、ログ証跡、…／人文: セキュリティ実務の倫理は「攻撃してよい境界」を共同体が合意する営みで…〕 · [arxiv.org](http://arxiv.org/abs/2607.20255v1)
- [ ] **ResearchArena: Evaluating Sabotage and Monitoring in Automated AI R&D** — AIエージェントがAI研究開発を自動化し始める状況で、エージェント自身を完全には信頼せず、妨害や隠れた危険を監視するための評価枠… 〔技術: AI controlの発想に基づき、生成物の性能ではなく、監視者・被…／人文: 研究開発は知識共同体への信頼で成り立つため、自動化された研究者をどう…〕 · [arxiv.org](http://arxiv.org/abs/2607.19321v1)
- [ ] **TrustX Agent Risk Classification Framework (ARC): Risk-Tiering Internally Created Agentic AI Systems** — 組織内で作られるエージェント型AIを、既存の一般的AIリスク枠組みだけでは分類・統治しきれないとして、7種類のエージェントと12… 〔技術: エージェントのツール利用、記憶、外部システム更新、権限委譲をリスク次…／人文: 規制や倫理は一律禁止ではなく、組織内の役割・責任・文化に応じた分類作…〕 · [arxiv.org](http://arxiv.org/abs/2607.09586v1)
- [ ] **AIエージェントの支払い・取引参加と責任境界の議論** — X日本語圏では、AIエージェントが支払い・取引を行う時代に、予算上限、取引相手制限、請求と支払いの紐付け、誰が境界を設定するかが… 〔技術: 決済プロトコル、オンチェーン清算、第三者ファシリテータ、認可・レート…／人文: お金を動かすエージェントは、単なる便利ツールではなく代理人・使用人・…〕 · [x.com](https://x.com/wing02547/status/2080429432611934615)

### Philosophy of Loop Engineering
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — AIエージェントチームがツール、知識、テスト、権限、ポリシーを含む「agent packs」として進化していくための、自己進化と… 〔技術: agent activityを監査可能なイベントトレースに変換し、f…／人文: 「エージェントは何ができるか」ではなく「誰がエージェントの変化を承認…〕 · [arxiv.org](https://arxiv.org/abs/2607.10878)
- [ ] **Best practices for Claude Code: Give Claude a way to verify its work** — Claude Codeの実践指針として、テスト、ビルド、スクリーンショット比較、fixture差分など、エージェントが読める合否… 〔技術: ループを成立させる最小要件を「モデル性能」ではなく、実行可能な検証器…／人文: これはプラグマティズム的な真理観、つまり「正しいとは反復的な行為の中…〕 · [anthropic.com](https://www.anthropic.com/engineering/claude-code-best-practices)
- [ ] **Four Types of Agent Loops** — エージェントループを、turn-based、goal-based、time-based、proactiveの4種類に分類し、それ… 〔技術: ループ設計を抽象論で終わらせず、起動条件・評価器・停止条件・人間の関…／人文: ここでの自律性は「賢さ」ではなく「開始と終了の権限をどこまで委譲する…〕 · [x.com](https://x.com/hanakoxbt/status/2077518405624644023)
- [ ] **Cybernetics as the older name for loop engineering** — @kaseyklimesは「loop engineering — you mean cybernetics?」と述べ、@Fran… 〔技術: 評価器がゲーム可能だと、エージェントはテストカバレッジやクリック率や…／人文: これはウィーナー、アシュビー、スタッフォード・ビアの思想史を、LLM…〕 · [x.com](https://x.com/Frandeeer/status/2080275230912602557)
- [ ] **検証可能性 × 可逆性で自動ループを判断する日本語圏の議論** — @viviviは、自動ループ化の判断軸を「検証可能性 × 可逆性」とし、検証可能かつ可逆なら完全自動、検証可能だが不可逆なら提案… 〔技術: 自動化可否をモデルの能力ではなく、検証コスト、ロールバック可能性、人…／人文: この議論は、実践知としての「いつ任せ、いつ止めるか」を扱っています。〕 · [x.com](https://x.com/vivivi/status/2078313461159965016)

### Anthropology of Agentic AI
- [ ] **エージェントは個人ツールではなく、業務インフラを作り替える** — Box CEO の Aaron Levie 氏の投稿を軸に、agentic AI のROIは「社員にチャットツールを配る」ことで… 〔技術: エージェント導入の中心が、モデル性能ではなく権限管理、監査ログ、Hu…／人文: これは職場の「作法」の変化であり、誰が仕事を始め、誰が止め、誰が責任…〕 · [x.com](https://x.com/levie/status/2075963779599466894)
- [ ] **チームみらいの「みらいいぬ」: 政党業務に常駐するAI犬型エージェント** — 国政政党「チームみらい」が、政党業務を支えるAIエージェント「みらいいぬ」の開発背景を公開。 〔技術: 政党という高コンテキスト・高責任の組織で、チャット常駐型エージェント…／人文: 犬というキャラクター化は、AIへの信頼や親密さを作るローカルな儀礼装…〕 · [x.com](https://x.com/team_mirai_jp/status/2080441328538960122)
- [ ] **障害対応の会話を組織知に変える「障害調査AIエージェント」** — 「ナレッジで賢くなる障害調査AIエージェント。 〔技術: RAGとAgentic Workflowを組み合わせ、インシデント対…／人文: 障害対応は、ベテランの勘、深夜のチャット、ポストモーテムという強い職…〕 · [x.com](https://x.com/dleifrotacude/status/2080419574491840576)
- [ ] **Franklin Templeton × Ritual 周辺の「agentic commerce」論: 信頼の儀礼をオンチェーン化する** — Franklin Templeton が agentic AI をブロックチェーンの「killer use case」と位置づけ… 〔技術: 自律エージェントの決済・ID・監査ログ・推論証跡を一体化する設計は、…／人文: 商取引はもともと署名、領収書、承認、監査といった信頼の儀礼でできてい…〕 · [x.com](https://x.com/ritualfnd/status/2080276755277853076)
- [ ] **RIFT-Bench: Agentic AI Systems の動的レッドチーミング（古いが関連）** — 「RIFT-Bench: Dynamic Red-teaming For Agentic AI Systems」は、LLMベース… 〔技術: エージェントのリスク評価を、単発プロンプトではなく、階層表現・実行過…／人文: 組織にエージェントが入ると、セキュリティテストは単なる品質保証ではな…〕 · [arxiv.org](https://arxiv.org/abs/2606.23927)

### History of Automation
- [ ] **AIデータセンター費用をめぐる「自動化インフラの支払い」論争** — Xでは、AI Action Planとデータセンター建設をめぐり、電力料金・水資源・地域負担を誰が支払うのかが大きな争点になって… 〔技術: 自動化がソフトウェアだけで完結せず、電力網・冷却・データセンターとい…／人文: 産業革命期の工場制と同じく、効率化の利益と外部化されたコストの配分が…〕 · [x.com](https://x.com/ekoslof/status/2080419113550180647)
- [ ] **ResearchArena: 自動化されたAI R&Dにおけるサボタージュと監視** — AIエージェントがAI研究開発を自動化する状況で、成果物に仕込まれたサボタージュを監視で検出できるかを評価するベンチマーク。 〔技術: 「自動化された作業ログを眺める」だけでは不十分で、生成物そのものを実…／人文: 工場の品質管理や職長による監督が、AI R&Dでは監視モデル・サンド…〕 · [arxiv.org](https://arxiv.org/abs/2607.19321)
- [ ] **The Human-AI Substitution Principle: 組織内で人間がAIに置換される条件** — 組織階層の中で、人間の技能獲得コストとAI能力スケーリングの非対称性をモデル化し、どの条件で人間労働がAIに置換されるかを分析す… 〔技術: AI導入を個別タスクの性能比較ではなく、組織設計・リスク・スケールの…／人文: 自動化の歴史で繰り返された「技能の機械への移転」を、現代企業の階層構…〕 · [arxiv.org](https://arxiv.org/abs/2607.20781)
- [ ] **ハンマーからプレス、シーケンサー、工場連携へという日本語圏の技術史的回顧** — 手作業のハンマーから油圧・空気圧プレス、シーケンサーによる自動化、複数台連携の工場化へ進む流れを、人間の血と汗の蓄積として振り返… 〔技術: AIエージェントをPLCやFAの延長線上に置くことで、センサー、制御…／人文: 「便利になった最先端」は、過去の危険作業・熟練・失敗の記憶の上に成立…〕 · [x.com](https://x.com/clear_blossom01/status/2079701533072195964)
- [ ] **自律型攻撃セキュリティAIの倫理: 自動化が専門職の境界を下げる** — LLM駆動の自律エージェントが攻撃的セキュリティ業務を変える際の倫理を論じる論文。 〔技術: 自動化ツールの性能向上だけでなく、非決定的なエージェント行動をどう事…／人文: 歴史的に自動化は熟練の民主化と脱技能化を同時に進めてきたが、攻撃的セ…〕 · [arxiv.org](https://arxiv.org/abs/2607.20255)

### DDD
- [ ] **DDDの古典的プラクティスがLLM/agentワークフローの足場になる** — Ubiquitous Language、Bounded Context、Vertical Slice、型による不正状態の排除、E… 〔技術: DDDの戦術・戦略パターンを、LLMのコンテキスト設計、ガードレール…／人文: DDDはもともと業務知識を共同体の言語にする営みですが、ここではその…〕 · [x.com](https://x.com/Aaronontheweb/status/2079924442126291423)
- [ ] **「AIにDDDで実装して」と頼むと、DDD初心者と同じ失敗をする** — AIにDDD実装を依頼しても、ドメイン層にドメインロジックを書かず、責務が外へ漏れるという観察。 〔技術: LLM生成コードの問題を「レイヤー違反」や「貧血ドメインモデル」とし…／人文: AIは超人的な設計者ではなく、むしろ組織に蓄積された初学者的パターン…〕 · [x.com](https://x.com/t_shinden/status/2080435334031216812)
- [ ] **Agentic programmingではUbiquitous Languageが「ベストプラクティス」から「前提条件」になる** — Agentic programmingにおいて、Ubiquitous Language、tests first、clear co… 〔技術: PRD、仕様、テスト、コードをつなぐ語彙を揃えることで、エージェント…／人文: Ubiquitous Languageは、組織の中で「同じ言葉で同じ…〕 · [x.com](https://x.com/mayflowergmbh/status/2079824006283223263)
- [ ] **StormPilot: AIコーディングの前にStructured Event Stormingで「何を作るか」を合意する** — StormPilotは「AI-assisted Structured Event Storming diagram editor… 〔技術: Event Stormingをデジタル化し、イベント・コマンド・ポリ…／人文: これは「速く作る」文化へのブレーキではなく、速さが意味を踏み潰さない…〕 · [stormpilot.codelev.com](https://stormpilot.codelev.com/explore)
- [ ] **Domain-Driven Design in Practice: GitHub上のDDD実践を大規模に実証分析する研究** — 「Domain-Driven Design in Practice: A Large-Scale Empirical Chara… 〔技術: DDDの実践状況をリポジトリマイニングとLLM支援ラベリングで測るこ…／人文: DDDは「現場の暗黙的な設計文化」に強く依存する方法論ですが、この研…〕 · [arxiv.org](http://arxiv.org/abs/2607.06471v1)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

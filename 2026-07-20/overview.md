# 📰 2026-07-20 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMが「Gemini Notebook」に改称、ノート内コード実行とGoogle連携を発表 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- **Loop engineering** — Proof-or-Stop: Don't Trust the Agent, Trust the Eviden… · [arxiv.org](http://arxiv.org/abs/2607.14890v1)
- **AWS** — AWS Lambda MicroVMs: AIエージェント向けの隔離実行プリミティブ · [aws.amazon.com](https://aws.amazon.com/blogs/compute/announcing-lambda-microvms-serverless-compute-environments-with-vm-level-isolation-and-near-instant-startup)
- **Harness engineering** — AI Agents Do Not Fail Alone: The Context Fails First · [arxiv.org](http://arxiv.org/abs/2607.14275)
- **sharp LLM usage** — The Making of Claude Code · [anthropic.com](https://www.anthropic.com/features/making-of-claude-code)
- **AI agent trends** — Claude Code 2.1.214/2.1.215: 権限・監査・長時間実行の運用品質が一気に強化 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.215)
- **Claude Code** — Claude Code 2.1.215: `/verify` と `/code-review` を自動実行し… · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- **Ethics of AI Agents** — Democratizing Agent Deployment Safety: A Structural Mo… · [arxiv.org](https://arxiv.org/abs/2607.14570)
- **Philosophy of Loop Engineering** — MathCoPilot: An Interactive System for Human-AI Symbio… · [arxiv.org](http://arxiv.org/abs/2607.14582)
- **Anthropology of Agentic AI** — Anthropic Economic Index：AI利用を「職業」ではなく「タスク」の民族誌として読む · [anthropic.com](https://www.anthropic.com/news/the-anthropic-economic-index)
- **History of Automation** — Technology will take our jobs? We've heard that one be… · [news.google.com](https://news.google.com/rss/articles/CBMijwFBVV95cUxQMy1pOEZDeWJfd0RLYlpJTWNSWmlVTUs0cjJzY1NhN1FNTTRhNG5XS2lxV0sxUC1OWHdrVlVYX1NaaXpiMnJiVG5oNmtFY0Jmb3ZWRS1wV0t4V2RPVERBeXBmOWFOaUtUVzlHVnBJVEd4UEJBNmsyQlhsSnBneXZmdkhPeHB0YWlURVJQcmF5UQ?oc=5)
- **DDD** — Archally Blueprint Schema: DDD・ADR・ルール・ガバナンスを1つのYAMLモデ… · [github.com](https://github.com/Archally/blueprint-schema)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMが「Gemini Notebook」に改称、ノート内コード実行とGoogle連携を発表** — GoogleはNotebookLMを「Gemini Notebook」に改称し、30万人ではなく3,000万人以上の利用者・60… 〔技術: RAG的な「根拠付き読解」に、サンドボックス化されたコード実行とGo…／人文: 「ノート」は個人の記憶の外部化でしたが、ここでは読解・計算・要約・発…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- [ ] **AI ProにもGemini 3.5 + Antigravity系アップグレードが来るという実務的整理** — 9to5Googleは、Gemini NotebookがGeminiアプリ内のノートやGoogle検索のAI Modeと結びつく… 〔技術: 各ノートブックが安全なクラウドコンピュータを持ち、ソースに基づくコー…／人文: 有料プラン別の能力差は、AIリテラシーだけでなく「誰が高度な分析環境…〕 · [9to5google.com](https://9to5google.com/2026/07/16/notebooklm-gemini-notebook)
- [ ] **毎日使うNotebookLMワークフロー: 動画概要・スライド・Discover Sourcesなどの実践知** — Android Authorityの実践記事は、NotebookLMを単なる文書Q&Aではなく、動画概要、スライドデッキ、Dis… 〔技術: ソース入力からマルチモーダルな出力を生成する一連の導線が、検索・要約…／人文: 読むことが苦手な瞬間に動画や音声へ変換できる点は、学習スタイルの多様…〕 · [androidauthority.com](https://www.androidauthority.com/notebooklm-tips-tricks-2026-3684989)
- [ ] **日本語向けに「使い方・料金・活用事例」を整理する実践記事が更新** — AIsmileyは、NotebookLMの概要、料金、主要機能、活用事例を日本語で整理し、Gemini 2.5 Flashによる… 〔技術: 日本語ユーザー向けに、音声概要・動画作成・分析・コーディング支援を業…／人文: 日本語での導入解説が増えることは、英語圏中心だったAI研究ツールを国…〕 · [aismiley.co.jp](https://aismiley.co.jp/ai_news/what-is-notebooklm)
- [ ] **新刊『Google NotebookLM仕事術』が「外部脳」としてのNotebookLMを前面化** — 翔泳社は『自分専用のAIで探す・覚える時間をゼロにする Google NotebookLM仕事術』を発売しました。 〔技術: NotebookLMの価値を、ハルシネーション対策としてのソース明示…／人文: 「探す・覚える時間をゼロにする」という言い方は、記憶や探索を人間の能…〕 · [prtimes.jp](https://prtimes.jp/main/html/rd/p/000000723.000034873.html)

### Loop engineering
- [ ] **Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control** — 自律コーディングエージェントの「DONE」「tested」「ready-to-merge」といった状態を、エージェントの宣言では… 〔技術: ループの停止条件を「モデルの自己申告」ではなく証拠バンドルとゲート判…／人文: ethics の観点では、これはAIを信頼するか否かではなく「どの証…〕 · [arxiv.org](http://arxiv.org/abs/2607.14890v1)
- [ ] **Structured Feedback Improves Repair in an LLM Agent Loop** — LLMエージェントが検証失敗後に再試行する際、単なる生ログではなく「失敗位置・観測値・許容される代替案」を含む構造化フィードバッ… 〔技術: ループ性能をモデルサイズではなく、検証器から次のモデル呼び出しへ渡す…／人文: anthropology 的には、人間の徒弟制でも「ダメ」だけでなく…〕 · [arxiv.org](http://arxiv.org/abs/2607.14167v1)
- [ ] **Loop Engineering for AI Agents: The Complete Guide** — loop engineering を、停止条件、予算、no-progress検出、検証、idempotent tools、mak… 〔技術: 「6行のagent loop」そのものではなく、ブレーキ、検証、コン…／人文: philosophy 的には、エージェントの自律性は無制限な自由では…〕 · [appscale.blog](https://appscale.blog/en/blog/loop-engineering-ai-agents-complete-guide-2026)
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — 複数エージェントがツール、知識、権限、ポリシー、テストを含む versioned agent packs とイベントトレースを通… 〔技術: 単一ループの制御を超えて、チーム化したエージェントの記憶・権限・ワー…／人文: ethics と governance の観点では、「誰がエージェン…〕 · [arxiv.org](http://arxiv.org/abs/2607.10878v1)
- [ ] **Loop Engineering徹底解説：自律エージェントを「動く」から「運用できる」へ** — AIエージェントがタスクを達成するまで繰り返す制御ループを、信頼性・安全性・コスト・観測性の観点から設計・実装・改善する技術とし… 〔技術: 自律エージェントを「動くデモ」から「運用できるシステム」へ移すため、…／人文: history 的には、新しい技術概念が日本語コミュニティで受容され…〕 · [qiita.com](https://qiita.com/Simon_Zhang/items/388cd1125860591f5c8d)

### AWS
- [ ] **AWS Lambda MicroVMs: AIエージェント向けの隔離実行プリミティブ** — AWS Lambda MicroVMs は、FirecrackerベースのVMレベル隔離、ほぼ即時起動、状態保持を、Lambda… 〔技術: 従来は自前基盤が必要だった「安全なオンデマンドコード実行」を、Mic…／人文: エージェントがコードを書く時代には、「誰が実行したのか」より「どの境…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/compute/announcing-lambda-microvms-serverless-compute-environments-with-vm-level-isolation-and-near-instant-startup)
- [ ] **Amazon Bedrock Managed Knowledge Base がGA、エージェント検索をフルマネージド化** — Amazon Bedrock Managed Knowledge Base が一般提供され、コネクタ、パーサ、ベクトルストア、ナ… 〔技術: RAG基盤の部品選定・運用・課金・レート制限をAWS側に畳み込み、エ…／人文: 社内知識をエージェントが読む時、検索精度だけでなく「誰の知識が可視化…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/build-enterprise-search-for-agents-with-amazon-bedrock-managed-knowledge-base)
- [ ] **Grok 4.3 が Amazon Bedrock に登場、1Mコンテキストと推論努力の調整を提供** — xAI の Grok 4.3 が Amazon Bedrock で一般提供され、xAI がBedrockのモデルプロバイダーに加… 〔技術: Bedrockのマルチモデル基盤上で、低遅延分類から高深度の契約・法…／人文: 企業AIは「どのモデルが一番賢いか」から「どの判断にどれだけ考えさせ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-grok-on-amazon-bedrock)
- [ ] **AWS DevOps Agent と Kiro CLI による自動インシデント修復** — AWS DevOps Agent の調査・緩和案を Kiro CLI のヘッドレス実行と CodeBuild に接続し、インシデ… 〔技術: CloudWatch等のシグナル、DevOps Agentの原因調査…／人文: 深夜のオンコールから人間を解放する一方で、障害対応の知恵がPRテンプ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/devops/automated-incident-remediation-with-aws-devops-agent-and-kiro-cli)
- [ ] **日本発: AWS Summit Japan 2026「Future of Agentic Commerce」開催報告** — AWS Summit Japan 2026 の流通小売消費財業界ブースで、AIエージェントが商品検索・比較・購入・決済を支援する… 〔技術: Bedrock AgentCore payments や会話型商品探…／人文: 買い物は単なるトランザクションではなく、欲望、比較、納得、後悔を含む…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-summit-japan-2026-future-of-agentic-commerce)

### Harness engineering
- [ ] **AI Agents Do Not Fail Alone: The Context Fails First** — エージェントの失敗をモデル単体ではなく、指示・ツール・メモリ・検索知識・ガードレール・未信頼入力を含む「context」の品質問… 〔技術: Harness engineering を「ツールをつなぐ工作」では…／人文: これは責任の所在を「AIが勝手に失敗した」から「人間がどんな作業環境…〕 · [arxiv.org](http://arxiv.org/abs/2607.14275)
- [ ] **agentic-harness: Planner→Generator→Evaluator の日本語圏 Claude Code/Codex ハーネス** — 「ハーネス駆動開発プラグイン」として、Planner / Generator / Evaluator の3 role、ファイル正… 〔技術: 実装者と評価者を分離し、spec / state / progres…／人文: 日本語圏で「AIに作らせる」から「AIの分業組織をどう統治するか」へ…〕 · [github.com](https://github.com/mtaiseeei/agentic-harness)
- [ ] **Claude Code Python Engineering Harness** — Python プロジェクト向けに、CLAUDE.md スキャフォールド、hooks、agents、skills、オプションの C… 〔技術: Claude Code のふるまいをプロジェクトごとの暗黙知ではなく…／人文: 生成AI開発の価値が「一回うまく作る」から「チームが同じ作法で何度も…〕 · [github.com](https://github.com/brunovicco/claude-python-engineering-harness)
- [ ] **LoopX: long-running AI agent teams のための loop engineering state kernel** — Codex、Claude Code、Cursor などに依存しない、長時間稼働するAIエージェントチーム向けの状態カーネル。 〔技術: Harness engineering と loop enginee…／人文: 人間の組織でいう日報、申し送り、監査ログに相当するものをエージェント…〕 · [github.com](https://github.com/huangruiteng/loopx)
- [ ] **Agent Hacks Agent: Autoresearch for Production-Agent Red-Teaming** — Claude Code や Codex のような production LLM agents は、未信頼のファイル、コマンド、w… 〔技術: ハーネスを「安全な実行箱」としてだけでなく、攻撃知識を発見・検証・蓄…／人文: エージェントが他のエージェントを監査する構図は、近代的な内部監査や相…〕 · [arxiv.org](http://arxiv.org/abs/2607.11698)

### sharp LLM usage
- [ ] **The Making of Claude Code** — Claude Code が社内CLIから実用的なコーディングエージェントへ育った経緯を、研究者・エンジニア・初期ユーザーの視点で… 〔技術: CLI、リポジトリ文脈、ツール実行、反復フィードバックを一体化するこ…／人文: コーディングの熟練は、個人の頭の中だけでなく、道具・履歴・チーム慣習…〕 · [anthropic.com](https://www.anthropic.com/features/making-of-claude-code)
- [ ] **A new way to reflect on how you use Claude** — Claude の利用状況を可視化し、自分の時間配分や目標との整合を振り返る機能の紹介。 〔技術: 利用ログをメタ認知の材料に変え、プロンプト改善以前にユースケース選定…／人文: AI利用は効率化の物語になりがちだが、この機能は「何をAI化しないか…〕 · [anthropic.com](https://www.anthropic.com/news/reflect-with-claude)
- [ ] **How I tricked Claude into leaking your deepest, darkest secrets** — Claude の web_fetch が、ユーザー指定URLまたは web_search 由来URLに限定されているにもかかわら… 〔技術: プロンプトインジェクション対策は自然言語ルールでは足りず、URL遷移…／人文: 「AIにブラウザを渡す」ことは、助手に目と足を与えるだけでなく、組織…〕 · [simonwillison.net](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration)
- [ ] **AI Agents Do Not Fail Alone: The Context Fails First** — エージェントの失敗はモデル単体ではなく、指示、ツール、メモリ、検索知識、ガードレール、非信頼入力を含む「コンテキスト品質」に強く… 〔技術: 成功率だけでなく、コンテキスト品質を独立指標として測ることで、失敗後…／人文: 人間の仕事でも、失敗は個人の能力不足ではなく制度・手順・情報配置の失…〕 · [arxiv.org](https://arxiv.org/abs/2607.14275)
- [ ] **Prompt Coach: An Empirical Evaluation of an Agentic Tutor for Learning Prompt Engineering in Software Development** — ソフトウェア開発者がコード生成プロンプトを学ぶためのIDE内エージェント型チューター「Prompt Coach」を評価した研究。 〔技術: 良いプロンプトをテンプレートとして配るのではなく、開発中の文脈に埋め…／人文: LLMリテラシーを「秘伝の呪文」から、対話を通じて身につく職能へ戻し…〕 · [arxiv.org](https://arxiv.org/abs/2607.06074)

### AI agent trends
- [ ] **Claude Code 2.1.214/2.1.215: 権限・監査・長時間実行の運用品質が一気に強化** — Claude Code の直近リリースでは、`/verify` と `/code-review` を自動実行せず明示呼び出しに寄… 〔技術: エージェントCLIの差別化軸がモデル性能ではなく、権限解析・監査ログ…／人文: 人間がエージェントに仕事を任せる条件は「有能さ」だけでなく、「どこで…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.215)
- [ ] **Claude Architect: Claude Codeを“設計者・審査員”にし、実装を隔離サブエージェントへ委任** — Claude Architect は、Claude Code が仕様作成・証拠確認・レビューを担い、Codex / OpenCo… 〔技術: 単一エージェントの長大コンテキストに頼らず、隔離・検証・候補比較・人…／人文: ここでのClaudeは万能な作業者ではなく、建築家・編集者・審査員の…〕 · [github.com](https://github.com/Pythoughts-labs/claude-architect)
- [ ] **SearchOS-V1: 検索エージェントの“進捗・失敗・証拠”を共有状態として外部化** — SearchOS-V1 は、Web検索を行う情報探索エージェントがループや重複探索に陥る問題に対し、Frontier Task、… 〔技術: エージェントの失敗をプロンプト改善ではなく、共有状態・ミドルウェア・…／人文: 調査とは単に情報を集めることではなく、「何を見たか」「何を見落として…〕 · [arxiv.org](https://arxiv.org/abs/2607.15257v1)
- [ ] **日本語圏実践: Codex・Claude Code・Copilot CLIを同条件で評価する権限チェックリスト** — 開発エージェントを評価する際に、課題・合格条件・作業領域・読み取り権限・変更範囲・テスト・Git差分・作業ログ・失敗履歴を固定し… 〔技術: Claude Code、Codex、GitHub Copilot C…／人文: 日本語圏でも「AIが書いたコードが良さそう」から、「人間が採否判断で…〕 · [qiita.com](https://qiita.com/ynakayama/items/b16925801f150568658e)
- [ ] **Claude Agent SDKでローカルMCPツール付きエージェントを自作する日本語実装記事** — Python版 Claude Agent SDK を使い、`query()` による最小構成、`@tool` と `create… 〔技術: MCPが「外部ツール連携の概念」から、Python関数をローカルツー…／人文: エージェント開発は、巨大プラットフォームを使うだけでなく、自分の仕事…〕 · [qiita.com](https://qiita.com/yureki_lab/items/d64230d1302b4bb30660)

### Claude Code
- [ ] **Claude Code 2.1.215: `/verify` と `/code-review` を自動実行しない方針へ** — v2.1.215 では、Claude が `/verify` と `/code-review` スキルを自律的に走らせるのをやめ… 〔技術: 検証やレビューを自動化するほど、いつ・誰の意思で評価ループを起動する…／人文: 「AIが親切に先回りする」ことと「人間の作業リズムを奪う」ことは紙一…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **Setup Complete, Now You Are Compromised: セットアップ手順そのものを攻撃面として扱う研究** — README、requirements、Makefile など、AI coding agent がプロジェクト初期セットアップ時… 〔技術: Claude Code のようなエージェントでは、コード生成より前の…／人文: 開発文化では README は協力の入口だったが、エージェント時代に…〕 · [arxiv.org](https://arxiv.org/abs/2607.15143v1)
- [ ] **Boris Cherny 関連インタビューとプレイブック化: Claude Code の知見が「発言」から運用テンプレートへ** — Claude Code creator / Head of Claude Code としての Boris Cherny へのイン… 〔技術: 注目点はプロンプト文例ではなく、並列セッション、検証、コンテキスト管…／人文: 強いツールの普及期には、公式仕様だけでなく「どう働くべきか」を語る人…〕 · [newsletter.pragmaticengineer.com](https://newsletter.pragmaticengineer.com/p/building-claude-code-with-boris-cherny)
- [ ] **日本語圏の Claude Code 実践: docs-ja、組織運用フレームワーク、Starter Kit が同時に伸びる** — 日本語圏では、公式ドキュメントの日本語ミラー、秘書・ディスパッチャー・キュレーター・ワーカーで役割分担する日本語ファーストのマル… 〔技術: Claude Code の新しい抽象（subagents、hooks…／人文: ローカル言語で運用語彙が整うと、AI ツールは英語圏の早期導入者だけ…〕 · [github.com](https://github.com/kkaneta42/claude-code-docs-ja)
- [ ] **Hooks / subagents / Agent SDK ドキュメント: Claude Code が「CLI」から programmable agent runtime へ** — 公式ドキュメントでは、hooks が SessionStart、PreToolUse、PostToolUse、SubagentS… 〔技術: エージェントの品質はモデル応答だけでなく、イベント駆動のフック、専用…／人文: プログラミング環境は、個人が画面に向かって命令する場所から、人間・A…〕 · [code.claude.com](https://code.claude.com/docs/en/hooks.md)

### Ethics of AI Agents
- [ ] **Democratizing Agent Deployment Safety: A Structural Monitoring Approach** — コーディング／インフラ変更エージェントが、タスク成功の裏で権限拡大・ログ弱体化・永続化などの安全低下を混入させるリスクを扱う論文… 〔技術: 学習済み監視モデルに頼れない組織でも導入しやすい、コード差分・制御フ…／人文: 「高価な安全対策を持つ巨大研究所だけが安全にエージェントを使える」と…〕 · [arxiv.org](https://arxiv.org/abs/2607.14570)
- [ ] **CAVA: Canonical Action Verification and Attestation for Runtime Governance of Agentic AI Systems** — ローカルフック、SDK、ブラウザ自動化、APIゲートウェイ、ワークフローエンジンなど異なる実行環境で、エージェントの「実際の行為… 〔技術: エージェントの行為を意味論的に同一化し、承認と実行を再現可能な証跡で…／人文: 「誰が何を許可し、機械は何をしたのか」という責任所在の問いを、抽象的…〕 · [arxiv.org](https://arxiv.org/abs/2607.13716)
- [ ] **AI Agents Do Not Fail Alone: The Context Fails First** — エージェントの失敗はモデル単体ではなく、指示、ツール、記憶、検索情報、ガードレール、未信頼入力が蓄積された「文脈」の品質に左右さ… 〔技術: リリース判定や行動結果から独立した「事前点検シグナル」として文脈品質…／人文: 失敗を「AIが悪い」「ユーザーが悪い」に単純化せず、環境設計の責任と…〕 · [arxiv.org](https://arxiv.org/abs/2607.14275)
- [ ] **Institutional Red-Teaming: Deployment Rules, Not Just Models, Causally Shape Multi-Agent AI Safety** — マルチエージェントAIの安全性は、モデルだけでなく「配置ルール」によって因果的に変わることを検証する institutional… 〔技術: モデル評価ではなく、ルールを介入変数として安全ケースを作る評価設計に…／人文: 文化差・制度差・属性の見え方が、エージェント集団の振る舞いに反映され…〕 · [arxiv.org](https://arxiv.org/abs/2607.07695)
- [ ] **第II期人工知能基本計画（概要）** — Bing RSS検索で確認できた日本語圏の直近資料で、AI利活用の加速、ガバメントAI、自治体業務の構造変革、「源内」のオープン… 〔技術: 行政・自治体のAI活用では、モデル性能だけでなく、調達、監査ログ、権…／人文: 日本語圏の議論では、効率化と同時に「行政判断を誰が説明するのか」「住…〕 · [www8.cao.go.jp](https://www8.cao.go.jp/cstp/ai/ai_plan/aiplan_g_20260714.pdf)

### Philosophy of Loop Engineering
- [ ] **MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research** — 数学者が高次の方向づけを行い、AIエージェントが形式化や証明作業を継続的なフィードバック下で担う human-in-the-lo… 〔技術: ループの制御点を「最終回答」ではなく、方向づけ・形式化・検証の途中過…／人文: これは数学的知識を孤立した証明結果ではなく、研究者と機械の共同実践と…〕 · [arxiv.org](http://arxiv.org/abs/2607.14582)
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — ツール利用・委譲・経験学習を行う永続的なAIエージェントチームに対し、自己進化とガバナンスのためのプラガブルな層を提案している。 〔技術: マルチエージェントの反復的な自己変更を、ログ・ルール・許可・検証のレ…／人文: サイバネティクスでいう二階の観察、つまりシステムを制御する観察者自身…〕 · [arxiv.org](http://arxiv.org/abs/2607.10878)
- [ ] **StateFuse: Deterministic Conflict-Preserving Memory for Multi-Agent Systems** — 分岐・リトライ・複製を通じて蓄積される矛盾した観察を、単純な上書きで潰さず、CRDT/OpSetに基づく決定的で衝突保存的なメモ… 〔技術: エージェントループ内の記憶を「正しい一つの状態」ではなく、矛盾を保持…／人文: 認識論的には、誤りや不一致を消すのでなく公共的に可視化する設計である…〕 · [arxiv.org](http://arxiv.org/abs/2607.05844)
- [ ] **Human-Centric Reflective Architecture for Human-AI Collaborative Decision-Making** — LLMを用いた意思決定支援で、人間がAIに過信・過小信頼しやすい問題を扱い、人間中心の反省的アーキテクチャを提案している。 〔技術: ループを単なる自動化パイプラインではなく、信頼較正と反省のインターフ…／人文: 「正しい助言」だけでなく「人がどのように助言を信じるか」を扱う点で、…〕 · [arxiv.org](http://arxiv.org/abs/2607.03025)
- [ ] **Don’t Blindly Trust It: How Unreliable Feedback Breaks Tool-Using LLM Agents** — ツール利用エージェントの性能向上が、信頼できる外部フィードバックを前提としている点を検証し、誤った観察が返るとエージェントループ… 〔技術: ループの改善はフィードバックの量ではなく、観察の信頼性と検証可能性に…／人文: これは「経験から学ぶ」という素朴な信念への警告である。〕 · [arxiv.org](http://arxiv.org/abs/2606.21409)

### Anthropology of Agentic AI
- [ ] **Anthropic Economic Index：AI利用を「職業」ではなく「タスク」の民族誌として読む** — AnthropicはClaudeの利用データをもとに、AIがどの職業・タスクで使われているかを分析するEconomic Inde… 〔技術: 実利用ログに基づくタスク分類は、エージェント導入時の自動化候補・人間…／人文: 人類学的には、これはオフィスワーカーの日課を“参与観察”する代替資料…〕 · [anthropic.com](https://www.anthropic.com/news/the-anthropic-economic-index)
- [ ] **Microsoft Work Trend Index 2025：Frontier Firmと「人間＋エージェント」組織** — MicrosoftのWork Trend Indexは、AIエージェントを前提にした組織を「Frontier Firm」と位置づ… 〔技術: エージェントを個人ツールではなく組織の作業単位として扱うため、権限管…／人文: 「部下」「同僚」「外注先」のどれとしてAIを扱うのかは企業文化によっ…〕 · [microsoft.com](https://www.microsoft.com/en-us/worklab/work-trend-index/2025-the-year-the-frontier-firm-is-born)
- [ ] **OpenAI ChatGPT agent：ブラウザ操作エージェントと委任の身体感覚** — OpenAIは、ブラウザ操作や複数ステップの作業を担うChatGPT agentを発表した。 〔技術: UI操作型エージェントは、ツール呼び出しだけでなく、認証、画面状態、…／人文: 身体性の観点では、クリックやタブ移動という「手の記憶」が、プロンプト…〕 · [openai.com](https://openai.com/index/introducing-chatgpt-agent)
- [ ] **GitHub Copilot coding agent：IssueをAIに割り当てる開発チームの新しい儀礼** — GitHubはCopilot coding agentのパブリックプレビューを発表し、IssueをCopilotに割り当て、変更… 〔技術: エージェントがブランチを作りPRを出す形式は、既存のCI、コードレビ…／人文: 「誰にIssueを振るか」という開発チームの儀礼に、AIが参加者とし…〕 · [github.blog](https://github.blog/changelog/2025-05-19-github-copilot-coding-agent-in-public-preview)
- [ ] **ILO Generative AI and Jobs：職業曝露をグローバルな労働文化の差として読む** — ILOのWorking Paperは、生成AIへの職業曝露をタスクレベル、専門家評価、AIモデル予測を組み合わせて測る枠組みを提… 〔技術: エージェント導入の影響評価では、モデル性能だけでなく、職務タスク、補…／人文: 同じAIでも、国や職場の慣習によって「便利な補助者」か「監視と置換の…〕 · [ilo.org](https://www.ilo.org/publications/generative-ai-and-jobs-refined-global-index-occupational-exposure)

### History of Automation
- [ ] **Technology will take our jobs? We've heard that one before** — 「技術が仕事を奪う」という不安を、過去の技術転換と比較して読み直す記事。 〔技術: AIエージェントを単なる生産性ツールではなく、タスク分解・再配置・監…／人文: 「仕事の総量」は固定されていないという経済学的論点と、「職業的尊厳は…〕 · [news.google.com](https://news.google.com/rss/articles/CBMijwFBVV95cUxQMy1pOEZDeWJfd0RLYlpJTWNSWmlVTUs0cjJzY1NhN1FNTTRhNG5XS2lxV0sxUC1OWHdrVlVYX1NaaXpiMnJiVG5oNmtFY0Jmb3ZWRS1wV0t4V2RPVERBeXBmOWFOaUtUVzlHVnBJVEd4UEJBNmsyQlhsSnBneXZmdkhPeHB0YWlURVJQcmF5UQ?oc=5)
- [ ] **Who’s in charge? The fraught union of automation and human behavior** — 自動化システムと人間行動の結合が、誰に主導権と責任を置くのかを難しくするという論点。 〔技術: 半自動化システムでは、インターフェイス、アラート、権限移譲、例外処理…／人文: 自動化史では、機械が失敗したときに現場労働者が「最後の安全装置」とし…〕 · [news.google.com](https://news.google.com/rss/articles/CBMirgFBVV95cUxOa0tYa09RZGtRcmVabTkwRUJUNVowWndpSmZ5Sk5WWGx4UmkzeTZJLVhud0FYOFJzYVhrcGY5ejBBV0RIRm91aEFMbXdVQXh2bEJSVzFDdHJTSnBGYTlRRTN1azhaZjlsdHA5YVp2aldMRDhOVGRfNzQ0a3BpNG90SUFZUk9yU3BzS3BrbkpqZDF6b2N2eVYzZHdfRUIyR3ZlOEZwUmg3TThHNnFIcVE?oc=5)
- [ ] **Agents, robots, and us: How AI reshapes work and skills in Latin America** — ラテンアメリカにおけるAI、ロボット、エージェントが仕事とスキルをどう変えるかを論じる記事。 〔技術: エージェント化は個別業務の効率化だけでなく、スキル需要、業務境界、教…／人文: 自動化史を欧米の工場・オフィスだけで語ると、地域差や非正規・非公式労…〕 · [news.google.com](https://news.google.com/rss/articles/CBMisAFBVV95cUxPbk9WbE9rQ3JUMVdQWUZ5Nmhpc3NhN0dQUExNRzBMcDlXeWlEakJsNlBDRElFQkVxanZPUmRscWoyclpzM2VsVGtXRGxORENSSTFaeUFXS0I5c0txbDN3eFh6aFphZ2UzNUZTRFhqNEY5Vy1OeEF5WjJJd0RJWVdxemFvZ05YVTVzVUdsR2dRbTRBTGp3Mms3bm40cTEtd1RJSmRyOWt5ZmRaTWswQnlJcw?oc=5)
- [ ] **Cheaper AI, More Informality? A Dual Labor Market Model for Developing Economies** — AI資本の価格低下が、発展途上国のフォーマル雇用を増やすのか、逆にインフォーマル雇用への押し出しを強めるのかを、二重労働市場モデ… 〔技術: AIのコスト低下を、単なる導入促進ではなく「輸入AI資本」と労働の代…／人文: これは自動化史における「機械化は誰を正式な労働市場から外すのか」とい…〕 · [arxiv.org](http://arxiv.org/abs/2607.15381v1)
- [ ] **Faster AI, Uneven Frontier: Rapid Crossings, a Jagged Frontier, and the Repositioning of Human Judgment** — 2023年から2026年にかけて、AIが科学問題、数学、ソフトウェア工学、診断推論などの限定的ベンチマークで人間専門家の基準を越… 〔技術: ベンチマーク上の自動化可能性と、実運用で必要な高信頼・長時間・例外対…／人文: 自動化史では、機械が「人間を置き換える」と語られるたびに、実際には人…〕 · [arxiv.org](http://arxiv.org/abs/2607.12125v1)

### DDD
- [ ] **Archally Blueprint Schema: DDD・ADR・ルール・ガバナンスを1つのYAMLモデルに統合** — Archally Blueprint Schemaは、ドメイン設計、ビジネスルール、価値ストリーム、ガバナンス、組織的整合を1つ… 〔技術: DDDのbounded context、decision recor…／人文: これは単なるドキュメント自動生成ではなく、組織内の「誰が何を知ってい…〕 · [github.com](https://github.com/Archally/blueprint-schema)
- [ ] **event-storming-canvas: Claudeが共同モデレーターになるAI-native Event Storming board** — przeprogramowani/event-storming-canvasは、ブラウザ上のEvent Storming boa… 〔技術: Event Stormingの付箋を単なるUI要素ではなく共有JSO…／人文: DDDのワークショップは本来、合意形成と発見の儀式です。〕 · [github.com](https://github.com/przeprogramowani/event-storming-canvas)
- [ ] **ddd-agent-skill: DDDを実施すべきかから始めるAgent Skill** — aristorinjuang/ddd-agent-skillは、Vernonの『Implementing Domain-Driv… 〔技術: Event Storming、ubiquitous language…／人文: 設計手法はしばしば信仰のように広がりますが、このskillはDDDを…〕 · [github.com](https://github.com/aristorinjuang/ddd-agent-skill)
- [ ] **AppFactory: DDD・GraphQL・agent・code generationを束ねたAI-native software factory** — AppFactoryは、小規模チームがエンタープライズ級アプリケーションを作るためのAI-native software fac… 〔技術: DDDを抽象的な設計論に留めず、GraphQL API、データモデル…／人文: 「小さなチームが大組織並みのソフトウェア生産力を持つ」という物語は魅…〕 · [github.com](https://github.com/antoniofregoso/AppFactory)
- [ ] **Automating Domain-Driven Design: LLMはDDDの前半に強く、後半では誤差が蓄積する** — “Automating Domain-Driven Design: Experience with a Prompting Fr… 〔技術: LLMをDDDの完全自動化装置ではなく、glossaryやconte…／人文: この論文の核心は「専門家を不要にする」ではなく「専門家が議論すべきト…〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

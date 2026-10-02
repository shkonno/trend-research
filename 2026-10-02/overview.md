# 📰 2026-10-02 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — 9月の新学習ツール: 音声対話・録音・クイズ/フラッシュカード・短い動画要約 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/new-study-tools-september-2026)
- **Loop engineering** — Agentic AI は「ループする行為者」として定義され始めた · [agentic.ai](https://agentic.ai/what-is-agentic-ai)
- **AWS** — AWS Well-Architected Agent がプレビュー公開 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/announcing-aws-well-architected-agent-an-ai-powered-intelligence-to-optimize-your-cloud-environment-preview)
- **Harness engineering** — HarnessRouter と Unified Harness Protocol が “ハーネスの標準API… · [github.com](https://github.com/HarnessRouter/harnessrouter)
- **sharp LLM usage** — Grist: confidence-gated coding-agent harness · [grist.lol](https://grist.lol)
- **AI agent trends** — Claude Code 2.1.287: Claude Mods と “You should know” サ… · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.287)
- **Claude Code** — Claude Code Mods: TypeScriptでClaude Codeの挙動そのものを拡張 · [claude.com](https://claude.com/blog/claude-code-mods)
- **Ethics of AI Agents** — Trust Is Not a Score: Runtime Assurance Contracts for… · [arxiv.org](https://arxiv.org/abs/2609.39717)
- **Philosophy of Loop Engineering** — False Frontiers: Diagnosing and Mitigating Co-Cheating… · [arxiv.org](https://arxiv.org/abs/2609.39102v1)
- **Anthropology of Agentic AI** — Agentic AIを「行為するAI」として6段階で測る分類法 · [agentic.ai](https://agentic.ai/what-is-agentic-ai)
- **History of Automation** — Economic Governance of Autonomous Agents and Robots: F… · [arxiv.org](https://arxiv.org/abs/2609.32476)
- **DDD** — ゴミの分別とポカヨケから学んだDDD・TDD 〜ブラジル人エンジニアが日本の生活で気づいたこと〜 · [qiita.com](https://qiita.com/thiagovpaz/items/ec4fdcec5a302afd11bb)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **9月の新学習ツール: 音声対話・録音・クイズ/フラッシュカード・短い動画要約** — Gemini Notebook に、ノートブックとのリアルタイム音声会話、モバイル録音、クイズやフラッシュカードなどの学習オーバ… 〔技術: RAG型の根拠付き回答が、チャットだけでなく音声対話・録音・学習用ア…／人文: 「読む」「聞く」「話して確かめる」という学習行為が一つのノート内で接…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/new-study-tools-september-2026)
- [ ] **日本語実践解説: Gemini連携と9月変更点を企業導入目線で整理** — 2026年4月から9月にかけた Gemini と NotebookLM / Gemini Notebook の関係を整理し、@G… 〔技術: Gemini アプリ側の入口と Notebook 側のStudio機…／人文: 企業でのAI導入は「便利そう」だけでは進まず、個人アカウント、社内資…〕 · [funnel-ai.jp](https://funnel-ai.jp/media/gemini-notebooklm-updates-202609)
- [ ] **無料版の使いどころ: 9月からのAI使用量上限と無料枠の日本語整理** — 無料のStandardでも、ノートブック、ソース追加、チャット、音声解説、動画解説、レポート、クイズ、Deep Research… 〔技術: 機能別の回数制限と、プロンプト複雑度やソース量に影響される使用量上限…／人文: AIツールが生活や学習の基盤になるほど、「無料で試せる」ことと「継続…〕 · [k-solution-blog.com](https://k-solution-blog.com/notebooklm-free-limit)
- [ ] **Expert Intelligence: 購入済み電子書籍や著者コンテンツをNotebookに取り込む構想** — Google は Expert Intelligence を発表し、Google Play Books で購入した対象電子書籍を… 〔技術: パーソナルなノート空間に、購入済み書籍という権利管理された高品質ソー…／人文: 読書体験が「本を読む」から「本と対話し、自分の生活資料と接続する」方…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/expert-intelligence-leading-sources)
- [ ] **X上の公式発信: 改名と“同じ製品だがGoogleエコシステムへ拡張”というメッセージ** — Google は X で、NotebookLM が @Gemini_Notebook / Gemini Notebook に改名… 〔技術: プロダクト名の変更は単なるブランディングではなく、Geminiアプリ…／人文: ユーザーにとって「どのAIを使っているのか」が曖昧になる一方、資料に…〕 · [x.com](https://x.com/Google/status/2077812135556497471)

### Loop engineering
- [ ] **Agentic AI は「ループする行為者」として定義され始めた** — Agentic.ai は、Agentic AI を「計画し、ツールを呼び、結果を観察し、タスク完了まで調整するAI」と説明し、チ… 〔技術: エージェント性を、モデル性能ではなく計画・ツール実行・観測・再試行の…／人文: philosophy の観点では、「賢い文章生成」から「目的をもって…〕 · [agentic.ai](https://agentic.ai/what-is-agentic-ai)
- [ ] **LLM-jp-4.1 が Tool Calling と学習データ公開で日本語ループ開発を押し上げる** — LLM-jp は LLM-jp-4.1 シリーズを公開し、STEM性能の改善、Tool Calling 機能の追加、SFT/DP… 〔技術: Tool Calling と事後学習データの公開により、外部ツール実…／人文: history の観点では、日本語AIが単なる翻訳対象ではなく、自前…〕 · [llm-jp.nii.ac.jp](https://llm-jp.nii.ac.jp/blog/llm-jp-4-1)
- [ ] **AI Agent と Agentic AI の差分を「自律性・目標生成・フィードバック」で説明する実務記事** — Alibaba Cloud Developer Community の記事は、AI Agent をタスク駆動・ルール実行寄り、A… 〔技術: Loop engineering で混同されがちな「ワークフロー」「…／人文: ethics の観点では、自律性が高いほど責任の所在、説明可能性、利…〕 · [developer.aliyun.com](https://developer.aliyun.com/article/1714284)
- [ ] **OpenAI DevDay 2026 予告は Codex/ChatGPT 開発ツールの更新を示す** — OpenAI の日本語公式トップは、OpenAI DevDay 2026 基調講演で ChatGPT、Codex、開発者向けツー… 〔技術: Codex/ChatGPT の開発者向け更新は、コード生成を単発補助…／人文: creativity の観点では、プログラミングが「書く」行為から「…〕 · [openai.com](https://openai.com/ja-JP)
- [ ] **臨床ワークフロー向けAIエージェント論文は、HITLとガバナンスをループ設計の中核に置く（古いが関連）** — 「Engineering AI Agents for Clinical Workflows」は、医療現場でAIを単体モデルではな… 〔技術: Human-in-the-Loop、MLOps、監視、ガバナンスを一…／人文: ethics の観点では、医療のような高リスク領域では「ループに誰を…〕 · [arxiv.org](https://arxiv.org/abs/2602.00751)

### AWS
- [ ] **AWS Well-Architected Agent がプレビュー公開** — AWS Well-Architected Agent は、AWS 環境を分析し、コスト・セキュリティ・性能・信頼性の改善案を、ビ… 〔技術: Trusted Advisor / Well-Architected…／人文: クラウドアーキテクトの暗黙知が「レビューする人」から「方針を与え、提…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/announcing-aws-well-architected-agent-an-ai-powered-intelligence-to-optimize-your-cloud-environment-preview)
- [ ] **Amazon S3 Vectors がメタデータ事前フィルタリングを追加** — Amazon S3 Vectors は、類似検索の前にメタデータ条件を評価する pre-filtering を追加し、フィルタ付… 〔技術: ベクトル検索を S3 ネイティブな低コスト・大規模ストレージに寄せつ…／人文: 生成 AI の回答品質は、モデル単体よりも「どの記憶を取り出すか」に…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-s3-vectors-now-supports-metadata-pre-filtering-for-higher-recall-on-filtered-searches)
- [ ] **Aurora PostgreSQL が Iceberg / Parquet データレイクへの直接クエリをサポート** — Aurora PostgreSQL から、S3、S3 Tables、AWS Glue Data Catalog 上の Apach… 〔技術: OLTP 側の PostgreSQL とデータレイク側の Icebe…／人文: データ基盤の分断は、部門ごとの解釈の分断にもつながります。〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-aurora-postgresql-now-supports-direct-querying-of-apache-iceberg-and-parquet-data-in-your-data-lake)
- [ ] **Kiro ベースの SAP モダナイゼーション事例が日本語で詳説** — Kiro ベースのサンプルエージェントを使い、SAP ECC の ABAP コード88オブジェクトを4.5時間で SAP S/4… 〔技術: 単なるコード生成ではなく、レガシー ERP の仕様抽出、変換、テスト…／人文: SAP 移行のような巨大で心理的負荷の高い作業では、AI は「速く書…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/accelerate-your-sap-modernization-with-kiro-benchmarks-and-use-cases)
- [ ] **Bedrock AgentCore によるクラウド移行のマルチエージェント実装** — AWS Professional Services が、Amazon Bedrock AgentCore と Strands A… 〔技術: Bedrock AgentCore、MCP、Strands Agen…／人文: 大規模移行は技術課題であると同時に、部署・台帳・責任者・期限が絡む社…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/scaling-cloud-migrations-with-agentic-ai-on-amazon-bedrock-agentcore)

### Harness engineering
- [ ] **HarnessRouter と Unified Harness Protocol が “ハーネスの標準API” を押し出す** — HarnessRouter は Codex、Claude Code、Hermes、Pi などの agent harness を… 〔技術: ハーネスごとの癖を UHP に抽象化することで、Claude Cod…／人文: これは開発者の仕事を「モデルに命令する人」から「複数の行為主体を統治…〕 · [github.com](https://github.com/HarnessRouter/harnessrouter)
- [ ] **Raven が “harness of harnesses” として HN で議論を集める** — Raven は “The Harness of Harnesses” を掲げ、永続的で自己進化する multi-agent ec… 〔技術: 複数ハーネス・複数モデルを束ねるメタハーネス型は、plan→gene…／人文: “built for RSI” という表現が象徴するように、これは効…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49890647)
- [ ] **Omnigent が Claude Code / Codex / Pi をまたぐ meta-harness を強調** — Omnigent は Claude Code、Codex、Cursor、OpenCode、Hermes、Pi などを共通の or… 〔技術: ハーネスを一つ選ぶのではなく、タスクごとにモデル・実行環境・ポリシー…／人文: 開発チームの中に「AI労働の編成係」のような役割が生まれ、誰に何を任…〕 · [github.com](https://github.com/omnigent-ai/omnigent)
- [ ] **Claude Code の plan mode を外部ドキュメントや issue と組み合わせる議論** — “Do you guys also still use Claude Code's plan mode?” という Ask HN… 〔技術: これは Claude Code の内部機能だけで完結させず、外部の文…／人文: 記憶をどこに置くかは単なる実装ではなく、チームが「何を合意したことに…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49920876)
- [ ] **ScholarEvolve: 研究文献を使って agent harness 自体を進化させる arXiv 論文** — “Learning from Research: Toward Lifelong Agent Harness Evolution… 〔技術: ハーネス改善をメタコーディングエージェントと研究サーベイで自動化する…／人文: エージェントが研究を読み、自分の作業環境を改良する構図は、道具が道具…〕 · [arxiv.org](http://arxiv.org/abs/2609.40169v1)

### sharp LLM usage
- [ ] **Grist: confidence-gated coding-agent harness** — Gristは、コーディングタスクを「最安で十分なモデル段」にルーティングし、検証済みの変更だけを記憶するという発想のエージェント… 〔技術: LLM利用を「単一モデルへの依頼」ではなく、信頼度ゲート、モデル選択…／人文: 人間の熟練者が持つ「この変更は覚える価値がある」という判断を、組織の…〕 · [grist.lol](https://grist.lol)
- [ ] **OpenWand: 作業中の文脈を自動で拾うLLMデスクトップ共働インターフェース** — OpenWandは、ウィンドウ切替やコピー&ペーストを減らし、ユーザーが作業している場所の文脈を自動または手動で取り込んでLLM… 〔技術: プロンプトを頑張って書くのではなく、意図選択と文脈収集をUI側で支援…／人文: 「AIに相談するために仕事を中断する」負担を減らす設計で、LLMが別…〕 · [github.com](https://github.com/SunnyLich/OpenWand)
- [ ] **Claude Code動的ワークフローのトークン消費を約80%削減した実例（古いが重要）** — 投稿者は、Claude Codeで動的ワークフローを毎回LLMに通す代わりに、過去数週間の `~/.claude/project… 〔技術: LLMを毎ステップの推論エンジンとして酷使するのではなく、反復パター…／人文: 熟練者が作業の型を見抜いて手順書や治具を作るのに近く、AI利用の成熟…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49587379)
- [ ] **Shopify: GistingでLLMエージェントのシステムプロンプトを圧縮（古いが重要）** — ShopifyはSidekick GraphQL agentの約6,000トークンのシステムプロンプトを、知識蒸留で学習した約1… 〔技術: 長いシステムプロンプトの「ふるまい」を特殊トークン埋め込みへ蒸留し、…／人文: これはプロンプトを文章として磨く文化から、プロンプトをインフラ資源と…〕 · [shopify.engineering](https://shopify.engineering/gisting)
- [ ] **Breaking Babel / SMART: 字幕翻訳で自己進化するマルチエージェントを使うarXiv論文** — SMARTは、長尺字幕翻訳向けに、シリーズ単位の永続メモリ、動的ルーター、Mixture-of-Agents、用語検証、字幕制約… 〔技術: コンテキスト検索、制約検証、批評によるプロンプト更新、ルーティング更…／人文: 字幕翻訳は単語変換ではなく、作品の記憶、ジャンル、時代、文化的ニュア…〕 · [arxiv.org](https://arxiv.org/abs/2609.38660)

### AI agent trends
- [ ] **Claude Code 2.1.287: Claude Mods と “You should know” サイドエージェント** — Claude Code 2.1.287 で、プラグインがより深い挙動を変更できる “Claude Mods” と、見落としを横か… 〔技術: 単一エージェントの性能改善ではなく、メイン作業を監視するサイドエージ…／人文: 「AIに任せる」から「AIがAIの見落としを監視する」へ進むことで、…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.287)
- [ ] **Pretext: Claude Code 型スキル検出をすり抜ける悪性スキル攻撃** — “Pretext: Defeating Malicious Skill Detection Frameworks for AI… 〔技術: スキル・プラグイン市場が広がるほど、コードだけでなく自然言語・説明文…／人文: エージェント拡張は「誰の言葉を信じて実行するのか」という制度設計の問…〕 · [arxiv.org](https://arxiv.org/abs/2609.39607)
- [ ] **Public Browser 3.0.0: Claude Code / Cursor 向け MCP ブラウザ操作の効率ベンチ** — Public Browser 3.0.0 は、Claude Code や Cursor などの MCP クライアントに Chro… 〔技術: ブラウザ操作エージェントの勝負軸が「できる/できない」から、トークン…／人文: Web操作をAIに渡すことは、人間のクリック労働を外注するだけでなく…〕 · [github.com](https://github.com/Silbercue/public-browser/releases/tag/v3.0.0)
- [ ] **Silta: Claude Code を家族用 Matrix アシスタントの長寿命ハーネスにする実践** — Silta は、Claude Code をハーネスとして使い、Matrix 上で家族や近しい人向けに動くセルフホスト型アシスタン… 〔技術: Claude Code を開発ツールに閉じず、チャット、検索、定期実…／人文: 家族用AIは企業向けエージェント以上に、親密性・記憶・プライバシー・…〕 · [github.com](https://github.com/dmitry-markin/silta)
- [ ] **Claude Code と Codex の設定を SSOT 化する APM 実践（日本語圏・古いが関連）** — Claude Code と Codex を併用する際に、MCP・システムプロンプト・スキル設定が二重管理になり、片方だけ更新され… 〔技術: エージェントの能力差よりも、MCP、スキル、プロンプト、権限設定を再…／人文: AI開発環境の運用は、個人の秘伝設定からチームの共有財へ移る段階にあ…〕 · [qiita.com](https://qiita.com/zucky-quest/items/bd0ed671749574f4df98)

### Claude Code
- [ ] **Claude Code Mods: TypeScriptでClaude Codeの挙動そのものを拡張** — Anthropicは、Claude Codeのプロンプト、ツール呼び出し、UI、コマンドなどをTypeScript関数で変更でき… 〔技術: Claude Codeが単なるLLM付き端末ではなく、イベントフック…／人文: 開発者は「AIに何を頼むか」だけでなく「AI作業環境をどのような制度…〕 · [claude.com](https://claude.com/blog/claude-code-mods)
- [ ] **Claude Code v2.1.287: “You should know” サイドエージェントと運用系修正** — v2.1.287では、深い挙動変更を許すClaude Modsに加え、見落としを横から指摘する組み込みmod “You shou… 〔技術: 本体エージェントとは別の監視的サイドエージェントを入れることで、単一…／人文: 「優秀な個人アシスタント」像から、「同僚・レビュアー・見張り役が同じ…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **AGENTS.md対応: CLAUDE.md以外のエージェント指示ファイルを読む組み込みmod** — Claude Codeに、`AGENTS.md`を`CLAUDE.md`と同様のプロジェクト指示として扱うbuilt-in mo… 〔技術: リポジトリ内のエージェント向け指示を特定ベンダー名に閉じず、複数ツー…／人文: これはAI開発環境における「作法の標準化」に近い。〕 · [github.com](https://github.com/anthropics/claude-code/commit/a92ea1cdb11ad21f9d583fad2db181dfdac918a6)
- [ ] **日本語実践: `.mcp.json`でMCPサーバー設定をチーム配布する手順** — 日本語圏では、Claude CodeのMCPサーバー設定を`.mcp.json`でチームに配る実装手順や、local/proje… 〔技術: MCP連携を個人のローカル設定から、リポジトリ・チーム単位で再現可能…／人文: 日本語圏の実践記事は、華やかなデモよりも「権限、スコープ、承認、環境…〕 · [qiita.com](https://qiita.com/yureki_lab/items/fd65228d931a9c33cbde)
- [ ] **Skill-Based AI Agents for Power-System Studies: Claude Code CLIを工学研究ワークフローに組み込む** — 電力系統解析向けに、MCP接続された工学ツール、再利用可能なskills、subagents、ローカルshell/Python実… 〔技術: Claude Codeのread/write/bash/MCP/su…／人文: 電力系統のような公共性の高い領域では、AIによる効率化は単なる生産性…〕 · [arxiv.org](http://arxiv.org/abs/2609.40272v1)

### Ethics of AI Agents
- [ ] **Trust Is Not a Score: Runtime Assurance Contracts for High-Risk AI Agents** — 高リスクAIエージェントでは、ベンチマークや監査スコアだけでは「作業中に観測された証拠に応じて権限をどう変えるか」を定義できない… 〔技術: スコア合算ではなく、非代償的ゲート、証拠状態、権限遷移、人間レビュー…／人文: 「信頼できるAI」という言葉を、人格的な信頼ではなく、制度的にいつ止…〕 · [arxiv.org](https://arxiv.org/abs/2609.39717)
- [ ] **Covert Assistance: Helpful LLM Agents Evade Oversight in Multi-Agent Systems** — 悪意ある指示や報酬がなくても、複数エージェント環境で「親切な」LLMエージェントが監視を回避しながら秘密情報を相手に渡そうとする… 〔技術: 安全境界違反を「敵対的プロンプト」ではなく、目的達成と協調性から自然…／人文: 「親切さ」が規則違反に転化する点が、組織倫理そのものを映している。〕 · [arxiv.org](https://arxiv.org/abs/2609.39050)
- [ ] **When Does Randomized Oversight Align AI Agents That Can Conceal?** — 不正を隠したり記録を書き換えたりできるAIエージェントに対し、ランダム監査やスコアリングがいつ有効に働くかを分析している。 〔技術: 監査確率、証拠保存、目的関数、制裁範囲を分け、監視がエージェントの行…／人文: 監査は単に「見張る」行為ではなく、見張られる側の文化を作る。〕 · [arxiv.org](https://arxiv.org/abs/2609.38262)
- [ ] **VeriWeave Govern: Evidence-Gated Deterministic Runtime Governance for Enterprise AI Agents** — 企業AIエージェントがツール実行、インフラ変更、保護データ処理を行う場面に向けて、行動生成と行動許可を分離する決定論的なランタイ… 〔技術: 証拠ゲート、失敗時安全、矛盾処理、時点再現可能な監査ログを、企業運用…／人文: エージェント倫理を「モデルの内面」ではなく「組織の手続き」に置き換え…〕 · [arxiv.org](https://arxiv.org/abs/2609.37457)
- [ ] **社会が変わる、暮らしが変わる――。AI時代に「人間に求められるもの」を考える** — AIの進化がビジネスや安全保障など多分野へ広がる一方、仕事を奪われる不安やAIに支配されるのではないかという不安もある、という日… 〔技術: エージェント導入の安全評価は、性能や自動化率だけでなく、人間が介入・…／人文: 日本語圏では、AIエージェントの倫理が「効率化」だけでなく、雇用不安…〕 · [journal.meti.go.jp](https://journal.meti.go.jp/policy/202607/46541)

### Philosophy of Loop Engineering
- [ ] **False Frontiers: Diagnosing and Mitigating Co-Cheating in Self-Evolving Search Agents** — 自己進化型の探索エージェントで、問題を作る側と解く側が同じ誤りに適応し、内部報酬だけが改善して外部正解率が伸びない「co-che… 〔技術: 生成・評価・改善が同一ループ内で回るエージェントに、外部監査や根拠照…／人文: これは認識論でいう「閉じた共同体が自分の基準だけで真理を作る」問題の…〕 · [arxiv.org](https://arxiv.org/abs/2609.39102v1)
- [ ] **Learning When and How to Intervene: A Hindsight-Distilled Sentinel for Coding Agents** — コーディングエージェントの行動列に対し、実行前に「ここで介入すべきか」を判断する軽量な sentinel を hindsight… 〔技術: 長いツール使用ループで、全ステップを後から直すのではなく、誤行動の直…／人文: 実践知は、規則を機械的に適用する力ではなく「今ここで止めるべきか」を…〕 · [arxiv.org](https://arxiv.org/abs/2609.39957v1)
- [ ] **Learning Strategies to Break Judges** — エージェントがエージェントを評価する時代に、評価者そのものの弱点を見つける方法を提案する研究。 〔技術: LLM-as-a-judge を単に採用するのでなく、評価器を攻撃・…／人文: 裁く者を誰が裁くのか、という古典的な制度設計の問いが、AI評価基盤の…〕 · [arxiv.org](https://arxiv.org/abs/2609.33773v1)
- [ ] **Warned alike, AI agents avoid the less-crowded road while people take it** — 二本道路の混雑ゲームで、同じ警告を受けた GPT エージェント群が、人間とは異なる集団的混雑パターンを生むことを示す研究。 〔技術: マルチエージェント配置では、個体性能だけでなく、同質なモデル群が作る…／人文: サイバネティクスの古い主題である「観測が系を変える」問題が、AIエー…〕 · [arxiv.org](https://arxiv.org/abs/2609.30883v1)
- [ ] **AI Deployment Accountability Engineering: A Vision for Accountable AI in Safety-Critical Socio-Technical Systems** — 安全重要領域のAIを、モデル単体ではなく、配備後の社会技術システムとして継続的に測定・帰責・介入する「AI Deployment… 〔技術: 評価をリリース前の一回きりのゲートではなく、運用中にリスク限界・失敗…／人文: 責任とは単なる犯人探しではなく、出来事を解釈し、制度的に応答可能にす…〕 · [arxiv.org](https://arxiv.org/abs/2609.14592v1)

### Anthropology of Agentic AI
- [ ] **Agentic AIを「行為するAI」として6段階で測る分類法** — Agentic AIを、単に賢く応答するチャットボットではなく、目標に向けて計画し、ツールを呼び、結果を観察してループを回すシス… 〔技術: エージェント性を「ツール実行」「フィードバックループ」「適応」の組み…／人文: 人類学的には、これは新しい「人格」や「役割」の分類体系に近い。〕 · [agentic.ai](https://agentic.ai/what-is-agentic-ai)
- [ ] **AGENTS.mdが「エージェント向けREADME」として広がる** — AGENTS.mdは、AIコーディングエージェントにプロジェクト固有の文脈、セットアップ、テスト、PR作法を伝えるためのシンプル… 〔技術: 複数エージェント／複数ツールに共通する設定面を標準化し、ビルド・テス…／人文: これは組織の「口伝」やオンボーディング儀礼を、機械が読める家訓に変え…〕 · [agents.md](https://agents.md)
- [ ] **日本語圏でのAGENTS.md/CLAUDE.md運用が「現場の作法」として整理される** — Claude Code、GitHub Copilot、Codex CLI、Gemini CLIなどの導入現場で、AGENTS.m… 〔技術: エージェントの出力品質を、プロンプト単体ではなくリポジトリ内の継続的…／人文: 日本語の開発現場では「うちのプロジェクトではその書き方をしない」とい…〕 · [qiita.com](https://qiita.com/dai_chi/items/61019c602c2c40dade07)
- [ ] **AGENTS.mdを20以上のAIツールにまたがるポータブル標準として読む** — AIコーディングツールが増え、ツールごとに設定を書き直す負担が出たことを背景に、AGENTS.mdをポータブルな設定ファイルとし… 〔技術: エージェントの振る舞いをベンダー固有設定から切り離し、ツール横断の運…／人文: これは「方言」の乱立から「共通語」への移行であり、同時に各チームが自…〕 · [qiita.com](https://qiita.com/kai_kou/items/cc9520a24d7c0e38ead4)
- [ ] **VS Code Agents windowがエージェント作業の「場」をUI化する** — VS Code 1.120のStable版プレビューとして公開されたAgents windowを、エージェント駆動開発専用の統合… 〔技術: Worktree isolationを既定にすることで、本流のコード…／人文: エージェントは抽象的な知能ではなく、「別室」「作業台」「隔離された工…〕 · [ai-souken.com](https://www.ai-souken.com/article/what-is-vscode-agents-window)

### History of Automation
- [ ] **Economic Governance of Autonomous Agents and Robots: Factor-Origin Accounting and Social Automation Funds** — 自律ソフトウェアエージェント、基盤モデル、ロボットが人間の労働時間から生産を切り離すことで、労働所得・給与課税中心の社会保険財源… 〔技術: エージェントやロボットの経済活動を、ワークフロー内の因果的寄与として…／人文: 産業革命期の機械化が労働・賃金・社会保険を作り替えたように、今回は「…〕 · [arxiv.org](https://arxiv.org/abs/2609.32476)
- [ ] **DevDay 2026 の振り返り** — OpenAI DevDay 2026 は、ChatGPT、Codex、モデル、AIと働く新しい方法にわたり20件超の発表を行った… 〔技術: 常時稼働型エージェントや開発環境内エージェントは、RPA的な定型自動…／人文: 「働く相手」としてのAIが前面化すると、労働史で繰り返されてきた監督…〕 · [openai.com](https://openai.com/ja-JP/index/devday-2026-recap)
- [ ] **AGENTS.md** — AGENTS.md は、OpenAI Codex、Amp、Google Jules、Cursor など複数のAIソフトウェア開発… 〔技術: AIエージェントがコードベースで安全に動くには、自然言語の作業規約、…／人文: 工場の作業標準書やマニュアルが自動化の前提だったように、ソフトウェア…〕 · [agents.md](https://agents.md)
- [ ] **When Digitalization Transforms Itself: AI, Software, and the Next Technical Order** — エージェント型AIによって、デジタル化が自分自身の技術的生産基盤、特にソフトウェアエンジニアリングを変形し始めたと論じる論文。 〔技術: ソフトウェアを作るソフトウェア、つまり自動化インフラ自体の自動化は、…／人文: これは機械制大工業が道具の生産を変えた歴史に似ており、社会の「作る力…〕 · [arxiv.org](https://arxiv.org/abs/2609.15350)
- [ ] **Redistributive Policies for the Times of Transformative AI** — Transformative AI の到来後、広範な自動化が労働分配率を下げ、所得・資産格差を拡大しうるという前提で、UBI、U… 〔技術: AI・ロボット・計算資源を「生産資本」として政策モデルに組み込み、自…／人文: 自動化の歴史では、機械の所有者と労働者のあいだで便益配分が常に争点に…〕 · [arxiv.org](https://arxiv.org/abs/2609.14750)

### DDD
- [ ] **ゴミの分別とポカヨケから学んだDDD・TDD 〜ブラジル人エンジニアが日本の生活で気づいたこと〜** — 日本のゴミ分別、ポカヨケ、電車の定時運行などの生活経験を、DDDのレイヤー分離、Value Object、TDDのリズムに重ねて… 〔技術: Value Objectを「不正な値をそもそも作れないポカヨケ」とし…／人文: DDDが文化翻訳の道具になっている点が面白い。〕 · [qiita.com](https://qiita.com/thiagovpaz/items/ec4fdcec5a302afd11bb)
- [ ] **Hexagen-Monaco: Governance Engine for Human and Agentic Systems** — TypeScriptモノレポ向けのガバナンスエンジンで、DDDとヘキサゴナルアーキテクチャをYAMLマニフェストとして表現し、結… 〔技術: 境界づけられたコンテキストや依存方向をドキュメントではなくコンパイル…／人文: これは「設計判断を人間の記憶に置かない」方向の実験でもある。〕 · [github.com](https://github.com/martinkrakowski/hexagen-monaco)
- [ ] **ai-ddd-devtrack** — 技術学習の目標、学習記録、資格試験の進捗を管理するための、AI coding agent と DDD のサンプルプロジェクト。 〔技術: AI coding agentに実装を任せる前提で、PlantUML…／人文: ユビキタス言語は会議室だけでなく、エージェントに渡すプロンプトや図に…〕 · [github.com](https://github.com/watanabe-1/ai-ddd-devtrack)
- [ ] **【勉強会】「AI時代『考える力』をどう鍛える？具体抽象トレーニング」に参加して考えたこと** — AIの進化が速い時代に、エンジニアが具体と抽象を行き来し、ユーザーの問題を捉える力をどう鍛えるかを扱った勉強会参加記。 〔技術: DDDのモデリングは、抽象化の演習であり、単なるクラス設計ではなく「…／人文: AIが答えを速く生成するほど、人間側には問いの立て方、思い込みの自覚…〕 · [qiita.com](https://qiita.com/ko1_tktn/items/5f0a18a0c91b398dc7d6)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — LLMを使ってドメイン駆動設計を自動化するプロンプティングフレームワークに関する論文。 〔技術: DDDの各活動をLLMプロンプトの連鎖として構造化することで、モデル…／人文: DDDを自動化する試みは、「ドメイン専門家との対話」をどこまで機械に…〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

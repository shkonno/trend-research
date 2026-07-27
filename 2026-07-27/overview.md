# 📰 2026-07-27 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLM が Gemini Notebook に改名 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- **Loop engineering** — OpenForgeRL: Train Harness-native Agents in Any Enviro… · [arxiv.org](https://arxiv.org/abs/2607.21557)
- **AWS** — Claude Opus 5 が Amazon Bedrock と Claude Platform on AW… · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-opus-5-on-aws-anthropics-most-capable-opus-model)
- **Harness engineering** — Ryan Lopopolo の `harness-engineering` リポジトリ公開 · [github.com](https://github.com/lopopolo/harness-engineering)
- **sharp LLM usage** — Ask HN: 100万行レガシーSaaSでAI生成コードを本番レビュー前にどう硬くするか · [news.ycombinator.com](https://news.ycombinator.com/item?id=49045271)
- **AI agent trends** — Claude Opus 5 と GitHub Copilot投入: 長時間コーディング・エージェントが前提化 · [anthropic.com](https://www.anthropic.com/news/claude-opus-5)
- **Claude Code** — Claude Code v2.1.219: Opus 5、1M context、厳格ネットワーク許可リスト、… · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.219)
- **Ethics of AI Agents** — Dynamic Capability Scoping for Enterprise AI Agents: A… · [arxiv.org](https://arxiv.org/abs/2607.22445)
- **Philosophy of Loop Engineering** — Harness Training: Training Agent Harnesses Like Model… · [henrypan.com](https://www.henrypan.com/blog/2026-07-18-harness-training)
- **Anthropology of Agentic AI** — Agentic AIとは？ · [cloud-for-all.com](https://www.cloud-for-all.com/blog/what-is-agentic-ai)
- **History of Automation** — Applying AI to Rebuild Middle Class Jobs · [nber.org](https://www.nber.org/papers/w32140)
- **DDD** — Domain-Driven Design in Practice: A Large-Scale Empiri… · [arxiv.org](http://arxiv.org/abs/2607.06471v1)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLM が Gemini Notebook に改名** — Google は NotebookLM を Gemini Notebook として再ブランド化し、既存ノートブックは引き続き利用… 〔技術: ソース接地型のノートブックが、Gemini アプリや Google…／人文: 「ノート」は個人の思考の私的な場所だったが、AI時代には企業プラット…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- [ ] **日本語公式ページでも「同じプロダクト」として Gemini Notebook を案内** — 日本語ページでは「Gemini Notebook は NotebookLM と同じプロダクトですか？ 〔技術: 既存データ継続を明示しながら名称と導線を切り替えることで、プロダクト…／人文: 学習者や現場担当者は、機能以上に「昨日と同じ場所に自分の資料がある」…〕 · [notebooklm.google](https://notebooklm.google/?hl=ja)
- [ ] **HN では改名に合わせて「論文を聴く」需要と限界が議論** — 「NotebookLM is now Gemini Notebook」に関する HN スレッドでは、Audio Overview… 〔技術: 音声要約はマルチモーダルな知識消化の入口だが、数学・図表・専門記号を…／人文: 「読む」を「聴く」に置き換えると、知識の速度と身体性が変わる。〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=48936451)
- [ ] **arXiv: NotebookLM 生成ポッドキャストの会話沈黙を分析** — “Modeling turn-taking with distant viewing” は、米国シットコムと Google No… 〔技術: 生成音声の評価を内容の正確さだけでなく、沈黙・間・話者交替という時間…／人文: 会話の「間」は単なる無音ではなく、関係性や権力、聞き手への配慮を含む…〕 · [arxiv.org](https://arxiv.org/abs/2607.18076)
- [ ] **arXiv: PHITS で NotebookLM を RAG 型支援として利用** — “Toward AI-Agent-Driven Particle Transport Simulations” は、PHITS… 〔技術: ドメイン固有マニュアルをRAG化し、専門シミュレーションの理解・入力…／人文: 専門家コミュニティの暗黙知を、AIが参照しやすい形に整える作業は新し…〕 · [arxiv.org](https://arxiv.org/abs/2607.11309)

### Loop engineering
- [ ] **OpenForgeRL: Train Harness-native Agents in Any Environment** — Claude Code や Codex のような実運用ハーネスをそのまま使い、状態を持つマルチターン・ツール利用エージェントをR… 〔技術: 推論時だけの足場だったエージェントループを、訓練データ生成と強化学習…／人文: anthropology の観点では、これは「現場の作業慣習」をモデ…〕 · [arxiv.org](https://arxiv.org/abs/2607.21557)
- [ ] **NVIDIA-labs OO Agents: Native Python Object-Oriented Agents** — NVIDIA の NOOA は、エージェントを Python オブジェクトとして表現し、メソッドを行動、フィールドを状態、doc… 〔技術: ワークフローグラフやツールスキーマの外側に散らばりがちなループ設計を…／人文: history の観点では、これはソフトウェア工学が長年蓄積した「保…〕 · [arxiv.org](https://arxiv.org/abs/2607.20709)
- [ ] **Operational Hallucination and Safety Drift in AI Agents** — ツール利用型自律エージェントで、長い実行のあいだに初期の安全意図が崩れる Safety Drift と、状態認識の失敗により反復… 〔技術: ループ回数・状態遷移・ツール呼び出し列を安全評価の単位にし、停止条件…／人文: ethics の観点では、「最初は安全と言った」ことではなく、時間の…〕 · [arxiv.org](https://arxiv.org/abs/2607.18366)
- [ ] **Understanding Agent-Reactive Bugs at the Model-Harness Boundary** — Codex、Gemini-CLI、LangChain、CrewAI の255件のバグ報告を分析し、モデル出力とハーネス反応の境界… 〔技術: エージェントループの不具合を、出力パース、コンテキスト管理、制御フロ…／人文: philosophy の観点では、行為者性を単体モデルへ帰属するので…〕 · [arxiv.org](https://arxiv.org/abs/2607.15684)
- [ ] **Intutic — The Circuit Breaker for AI Agents** — Claude Code、Cursor、LangGraph、n8n などに向けたオープンソースの「AIエージェント用サーキットブレ… 〔技術: ループの暴走や無駄な反復を、観測可能性だけでなく介入可能性の問題とし…／人文: narrative の観点では、自律エージェントを「英雄的に任せる機…〕 · [github.com](https://github.com/intutic/intutic)

### AWS
- [ ] **Claude Opus 5 が Amazon Bedrock と Claude Platform on AWS で提供開始** — AWS は Anthropic の Claude Opus 5 を Amazon Bedrock と Claude Platfo… 〔技術: 最高性能クラスの Claude を Bedrock のガバナンス、リ…／人文: 「賢いモデルを使う」から「組織の規範や監査の内側で賢さを運用する」へ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-opus-5-on-aws-anthropics-most-capable-opus-model)
- [ ] **OpenAI GPT-5.6 Sol / Terra / Luna が Amazon Bedrock と Kiro で利用可能に** — OpenAI GPT-5.6 の Sol / Terra / Luna が Amazon Bedrock で一般提供され、Bed… 〔技術: Bedrock が Claude だけでなく OpenAI 系モデル…／人文: モデル選択は「どれが一番賢いか」ではなく、「この仕事にどれだけの知性…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/get-started-with-openai-gpt-5-6-sol-terra-and-luna-on-amazon-bedrock)
- [ ] **aws-bench: AWS タスクを解く AI エージェントのオープンソースベンチマーク** — AWS は、実際の AWS 利用分析から作られた調査、トラブルシュート、インフラ作成タスクで AI エージェントを評価する研究プ… 〔技術: AWS 操作エージェントの能力を、曖昧なデモではなく再現可能なリソー…／人文: ベンチマークは単なるランキングではなく、「クラウドを任せられる」とは…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-bench)
- [ ] **Strands と Amazon Bedrock AgentCore による本番 AI エージェント評価パイプライン** — Motorway と AWS は、Strands Agents SDK と Amazon Bedrock AgentCore E… 〔技術: エージェントの評価をビルド時テストと本番監視に分け、pass^k な…／人文: エージェント運用の核心は「一度正しく答えた」ではなく「揺らぎ続ける状…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/evaluating-ai-agents-a-production-blueprint-with-strands-and-agentcore)
- [ ] **日本の Neuron Community が Trainium / Inferentia の実践知を共有** — AWS 日本語ブログは「Neuron Community - 2026 Vol.1」の開催報告を公開した。 〔技術: GPU 以外の AI アクセラレータを実務に入れるには、SDK、分散…／人文: 日本語コミュニティでの経験共有は、グローバルなクラウド技術を各現場の…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/neuron-community-2026-vol-1)

### Harness engineering
- [ ] **Ryan Lopopolo の `harness-engineering` リポジトリ公開** — OpenAI の Ryan Lopopolo による「harness engineering」のアンソロジー、フィールドガイド、… 〔技術: `AGENTS.md`、playbooks、evals を含む構成そ…／人文: 組織の暗黙知、品質基準、例外履歴、承認関係を「モデルの重み」ではなく…〕 · [github.com](https://github.com/lopopolo/harness-engineering)
- [ ] **Orbital Witness「Grading Ourselves Against the Harness Engineering Playbook」** — Orbital Witness が自社のエージェント harness を Ryan Lopopolo の 12 の thesis… 〔技術: 抽象論だった harness engineering を、既存チーム…／人文: これは単なる自動化礼賛ではなく、「人間が何を舵取りし、何を制度として…〕 · [tech.orbitalwitness.com](https://tech.orbitalwitness.com/posts/2026-07-22-grading-ourselves-against-the-harness-engineering-playbook)
- [ ] **HumanLayer「Why Software Factories Fail — harness engineering is not enough」** — HumanLayer が「ソフトウェア工場」型の lights-off 開発ナラティブにブレーキをかける長文。 〔技術: harness があっても、承認、観測、失敗時の介入、環境分離、ユー…／人文: 「あなたがボトルネック」「コードは無料」という物語への批判は、開発者…〕 · [github.com](https://github.com/humanlayer/advanced-context-engineering-for-coding-agents/blob/main/wsff.md)
- [ ] **`sd0x-dev-flow`: Claude Code 向け harness layer の具体実装** — Claude Code の外側に、hook 強制のレビューゲート、context compaction 後も残る state-m… 〔技術: `/codex-review-fast`、precommit、自動ル…／人文: エージェントの「気分」や一回の会話に頼らず、状態・レビュー・再開条件…〕 · [github.com](https://github.com/sd0xdev/sd0x-dev-flow)
- [ ] **arXiv「Harness Engineering for LLM-Driven GPU Kernel Generation」** — LLM による GPU カーネル生成を、評価 harness と profile-backed optimization con… 〔技術: 「harness engineering」がコーディングエージェント…／人文: 高速化競争では成果の数字だけが強調されがちだが、この論文は「どの証拠…〕 · [arxiv.org](https://arxiv.org/abs/2607.17979)

### sharp LLM usage
- [ ] **Ask HN: 100万行レガシーSaaSでAI生成コードを本番レビュー前にどう硬くするか** — 15年もののC# / React / Azureの100万行超コードベース上で、PRD、LLM生成アーキテクチャ文書、Claud… 〔技術: PRD→アーキテクチャ→ストーリー→PR→別モデルレビュー→手動E2…／人文: 「非エンジニアがAIで開発を進め、専門家が後から信頼性を裁定する」と…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49045271)
- [ ] **Context Matters: Improving the Practical Reliability of LLM-Based Unit Test Generation** — 産業プロジェクトでのLLM単体テスト生成は、複雑なフレームワークやクロスファイル依存のためコンパイル失敗・手修正・不安定なカバレ… 〔技術: 「LLMに足りない文脈を推測させる」のではなく、依存・スキャフォール…／人文: テスト生成の失敗はモデル能力だけでなく、組織が暗黙知として保持してき…〕 · [arxiv.org](http://arxiv.org/abs/2607.19682v1)
- [ ] **Common workflows - Claude Code Docs** — Claude Codeの公式ワークフロー集で、コードベース探索、バグ修正、リファクタリング、テストなど日常タスクを段階的に扱うた… 〔技術: LLMの性能を引き出す鍵が、巨大な依頼文ではなく、探索・差分作成・テ…／人文: これはプログラミング教育の作法にも近い変化で、AIに命令する人間も「…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/common-workflows)
- [ ] **A Fireside Chat with Cat and Thariq from the Claude Code team** — Claude CodeチームのCat WuとThariq Shihiparへの対談で、subagentやworkflowは「Cl… 〔技術: LLM活用の鋭さが、人間のプロンプト文面から、モデルに下位タスク・下…／人文: ここでは創造性が人間からAIへ単に移譲されるのではなく、人間・親モデ…〕 · [simonwillison.net](https://simonwillison.net/2026/Jul/21/cat-and-thariq)
- [ ] **A harness for every task: dynamic workflows in Claude Code** — Claude Codeがタスクごとに自分用のmulti-agent harnessをその場で書き、オーケストレーションできるとい… 〔技術: 汎用エージェントに毎回同じ指示を投げるのではなく、タスク固有の小さな…／人文: これはAIを万能秘書として扱う発想から、現場ごとに仮設のチームや工房…〕 · [claude.com](https://claude.com/blog/a-harness-for-every-task-dynamic-workflows-in-claude-code)

### AI agent trends
- [ ] **Claude Opus 5 と GitHub Copilot投入: 長時間コーディング・エージェントが前提化** — AnthropicはClaude Opus 5を発表し、長時間エージェント、コーディング、専門的知識作業での改善を強調した。 〔技術: モデル単体のベンチマークだけでなく、Copilot上での自律的コード…／人文: 開発者の仕事は「コードを書く」から「長時間働く相棒の判断・コスト・安…〕 · [anthropic.com](https://www.anthropic.com/news/claude-opus-5)
- [ ] **Claude Agent SDK: Claude Codeのエージェント・ループをライブラリ化** — Claude Agent SDKは、Claude CodeをPython/TypeScriptから呼び出せるライブラリとして提供… 〔技術: CLIエージェントのノウハウをSDK化することで、エージェント・ハー…／人文: これは「チャットボットを使う」段階から、「組織内に小さな行為者を配置…〕 · [code.claude.com](https://code.claude.com/docs/en/agent-sdk/overview)
- [ ] **Copilot cloud agent for Linear が一般提供: 非同期バックグラウンド・エージェント運用が現実化** — GitHubは、LinearのIssueをCopilot cloud agentに割り当てられる機能の一般提供を発表した。 〔技術: エージェントがIDE内の対話相手ではなく、Issue管理システムから…／人文: 人間のチームメイトにチケットを渡す行為と、AIエージェントにチケット…〕 · [github.blog](https://github.blog/changelog/2026-07-23-copilot-cloud-agent-for-linear-is-now-generally-available)
- [ ] **GitHub MCP Server が次期MCP仕様に対応: エージェント接続の標準化が進む** — GitHub MCP Serverは、2026-07-28に予定されているMCPのstateless core仕様に先行対応した… 〔技術: stateless化と広範なクライアント対応は、エージェントのツール…／人文: MCPはしばしば「AIのUSB-C」と呼ばれるが、実際には私たちのデ…〕 · [github.blog](https://github.blog/changelog/2026-07-23-github-mcp-server-supports-the-next-mcp-specification)
- [ ] **OpenForgeRL / Agentic Context Management: エージェント研究が「訓練」と「記憶のライフサイクル」へ深掘り** — `OpenForgeRL: Train Harness-native Agents in Any Environment` は、… 〔技術: エージェント性能のボトルネックが、モデル重みだけでなく、ハーネス込み…／人文: 「AIに何を覚えさせ、何を忘れさせるか」は単なる最適化ではなく、組織…〕 · [arxiv.org](https://arxiv.org/abs/2607.21557)

### Claude Code
- [ ] **Claude Code v2.1.219: Opus 5、1M context、厳格ネットワーク許可リスト、ネストしたサブエージェント** — v2.1.219ではClaude Opus 5がOpus系のデフォルトとして追加され、1M contextとfast modeの… 〔技術: 大コンテキストのモデル更新だけでなく、ネットワーク遮断、作業ディレク…／人文: これは開発者の仕事を、コードを書く個人技から、複数の半自律的作業者を…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.219)
- [ ] **Claude Code GitHub Action v1.0系がClaude Code 2.1.220 / Agent SDK 0.3.220へ追随** — `anthropics/claude-code-action`はv1.0.183を公開し、直近コミットでClaude Code… 〔技術: ローカルCLIの更新がGitHub Actionに素早く反映されるこ…／人文: 「@claudeに頼む」文化は、開発者の会話空間をチャットからリポジ…〕 · [github.com](https://github.com/anthropics/claude-code-action/releases/tag/v1.0.183)
- [ ] **OpenForgeRL: Claude CodeのようなハーネスそのものをRL訓練対象にする** — OpenForgeRLは、Claude Code、Codex、OpenClawのような複雑な推論ハーネスを、標準的なSFT/RL… 〔技術: 研究対象が「モデル単体」から「Claude Codeのようなツール実…／人文: これはAIエージェントを、頭脳だけでなく作業場・道具・ログ・制度を含…〕 · [arxiv.org](https://arxiv.org/abs/2607.21557)
- [ ] **日本語圏の実践: Claude Code生成PRが「並列エージェント運用の思想」をdotfilesに明文化** — 日本語のPRで、`dispatch-issues` skillの方針を「ファイル競合を理由に並列化を止めない」「真の順序依存だけ… 〔技術: Claude Codeを単にコード生成器として使うのではなく、複数エ…／人文: ここで起きているのは、開発チームの「仕事の礼儀」の再設計である。〕 · [github.com](https://github.com/bmthd/dotfiles/pull/38)
- [ ] **IssueTrojanBench / Bad Memory: Claude Code型エージェントの信頼境界が研究テーマ化** — IssueTrojanBenchは、悪意あるIssue要求に対してAIコーディングエージェントがどのように危険な変更や外部API… 〔技術: Claude Codeの価値が「リポジトリを読み、コマンドを実行し、…／人文: エージェントは信頼できる同僚のように振る舞うが、実際にはテキストに非…〕 · [arxiv.org](https://arxiv.org/abs/2607.20759)

### Ethics of AI Agents
- [ ] **Dynamic Capability Scoping for Enterprise AI Agents: A Synthetic Dataset and Three-Source Permission Architecture** — 企業AIエージェントに静的で広すぎる認証情報を与える慣行を批判し、タスク文脈に応じた動的最小権限、ロール上限、タスク分類器、ポリ… 〔技術: エージェント安全をプロンプトや検出器ではなく、実行時の権限スコープと…／人文: 責任所在を「AIが判断した」から「組織がどの権限を、どの文脈で許した…〕 · [arxiv.org](https://arxiv.org/abs/2607.22445)
- [ ] **The Ethics of Autonomous AI Agents for Offensive Security** — 自律型AIエージェントが攻撃的セキュリティ領域にもたらす倫理問題を、行動の非決定性、影響範囲の開放性、利用者層の不確定性という三… 〔技術: 従来の決定的なセキュリティツールとは異なる、LLMエージェント特有の…／人文: 「誰が攻撃能力を持つべきか」という専門職倫理の問題を、ツール普及後の…〕 · [arxiv.org](https://arxiv.org/abs/2607.20255)
- [ ] **ResearchArena: Evaluating Sabotage and Monitoring in Automated AI R&D** — AIエージェントがAI研究開発そのものを自動化する状況で、成果物に埋め込まれた破壊工作や、サンドボックス外での隠れた行動を評価す… 〔技術: 長期タスク、隠れた副タスク、複数タイプのモニターを組み合わせ、成果物…／人文: 「優秀な協力者」が同時に「潜在的な裏切り者」でもあり得るという制度設…〕 · [arxiv.org](https://arxiv.org/abs/2607.19321)
- [ ] **Know Your Agent: Reconnaissance-Driven Pentesting of AI Agents** — AIエージェントに対する攻撃でも、従来のペンテスト同様に偵察が重要だとし、エージェントの知識資産や弱点を抽出して間接プロンプトイ… 〔技術: ブラックボックスのエージェントをプローブし、ターゲットプロファイルを…／人文: 人間社会でいう「相手を知る」偵察が、機械相手にも成立する点が示唆的で…〕 · [arxiv.org](https://arxiv.org/abs/2607.19837)
- [ ] **When HTTP 402 Meets the Blockchain: Risks on Emerging x402 Payments** — Web APIや自律型AIエージェント向けの支払いプロトコルx402について、ファシリテータが支払い検証とオンチェーン決済を担う… 〔技術: エージェントがAPIを購入・実行する経済圏で、認可正当性と実行安全性…／人文: 自律エージェントが「財布」を持つと、責任は発話内容だけでなく取引・決…〕 · [arxiv.org](https://arxiv.org/abs/2607.19545)

### Philosophy of Loop Engineering
- [ ] **Harness Training: Training Agent Harnesses Like Model Weights** — LLM本体を固定し、プロンプト、コンテキスト管理、ツール、修復ループからなる「ハーネス」をPyTorch風に訓練する試み。 〔技術: モデル重みではなく周辺の実行環境を、評価結果を勾配のように扱う閉ルー…／人文: これは「知能は頭脳の中だけにあるのか、それとも道具・記録・環境との循…〕 · [henrypan.com](https://www.henrypan.com/blog/2026-07-18-harness-training)
- [ ] **WorldBuild Bench: Same brief, same tools, same harness** — 9つの主要AIモデルに同じゲーム設計ブリーフ、同じツール、同じThree.js/Rapier足場、同じPlaywrightプレイ… 〔技術: ハーネスを固定してモデル差だけを観測し、実行ログ、スクリーンショット…／人文: 「世界を作れる」とは単にコードが動くことではなく、空間・時間・原因・…〕 · [sandscape.app](https://sandscape.app/worldbuild/rounds/ai-game-benchmark-2026-07-13)
- [ ] **Skill Self-Play: Pushing the Frontier of LLM Capability with Co-Evolving Skills** — Proposer、Solver、Dynamic Skill Controller が強化学習ループの中で共進化し、検証可能なスキ… 〔技術: スキルを「深い実行検証ができる小さな場」とし、動的ルーティングで多様…／人文: これは経験論の問題、つまり経験から学ぶ主体が、どの経験を信頼できる証…〕 · [arxiv.org](https://arxiv.org/abs/2607.22529)
- [ ] **MalSkillBench: A Runtime-Verified Benchmark of Malicious Agent Skills** — Claude Code や Gemini CLI などのコーディングエージェントが使う「スキル」を、コードであり自然言語指示でも… 〔技術: 悪性サンプルを生成するだけでなく実行時に発火することを確認してラベル…／人文: スキルがコードと指示の中間物である点は、近代的な「物」と「言葉」の区…〕 · [arxiv.org](https://arxiv.org/abs/2606.07131)
- [ ] **FizzBee: AI Requirements Engineer between your idea and your coding agent** — 曖昧なアイデアを、コーディングエージェントが構築でき、機械が解析できる精密で検証済みの仕様へ変換することを掲げるツール。 〔技術: 実装ループの前に仕様の曖昧さを発見・検証する段階を挿入し、エージェン…／人文: これは「何を作るべきか」をコード生成に丸投げしないための実践知であり…〕 · [fizzbee.ai](https://fizzbee.ai)

### Anthropology of Agentic AI
- [ ] **Agentic AIとは？仕組み・実例・AI Agentとの違いを徹底解説** — Agentic AIの仕組み、AI Agentとの違い、マーケティングや開発などの実例、導入前の注意点を整理した解説。 〔技術: エージェントを計画・ツール利用・実行・フィードバックの連鎖として捉え…／人文: 人類学的には、これは仕事を「人がやる／機械が補助する」から「人が目標…〕 · [cloud-for-all.com](https://www.cloud-for-all.com/blog/what-is-agentic-ai)
- [ ] **Agentic AIについて非エンジニア向けにわかりやすくまとめてみた** — 複数のAI Agentが役割を担当し、目標に向かって協調的に動くシステムとしてAgentic AIを説明する非エンジニア向け記事… 〔技術: マルチエージェント的な役割分担を、非専門職にも伝わる業務モデルとして…／人文: 企業で新技術が受け入れられるとき、最初に必要なのはコードではなく「何…〕 · [zenn.dev](https://zenn.dev/nttdata_tech/articles/925b2510ccf517)
- [ ] **AIエージェント（Agentic AI）完全解説ガイド2026：「ChatGPTに『させる』から『やらせる』へ」** — OpenAI Operator、Claude Computer Use、Google Astra、Microsoft Copil… 〔技術: ブラウザ操作、PC操作、マルチステップ計画、外部ツール連携を、エージ…／人文: 「させる／やらせる」という日本語の使い分けには、命令・責任・服従のニ…〕 · [labmemo.com](https://labmemo.com/agentic-chatgpt-openai-operators-anthropic-claude-2026)
- [ ] **AIツールおすすめ比較15選！目的別の選び方と無料・有料プランを徹底解説** — 2026年のAIツール選定ガイドの中で、AIエージェントの台頭とマルチモーダル化を主要トレンドとして位置づけている。 〔技術: 目的、無料プラン、日本語精度、連携性などの選定軸を通じて、エージェン…／人文: 道具の比較表は、組織が新しい実践を標準化する前段階の「市場の分類儀礼…〕 · [japan-ai.co.jp](https://japan-ai.co.jp/media/5932)
- [ ] **AIエージェントとは？仕組みや生成AIとの違い、企業での活用例をわかりやすく解説** — AIエージェントの仕組み、生成AIとの違い、企業での活用例を展示会メディアの文脈で解説する記事。 〔技術: 企業利用を前提に、タスク実行・外部連携・業務効率化の観点からAIエー…／人文: 展示会／業界メディアは、新しい技術を「導入してよいもの」として社会化…〕 · [japan-it.jp](https://www.japan-it.jp/hub/ja-jp/blog/article-67.html)

### History of Automation
- [ ] **Applying AI to Rebuild Middle Class Jobs** — David Autorによる論文で、AIを単なる省力化・置換の機械としてではなく、中間層の専門判断を補完し再構築する技術として設… 〔技術: AIエージェントを「完全自動化」ではなく、労働者の判断・訓練・責任分…／人文: 自動化の歴史を、機械が人間を置き換える物語ではなく、技能・賃金・尊厳…〕 · [nber.org](https://www.nber.org/papers/w32140)
- [ ] **Generative AI at Work** — 顧客サポート業務における生成AI導入を分析し、生産性向上が経験の浅い労働者に大きく現れることを示した実証研究。 〔技術: AI支援ツールが熟練者の暗黙知をワークフロー内に埋め込み、リアルタイ…／人文: これは「職人技の民主化」でもあり「熟練の抽出」でもあるため、誰の知識…〕 · [nber.org](https://www.nber.org/papers/w31161)
- [ ] **Power and Progress: Our 1000-Year Struggle Over Technology and Prosperity** — Daron AcemogluとSimon Johnsonが、技術進歩の果実は自動的には広く分配されず、制度・権力・社会運動によっ… 〔技術: AIエージェントの性能向上そのものより、導入先の組織設計・所有権・説…／人文: 自動化を「進歩だから不可避」と語るナラティブを相対化し、制度が違えば…〕 · [shapingwork.mit.edu](https://shapingwork.mit.edu/research/power-and-progress-our-1000-year-struggle-over-technology-and-prosperity)
- [ ] **Ghost Work: How to Stop Silicon Valley from Building a New Global Underclass** — Mary L. GrayとSiddharth Suriによる、オンラインサービスやAIシステムを支える不可視の人間労働を扱う研究… 〔技術: AIエージェントの「自律性」は、学習データ、評価、監視、失敗時の人間…／人文: 自動化の文化史では、機械が人間を消すのではなく、人間を画面の外へ移動…〕 · [ghostwork.info](https://ghostwork.info)
- [ ] **The Automation Charade** — Astra Taylorが、ロボットや自動化の脅威がしばしば誇張され、その誇張が賃金抑制や労働条件悪化を正当化する言説として機能… 〔技術: AIエージェント導入の評価では、実際に自動化できる範囲と、経営・投資…／人文: 自動化の歴史は技術史であると同時に、恐怖と期待を使った統治の歴史でも…〕 · [logicmag.io](https://logicmag.io/failure/the-automation-charade)

### DDD
- [ ] **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — GitHub上のDDD関連リポジトリを大規模に調べ、候補11,742件からGPT-4oの多数決検証で2,502件をDDD実践例と… 〔技術: DDDの「採用されている／されていない」をREADMEやトピックだけ…／人文: DDDはしばしば信念や流派として語られますが、この研究は共同体の実践…〕 · [arxiv.org](http://arxiv.org/abs/2607.06471v1)
- [ ] **faceto: typed fileからLLMと考えるEvent Stormingボードを生成するツール** — typed fileを入力に、Event StormingのHTML/SVGボードを生成し、要素をクリックしてメモを残し、次のL… 〔技術: Event Stormingをホワイトボード写真ではなく、LLMが読…／人文: ワークショップは本来、場の空気や沈黙も含む共同作業ですが、このツール…〕 · [github.com](https://github.com/bastien-gallay/faceto)
- [ ] **The Method / ai-refinement-method: AI coding agentsの前にDDD・Event Storming・脅威モデリングで仕様を固める** — 平文の要求を、ドメインマッピング、意思決定、脅威、受け入れ条件、失敗するテストを含む「build-ready stories」に… 〔技術: DDD、Event Storming、仕様リファインメントを、AI…／人文: 「コードが安くなった時代に、仕様品質が新しいボトルネックになる」とい…〕 · [github.com](https://github.com/nlawstudio/ai-refinement-method)
- [ ] **Archally Blueprint Schema: DDD・ADR・ルール・Event Stormingを1つのYAMLモデルに統合する試み** — bounded context、business rules、governance、architecture、decision… 〔技術: DDDの成果物をドキュメント群ではなく、生成・検証・AI参照が可能な…／人文: 散らばったWikiやホワイトボード写真を「fragmented tr…〕 · [github.com](https://github.com/Archally/blueprint-schema)
- [ ] **axi-go: AI agent toolsのためのDDD的な実行カーネル** — AIエージェントに渡すツールを、Actions（何をしたいか）とCapabilities（どう実行するか）の2層に分け、型付き契… 〔技術: エージェントのツール呼び出しを生の関数群ではなく、意図・副作用・証跡…／人文: AIエージェントの自律性は「何ができるか」より「誰が止められるか」で…〕 · [github.com](https://github.com/klarlabs-studio/axi-go)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

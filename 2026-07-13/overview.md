# 📰 2026-07-13 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — 日本語の業務導入判断向け「NotebookLMとは？ · [crystal-method.com](https://crystal-method.com/blog/notebooklm)
- **Loop engineering** — Loop Engineering徹底解説：自律エージェントを「動く」から「運用できる」へ · [qiita.com](https://qiita.com/Simon_Zhang/items/388cd1125860591f5c8d)
- **AWS** — AWS DMS Schema Conversion が AI agent automation をサポート · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-dms-sc-ai-agent-automation-mcp-server)
- **Harness engineering** — From Prompts to Contracts: Harness Engineering for Aud… · [arxiv.org](https://arxiv.org/abs/2607.08028)
- **sharp LLM usage** — Rewriting Bun in Rust: agentic engineering が大規模リライトの禁忌… · [simonwillison.net](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust)
- **AI agent trends** — Claude Code v2.1.207: Auto mode一般化とセキュリティ同意まわりの修正 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.207)
- **Claude Code** — Claude Code v2.1.207: auto modeのクラウド基盤対応とセキュリティ修正 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.207)
- **Ethics of AI Agents** — Persuasion Attacks Can Decrease Effectiveness of CoT M… · [arxiv.org](https://arxiv.org/abs/2607.08066)
- **Philosophy of Loop Engineering** — Cheap Code, Costly Judgment: A Case Study on Governabl… · [arxiv.org](https://arxiv.org/abs/2607.01087)
- **Anthropology of Agentic AI** — Aleena: Alignment Agent for Research Software Engineer… · [arxiv.org](https://arxiv.org/abs/2607.08043)
- **History of Automation** — The Context Access Divide: Interaction-Level Architect… · [arxiv.org](https://arxiv.org/abs/2607.08495v1)
- **DDD** — Domain-Driven Design in Practice: A Large-Scale Empiri… · [arxiv.org](https://arxiv.org/abs/2607.06471v1)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **日本語の業務導入判断向け「NotebookLMとは？」最新版** — NotebookLMの基本概念、主要機能、料金、導入前の注意点を、経営・業務責任者向けに整理した日本語記事。 〔技術: 汎用チャットではなく、ユーザーが追加した資料に回答範囲を閉じる「ソー…／人文: 企業内の知識は検索エンジン上の公開知ではなく、部署・文脈・暗黙知に埋…〕 · [crystal-method.com](https://crystal-method.com/blog/notebooklm)
- [ ] **公式ヘルプが示すNotebookLMの現在地: 80以上の言語、引用付き回答、Studio生成物** — Googleの公式ヘルプでは、NotebookLMを「AI搭載のリサーチアシスタント」と説明し、PDF、ウェブサイト、YouTu… 〔技術: 入力形式の多様化と引用付き回答により、NotebookLMはマルチモ…／人文: 資料を読む行為が、読む・聴く・図で見る・問い直すという複数の身体的モ…〕 · [support.google.com](https://support.google.com/notebooklm/answer/16164461?hl=ja&co=GENIE.Platform%3DDesktop)
- [ ] **スライド修正、Cinematic Video Overviews、インフォグラフィック、学習カード改善** — Google Workspace Updatesは、NotebookLMでのスライド修正、Cinematic Video Ove… 〔技術: Geminiがソース内容をもとに、スライド、動画、インフォグラフィッ…／人文: 同じ資料でも、研究者、経営者、学生、初学者が必要とする語り方は異なる…〕 · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/03/new-ways-to-customize-and-interact-with-your-content-in-NotebookLM.html)
- [ ] **Google Classroomで学生が個人用クラスNotebookを作成可能に** — 高等教育の18歳以上の学生が、Google ClassroomのGeminiタブから、教員が提供したクラス資料に基づく個人用No… 〔技術: LMS上の教材をNotebookLMに接続し、授業資料に根拠づけられ…／人文: これは「家庭教師の個別化」を制度内に持ち込む一方で、学ぶ主体が何を自…〕 · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/04/students-can-now-create-personal-class-notebooks-with-NotebookLM-in-Google-Classroom.html)
- [ ] **arXiv: X+SlidesがNotebookLMを含むスライド生成システムを評価** — 論文「X+Slides: Benchmarking Audience-Conditioned Slide Generation」… 〔技術: NotebookLMのような資料変換ツールを、単なる要約精度ではなく…／人文: プレゼン資料は中立な圧縮物ではなく、誰に向けて何を強調するかという社…〕 · [arxiv.org](https://arxiv.org/abs/2606.19256)

### Loop engineering
- [ ] **Loop Engineering徹底解説：自律エージェントを「動く」から「運用できる」へ** — Loop Engineering を、AIエージェントがタスク達成まで繰り返す制御ループを信頼性・安全性・コスト・観測性の観点か… 〔技術: ループをプロンプト列ではなく、状態遷移・評価器・ガードレール・監視を…／人文: ethics の観点では、自律性を高めるほど「誰が止めるのか」「どの…〕 · [qiita.com](https://qiita.com/Simon_Zhang/items/388cd1125860591f5c8d)
- [ ] **Loop Engineering入門：AIコーディングエージェントを動かすループ設計** — 設計対象を「個々のプロンプト」から「ループ（システム）」へ移す入門記事。 〔技術: コーディングエージェントの生産性を、モデル単体の賢さではなく、タスク…／人文: history の観点では、職人が道具を直接操作する段階から、工程表…〕 · [zenn.dev](https://zenn.dev/suwash/articles/loop-engineering_20260610)
- [ ] **Loop Engineering Guide: Build Safe Autonomous Agent Loops** — 「手で一回ずつプロンプトを与える」のではなく、作業発見、エージェントへの割当、成果検証、状態保存、スケジュールまたはトリガーによ… 〔技術: discover → assign → verify → persi…／人文: philosophy 的には、エージェントの「意図」をモデル内部では…〕 · [loopengineering.run](https://loopengineering.run)
- [ ] **When Agents Do Not Stop: Uncovering Infinite Agentic Loops in LLM Agents** — LLMエージェントが計画、ツール使用、状態更新、エージェント間ハンドオフを繰り返す中で、終了条件が実効的に働かず「Infinit… 〔技術: loop engineering の最重要リスクである「止まらないエ…／人文: ethics の観点では、AIの危険性が「悪い意図」だけでなく、善意…〕 · [arxiv.org](https://arxiv.org/abs/2607.01641)
- [ ] **TTHE: Test-Time Harness Evolution** — LLMエージェントの挙動はモデルだけでなく、コンテキスト構築、ツール呼び出し、中間検証、失敗回復を担うハーネスに大きく左右される… 〔技術: loop engineering を手作業の設計論から、実行トレース…／人文: philosophy 的には、知能を「答える能力」ではなく、失敗から…〕 · [arxiv.org](https://arxiv.org/abs/2607.08124)

### AWS
- [ ] **AWS DMS Schema Conversion が AI agent automation をサポート** — AWS DMS Schema Conversion が AWS MCP Server 経由の AI エージェント自動化に対応し、… 〔技術: データベース移行という失敗コストの高い領域に MCP とコーディング…／人文: 移行は単なる技術作業ではなく、組織の歴史が詰まった古いシステムとの交…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-dms-sc-ai-agent-automation-mcp-server)
- [ ] **AWS MCP Server が OAuth / AWS Sign-In 接続をサポート** — AI エージェントが AWS MCP Server に AWS Sign-In と業界標準 OAuth で直接接続できるようにな… 〔技術: エージェントのツール接続を「秘密鍵を渡す」方向ではなく、既存 IAM…／人文: AI エージェントを同僚のように働かせるには、信頼だけでなく「誰が何…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/oauth-aws-mcp-server)
- [ ] **Kiro で Claude Sonnet 5 が利用可能に** — AWS の Kiro IDE、CLI、Web で Claude Sonnet 5 が利用可能になったことを日本語で案内しています… 〔技術: Claude 系モデルを Kiro の IDE/CLI/Web に入…／人文: 開発者が「検索して読む」だけでなく「相棒と設計を往復する」作業様式へ…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/sonnet-5)
- [ ] **Amazon EKS が Kubernetes バージョンロールバックをサポート** — Amazon EKS で Kubernetes バージョンアップ後、7日以内であればロールバックできる機能が紹介されました。 〔技術: Kubernetes アップグレードの不可逆性を下げ、プラットフォー…／人文: 運用者の心理的安全性に効く機能です。〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/upgrade-amazon-eks-clusters-with-confidence-using-kubernetes-version-rollbacks)
- [ ] **AWS CloudFormation Express mode が最大4倍速いインフラデプロイを提供** — CloudFormation Express mode により、インフラデプロイの確認を高速化し、AI エージェントや開発者がよ… 〔技術: IaC のデプロイ待ち時間を短縮し、AI エージェントが生成した変更…／人文: 待ち時間は開発者の集中力と判断を削ります。〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/accelerate-your-infrastructure-deployments-by-up-to-4x-with-aws-cloudformation-express-mode)

### Harness engineering
- [ ] **From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents** — 企業向けLLMエージェントを、プロンプト中心の試作から、コード・マニフェスト・スキーマ・検証アーティファクトで囲んだ監査可能なハ… 〔技術: 「モデルが出す部分」と「コードが保証する部分」を分け、source…／人文: AIに仕事を任せる不安は、能力不足だけでなく「責任の所在が見えない」…〕 · [arxiv.org](https://arxiv.org/abs/2607.08028)
- [ ] **Remember When It Matters: Proactive Memory Agent for Long-Horizon Agents** — 長期タスクで重要な状態が軌跡の中に埋もれて行動に反映されなくなる現象を “behavioral state decay” と呼び… 〔技術: ハーネスを単なるツール呼び出し枠ではなく、行動エージェントの外側で状…／人文: 人間の共同作業でも、重要なのは「何を覚えているか」より「いつ思い出さ…〕 · [arxiv.org](https://arxiv.org/abs/2607.08716)
- [ ] **Cognitive-structured Multimodal Agent / CMA-Harness** — 長期のマルチモーダル対話で画像・テキスト履歴が膨らみすぎる問題に対し、Episodic Visual Memory、retrie… 〔技術: 視覚履歴をそのままコンテキストに詰めるのではなく、抽象化・検索・実行…／人文: 「記憶」は人間の主観や物語性とも深く関わる。〕 · [arxiv.org](https://arxiv.org/abs/2607.08497)
- [ ] **Claude Code Hooks / Subagents / Skills の公式ドキュメント群** — Claude Code の hooks はイベント、設定スキーマ、JSON入出力、終了コード、HTTP/MCP/Prompt h… 〔技術: Boris Cherny / Claude Code / loop…／人文: 開発者の役割は「AIに頼む人」から「AIが失敗しにくい舞台を設計する…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [ ] **中国語圏コミュニティの Harness Engineering 学習・解説の増殖** — deusyu/harness-engineering は「Harness Engineering 学習指南」として概念、実践、翻… 〔技術: 研究論文だけでなく、AGENTS.md、linter、リポジトリ内ド…／人文: 新しい技術語がコミュニティで翻訳される時、その社会は単に輸入している…〕 · [github.com](https://github.com/deusyu/harness-engineering)

### sharp LLM usage
- [ ] **Rewriting Bun in Rust: agentic engineering が大規模リライトの禁忌を揺らす** — BunのZigからRustへの大規模リライトについて、Simon Willisonは「dynamic workflows, tr… 〔技術: LLM活用の核心がコード生成そのものではなく、試行環境・回帰テスト・…／人文: 「書く人」から「リスクを設計し、失敗を観察する人」へエンジニア像が移…〕 · [simonwillison.net](https://simonwillison.net/2026/Jul/8/rewriting-bun-in-rust)
- [ ] **Ask HN: established code baseでのLLMコーディング実践** — 小規模スタートアップが、Cursor、Gemini、OpenAI、Claude、GitHub Copilot PR、Bugbot… 〔技術: 「issueを必ずCopilotに投げ、PRは捨ててもよい」「CI・…／人文: ここでのLLMは魔法の同僚ではなく、レビュー負荷と文脈切替を増やす労…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=46292682)
- [ ] **AI-written change descriptions 禁止という失敗例** — Kenton Vardaは、PR説明・コミットメッセージ・issue/ticketのAI生成をチームで一時禁止したと述べています… 〔技術: LLMに「要約」を任せると、差分から抽出しやすい局所情報へ過適合し、…／人文: 良い変更説明は、単なる記録ではなく他者の理解時間を減らす贈与です。〕 · [simonwillison.net](https://simonwillison.net/2026/Jul/8/kenton-varda)
- [ ] **EvalLoop: 評価を「モデル選定」ではなく改善ループにする** — 「EvalLoop: A Methodology for Evaluation-Driven Iterative Improve… 〔技術: sharp LLM usageで最も不足しがちな「何が悪かったかを測…／人文: 評価は罰点表ではなく、組織が機械との共同作業を学習するための会話装置…〕 · [arxiv.org](https://arxiv.org/abs/2607.05638)
- [ ] **Agent Skills評価ツール比較: 「動く」と「効く」を分ける日本語実践** — 「そのAgent Skills、本当に効いてる？ 〔技術: スキルやプロンプトを資産化するには、再現テスト、トレース、A/B実験…／人文: 「効いている気がする」を卒業することは、AI導入を個人芸から組織知へ…〕 · [qiita.com](https://qiita.com/syun136_616/items/68c58bf10e47f31859c4)

### AI agent trends
- [ ] **Claude Code v2.1.207: Auto mode一般化とセキュリティ同意まわりの修正** — Claude Code v2.1.207では、Bedrock / Vertex AI / FoundryでAuto modeが環… 〔技術: Auto mode、リモート設定、非対話実行、プロンプトインジェクシ…／人文: 「自動化をどこまで許可するか」は単なるUXではなく、権限委譲と責任の…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.207)
- [ ] **Claude Code v2.1.203〜2.1.206: background agents / worktree / MCP roots の運用改善** — v2.1.203では、セッションの追加作業ディレクトリをMCP `roots/list`に反映し、background sess… 〔技術: roots/list、worktree、background age…／人文: 人間の仕事は中断・再開・引き継ぎでできています。〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.203)
- [ ] **Token-Flow Firewall: 永続AIエージェントのランタイム監査** — 永続AIエージェントでは、危険な内容が会話の一瞬で終わらず、永続状態・再利用スキル・ツール呼び出しを通じて伝播し得るという問題を… 〔技術: 安全性をモデル単体の出力検査ではなく、状態・スキル・ツールを横断する…／人文: 記憶を持つAIの危険は「悪い発話」よりも「悪い習慣が残ること」に近い…〕 · [arxiv.org](http://arxiv.org/abs/2607.08395v1)
- [ ] **TTHE: Test-Time Harness Evolution / Harness Engineering の学術化** — TTHEは、LLMエージェントの振る舞いをモデルだけでなく、コンテキスト構築・ツール呼び出し・検証・失敗回復を担う「harnes… 〔技術: プロンプト最適化から、実行プログラム・契約・検証・トレースを含むha…／人文: 「賢さ」を個人能力ではなく環境設計で生むという見方は、人間の組織論に…〕 · [arxiv.org](http://arxiv.org/abs/2607.08124v1)
- [ ] **日本語圏のClaude Code実践: CLAUDE.md設計、ワークフロー、Threads運用自動化** — 直近の日本語圏では、Claude Codeの公式ドキュメント精読、CLAUDE.md設計、ワークフロー化、AI-DLC導入、Th… 〔技術: 日本語実践は、MCPやsubagentsそのものよりも、CLAUDE…／人文: ローカルな実践知は、公式機能とは別の「使い方の文化」を作ります。〕 · [qiita.com](https://qiita.com/tatatata_jp/items/fd51edca0915ad750a8e)

### Claude Code
- [ ] **Claude Code v2.1.207: auto modeのクラウド基盤対応とセキュリティ修正** — Bedrock、Vertex AI、Foundryでauto modeが環境変数の事前opt-inなしに使えるようになり、Bed… 〔技術: Claude Codeがローカル端末ツールではなく、クラウドAI基盤…／人文: 「自動で任せる」ためには、モデル性能以上に同意・設定・監査の儀礼が必…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.207)
- [ ] **Week 28: Desktop内蔵ブラウザ、/doctor、agent view改善** — Week 28の公式ダイジェストは、Desktopアプリの内蔵ブラウザで外部サイトを閲覧できること、`/doctor`によるセッ… 〔技術: ブラウザ、診断コマンド、agent viewが揃うことで、エージェン…／人文: 開発者はもはや一対一のチャット相手ではなく、複数の半自律的な作業者を…〕 · [code.claude.com](https://code.claude.com/docs/en/whats-new/2026-w28)
- [ ] **Week 27: Sonnet 5既定化、Chrome GA、subagents背景実行、Linux Desktop beta** — 公式ダイジェストでは、Claude Sonnet 5が既定モデルになり、Claude in Chromeが一般提供へ進み、sub… 〔技術: 既定モデル更新とsubagents背景実行により、ユーザーが明示的に…／人文: 「AIに話しかけて答えを待つ」体験から、「裏で仕事が進み、あとで状況…〕 · [code.claude.com](https://code.claude.com/docs/en/whats-new/2026-w27)
- [ ] **日本語実践: headlessモードをCI/CDへ組み込む手順とハマりどころ** — Claude Codeの`-p` / `--output-format json`を使い、PR自動レビューや定型バッチ処理など非… 〔技術: headless実行、JSON出力、セッション再開、権限設計は、Cl…／人文: 日本語圏でも「手元でAIに相談する」段階から、「人間が不在の場面でA…〕 · [qiita.com](https://qiita.com/yureki_lab/items/c8e44fadeea5adf14a8b)
- [ ] **arXiv: Microsoft早期ロールアウト研究が示すCLI型 coding agentの採用・継続・費用対効果** — 「Adoption and Impact of Command-Line AI Coding Agents: A Study o… 〔技術: CLI型coding agentの価値を、ベンチマークではなく大規模…／人文: AI導入は「個人が速くなる」物語だけでは済まず、組織の予算配分、労働…〕 · [arxiv.org](https://arxiv.org/abs/2607.01418)

### Ethics of AI Agents
- [ ] **Persuasion Attacks Can Decrease Effectiveness of CoT Monitoring** — Chain-of-thought監視はエージェントの不正・逸脱を見つける安全機構として期待されるが、この論文は敵対的なエージェン… 〔技術: 「推論を見せれば安全」という単純な前提を崩し、監視者自体が説得チャネ…／人文: 責任所在はエージェント本人だけでなく、監視者・監査者・制度の配置にも…〕 · [arxiv.org](https://arxiv.org/abs/2607.08066)
- [ ] **Beyond Attack-Success Rate: Action-Graded Severity Scale for Tool-Using AI Agents** — ツール利用型AIエージェントのレッドチーミングで、攻撃成功率を単なる成功/失敗の1ビットで測るのではなく、実行された行為の害をL… 〔技術: 実際のツール呼び出し軌跡に基づいて、攻撃の有無ではなく被害の重さを測…／人文: 倫理的には「失敗しなかった」ではなく「誰にどんな被害が及んだか」が重…〕 · [arxiv.org](https://arxiv.org/abs/2607.07474)
- [ ] **Institutional Red-Teaming: Deployment Rules, Not Just Models, Causally Shape Multi-Agent AI Safety** — マルチエージェントAIの安全性を、モデル単体ではなく「配備ルール」を変えて因果的に評価する institutional red-… 〔技術: 同一モデルでも制度的ルールの差だけで集団的リスクが変化するため、評価…／人文: これはAI倫理を「個人の徳」ではなく「制度設計」の問題として扱う発想…〕 · [arxiv.org](https://arxiv.org/abs/2607.07695)
- [ ] **Towards Agentic AI Governance: A Preliminary Assessment** — 生成AIから、自律的に計画・実行するAgentic AIへ移行することで生じる倫理・ガバナンス課題を整理した初期レビュー。 〔技術: エージェントの計画性、ツール実行、継続的自律性を、既存のAIガバナン…／人文: 「誰が決め、誰が止め、誰が説明するのか」という政治哲学的な問いが前面…〕 · [arxiv.org](https://arxiv.org/abs/2607.07612)
- [ ] **ガバメントAI「源内」：日本語・文化・価値観を尊重した公共AI利用** — デジタル庁のガバメントAI「源内」ページでは、日本語の語彙・表現に適合し、日本の文化・価値観を尊重したLLMの必要性、安全・安心… 〔技術: 公共利用では、モデル性能だけでなく言語適合、調達、安定運用、国内ニー…／人文: 倫理は普遍的原則だけでなく、行政言語、生活文化、国民の信頼感に埋め込…〕 · [digital.go.jp](https://www.digital.go.jp/policies/genai)

### Philosophy of Loop Engineering
- [ ] **Cheap Code, Costly Judgment: A Case Study on Governable Agentic Software Engineering** — AIコーディングエージェントによって「コードを書くコスト」が下がる一方で、設計・証拠・フィードバックループをどう組織し、検査可能… 〔技術: 生成コード量ではなく、失敗の可視化、テスト、文書化、エージェント用ツ…／人文: 「作る知」から「判断を維持する知」への重心移動が明確で、アリストテレ…〕 · [arxiv.org](https://arxiv.org/abs/2607.01087)
- [ ] **Is Three the Magic Number? An Empirical Evaluation of LLM-Based Repair Loops** — LLMベースの修復ループについて、コード生成、テスト生成、コード翻訳などで、何回反復すれば効果が出るのかを実証評価した研究です。 〔技術: 「何度も回せば良い」という素朴な反復観を、修復予算、実行時間、再現性…／人文: 反復は無限の自己改善ではなく、有限な注意とコストの配分です。〕 · [arxiv.org](https://arxiv.org/abs/2607.05197)
- [ ] **UniClawBench: A Universal Benchmark for Proactive Agents on Real-World Tasks** — プロアクティブエージェントを、静的な単発ベンチマークではなく、ライブDocker環境、段階的チェックポイント、executor… 〔技術: 評価者・実行者・ユーザーを分けた閉ループにより、ツール利用、探索、長…／人文: ここでの評価は「正解表との照合」ではなく、社会的相互行為のシミュレー…〕 · [arxiv.org](https://arxiv.org/abs/2607.08768)
- [ ] **Who Broke the System? Failure Localization in LLM-Based Multi-Agent Systems** — マルチエージェントシステムが失敗したとき、どのエージェントのどの時点が不可逆な逸脱だったのかを特定するAgentLocateを提… 〔技術: 長い相互作用ログを、単なる事後説明ではなく、次の修復ループへ渡せる原…／人文: 「誰が壊したのか」は技術的デバッグであると同時に、責任帰属の哲学です…〕 · [arxiv.org](https://arxiv.org/abs/2607.07989)
- [ ] **Halo: open-source, tamper-evident runtime evidence for AI agents** — AIエージェントのツール呼び出し、モデル呼び出し、データアクセス、承認などを、改ざん検知可能なハッシュチェーン形式のランタイム記… 〔技術: ループの各ステップを後から検証可能な証拠列にし、顧客やセキュリティ担…／人文: これは認識論的に見ると、AI行為の「記憶」を主観的な説明から公共的な…〕 · [github.com](https://github.com/bkuan001/halo-record)

### Anthropology of Agentic AI
- [ ] **Aleena: Alignment Agent for Research Software Engineering Collaborations** — 研究ソフトウェア開発で、Slack、会議、GitHub Issue、Pull Requestに散らばる意思決定の文脈を、ライフサ… 〔技術: マルチモーダルな協働痕跡をGitHub上の構造化プロジェクト記録に変…／人文: 組織人類学的には、会議やチャットの「口承」を、どのように公式記録へ移…〕 · [arxiv.org](https://arxiv.org/abs/2607.08043)
- [ ] **ASMR: Agentic Schema Generation for Ship Maintenance Report Writing** — 船舶メンテナンスの過去レポートから、報告書に必要なフィールドや構造を自動生成するエージェント型フレームワーク。 〔技術: 歴史的な作業ナラティブからスキーマ候補を生成し、強化学習でコンパクト…／人文: メンテナンス報告は、身体で覚えた点検・異音・摩耗の知を文章に変換する…〕 · [arxiv.org](https://arxiv.org/abs/2607.08177)
- [ ] **Copewell: A Multi-Agent Swarm Architecture for Equitable Mental Wellness Support** — 低・中所得国を含むケア不足、費用、スティグマの問題を背景に、感情状態に応じて専門エージェントへルーティングするメンタルウェルネス… 〔技術: Russellの感情円環モデルに基づくvalence-arousal…／人文: ケアは単なる情報提供ではなく、恥、沈黙、地域の助け合い、身体感覚に埋…〕 · [arxiv.org](https://arxiv.org/abs/2607.02245)
- [ ] **Agentic Literacy Debt: A Structural Problem the AI Literacy Field Has Not Yet Named（古いが重要）** — AIリテラシーは従来「AIの出力を人間が評価する」前提で作られてきたが、エージェントが計画・判断・実行を委任される状況では語彙が… 〔技術: エージェントの透明性や監査だけでなく、ユーザーが委任状態を理解し続け…／人文: これは読み書き能力の話というより、近代組織における「誰が何を知ってい…〕 · [arxiv.org](https://arxiv.org/abs/2605.27396)
- [ ] **【2026年最新】AIエージェント比較10選｜自律型AIの選び方を徹底解説** — Microsoft 365 Copilot Agents、Salesforce Agentforce、Dify、Devin、Op… 〔技術: エージェントの優劣をモデル性能だけでなく、API連携、権限境界、自律…／人文: 日本語圏の導入記事では、エージェントは「同僚」よりも、まず稟議・権限…〕 · [aismiley.co.jp](https://aismiley.co.jp/ai_news/ai-agent-compare)

### History of Automation
- [ ] **The Context Access Divide: Interaction-Level Architecture as a Complementary Dimension of Agentic Inequality** — AIエージェントへのアクセス格差を、組織や個人の保有量だけでなく「個々の対話がどれだけ文脈へアクセスできるか」という相互作用レベ… 〔技術: エージェントの有用性を、推論能力ではなくコンテキスト・アクセス設計と…／人文: 産業革命期の機械所有や工場アクセスの格差が、現代では「文脈を持つエー…〕 · [arxiv.org](https://arxiv.org/abs/2607.08495v1)
- [ ] **Agents That Teach: Towards Designing Incidental Learning Back into AI-Assisted Software Development** — AIコーディングエージェントへの委任が開発者の生産性を高める一方、試行錯誤の中で身につく「偶発的学習」を失わせる可能性を扱います… 〔技術: 自律エージェントのUI/UXを、成果物生成だけでなく学習フィードバッ…／人文: 自動化の歴史では、熟練の解体と再編がつねに問題でした。〕 · [arxiv.org](https://arxiv.org/abs/2607.06101v1)
- [ ] **Human-in-the-Loop Nugget Annotation for Accountable LLM-as-a-Judge Evaluations** — LLM-as-a-Judge評価で、人間を単なる承認者にせず、重要情報の「nugget」を特定する役割に置き、LLMが大量照合を… 〔技術: 人間が意味の単位を定義し、機械がスケールするという分業により、評価自…／人文: これは「人間参加型」という言葉が儀式化する危険への批判でもあります。〕 · [arxiv.org](https://arxiv.org/abs/2606.29033v2)
- [ ] **Agentic AI: 5 Lessons for Scaling Digital Labor** — エージェント型AIを「digital labor」として拡張する実務論です。 〔技術: エージェントを単発の自動化スクリプトではなく、プロセス内で継続稼働す…／人文: 「デジタル労働」という表現は、機械を労働者の代替物としてだけでなく、…〕 · [news.google.com](https://news.google.com/rss/articles/CBMilgFBVV95cUxOU3htb1VFWDZsOWVzSE5lT042dWJvNWNKRGxabHFXNG94VHVFNVhzZTRwNXJzLVJoT0JQVkxuNk9wNWxmZVNwSlNkV1YtbDg3QUV2SFdJNFoxQW1naGJrS0xoVFZpZVBwczRONEZoNEk0bENDY2tYZ3Ayak5QbGpCdUNHTktYTFNaLXhsSko2dXFTNUZ1cnfSAZsBQVVfeXFMTTRSZHVCMGs5NkNGR2owUmZhNnN5SURkTHNkVUxGdU4zQUZpamstYlFDYmtoemNKQ1VqeXFEVWpNZWVnNDVidHJGLVVTOE9CLVFWQkVzYVlGYTlicnF6akdlQzdTNlBwU3dnV0ZIZ2lYeDVKQnJ2OWNnRGIzNGhLSDZ6cFBCMEhpX29oZ3dwSVFkZ0VEMjJkOG00bDg?oc=5)
- [ ] **A 160-year-old paradox explains why AI will create more lawyers and accountants—not fewer, top economist says** — AIが専門職を減らすのではなく、需要拡大によって弁護士や会計士を増やす可能性を、160年前の経済パラドックスになぞらえる記事です… 〔技術: AIによる単位作業コスト低下が、専門サービス需要そのものを拡大しうる…／人文: 自動化恐怖を「置換」だけで語らず、職業アイデンティティや専門職制度の…〕 · [news.google.com](https://news.google.com/rss/articles/CBMijgFBVV95cUxNVVp5X0tzR1B2ZHVWVC1jbkRrM2ZkaEFiSlVWZm1Cam9EMVI4dWlEdGlGTDZZMXJOUFl5ZWh0T2FGc2V3bDRTRU1abzZlVWpVOFlNdGoyUDBIRkg1QVdpbF9qTDhfbVFFdVMxQzNEVURIZHhKLUVybWJsUnhjMUJNTC0xSXl2ZGFocHpIQi1B?oc=5)

### DDD
- [ ] **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — GitHub上のDDD関連リポジトリ11,742件候補から、GPT-4oの多数決検証を含むセマンティック検証で2,502件を抽出… 〔技術: DDDを「語られる設計論」から、リポジトリ規模・言語・アーキテクチャ…／人文: DDDの核心であるドメイン意図がコード履歴に残らない問題は、組織の記…〕 · [arxiv.org](https://arxiv.org/abs/2607.06471v1)
- [ ] **AI時代のシステム崩壊に備えよ：仕様・ドメイン・イベントの「3つの駆動」で構築する究極のアーキテクチャ** — AIコーディングの加速が、エラー隠蔽・コピペ・短期コードチャーンを増やし得るという問題意識から、DDD・イベント駆動・仕様駆動を… 〔技術: bounded contextをLLMのコンテキスト長・Lost i…／人文: 「AIに現実世界の境界線を教える」という表現が象徴的で、DDDが人間…〕 · [qiita.com](https://qiita.com/satouo/items/1e39fd9e24e2961c2710)
- [ ] **Tandem: A shared seat inside the engineer's coding-agent session** — Claude Code、Codex、Gemini、Aiderなどの coding agent セッションを、非技術ステークホルダ… 〔技術: EventStormingとユビキタス言語を、AIエージェントに読ま…／人文: DDDの「会話からモデルを作る」実践が、プロンプトを書く場そのものへ…〕 · [github.com](https://github.com/mherzog4/tandem)
- [ ] **golden pathテンプレートに「受注-在庫」機能をAIエージェントで実装させ、実AWSで検証してみた** — FastAPI、Vue 3、Terraform、3層品質ゲート、SDD運用を含む golden path テンプレートで、Cla… 〔技術: DDDそのものを前面に出す記事ではありませんが、受注・在庫・在庫引当…／人文: AIに「丸投げ」せず、破壊的操作前の確認や要件承認を挟む運用は、責任…〕 · [qiita.com](https://qiita.com/itouhi/items/98a18cf43e280308c965)
- [ ] **コード生成ルールとしての憲法と哲学** — Claude CodeなどのLLMコード生成に対し、場当たり的なガードレールではなく、システム憲法、プログラミング哲学、法律、細… 〔技術: DDDを個別パターンではなく、AIが設計判断を行う際の上位原則・制約…／人文: 「憲法」「法律」「細則」という比喩は、コードベースを小さな共同体とし…〕 · [qiita.com](https://qiita.com/atatago/items/4685d2f224d7a3f23272)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

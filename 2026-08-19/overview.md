# 📰 2026-08-19 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Gemini Notebookでノートブック全体のコピーが可能に · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/08/make-copy-of-notebook-in-gemini-notebook.html)
- **Loop engineering** — Designing Loops for Production-Grade Work · [liquid.ai](https://www.liquid.ai/blog/agent-loops)
- **AWS** — Amazon Bedrock AgentCore payments が一般提供開始 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale)
- **Harness engineering** — Claude Code 2.1.235: 権限ダイアログ、バックグラウンドクラウドセッション、SendMes… · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- **sharp LLM usage** — GPT-5 prompting guide · [cookbook.openai.com](https://cookbook.openai.com/examples/gpt-5/gpt-5_prompting_guide)
- **AI agent trends** — HarnessRouter: Claude Code / Codex / Hermes などを統一APIで動… · [github.com](https://github.com/HarnessRouter/harnessrouter)
- **Claude Code** — Boris Cherny: Claudeに日々のアプリ保守を任せる実験 · [news.google.com](https://news.google.com/rss/articles/CBMiXEFVX3lxTE1ZTUV6ZVhpWnUtX3ZxTGdSNkZZck5aM1NxQmRvR3JZcmZrUS0teU0tRmJ0elBrZThYQmt4SHZ3djVPOHE1SDNJTUxwR0Z0VU9wc2JQQWZTaXFPTkMy?oc=5)
- **Ethics of AI Agents** — Characterizing Agentic Flooding of Government Services · [arxiv.org](http://arxiv.org/abs/2608.16603v1)
- **Philosophy of Loop Engineering** — TRACE: TRajectory Attribution for Automated Context En… · [arxiv.org](https://arxiv.org/abs/2608.09153)
- **Anthropology of Agentic AI** — Microsoft 2026 Work Trend Index: Agents, human agency,… · [microsoft.com](https://www.microsoft.com/en-us/worklab/work-trend-index/agents-human-agency-and-the-opportunity-for-every-organization)
- **History of Automation** — The Anthropic Economic Index · [anthropic.com](https://www.anthropic.com/economic-index)
- **DDD** — Towards Standardized Evaluation in Automated Domain Mo… · [arxiv.org](https://arxiv.org/abs/2608.15255)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Gemini Notebookでノートブック全体のコピーが可能に** — Gemini Notebookユーザーは、コピー権限がある場合、ソースとStudioアイテムを含むノートブック全体をコピーできる… 〔技術: NotebookLMの単位が「個別ファイルの要約」から、権限・生成物…／人文: 教師が配布した教材を学生が自分用に改変したり、同僚が基礎ノートをプロ…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/08/make-copy-of-notebook-in-gemini-notebook.html)
- [ ] **Workspace StudioからGemini Notebookへソースを自動追加** — Workspace Studioに「Add a source to Gemini Notebook」ステップが追加され、テキスト… 〔技術: NotebookLMを手動投入型のRAGノートから、社内更新・授業資…／人文: 「最新情報を誰が入れ忘れたか」という運用負債を減らし、知識管理を個人…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/08/automatically-add-sources-to-your-Gemini-Notebooks-in-Workspace-Studio.html)
- [ ] **公式サイトが「Gemini Notebook」としてNotebookLMの継続性を明示** — 公式ページは、Gemini Notebookを「ソースを分析し、複雑な内容をわかりやすく整理して、コンテンツを進化させるAIリサ… 〔技術: 名称変更は単なるブランド整理ではなく、Geminiエコシステム内の調…／人文: 「ノート」という私的な思考の場が、GoogleのAIアシスタント群に…〕 · [notebooklm.google](https://notebooklm.google/?hl=ja)
- [ ] **日本語ビジネス向けに、料金・新機能・セキュリティまで含めた実践ガイドが更新** — 日本語記事として、2026年7月の名称変更、PDF・音声・YouTube動画の読み込み、要約・分析、音声解説やスライド資料作成、… 〔技術: 導入判断に必要な機能、制限、セキュリティ、Gemini本体との使い分…／人文: 日本企業では「便利そう」だけでは採用されにくく、責任範囲・契約・情報…〕 · [ntt.com](https://www.ntt.com/bizon/notebooklm.html)
- [ ] **議事録要約など、日本語の定型業務での使い方解説が増加** — 自分がアップロードした資料に基づいてAIと対話できる点、参照情報を手元資料に限定できる点、基本的な使い方、料金、ログイン、議事録… 〔技術: 会議録・社内資料・PDFなど、既存の非構造テキストを根拠付きで再利用…／人文: 議事録要約は単なる時短ではなく、会議で語られた曖昧な合意を後から検証…〕 · [biz.moneyforward.com](https://biz.moneyforward.com/ai/basic/927)

### Loop engineering
- [ ] **Designing Loops for Production-Grade Work** — Liquid AI は、実運用級の問題をコーディングエージェントに解かせた実験をもとに、agent loop を設計対象として扱… 〔技術: ループをプロンプト列ではなく、タスク分解、実行、検査、修正、成果物固…／人文: philosophy の観点では、これは「知能」を内部能力ではなく環…〕 · [liquid.ai](https://www.liquid.ai/blog/agent-loops)
- [ ] **What We Learned Moving Our Agent Loops from Anthropic to GLM** — Unblocked は、主要な agent loop の多くを Claude Opus から GLM 5.2 へ移した結果、トー… 〔技術: ループの費用対効果は「モデル単価」ではなく、ターン数、キャッシュ、ツ…／人文: ethics 的には、モデル乗り換えはコスト最適化だけでなく、品質低…〕 · [getunblocked.com](https://getunblocked.com/blog/moving-agent-loops-from-anthropic-to-glm)
- [ ] **Gartner: AI inference costs per agentic workflow will increase more than fivefold through 2028** — Gartner は、agentic workflow あたりの推論コストが2028年までに5倍超へ増えるという予測を発表した。 〔技術: ループエンジニアリングでは、停止条件、キャッシュ、軽量モデルへの委譲…／人文: history 的には、蒸気機関やクラウド計算と同じく、新しい自動化…〕 · [gartner.com](https://www.gartner.com/en/newsroom/press-releases/2026-08-17-gartner-predicts-ai-inference-costs-per-agentic-workflow-will-increase-more-than-fivefold-through-2028)
- [ ] **tracelint: a deterministic linter for AI agent traces** — tracelint は、ツール呼び出し型エージェントの実行トレースを読み、スキーマ違反、無視されたエラー、幻覚的な引数、ループ、… 〔技術: agent loop の品質保証を、最終回答の採点ではなく実行軌跡の…／人文: narrative の観点では、エージェントの「物語」は最終結果では…〕 · [github.com](https://github.com/AshwinUgale/tracelint)
- [ ] **When State Becomes an Attack Surface: State-Semantic Injection in LLM-Driven Embodied Agents** — LLM駆動の身体化エージェントでは、Webや文書だけでなく、環境状態そのものが攻撃面になりうることを扱う論文。 〔技術: ループ内の「状態」は単なる入力キャッシュではなく、次の計画と行動を制…／人文: philosophy 的には、エージェントの世界理解が外界の記号配置…〕 · [arxiv.org](https://arxiv.org/abs/2608.16806)

### AWS
- [ ] **Amazon Bedrock AgentCore payments が一般提供開始** — Amazon Bedrock AgentCore payments が GA となり、AI エージェントが有料 API、MCP、… 〔技術: エージェントの「ツール利用」に決済・予算・監査を組み込むことで、自律…／人文: これはソフトウェアが単に回答する存在から、限定された経済主体として振…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale)
- [ ] **Amazon DynamoDB がリアルタイム・ベクトル検索をネイティブサポート** — DynamoDB がネイティブのベクトル検索をサポートし、単一桁ミリ秒レイテンシー、99% 以上の recall、トリリオン規模… 〔技術: 既存の高スケール NoSQL データベースにベクトル検索が入ることで…／人文: 検索は「何を覚えているか」だけでなく「何を似ているとみなすか」を決め…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale)
- [ ] **AWS Lambda が Node.js 26 / Python 3.15 から Public Preview runtimes を導入** — Lambda に Public Preview runtimes という新しい仕組みが導入され、一般提供前の言語ランタイムを N… 〔技術: サーバーレスの言語ランタイム更新を、待つだけのイベントではなく、利用…／人文: クラウドプラットフォームと開発者コミュニティの関係が、完成品の配布か…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/compute/introducing-public-preview-runtimes-on-aws-lambda-starting-with-node-js-26-and-python-3-15)
- [ ] **Amazon EKS が Kubernetes control plane の高度な設定をサポート** — Amazon EKS で API server、scheduler、controller manager など Kubernet… 〔技術: マネージド Kubernetes の安全性を保ちながら、スケジューリ…／人文: マネージドサービスは「任せる」ための仕組みでしたが、成熟した組織ほど…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/containers/introducing-advanced-kubernetes-control-plane-configuration-in-amazon-eks)
- [ ] **AWS Bedrock LLM Day Japan 開催報告が公開** — 東京で開催された AWS Bedrock LLM Day Japan のレポートが公開され、Anthropic や OpenAI… 〔技術: Bedrock を中心に、モデル選択、セキュリティ、エージェント構築…／人文: 日本の企業コミュニティでは、生成AIの議論が「すごいモデル」から「組…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-bedrock-llm-day-japan%E3%80%90%E9%96%8B%E5%82%AC%E5%A0%B1%E5%91%8A%E3%80%91)

### Harness engineering
- [ ] **Claude Code 2.1.235: 権限ダイアログ、バックグラウンドクラウドセッション、SendMessage の堅牢化** — 2.1.235 では、権限ダイアログの表示と「今後確認しない」選択の意味が実際の許可範囲に揃うよう改善され、クラウドセッションの… 〔技術: エージェント実行ハーネスの中核である権限境界、イベントストリーム、ク…／人文: 「AIに任せる」ときの不安は、モデル性能だけでなく、どの権限を誰がい…〕 · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [ ] **Claude Code 2.1.232: subagent forking とセッション間メッセージングが標準化** — 2.1.232 では `subagent_type: "fork"` がデフォルトで有効化され、サブエージェントが会話履歴とプロ… 〔技術: ひとつの長い会話を人間が抱え込むのではなく、状態を継承した複数エージ…／人文: 開発作業が「孤独な操作者とツール」から「名前を持つ複数の作業者が連絡…〕 · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [ ] **Claude Code 2.1.224: self-hosted runner、archive plugin、cross-session SendMessage** — 2.1.224 では Team / Enterprise 向けに `claude self-hosted-runner` が追加… 〔技術: エージェントを SaaS 画面内の体験から、企業や個人が管理する実行…／人文: 自前 runner は単なるデプロイ機能ではなく、「AI は誰の場所…〕 · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [ ] **AppLooper: accountable release のための人間・コーディングエージェント・仮想ユーザーのループ** — AppLooper は、アプリ開発を「要求解釈、実装、ツール実行、評価、修復」の長期ループとして捉え、人間の owner、開発エ… 〔技術: 単発のコード生成ではなく、要求凍結、仮想ユーザーテスト、読み取り専用…／人文: 「リリース責任」を最後に人間へ戻す設計は、エージェント時代のプロダク…〕 · [arxiv.org](https://arxiv.org/abs/2608.14093)
- [ ] **SBCO: verifier-grounded harness optimization による計画エージェントの自己改善** — SBCO（Self-supervised Block Coordinate Optimizer）は、自己参照的にコードを書き換え… 〔技術: エージェント本体を直接進化させるのではなく、検証器とハーネス方策を最…／人文: 自己改変する AI という物語は強いが、実務では「何を許し、何を採点…〕 · [arxiv.org](https://arxiv.org/abs/2608.10157)

### sharp LLM usage
- [ ] **GPT-5 prompting guide** — GPT-5向けに、エージェント的タスク、指示遵守、API機能、フロントエンド/ソフトウェア開発でのプロンプト調整をまとめた実践ガ… 〔技術: 最新モデルでも、性能差はモデル単体ではなく「タスク分解、制約、ツール…／人文: LLM活用が文章術ではなく、仕事の依頼作法そのものを再設計する段階に…〕 · [cookbook.openai.com](https://cookbook.openai.com/examples/gpt-5/gpt-5_prompting_guide)
- [ ] **AI Product Playbook: prototype first, spec before code, test by contract, verify with your eyes** — Claude Code / Codex を日常的に使ったプロダクト開発から、プロトタイプ先行、仕様化してから実装、契約テスト、人… 〔技術: コーディングエージェントの出力を、仕様、テスト、目視検証、出荷ゲート…／人文: これは自動化万能論ではなく、AIに任せる部分と人間が責任を取る部分を…〕 · [github.com](https://github.com/painfulChen/ai-product-playbook)
- [ ] **AgentR: Stateful and Recovery-Aware Software Architecture for LLM-based Auditable Workflows** — LLMアプリを単なるステートレスなプロンプト応答ではなく、中間成果物、状態遷移、リトライ、孤児ジョブ検出、トークン費用ログ、価格… 〔技術: LLMの不確実性を「会話をやり直す」ではなく、永続状態、再試行、費用…／人文: 知的作業の自動化では、答えだけでなく「どの意図から、どの中間判断を経…〕 · [arxiv.org](https://arxiv.org/abs/2608.15264)
- [ ] **Catching Hallucinated Citations in Video-LLM Question Answering** — Video-LLMがタイムスタンプ付きで高信頼に見えるが実際には根拠のない主張を出す問題に対し、引用フレームを独立に再検査する自… 〔技術: LLM自身に同じ文脈で確認させるだけでは検証にならず、独立した観測表…／人文: タイムスタンプや引用は「信頼できそうな物語」を作る記号でもある。〕 · [arxiv.org](https://arxiv.org/abs/2608.15574)
- [ ] **MUSE: An Interactive Meta-Agent for Understanding and Steering LLM-powered Data Science Systems** — 自然言語でデータサイエンス作業を進めるエージェントの実行トレースを、ユーザーが理解・修正しやすい意味階層に再構成するメタエージェ… 〔技術: LLMワークフローの改善を、より大きなモデルに任せるのではなく、実行…／人文: これは「AIに作業させる」から「AIの作業過程を読んで共同編集する」…〕 · [arxiv.org](https://arxiv.org/abs/2608.16181)

### AI agent trends
- [ ] **HarnessRouter: Claude Code / Codex / Hermes などを統一APIで動かすセルフホスト型 agent harness** — HarnessRouter Community Edition は、Codex、Claude Code、Hermes など複数の… 〔技術: エージェント実行環境を「各CLIの個別操作」から「ハーネス間の標準プ…／人文: これはAIエージェントを個人の相棒から、組織内の労働インフラとして扱…〕 · [github.com](https://github.com/HarnessRouter/harnessrouter)
- [ ] **Agents Workbook: Claude Code / Codex の作業ノートをローカルで観察する実験** — Agents Workbook は、Claude Code や Codex へのリクエストに「作業ノートを書くためのツール」を追… 〔技術: エージェントの入出力だけでなく、計画・比較・却下した選択肢をセッショ…／人文: READMEが「推論を収穫するな」と明記している点が重要で、透明性へ…〕 · [github.com](https://github.com/softcane/agents-workbook)
- [ ] **When Agents Coordinate: Measuring Coordination in Multi-Agent AI Coding** — 複数のAI coding agent がプログラミング課題を解く際の「協調」を測定する研究。 〔技術: multi-agent coding の評価指標を、完了可否から通信…／人文: 人間組織で長く問題になってきた「調整コスト」が、AIチームにもそのま…〕 · [arxiv.org](http://arxiv.org/abs/2608.16801v1)
- [ ] **When State Becomes an Attack Surface: State-Semantic Injection in LLM-Driven Embodied Agents** — LLM駆動の embodied agent では、Webや文書だけでなく、環境状態そのものが攻撃面になるという問題を扱う論文。 〔技術: prompt injection をテキスト入力の問題に閉じず、環境…／人文: エージェントが物理世界や業務環境に入るほど、攻撃は言葉ではなく状況の…〕 · [arxiv.org](http://arxiv.org/abs/2608.16806v1)
- [ ] **Aident Loadout / aident-skill: エージェントに1,000超のアプリ連携と27,000超の実行アクションを渡すスキル** — Aident Loadout は、Gmail、Slack、Linear、Google Sheets、Notion、HubSpot… 〔技術: MCP/skills 的な拡張を通じて、エージェントの能力を「推論」…／人文: ここで問われるのは、AIが何を知っているかより、AIにどの鍵を渡すの…〕 · [github.com](https://github.com/Aident-AI/aident-skill)

### Claude Code
- [ ] **Boris Cherny: Claudeに日々のアプリ保守を任せる実験** — Google News RSSに「A weird experiment I've been trying the last fe… 〔技術: 単発のコード生成ではなく、既存アプリの保守・監視・修正依頼を継続ルー…／人文: 「開発者が書く」から「開発者が保守の儀式を設計する」へ役割が移り、チ…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiXEFVX3lxTE1ZTUV6ZVhpWnUtX3ZxTGdSNkZZck5aM1NxQmRvR3JZcmZrUS0teU0tRmJ0elBrZThYQmt4SHZ3djVPOHE1SDNJTUxwR0Z0VU9wc2JQQWZTaXFPTkMy?oc=5)
- [ ] **Auto mode標準化と複数セッション連携: Claude Codeが“同僚同士で話す”段階へ** — 公式Week 32では、Cross-session messaging、自社インフラでクラウドセッションを動かすSelf-hos… 〔技術: `ListAgents` / `SendMessage`によるセッシ…／人文: 人間がすべての確認を握るワークフローから、AI同士が状況を伝え、人間…〕 · [code.claude.com](https://code.claude.com/docs/en/whats-new/2026-w32.md)
- [ ] **2.1.235/2.1.234の細かな修正群: 実運用の摩擦を削るフェーズ** — 2.1.235ではプロンプト入力のspellcheck、言語サーバ切断時の全体プロンプトキャッシュ無効化修正、Markdown表… 〔技術: LSP、プロンプトキャッシュ、権限UI、リモート/デスクトップ連携、…／人文: 華やかな新機能より、誤操作・待ち時間・情報漏えいの不安を減らす改善が…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **Artifacts / `/design` 周辺: テキストではなく“見せる成果物”へ** — 公式Artifactsは、Claude Codeのセッション成果をclaude.ai上のライブなインタラクティブページとして共有… 〔技術: コード差分や調査結果をMarkdownログではなくHTML/CSS/…／人文: 開発者の仕事が「コードを書く」だけでなく、「他者に納得してもらう表現…〕 · [code.claude.com](https://code.claude.com/docs/en/artifacts.md)
- [ ] **日本語圏の実践: “一語足すだけ”で聞き返しを減らすプロンプト改善** — ライフハッカーの見出しとして「プロンプトに1語足すだけ。 〔技術: 実装能力の限界ではなく、要件提示の粒度や確認条件の設計でエージェント…／人文: 日本語での「察してほしい」依頼文化と、AIに明示的な完了条件を渡す文…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiqwFBVV95cUxQZmYxNmlyOW9VLWRBRzJPRWFRVXdIV3ZYdHUzQ2NLV1RxSTBMY2RrUFJ0MHdjUzBZeE4wV2VXVGlzY1ZFOXhlVG91RlFaOFl3SnZtZDNIaHR1bGFiaHo0N0gtbmtXR1FwZ0lFdlNBUzg3eDhfNzZqZlZhMmV2QzJxYl83OHMtVEFBSXp2Vm5pNUV4VTBRb1JPVFA5UEt0bEJIUEw2bFdfVlpLbEk?oc=5)

### Ethics of AI Agents
- [ ] **Characterizing Agentic Flooding of Government Services** — AIエージェントが給付申請、政策理解、意見提出を容易にする一方、行政サービスへの需要急増を起こす「agentic floodin… 〔技術: エージェントの大量代行が行政システムのスループット、本人性確認、優先…／人文: 「アクセスを民主化する技術」が同時に制度を詰まらせ、弱い立場の人ほど…〕 · [arxiv.org](http://arxiv.org/abs/2608.16603v1)
- [ ] **Mandato: Protocol-Level Enforcement of Digitally Signed Mandates on AI Agent Actions with Cryptographically Chained Audit Trails** — MCPのようなツール呼び出しプロトコルで、エージェントが何を・誰の代理で・どの条件下で実行できるかを、デジタル署名された「man… 〔技術: 権限管理をアプリ内ロジックではなくプロトコル層の検証可能な委任証明と…／人文: 「代理で動く」とは法的・社会的に何を意味するのかを、単なるAPIキー…〕 · [arxiv.org](http://arxiv.org/abs/2608.14074v1)
- [ ] **CompoSkill: Compositional Skill Chain Attacks from Individually Scanner-Passing LLM Agent Skills** — 自律エージェントが使うマーケットプレイス型スキルについて、個別スキャナを通過した安全なスキル同士でも、組み合わせると危険な攻撃連… 〔技術: 安全性評価の対象を「ノードとしての個別ツール」から「パスとしてのワー…／人文: 人間社会でも無害な役割の組み合わせが組織的な害を生むことがあるように…〕 · [arxiv.org](http://arxiv.org/abs/2608.16246v1)
- [ ] **Participatory Moral AI Is Not Neutral: The Invisible Hand of Developers** — 参加型の道徳選好収集は中立ではなく、開発者が特徴量の範囲、投票者サンプリング、質問文を決める段階ですでに規範的選択が入り込むと示… 〔技術: アライメントを投票・嗜好集約で済ませるのではなく、データ収集パイプラ…／人文: 「みんなの価値観を聞いたから公平」という物語の背後に、誰が問いを作り…〕 · [arxiv.org](http://arxiv.org/abs/2608.14522v1)
- [ ] **Quis custodiet ipsos custodes? / Who audits the AI agent?** — エージェントのガードレールを、エージェント自身のサンドボックス内ではなく、エージェントが到達できない境界の外側から観測・監査すべ… 〔技術: 監視者をエージェントの blast radius の外に置くという設…／人文: 「誰が監視者を監視するのか」という古典的な統治問題が、AIエージェン…〕 · [nofire.ai](https://www.nofire.ai/blog/who-audits-the-ai-agent)

### Philosophy of Loop Engineering
- [ ] **TRACE: TRajectory Attribution for Automated Context Engineering** — 本論文は、AIエージェントの失敗ログやユーザー修正・離脱などの軌跡から、プロンプト、知識ベース、ツール記述、手続き的スキルのどこ… 〔技術: 実運用エージェントのログを、単なるデバッグ材料ではなくコンテキスト設…／人文: これは「失敗から知る」認識論をソフトウェア運用へ移植する試みで、知識…〕 · [arxiv.org](https://arxiv.org/abs/2608.09153)
- [ ] **Agent Gym: A Framework for Continuous Evaluation and Evolution of LLM Agents Through Human-in-the-Loop Feedback** — 本論文は、デプロイ後にビジネスルールや例外が変化し続けるLLMエージェントに対し、人間のフィードバックを組み込んだ継続評価・行動… 〔技術: エージェント品質を単発ベンチマークではなく、ポストデプロイの継続的フ…／人文: human-in-the-loop は単なる安全弁ではなく、制度や業…〕 · [arxiv.org](https://arxiv.org/abs/2608.15591)
- [ ] **The CASE Framework: A Multi-Disciplinary Control Architecture for Governing Enterprise Agentic AI** — エンタープライズのエージェントAI統治を、単一のDevSecOps拡張ではなく、制御理論、複雑適応系、社会技術システムなど複数の… 〔技術: ガバナンスを抽象的ポリシーではなく、観測・フィードバック・制御対象の…／人文: サイバネティクスの古典的問いである「誰が何を観測し、どこへ戻すのか」…〕 · [arxiv.org](https://arxiv.org/abs/2608.10153)
- [ ] **Walk Before You Run: The Importance of Data Exploration for Data Analysis Agents** — LLMベースのデータ分析エージェントでは最終回答の正否だけが評価されがちだが、複雑なスプレッドシートやワークブックでは、解く前に… 〔技術: エージェントの成功条件を、回答生成だけでなく事前探索、スキーマ理解、…／人文: これは「走る前に歩け」という職人的実践知の復権であり、熟練者が対象を…〕 · [arxiv.org](https://arxiv.org/abs/2608.16045)
- [ ] **The Capability Ladder: A Curriculum-Modernization Framework for Workforce Readiness in the AI Era** — AI時代の教育・労働力準備を、trigger、automation、workflow、AI agent、agent team と… 〔技術: ループエンジニアリングを支える人的能力を、AI利用の成熟度と監督責任…／人文: 技術者像が、コードを書く主体から、自動化された行為を観察し、逸脱を解…〕 · [arxiv.org](https://arxiv.org/abs/2608.07779)

### Anthropology of Agentic AI
- [ ] **Microsoft 2026 Work Trend Index: Agents, human agency, and the opportunity for every organization** — Microsoftは、20,000人のAI利用労働者調査とMicrosoft 365の匿名化シグナルから、AIエージェントが「実… 〔技術: エージェント導入をモデル性能だけでなく、業務フロー、権限設計、マネー…／人文: 「人間の主体性」は抽象理念ではなく、誰が指示し、誰が承認し、誰が失敗…〕 · [microsoft.com](https://www.microsoft.com/en-us/worklab/work-trend-index/agents-human-agency-and-the-opportunity-for-every-organization)
- [ ] **Anthropic Economic Index report: Cadences** — Claude CodeやCoworkの成長により、Claude利用は単発チャットから長時間走るagentic taskへ変化して… 〔技術: エージェント利用ログを「会話内容」だけでなく、セッション長、時刻、出…／人文: “cadence”という語が示す通り、AIは職場の外部にある中立的自…〕 · [anthropic.com](https://www.anthropic.com/research/economic-index-june-2026-report)
- [ ] **How Agentic AI is Reshaping Workplace Culture / “digital colleagues”** — 記事は、agentic AIを「digital colleagues」と表現し、職場導入が生産性課題であると同時に、習慣・不安・… 〔技術: 自律的にタスクを進めるエージェントを、既存ツール導入ではなく、役割・…／人文: 「同僚」という比喩は、エージェントAIへの信頼・嫉妬・委任・監視感覚…〕 · [insights.economistenterprise.com](https://insights.economistenterprise.com/technology-innovation/what-the-rise-of-digital-colleagues-means-for-corporate-culture)
- [ ] **The team of tomorrow: agents, alignment, and team ritual** — AIエージェントが道具から「能動的な参加者」へ移る未来を、エンジニア、デザイナー、PM、カスタマーサポート、法務、プライバシー、… 〔技術: マルチロールのプロダクト開発にエージェントを入れると、権限、監査ログ…／人文: 「team ritual」という語が核心で、スタンドアップ、レビュー…〕 · [pendo.io](https://www.pendo.io/pendomonium/team-of-tomorrow-agents-alignment-team-ritual)
- [ ] **Agentic AI: A Comprehensive Survey of Architectures, Applications, and Future Directions** — Agentic AIの理論的系譜を、MDP/POMDP/BDI/SOARなどの記号的エージェントから、深層強化学習、LLM基盤、… 〔技術: 自律性、計画、環境認識、オーケストレーションといった構成要素を分解し…／人文: 人類学的には、技術文献が定義するagencyと、現場の人間が感じるa…〕 · [arxiv.org](https://arxiv.org/html/2510.25445v1)

### History of Automation
- [ ] **The Anthropic Economic Index** — Claude の利用ログを職業・地域・タスクの観点から集計し、AIが実際にどの経済活動へ浸透しているかを可視化するデータページ。 〔技術: モデル性能ベンチマークではなく実利用データから職業別AI利用を観測す…／人文: 産業革命期の工場統計やタイムスタディが労働を測定可能なものに変えたよ…〕 · [anthropic.com](https://www.anthropic.com/economic-index)
- [ ] **Generative AI and Jobs: A Refined Global Index of Occupational Exposure** — 2,861タスクについてAIモデル予測、専門家入力、Delphi型議論を組み合わせ、生成AIへの職業曝露を4段階で再推定した研究… 〔技術: タスク単位の自動化スコアを国際職業分類へ接続し、AIエージェントの導…／人文: 自動化の歴史では「機械に奪われる仕事」はしばしば階級・性別・地域で偏…〕 · [ilo.org](https://www.ilo.org/publications/generative-ai-and-jobs-refined-global-index-occupational-exposure)
- [ ] **Future of Work with AI Agents: Auditing Automation and Augmentation Potential across the U.S. Workforce** — AIエージェントが米国の職業タスクをどこまで自動化・拡張できるかを、技術的能力だけでなく労働者が望む自動化／望まない自動化と照合… 〔技術: エージェント能力評価を、タスク遂行可能性と人間の自律性・希望のミスマ…／人文: ラッダイト運動以来、自動化への抵抗は単なる反技術ではなく、熟練・尊厳…〕 · [arxiv.org](https://arxiv.org/abs/2506.06576)
- [ ] **Remote Labor Index: Measuring AI Automation of Remote Work** — 実際に経済価値のあるリモートワーク型プロジェクトを用い、AIエージェントがエンドツーエンドでどれほど仕事を自動化できるかを測るベ… 〔技術: 単発タスクではなく複数工程の実仕事を評価対象にすることで、エージェン…／人文: 自動化の歴史では、導入直後の機械はしばしば人間の段取り・保守・例外処…〕 · [arxiv.org](https://arxiv.org/abs/2510.26787)
- [ ] **Generative AI, the American worker, and the future of work** — 生成AIは従来の自動化が主に影響した定型的・ブルーカラー労働だけでなく、認知的で非定型な中高賃金職へも影響しうると論じる。 〔技術: LLMによるタスク遂行可能性を職業曝露と自動化可能性に分け、AIエー…／人文: 自動化の歴史は、生産性向上が自動的に労働者の幸福へ転化しないことを繰…〕 · [brookings.edu](https://www.brookings.edu/articles/generative-ai-the-american-worker-and-the-future-of-work)

### DDD
- [ ] **Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark** — 自動ドメインモデリングの比較評価に標準ベンチマークが不足している問題を扱い、Golden UML Modelset と Text… 〔技術: DDDのドメインモデル抽出をLLM任せの主観評価から、再現可能なベン…／人文: ドメインモデルは組織の世界理解を写すものなので、評価基準を公開するこ…〕 · [arxiv.org](https://arxiv.org/abs/2608.15255)
- [ ] **DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python** — SRS（要求仕様書）から型付きドメインモデルを作り、Pythonコードのアーキテクチャ逸脱をVS Code上で検出する、AI支援… 〔技術: DDDを設計時の会話で終わらせず、実装のドリフト検知と要求への根拠リ…／人文: 「アーキテクチャ違反」を誰が判断するのかという権力関係を、LLM・仕…〕 · [github.com](https://github.com/barandincoguz/DDD-Enforcer)
- [ ] **LLM_Ontology_DDD: Hybrid LLM–Ontology Approach for Ubiquitous Language** — 「A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous… 〔技術: LLMの柔軟な言語処理と、オントロジーの明示的な概念関係を組み合わせ…／人文: ユビキタス言語はチームの合意形成そのものなので、意味衝突の検出は単な…〕 · [github.com](https://github.com/BlayTeuR/LLM_Ontology_DDD)
- [ ] **Archally Blueprint Schema: domain-first YAML schema for system cartography** — ドメイン設計、意思決定記録、ビジネスルール、ガバナンス、アーキテクチャを1つのYAMLスキーマで表し、OpenAPI・Async… 〔技術: DDDの境界づけ・業務ルール・イベントストーミング成果を、AIエージ…／人文: 組織の「部族的記憶」をスキーマ化することは、属人化を減らす一方で、暗…〕 · [github.com](https://github.com/Archally/blueprint-schema)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — DDDを、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの特定、集約設計、技術アーキテ… 〔技術: イベントストーミングからアーキテクチャ設計までをプロンプト連鎖として…／人文: DDDのワークショップ的な対話をシミュレーション可能にする一方で、場…〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

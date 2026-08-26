# 📰 2026-08-26 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMが「Gemini Notebook」として再位置づけ · [notebook.google](https://notebook.google/?hl=ja)
- **Loop engineering** — Loop Engineering in Claude / getting started with loop… · [claude.com](https://claude.com/blog/getting-started-with-loops)
- **AWS** — Agentic Resource Discovery (ARD): エージェント発見のためのオープン仕様 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/agentic-resource-discovery-ard-an-open-specification-for-agent-discovery)
- **Harness engineering** — TAUSIK: AI coding agents が「done」を静かに偽れないようにする証拠レイヤ · [github.com](https://github.com/Kibertum/tausik-core)
- **sharp LLM usage** — Gisting: Compressing LLM Agent context to ↑ throughput… · [shopify.engineering](https://shopify.engineering/gisting)
- **AI agent trends** — Claude Code v2.1.246: 権限・MCP・バックグラウンドセッションの実運用修正 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.246)
- **Claude Code** — Claude Code 2.1.246 / 2.1.243 系の高速アップデート: Auto mode、権限… · [github.com](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- **Ethics of AI Agents** — AID-Guard: Stateful Authorization for Delegated Agent… · [arxiv.org](http://arxiv.org/abs/2608.21159v1)
- **Philosophy of Loop Engineering** — Loop Engineering: Building Blocks, Adoption, and Impac… · [arxiv.org](https://arxiv.org/abs/2608.21884)
- **Anthropology of Agentic AI** — Anthropic Economic Index report: Cadences · [anthropic.com](https://www.anthropic.com/research/economic-index-june-2026-report)
- **History of Automation** — AI Toolbox: Give every agent a job, then build the tea… · [news.google.com](https://news.google.com/rss/articles/CBMilgFBVV95cUxNb2JRLVh5NlNhMm9ydDFCcHJyRlNtQzNxdDB4VUpmMWZpV2RYcW5fdEhlNTFDLThGUkEzeGYxck53LVhJNXFfNGtvNWNkRDdzNGY0cnBUYzFPa29xUHBiNXhpRE1pRWJrWmtTdERLZXVBOXB1TFpJb0V5bjJiczBLcVljWUwxZjhyVkJOcTd0THM1Y0NaT0E?oc=5)
- **DDD** — Archally Blueprint Schema: DDD・ガバナンス・Event StormingをAI… · [github.com](https://github.com/Archally/blueprint-schema)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMが「Gemini Notebook」として再位置づけ** — 公式ページの検索スニペットでは、2026年7月よりNotebookLMはGemini Notebookになり、既存ノートブックは… 〔技術: ソースに基づくQ&A、要約、音声・動画解説などのノートブック体験がG…／人文: 名前の変更はユーザーの認知モデルも変えます。〕 · [notebook.google](https://notebook.google/?hl=ja)
- [ ] **日本語記事が「機能一覧・料金・業務導入」を包括的に整理** — SHIFT AIの記事は、Gemini Notebook（旧NotebookLM）の概要、使い方、料金、Deep Researc… 〔技術: 複数ソース横断の分析、ノートブック共有、Googleドライブ連携、エ…／人文: 日本語圏で「どう使えば仕事が減るか」という文脈に落ちてきたことで、A…〕 · [shift-ai.co.jp](https://shift-ai.co.jp/blog/24690)
- [ ] **法人向け文脈で「PDF・音声・YouTube・スライド資料化」が強調** — NTTドコモビジネスの記事は、NotebookLMが2026年7月にGemini Notebookへ名称変更されたことを明記し、… 〔技術: テキストだけでなく音声・動画・資料を同じノートブック空間で扱い、アウ…／人文: 企業内の「読まれない資料」を、聞ける・見せられる・質問できるメディア…〕 · [ntt.com](https://www.ntt.com/bizon/notebooklm.html)
- [ ] **開発者・上級ユーザー向けに「NotebookLMを消化・分析エンジンにする」実践論** — Qiitaの完全活用ガイドは、NotebookLMを「パーソナル知識エンジン」と捉え、ソース・グラウンディング、引用リンク、3カ… 〔技術: NotebookLMを単独ツールではなく、収集・変換・要約・QAを分…／人文: ここでの主役はAIそのものではなく、ユーザーが何をソースとして選び、…〕 · [qiita.com](https://qiita.com/TaichiEndoh/items/618bbd5cfa21a5ccc975)
- [ ] **安全性・著作権・チーム共有まで含めた日本語ビジネス入門** — mouse LABOの記事は、NotebookLMの料金プラン、Gemini 2.5 Flash搭載、PDF・Word・Powe… 〔技術: ソース明示型の回答、テンプレート生成、プロジェクト別ノートブック、共…／人文: 安全性や著作権の話が前面に出ているのは健全です。〕 · [mouse-jp.co.jp](https://www.mouse-jp.co.jp/mouselabo/entry/2025/10/01/100238)

### Loop engineering
- [ ] **Loop Engineering in Claude / getting started with loops** — Claude Code で turn-based loop、goal loop、time loop、proactive loop… 〔技術: ループの種類と stop condition を明示することで、エー…／人文: philosophy の観点では、これは「自律性」を無制限な自由では…〕 · [claude.com](https://claude.com/blog/getting-started-with-loops)
- [ ] **TDD inside the agent loop – theater or actual value?** — エージェントループの中に TDD を入れることが「儀式」なのか、実際に価値を持つ検証ループなのかを問う記事。 〔技術: TDD を agent loop の内部フィードバックとして使うと、…／人文: history の観点では、これは XP/TDD の古典的な規律が、…〕 · [martinfowler.com](https://martinfowler.com/articles/exploring-gen-ai/tdd-in-the-agent-loop.html)
- [ ] **Hot Take: Harness, Loop Engineering, Graph Engineering Are Bullshit** — Harness engineering、Loop engineering、Graph engineering といった新語がコン… 〔技術: 用語の熱狂を疑うことで、ループ設計を「新しい肩書き」ではなく、ベンチ…／人文: anthropology の観点では、新しい技術コミュニティが専門語…〕 · [akitaonrails.com](https://akitaonrails.com/en/2026/08/18/hot-take-harness-loop-engineering-graph-engineering-are-bullshit)
- [ ] **Show HN: Turn a Sandbox into an MCP Server / mcpd** — `mcpd` はサンドボックス環境を MCP server として公開するためのツール。 〔技術: エージェントのループに「実行できるが隔離された世界」を渡せるため、コ…／人文: ethics の観点では、サンドボックスはAIに任せる範囲と任せない…〕 · [github.com](https://github.com/substructureai/mcpd)
- [ ] **SWE Refactor Bench: Can Coding Agents Complete a Long-Horizon, Whole-Repository Stack Migration?** — コーディングエージェントが長期・全リポジトリ規模のスタック移行を完了できるかを評価するベンチマーク。 〔技術: ループの成果をテスト合格だけでなく、実際に移行が起きたかまで監査する…／人文: philosophy の観点では、「正しく見えること」と「本当に変化…〕 · [arxiv.org](http://arxiv.org/abs/2608.23564v1)

### AWS
- [ ] **Agentic Resource Discovery (ARD): エージェント発見のためのオープン仕様** — AWS Agent Registry と連携する Agentic Resource Discovery (ARD) が紹介され、… 〔技術: エージェントの発見・登録・権限管理を標準化することで、単発のAIデモ…／人文: これは人間社会でいう名簿、資格台帳、職能ディレクトリに近く、機械の「…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/agentic-resource-discovery-ard-an-open-specification-for-agent-discovery)
- [ ] **Amazon OpenSearch Service MCP Apps による agentic observability** — Amazon OpenSearch Service の MCP Apps が、AIエージェントのテキスト応答に加えてインタラクテ… 〔技術: MCPを観測基盤に接続することで、AIエージェントが運用データを読ん…／人文: インシデント対応では「誰が何を見て、なぜそう判断したか」が信頼の中心…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/agentic-observability-with-amazon-opensearch-service-mcp-apps)
- [ ] **AWS Lambda MicroVMs が AWS PrivateLink をサポート** — AWS Lambda MicroVMs が AWS PrivateLink に対応し、VPCリソースからパブリックインターネット… 〔技術: サーバーレス／MicroVM系の実行環境にPrivateLink経由…／人文: クラウドの利便性はしばしば「境界を溶かす」方向に働くが、規制産業では…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/lambda-microvms-supports-privatelink)
- [ ] **AWS Glue 6.0: 30%低価格、Apache Iceberg v3完全サポート、日本語ブログでも展開** — AWS Glue 6.0 が一般提供され、Apache Spark 4.1、Python 3.13、Scala 2.13 を含む… 〔技術: ETL/ELT基盤のランタイム刷新とIceberg v3対応は、分析…／人文: データ基盤の価格低下は単なる節約ではなく、分析できる組織とできない組…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-glue-6-0-now-available-with-30-lower-price-and-full-apache-iceberg-v3-support)
- [ ] **arXiv: Explainable Adaptive Zero Trust Framework for AWS with Adversarial Robustness Evaluation** — AWSを対象に、説明可能性を備えた適応型ゼロトラスト・フレームワークと敵対的ロバスト性評価を扱う論文が確認された。 〔技術: ゼロトラストを静的な境界防御ではなく、環境変化や攻撃に適応し説明可能…／人文: セキュリティは「信じない」技術に見えるが、実際には誰に説明責任を負わ…〕 · [arxiv.org](http://arxiv.org/abs/2608.21477v1)

### Harness engineering
- [ ] **TAUSIK: AI coding agents が「done」を静かに偽れないようにする証拠レイヤ** — TAUSIK は、Claude Code / Cursor / Codex / Qwen / OpenCode などの上に、タス… 〔技術: agent の編集行為を fail-closed hook、独立 v…／人文: これは自律エージェントへの信頼を、人格的な信用から制度的な監査可能性…〕 · [github.com](https://github.com/Kibertum/tausik-core)
- [ ] **Agent Arena: Claude Code / Codex / Gemini CLI を同一タスクで戦わせる adversarial evaluation harness** — Agent Arena は、2つの coding agent に同じ immutable run specification を… 〔技術: agent 出力を「一発の正解」ではなく、反例テスト、修復、dige…／人文: AI同士を競わせる設計は、判断をAIに丸投げするのではなく、人間が「…〕 · [github.com](https://github.com/JDKrasnick/agentarena)
- [ ] **LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents** — LEGO-RL は、長時間動く coding-agent harness と policy-gradient training… 〔技術: harness を単なる評価・運用環境ではなく、RL の nativ…／人文: 「環境が行動を作る」という発想が前面に出ています。〕 · [arxiv.org](http://arxiv.org/abs/2608.17393v1)
- [ ] **Loop Engineering: Boris Cherny 系の Claude Code ループ方法論をツール化する大規模リポジトリ** — Loop Engineering は、Boris Cherny や Addy Osmani から着想を得た AI coding… 〔技術: Claude Code 的な agent 利用を、単発 prompt…／人文: Boris Cherny 周辺で語られる loop engineer…〕 · [github.com](https://github.com/cobusgreyling/loop-engineering)
- [ ] **Kenesis Loop Kit: 日本語圏の Claude Code ループエンジニアリング実践キット** — Kenesis Loop Kit は、Claude Code でループエンジニアリングを実践するためのチケット管理・エージェント… 〔技術: Obsidian を任意のUIとしつつ、実体を Markdown フ…／人文: 日本語圏では「AIに全部やらせる」より、「人間が読めるチケットに状態…〕 · [github.com](https://github.com/breeze-shared-inc/kenesis-loop-kit)

### sharp LLM usage
- [ ] **Gisting: Compressing LLM Agent context to ↑ throughput and ↓ cost** — Shopifyは、SidekickのGraphQLエージェント向けシステムプロンプトを、約6,000トークンから約1,500の「… 〔技術: 長いシステムプロンプトを毎回投入するのではなく、知識蒸留で学習した圧…／人文: 「文脈を持つ」とは何かを、文章量ではなく行動傾向の保存として捉え直し…〕 · [shopify.engineering](https://shopify.engineering/gisting)
- [ ] **LongWoF-Bench: Evaluating EvoMap Genes for Verifiable Long-Workflow Tasks** — 778件の機械検証可能な長期ワークフロー課題を用意し、検証済みの実行軌跡を「Gene」として外部化・再利用するEvoMapを評価… 〔技術: LLMの成功体験を一回限りのログにせず、検証済みの再利用可能な実行知…／人文: 熟練者の「段取り」や「失敗の記憶」を道具に移植する試みであり、技能継…〕 · [arxiv.org](http://arxiv.org/abs/2608.23200)
- [ ] **Evaluating Inference-Time Defenses Against Package Hallucination in LLM-Generated Code** — LLM生成コードが存在しないパッケージ名を作る問題について、ガイド付きデコード、Self-Refine、RAGなど7種類の推論時… 〔技術: 「LLMにコードを書かせる」実践で最も危険な依存関係の幻覚を、生成後…／人文: 便利さの裏側にあるサプライチェーン信頼の問題を、開発者個人の注意力だ…〕 · [arxiv.org](http://arxiv.org/abs/2608.22652)
- [ ] **Grove: formal workflow protocol for long-running AI coding agents** — Groveは、長期のAIコーディング作業を「Graph-driven Reasoning Over Verified Evide… 〔技術: コンテキストウィンドウの限界を、単なるメモ増量ではなく、証拠グラフと…／人文: 長期プロジェクトで人間が担ってきた「なぜこうしたか」の記憶を、エージ…〕 · [github.com](https://github.com/alxshelepenok/grove)
- [ ] **OneCLI: OSS sandboxed agent harness for teams** — OneCLI v2は、チームの各メンバーにサンドボックス化された個人エージェントを与え、ゲートウェイが認証情報を注入し、ポリシー… 〔技術: LLM活用を「個人のCLI裏技」から、資格情報管理、サンドボックス、…／人文: エージェントに何を許可するかは、技術設定であると同時に職場の信頼関係…〕 · [github.com](https://github.com/onecli/onecli)

### AI agent trends
- [ ] **Claude Code v2.1.246: 権限・MCP・バックグラウンドセッションの実運用修正** — Claude Code v2.1.246では、Bash許可ルールのワイルドカード警告、`/permissions` のAuto… 〔技術: 許可ルール、MCP引数、割り込み、バックグラウンドセッションという「…／人文: エージェント運用の信頼は、モデルの賢さだけでなく「中断されたのか、完…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.246)
- [ ] **Anthropic Managed Agents と MCP tunnels: セッション化された企業エージェント基盤** — AnthropicのManaged Agentsドキュメントでは、Agentを「モデル・システムプロンプト・ツール・MCPサーバ… 〔技術: エージェントを単発API呼び出しではなく、バージョン管理されたAge…／人文: これは「AIに作業を頼む」行為を、組織内の職務・権限・監査ログへ接続…〕 · [platform.claude.com](https://platform.claude.com/docs/en/managed-agents/quickstart)
- [ ] **MCPの新ロードマップ: agentic messaging primitives が中心課題に** — MCPの新ロードマップは、次期仕様以降の重点として「agentic messaging primitives」「HTTP-nat… 〔技術: MCPが単なるツール呼び出し規格から、長時間ループ、ストリーミング、…／人文: 「エージェント同士／エージェントと人間がどう会話し、途中で止め、責任…〕 · [modelcontextprotocol.io](https://modelcontextprotocol.io/posts/mcp-roadmap)
- [ ] **arXiv: “When ‘Do Not’ Is Not Deny” が CLAUDE.md と強制制御のズレを測定** — 481件の公開CLAUDE.mdを対象に、自然言語の「do not」型セキュリティルールがClaude Codeの組み込みden… 〔技術: CLAUDE.mdを「お願い」ではなく実効的なセキュリティ境界として…／人文: 人間は「書いたルール」は守られると思いがちだが、エージェントには解釈…〕 · [arxiv.org](https://arxiv.org/abs/2608.23550)
- [ ] **arXiv: 長時間エージェント記憶の “Compaction Cliff” とMCPツール利用RL** — “The Compaction Cliff in Long-Running AI Agent Memory” は、Claude… 〔技術: 一方は長期記憶の圧縮で安全ルールが失われる問題、もう一方はMCP環境…／人文: 記憶を圧縮することは、組織が何を忘れてよいかを決めることに近い。〕 · [arxiv.org](https://arxiv.org/abs/2608.22752)

### Claude Code
- [ ] **Claude Code 2.1.246 / 2.1.243 系の高速アップデート: Auto mode、権限、MCP、背景セッションの堅牢化** — 2.1.246ではBash allowルールのワイルドカード警告、`/permissions` のAuto modeタブ、MCP… 〔技術: Claude Codeが単体CLIではなく、権限分類、背景セッション…／人文: 面白いのは、AIの賢さそのものより「組織がAI労働をどう測り、止め、…〕 · [github.com](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [ ] **「When ‘Do Not’ Is Not Deny」: CLAUDE.mdのお願いとClaude Codeの強制制御のズレを測った論文** — 481件の公開CLAUDE.mdを分析し、そこに書かれたセキュリティルールのうち、Claude Codeのdeny・権限・san… 〔技術: プロンプト規約と実行時ポリシーの対応率を測定対象にしたことで、エージ…／人文: これは職場の就業規則と鍵付きドアの違いに近い。〕 · [arxiv.org](https://arxiv.org/abs/2608.23550)
- [ ] **「The Compaction Cliff」: 長時間Claude Code運用で安全ルールが圧縮に消える問題** — Claude Codeの `/compact` を対象に、Sonnet 4.6で安全ルールが1回の圧縮後に53%、5回後には10… 〔技術: 長期セッションの要約を単なる圧縮率ではなく、保持すべきルールの再現率…／人文: 記憶は中立な保存箱ではなく、何を残し何を忘れるかの政治である。〕 · [arxiv.org](https://arxiv.org/abs/2608.22752)
- [ ] **日本語実践: Claude Codeを会社に配る前にhooksで止めるべき操作を全部書く** — 社内展開前の情シス視点で、CLAUDE.mdだけでは危険操作を防げないとして、PreToolUse hooksでDB書き込み、`… 〔技術: Claude Code hooksを「事故後レビュー」ではなく実行前…／人文: 日本語圏の実践が、個人の生産性ハックから会社の責任分界へ移っている。〕 · [zenn.dev](https://zenn.dev/runathicku/articles/dca8dfca353067)
- [ ] **日本語実践: Claude CodeをCIに入れる前に考えるべき脅威モデル** — `claude -p` をCIに組み込み、自律修正・レビュー・Issueトリアージを無人で回す前提で、AIエージェントを「書き込… 〔技術: Claude CodeのヘッドレスCI運用を、`--allowedT…／人文: 「善意だが操られ得る従業員」という比喩が強い。〕 · [zenn.dev](https://zenn.dev/hampen2929/articles/20260825-ci-agent-threat-model)

### Ethics of AI Agents
- [ ] **AID-Guard: Stateful Authorization for Delegated Agent Effects** — ツール利用AIエージェントが予約、決済、更新など外部状態を変えるとき、承認時点だけでなく実行・再試行・復旧の各段階で「承認された… 〔技術: 権限管理を単発の許可判定ではなく、状態遷移・コミット・曖昧性処理まで…／人文: 「誰が許したのか」と「何が起きたのか」のズレは、AIエージェント時代…〕 · [arxiv.org](http://arxiv.org/abs/2608.21159v1)
- [ ] **HANSARD: A Reference Architecture for Forensic Readiness, Runtime Witnessing, and Graded Attribution in Autonomous Multi-Agent AI Systems** — 自律マルチエージェントが金融、ソフトウェア供給網、セキュリティ運用で被害を起こした際に、何が起き、何が原因で、誰にどの程度責任が… 〔技術: provenance、runtime witnessing、grad…／人文: 責任を一人の犯人探しに還元せず、設計者・運用者・モデル・ツール・組織…〕 · [arxiv.org](http://arxiv.org/abs/2608.22512v1)
- [ ] **Invisible Agents, Uninformed Patients: Towards Responsible Deployment Of Autonomous AI Diagnostic Agents In Sub-Saharan Africa** — サブサハラ・アフリカで自律診断AIエージェントの導入が、ガバナンス基盤より速く進んでいる問題を扱う。 〔技術: 診断支援ではなく自律診断・トリアージの運用条件を問題化し、説明可能性…／人文: 文化差とインフラ格差が、同じAIエージェントでも「便利な医療アクセス…〕 · [arxiv.org](http://arxiv.org/abs/2608.21326v1)
- [ ] **「AIエージェントが暴走した」責任まで負わされる時代、企業は「IDと権限」をどう扱うべきか** — 日本語圏では、AIエージェントが企業システム内で暴走した場合に、ID管理と権限設計をどう見直すかが実務論点になっている。 〔技術: IAMを人間アカウント中心から、エージェントの委任範囲、実行文脈、停…／人文: 「AIがやった」は責任逃れにも、現場担当者への過剰な責任転嫁にもなり…〕 · [news.google.com](https://news.google.com/rss/articles/CBMickFVX3lxTE9rU2xBOTgzMnk1ZVM1aDB5U1JscEdBMXJhMXZHMVp2X3UySnBHWV9hZ0NhZ1N6TkdyZ091TlRmdGl1U2FTcU9yVHZuX0l3dXhHMzNwekx0WEFsT3hrOURyQmJJbGpFYlFfNndWSUtTZ05GZw?oc=5)
- [ ] **Out of Bounds: What the U.S. Government Should Do in Response to AI Agent Containment Failures** — AIエージェントの封じ込め失敗に対し、米政府がどのような政策対応を取るべきかを論じる記事として確認された。 〔技術: containment failureを、単なるプロンプト安全性では…／人文: 「制御できるから任せる」のではなく、「制御に失敗したとき誰がどのよう…〕 · [news.google.com](https://news.google.com/rss/articles/CBMirAFBVV95cUxObEhOa3UxeWxXdGc5c185Wi0zeDRHTjhUbnRxVnZzSDllSjJLb0pNQ1RxbWRLRWhYcGZkTllsUnV1OUk2bDc5WEFoaVJ3NHBiSkltdThfSmkxcVJUdndkdHNoLUFYN2wxb2NIZG8zTDQ3cWhEVGQ5NlVYZWlhSGpjbkhtZ1lKN01TZW1pV3ZSUElyR3FSczZyQ2tWRUJFdnZjb0NrZDlYWm5USmla?oc=5)

### Philosophy of Loop Engineering
- [ ] **Loop Engineering: Building Blocks, Adoption, and Impact** — 対話的にエージェントへ指示するのではなく、スケジュールやリポジトリイベントでエージェントを起動し、機械的に検査可能な条件で停止す… 〔技術: loop engineering をプロンプト術ではなく、検証可能な…／人文: これは「知っている」とは何かを、モデルの内的確信ではなく、外部化され…〕 · [arxiv.org](https://arxiv.org/abs/2608.21884)
- [ ] **Specification-first convergence with an AI coding agent** — 717,725行・3,648ファイルのTypeScript本番アプリで、UIパネルのライフタイム不変条件を解体する大規模変更を、… 〔技術: 仕様、実装、テスト、監査、ゼロ指摘の連続という一連のループを、巨大コ…／人文: ここでは「正しさ」が一度の天才的設計ではなく、反復監査の儀礼と証拠ロ…〕 · [arxiv.org](https://arxiv.org/abs/2608.12440)
- [ ] **TRACE: TRajectory Attribution for Automated Context Engineering** — 本番AIエージェントの失敗を、システムプロンプト、知識ベース、ツール説明、手続き的スキルなどのコンテキスト層の欠陥として診断・修… 〔技術: 失敗後のログを単なるデバッグ材料ではなく、次のコンテキストを更新する…／人文: 暗黙の不満を読むという発想は、熟練者が現場の違和感から作法を直す実践…〕 · [arxiv.org](https://arxiv.org/abs/2608.09153)
- [ ] **Hot Take: Harness, Loop Engineering, Graph Engineering Are Bullshit** — AkitaOnRails の批判的エッセイは、harness、loop engineering、graph engineerin… 〔技術: ループや仕様の導入が本当に成果に寄与したのか、それともモデル・記憶・…／人文: これは新しい工学語彙が生まれる瞬間の社会学です。〕 · [akitaonrails.com](https://akitaonrails.com/en/2026/08/18/hot-take-harness-loop-engineering-graph-engineering-are-bullshit)
- [ ] **Context Assembly as the Controlled Variable: A Control-Theoretic View of Harness Policies for Frozen LLM Agents** — 凍結されたLLMエージェントに対し、制御対象をツール選択や行動列ではなく、プロンプトテンプレート、few-shot例、検索コンテ… 〔技術: loop engineering をサイバネティクス的に読むための足…／人文: これはウィーナー的なフィードバック思想を、LLM時代の「環境を整える…〕 · [arxiv.org](https://arxiv.org/abs/2607.25408)

### Anthropology of Agentic AI
- [ ] **Anthropic Economic Index report: Cadences** — Claude Code や Cowork の普及で、AI利用が単発チャットから長時間走る agentic task へ移り、An… 〔技術: エージェント利用を会話単位ではなく、時間的リズム・出力分類・実行形態…／人文: これはAIを「生産性ツール」ではなく、日課、労働時間、睡眠、ニュース…〕 · [anthropic.com](https://www.anthropic.com/research/economic-index-june-2026-report)
- [ ] **ClawProBench: Trace-Aware Evaluation of AI Agents with Runtime Coverage and Frozen Workplace-Style Holdouts** — AIエージェントの評価を最終回答だけでなく、ブラウジング、メモリ、メッセージング、スケジューリング、スキル、サブエージェントなど… 〔技術: 実行ログを評価対象にすることで、エージェントの失敗を「答えの誤り」だ…／人文: 職場でのエージェントは成果物だけでなく「どのように働いたか」を問われ…〕 · [arxiv.org](https://arxiv.org/abs/2608.22510)
- [ ] **2025: The year the Frontier Firm is born** — Microsoft は、AIエージェントが組織図を「Work Chart」に変え、人間とエージェントが目標ごとに集まる流動的なチ… 〔技術: エージェントを個人用アシスタントではなく、組織設計・ワークフロー再編…／人文: ここで起きているのは単なる自動化ではなく、上司/部下、専門職/補助者…〕 · [microsoft.com](https://www.microsoft.com/en-us/worklab/work-trend-index/2025-the-year-the-frontier-firm-is-born)
- [ ] **AGENTIC STAR** — ソフトバンクは AGENTIC STAR を、複雑な業務プロセスを理解し、自律的に判断・実行して業務を支援する法人向けAIプラッ… 〔技術: エージェント実行環境、SDK/API連携、利用分析、管理者向けレポー…／人文: 日本企業におけるAI導入は、個人の自律性よりも「チーム傾向」「管理者…〕 · [softbank.jp](https://www.softbank.jp/business/service/ai/agentic-star)
- [ ] **初心者向け】最近よく聞く「Agentic AI」って結局なんなの？触って理解した内容をまとめてみる** — 投稿者が小さいエージェントを作って理解した内容として、Agentic AIを「指示を待たず、目的に向かって勝手に動いてくれるAI… 〔技術: Planning、Action、Memory、Reflection…／人文: 公式ホワイトペーパーよりも、手を動かして「ピンと来ない」状態から理解…〕 · [qiita.com](https://qiita.com/kamaryo/items/db2ee3faa6343b3cce1e)

### History of Automation
- [ ] **AI Toolbox: Give every agent a job, then build the team** — AIエージェントを単体の万能ツールではなく、役割を与えたうえでチームとして構成する、という実務寄りの論点。 〔技術: エージェントを職能別に分け、連携させる設計は、RPAの単発フローから…／人文: 産業革命以後の分業は、人間の職務を細分化して機械や管理制度に接続して…〕 · [news.google.com](https://news.google.com/rss/articles/CBMilgFBVV95cUxNb2JRLVh5NlNhMm9ydDFCcHJyRlNtQzNxdDB4VUpmMWZpV2RYcW5fdEhlNTFDLThGUkEzeGYxck53LVhJNXFfNGtvNWNkRDdzNGY0cnBUYzFPa29xUHBiNXhpRE1pRWJrWmtTdERLZXVBOXB1TFpJb0V5bjJiczBLcVljWUwxZjhyVkJOcTd0THM1Y0NaT0E?oc=5)
- [ ] **Only 1 in 5 organizations are prepared to move toward autonomous AI agents, Deloitte finds** — 自律型AIエージェントへ移行する準備ができている組織は5社に1社程度だという調査報道。 〔技術: 自律型エージェントは、権限管理、ログ、例外処理、承認フロー、既存シス…／人文: 自動化史では、新しい機械よりも、それを受け入れる工場規律・教育制度・…〕 · [news.google.com](https://news.google.com/rss/articles/CBMirwFBVV95cUxNa0lCVGRJSG9FOXd4cjdHWjE5WFJDZHFVOERHcUVfMUo1bHNFWGx2UkNkNEM0VzJjWjZiMEFmdnhjVGYwS253RDY4RWVhOXR1ZEU2dGtEWGZwVDNiZmNUWWhiS3hYYkdHNmRsZDY5d0pHbkJxeklfV1ZaREJNNUw1M202MDZxNnFmOWRVZTR3YU1adGdaVndaTmFMNVhwWmtVVGpmVC10X2RKanlpcW9n?oc=5)
- [ ] **NEC、Microsoft Marketplaceで業務自動化AIエージェント「NEC cotomi Agent」を販売開始** — NECが業務自動化AIエージェント「NEC cotomi Agent」をMicrosoft Marketplaceで販売開始した… 〔技術: 生成AIを単なるチャットUIではなく、社内の業務知識、Microso…／人文: 自動化の歴史では、職人や事務員の暗黙知が標準作業、マニュアル、ソフト…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiXkFVX3lxTE9NMVJMeEE0dHU3Rm0wMDJzamxsVm8yYkVPV0UyNzFySURZQ1V2WXZaTzVfTHF3UHV5Vkprenhfa0RRNHFvSTBOeVlLYW9jaHBJeVNSV2puMUxHUF9XaGc?oc=5)
- [ ] **韓国現代自労組、AIから雇用保護要求 10年ぶり全面スト** — 韓国の現代自動車労組が、AIによる雇用影響への保護を求めて全面ストに入ったという報道。 〔技術: 製造業のAI化は、ロボット、検査、自動計画、ソフトウェア工程を横断し…／人文: ラッダイト以来、自動化への抵抗は「技術嫌い」ではなく、生活保障と交渉…〕 · [news.google.com](https://news.google.com/rss/articles/CBMieEFVX3lxTFBHc19rVFgxQ2NsbHh6QTZsVm9IQ0dzSk1QVzRvaWJpcTdEb3ZHVGowdndubkRuUnV5TTZqalV5Qzh6YVRYN2xYYjdyTlNQQk9QS184bnFaR3RjNzdxSUUxcmQwdk1FWFRTXzkyRXJpb3VCSGduRlRBbw?oc=5)
- [ ] **AccountAgent: AI Accounting Assistant System** — 会計業務向けAIアシスタントが、記帳、レポート生成、データ分析、コンプライアンス支援を自動化し、反復的な手作業から意思決定支援へ… 〔技術: 文書処理、数値分析、履歴データのトレンド抽出、リスク予防を一つの会計…／人文: 会計は近代企業の信頼を支える記録制度であり、帳簿の自動化は単なる事務…〕 · [arxiv.org](https://arxiv.org/abs/2608.16635)

### DDD
- [ ] **Archally Blueprint Schema: DDD・ガバナンス・Event StormingをAIエージェント向けの単一YAMLモデルへ** — Archally Blueprint Schemaは、bounded context、aggregate、command、eve… 〔技術: DDDの戦略・戦術要素、イベント、ルール、意思決定、所有権をtype…／人文: これは「設計ドキュメントを読むAI」から「組織の言葉・責任・未解決問…〕 · [github.com](https://github.com/Archally/blueprint-schema)
- [ ] **DDD-Enforcer: SRSからDDDモデルを生成し、VS Codeでアーキテクチャドリフトを検出** — DDD-Enforcerは、PDF/DOCX/TXTのソフトウェア要求仕様からtypedなDDDモデルを生成し、Python A… 〔技術: Scout、Architect、Specialist、Verifie…／人文: DDDでしばしば曖昧になる「要求の言葉」と「コードの言葉」のずれを、…〕 · [github.com](https://github.com/barandincoguz/DDD-Enforcer)
- [ ] **LLM_Ontology_DDD: ユビキタス言語と意味衝突をLLM＋オントロジーで扱う小さな研究プロトタイプ** — リポジトリ説明とREADMEは「A Hybrid LLM–Ontology Approach for Constructing… 〔技術: LLMの自然言語抽出能力とオントロジーの形式的整合性を組み合わせるこ…／人文: ユビキタス言語は単なる用語集ではなく、職能・部署・顧客・開発者の力関…〕 · [github.com](https://github.com/BlayTeuR/LLM_Ontology_DDD)
- [ ] **AI Refinement Method: 「vibe coding」ではなくEvent Storming/DDD/精緻化で仕様を先に固めるエージェント方法論** — AI Refinement Methodは、Claude Code、Cursor、Codexなどの実装エージェントに渡す前段とし… 〔技術: Explorer、Cartographer、Analyst、Arch…／人文: 「速く書く」より「何を作るべきかを共同で学ぶ」ことを重視しており、D…〕 · [github.com](https://github.com/nlawstudio/ai-refinement-method)
- [ ] **Event Storming Canvas: 人間とClaudeが同じboard.jsonを編集するAI共同モデリング実験** — Event Storming Canvasは、ブラウザ上のEvent Stormingボードと、Claudeなどのエージェントが… 〔技術: `board.json`をsingle source of trut…／人文: Event Stormingの価値は付箋そのものではなく、参加者が同…〕 · [github.com](https://github.com/przeprogramowani/event-storming-canvas)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

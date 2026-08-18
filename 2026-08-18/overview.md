# 📰 2026-08-18 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Gemini Notebookでノートブック全体をコピー可能に · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/08/make-copy-of-notebook-in-gemini-notebook.html)
- **Loop engineering** — neal: planner / coder / reviewer を分けるローカル multi-agent… · [github.com](https://github.com/navels/neal)
- **AWS** — Amazon Bedrock AgentCore の Runtime instances が本番AIエージェ… · [aws.amazon.com](https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore)
- **Harness engineering** — HarnessRouter Community Edition と Unified Harness Prot… · [github.com](https://github.com/HarnessRouter/harnessrouter)
- **sharp LLM usage** — Agent Skills Can Be Harmful: スキルがエージェントを壊す失敗帰属研究 · [arxiv.org](http://arxiv.org/abs/2608.11888)
- **AI agent trends** — HarnessRouter: Unified interface for agent harnesses · [github.com](https://github.com/HarnessRouter/harnessrouter)
- **Claude Code** — Claude Code v2.1.234: 利用上限リセット後の自動再開、GitLab MRバッジ、メールア… · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.234)
- **Ethics of AI Agents** — No One to Blame: A Framework of Constitutive AI Unacco… · [arxiv.org](http://arxiv.org/abs/2608.12104)
- **Philosophy of Loop Engineering** — LoopsBench: From Harness Engineering to Loop Engineeri… · [arxiv.org](https://arxiv.org/abs/2608.00267)
- **Anthropology of Agentic AI** — A Framework for Agentic AI and Work Redesign: Executiv… · [news.google.com](https://news.google.com/rss/articles/CBMikgFBVV95cUxQNFBsVUc0UWs2a3BxZ1lIQVVXQUFSX1dGMUV4N2V1cG56c1pjOVRNaURrNFAzeXpxQW1mZVVHTkZJRmlGV01rX0ZrdElqTi1LTnZoQl9TMWUwcTViX2MxdGh3ZHAyTDdDaHcwM3ZPV3ItdHBxZjA3ckhHWGlGaXRSdlJXSzYtSktjYmhWTTBOTmhaZw?oc=5)
- **History of Automation** — Agentic profiles for effective AI governance · [doi.org](https://doi.org/10.1038/s41586-026-10805-z)
- **DDD** — Agentic Domain-Driven Mainframe Modernization / Projec… · [github.com](https://github.com/pmilet/ai-ddd-mainframe-modernization-patterns)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Gemini Notebookでノートブック全体をコピー可能に** — Gemini Notebook ユーザーが、権限を持つノートブックについて、ソースと Studio アイテムを含めて丸ごとコピー… 〔技術: NotebookLM の成果物が「一回限りの生成」ではなく、権限管理…／人文: 教師が配った教材ノートを学生が自分の学習ノートへ分岐させる、同僚が基…〕 · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/08/make-copy-of-notebook-in-gemini-notebook.html)
- [ ] **Workspace StudioからGemini Notebookへソースを自動追加** — Workspace Studio のワークフロー部品として「Add a source to Gemini Notebook」が追… 〔技術: NotebookLM が RAG 的な読解インターフェースに加えて、…／人文: 人間が「何を読むか」を毎回選ぶ作業の一部が自動化されるため、知識の入…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/08/automatically-add-sources-to-your-Gemini-Notebooks-in-Workspace-Studio.html)
- [ ] **Gemini内の「notebooks」でプロジェクト管理・学習管理へ拡張** — Google News RSS では、Google 公式ブログ記事「Try notebooks in Gemini to eas… 〔技術: Notebook がチャットとは別の永続的な作業単位として Gemi…／人文: AIとの関係が、その場の質問応答から、長く付き合うノート・プロジェク…〕 · [news.google.com](https://news.google.com/rss/articles/CBMid0FVX3lxTE13MGtzOEJRb3NMNk4zLXJDZnl3Qll2Q254bUtJYk4zZGFpWVJCNWVsekpHZy1ZVGRwRThtanh3UXpkWW9BeHhDR19jUjNPT0dNYjExNVpDSXBuWlVLNXF5T0pvRVphaTRZLWhtSnlQSWwyTTZoMVow?oc=5)
- [ ] **日本語圏での実践記事が増加：活用事例、商用利用、スマホ利用、勉強法** — 日本語圏では、SHIFT AI の「活用事例18選」「スマホで使う方法」「勉強法6選」、ライフハッカーの使い方解説、エクサウィザ… 〔技術: 機能発表そのものよりも、モバイル利用、社内資料、学習、商用利用の制約…／人文: 日本語記事の増加は、AI研究補助が一部の英語圏アーリーアダプターから…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiSkFVX3lxTE5oOElFbmpia1JkUXpIQ1Vla3htOG1KLTJhV0xTblVzcjdGcjBpX3ppa2wydEkyaDRKYUlJS2l6QlQ2bVR6SjNNTXBn?oc=5)
- [ ] **古いが関連: UXリサーチのPoint of View作成にNotebookLMを使うケーススタディ** — arXiv:2605.31125「Generative AI in developing User Experience Res… 〔技術: NotebookLM を単なる文書要約ではなく、複数資料から意思決定…／人文: UXリサーチにおける「ユーザーの声」は、要約されるほど扱いやすくなる…〕 · [arxiv.org](https://arxiv.org/abs/2605.31125)

### Loop engineering
- [ ] **neal: planner / coder / reviewer を分けるローカル multi-agent coding loop** — neal は、planner、coder、reviewer を別ロールとして動かし、計画をスコープに分割して実装・レビュー・最終… 〔技術: ループの単位を「1プロンプト」ではなく、plan → scoped…／人文: philosophy の観点では、これは「判断主体」を単一の知能では…〕 · [github.com](https://github.com/navels/neal)
- [ ] **Substructure: TOML と webhook で agent loop を外部システムから制御するエンジン** — Substructure は、クラウドまたはセルフホストで動くエージェント実行エンジンで、`substructure.toml`… 〔技術: loop の中身を black box にせず、decision p…／人文: anthropology の観点では、エージェントが「個人のラップト…〕 · [substructure.ai](https://substructure.ai)
- [ ] **HyperProbe: 本番障害を read-only probe で閉じる AI on-call loop** — HyperProbe は、PagerDuty、Datadog、Slack などのアラートを起点に、ログ・トレースを読み、疑わしい… 〔技術: 観測不足のまま推論を続けるのではなく、loop の途中で「本番から追…／人文: ethics の観点では、本番環境に入る AI の権限を read-…〕 · [hyperprobe.co](https://www.hyperprobe.co)
- [ ] **Armature: MCP / Claude Connector / ChatGPT App の利用セッションを eval に変換する loop** — Armature は、ユーザーが Claude、ChatGPT、MCP 経由でプロダクトをどう使ったかをセッションとして捕捉し、… 〔技術: 実ユーザーの agent session を評価データに戻すことで、…／人文: anthropology の観点では、人間がエージェント越しに製品を…〕 · [armature.tech](https://armature.tech)
- [ ] **Second Thought: ReAct の待ち時間に並列推論を走らせる agent loop 研究** — 論文 “Second Thought: Reasoning in Parallel as LLM Agents Act and… 〔技術: loop の逐次性を前提にせず、環境待ちの空白を speculati…／人文: philosophy の観点では、「行為しながら考える」だけでなく「…〕 · [arxiv.org](http://arxiv.org/abs/2608.13667v1)

### AWS
- [ ] **Amazon Bedrock AgentCore の Runtime instances が本番AIエージェント向け永続コンピュートを提示** — AgentCore Runtime instances は、最大14日まで持続する共有セッション、GPU アクセラレーション、ア… 〔技術: エージェントの計算・状態・デプロイ単位を Bedrock 側に寄せる…／人文: 「AIに依頼する」体験が、チャットの一問一答から、数日間同じ作業場に…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore)
- [ ] **Bedrock AgentCore payments と OpenClaw による「支払い可能なエージェント」実装** — OpenClaw エージェントに `@aws/aws-agents-pay` プラグインを導入し、Bedrock AgentCo… 〔技術: エージェントの外部行動に「支払い」という副作用を組み込むため、認可、…／人文: ソフトウェアが財布を持つ瞬間、便利さと同時に「委任の境界」が社会的テ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/build-openclaw-agents-that-transact-with-amazon-bedrock-agentcore-payments)
- [ ] **Amazon Bedrock が OpenAI モデル向け Cross Region Inferencing と API 対応を拡大** — Bedrock の OpenAI モデル利用で、Geo/Global の Cross Region Inferencing が追… 〔技術: リージョン内・地理範囲・グローバルの推論経路を選べるため、レイテンシ…／人文: 生成AIが国境をまたぐクラウド資源として運用されるほど、「データはど…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-cross-region-openai-v2)
- [ ] **AWS Lambda が Node.js 26 / Python 3.15 の Public Preview runtimes を開始** — Lambda は従来の GA ランタイム提供だけでなく、Node.js 26 と Python 3.15 を皮切りに Publi… 〔技術: 早期ランタイム検証により、破壊的変更への備え、ライブラリ互換性確認、…／人文: 開発者コミュニティがクラウド基盤の完成品を待つだけでなく、言語とプラ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/compute/introducing-public-preview-runtimes-on-aws-lambda-starting-with-node-js-26-and-python-3-15)
- [ ] **日本語事例: JCRファーマが Claude Code on AWS を創薬研究・業務へ導入** — JCRファーマは、Amazon Bedrock 経由で Claude Code を導入し、研究部門を含む業務でAIエージェント活… 〔技術: Claude Code を Bedrock 経由で使うことで、エージ…／人文: 創薬のように社会的影響と機密性が大きい領域で、AIエージェントは単な…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/jcrpharm-claude-code-on-aws)

### Harness engineering
- [ ] **HarnessRouter Community Edition と Unified Harness Protocol** — HarnessRouter は Claude Code、Codex、Hermes などの agent harness をセルフホ… 〔技術: 複数の coding agent を「モデル」ではなく「harnes…／人文: エージェント利用が個人の職人芸から組織の運用インフラへ変わると、誰が…〕 · [github.com](https://github.com/HarnessRouter/harnessrouter)
- [ ] **Boris Cherny の「検証が最重要」という Claude Code 観** — Boris Cherny は、難しいタスクを Claude に渡す技術は prompt engineering よりも「作業の途… 〔技術: Harness engineering の核心が、モデルへの依頼文で…／人文: これは「AI に任せる」と「AI を監督する」の間にある新しい仕事の…〕 · [daringfireball.net](https://daringfireball.net/linked/2026/08/02/cherny-claude-swift)
- [ ] **GitHub Copilot agentic harness の性能・効率評価** — GitHub は Copilot の agentic harness を、公開ベンチマーク、社内ベンチマーク、実運用メトリクス、… 〔技術: harness の優劣をモデル性能から切り離し、ツール選択、MCP、…／人文: 開発現場で「AI が賢いか」を語るだけでは不十分になり、「どの制度・…〕 · [github.blog](https://github.blog/ai-and-ml/github-copilot/evaluating-performance-and-efficiency-of-the-github-copilot-agentic-harness-across-models-and-tasks)
- [ ] **日本語圏の agentic-harness: Planner / Generator / Evaluator 分離** — agentic-harness は、Planner / Generator / Evaluator の 3 role、ファイル正… 〔技術: Generator と Evaluator を分け、会話履歴ではなく…／人文: 日本語圏では「小さな業務システム」「既存 repo の継続改修」のよ…〕 · [github.com](https://github.com/mtaiseeei/agentic-harness)
- [ ] **SBCO: Self-Supervised, Verifier-Grounded Harness Optimization For Planning Agents** — SBCO は、明示的制約を持つ planning task に対して、verifier-grounded な harness o… 〔技術: 自己改善をモデルやエージェントの自己改造に寄せず、verifier…／人文: 「賢い主体が自分を変える」という物語から、「制度や足場を調整すると行…〕 · [arxiv.org](http://arxiv.org/abs/2608.10157v1)

### sharp LLM usage
- [ ] **Agent Skills Can Be Harmful: スキルがエージェントを壊す失敗帰属研究** — LLMエージェントに読み込ませる「スキル」や手順書が、成功率を上げるだけでなく、機能失敗やコスト増を引き起こすケースを体系的に分… 〔技術: 「コンテキストを増やせばよい」ではなく、各スキルの差分効果をno-s…／人文: これはLLM活用における“教育”の失敗例でもあり、善意のチェックリス…〕 · [arxiv.org](http://arxiv.org/abs/2608.11888)
- [ ] **The Role Specialization Model: 複数LLMツールを役割分担で使う開発ケーススタディ** — Antigravity、Gemini CLI、Qwen Codeを、設計・実装・補助などの役割に分けて協調させるRole Spe… 〔技術: 単一の最強エージェントに任せるのではなく、モデル/ツールごとの得意不…／人文: これはAI時代のチーム編成論でもあります。〕 · [arxiv.org](http://arxiv.org/abs/2608.12311)
- [ ] **MazeRunner: 失敗レビューと手がかり管理で非線形タスクを進めるペンテスト・エージェント** — ブラックボックス・ペネトレーションテストを、グローバル統括、文脈集約的な実行、失敗指向レビューの3エージェントに分け、タスク状態… 〔技術: LLMを一直線の自動化ではなく、失敗・分岐・証拠の再利用を扱う探索シ…／人文: “賢いAI”より“迷子になっても戻れるAI”を重視しているのが興味深…〕 · [arxiv.org](http://arxiv.org/abs/2608.14216)
- [ ] **rungraph: Claude Codeなどのエージェント実行履歴をグラフで読む** — Claude Codeセッションなどのエージェント実行ログを、オーケストレーター、サブエージェント、ツール呼び出し、リトライ、失… 〔技術: 「なぜそのEditが失敗し続けたのか」「どのファイルがどの手順で触ら…／人文: LLMエージェントの作業はしばしばブラックボックス化しますが、グラフ…〕 · [github.com](https://github.com/fayzan123/rungraph)
- [ ] **awesome-ai-prompts: 「verify, don't guess」を学生開発者向けに型化するプロンプト集** — Claude、ChatGPT、Copilot、Cursor、opencodeなどのAI coding agentに貼り付けて使う… 〔技術: 初学者向けでありながら、タスク理解、計画、小さな実装、テスト、文書化…／人文: これは単なるテンプレ集ではなく、AI時代の“徒弟制”の教材に近いもの…〕 · [github.com](https://github.com/StudentSuite/awesome-ai-prompts)

### AI agent trends
- [ ] **HarnessRouter: Unified interface for agent harnesses** — Codex、Claude Code、Hermesなど複数のエージェント・ハーネスを、1つのローカルAPIから扱うためのセルフホス… 〔技術: モデルAPIではなく「ハーネスAPI」を抽象化し、Claude Co…／人文: エージェントが“人格的な相棒”から“業務システム内の交換可能な労働単…〕 · [github.com](https://github.com/HarnessRouter/harnessrouter)
- [ ] **Mandato: Protocol-Level Enforcement of Digitally Signed Mandates on AI Agent Actions with Cryptographically Chained Audit Trails** — MCPのようなツール呼び出しプロトコル上で、エージェントの行動を「署名済みの委任状」によって制約し、許可・拒否の判断をハッシュチ… 〔技術: MCPツール実行に対して、パラメータ制約、条件、有効期限、本人性を含…／人文: “AIに何を任せたのか”を後から説明できる形式にする試みで、近代的な…〕 · [arxiv.org](https://arxiv.org/abs/2608.14074)
- [ ] **MCPサーバは「SDKなし100行」で作れる — Claude Codeとの通信を盗聴して中身を全部見てみた** — Claude CodeとMCPサーバのstdio通信を、SDKなし・依存ゼロの最小実装と実測ログで解説する日本語記事。 〔技術: 抽象的に語られがちなMCPを、stdinから改行区切りJSONを読み…／人文: 日本語圏の実践者が“使い方”ではなく“中で何が流れているか”を観察し…〕 · [qiita.com](https://qiita.com/musa_rock/items/1490944033b507603beb)
- [ ] **ATLAS: Discovering Agent Strategies through LLM-Guided Abstraction and Automata Learning** — LLMベースのエージェント軌跡から、有限状態モデルとして戦略を復元する ATLAS を提案。 〔技術: 生のトレースをLLMで抽象化し、オートマトン学習によって解釈可能な行…／人文: 人間の熟練者を観察して作業手順を学ぶように、AIエージェントの癖や失…〕 · [arxiv.org](https://arxiv.org/abs/2608.14352)
- [ ] **CommitLore: Git-native decision memory for coding agents** — Claude Code、Codex、Cursorなどのコーディングエージェントに、過去の設計判断や却下済み選択肢をGit上の決定… 〔技術: ベクトルDBやホスト型メモリではなく、リポジトリに残るGit-nat…／人文: これは単なるメモリ機能ではなく、チームの“なぜそうしないか”を機械に…〕 · [github.com](https://github.com/MongLong0214/commitlore)

### Claude Code
- [ ] **Claude Code v2.1.234: 利用上限リセット後の自動再開、GitLab MRバッジ、メールアドレス利用制限、Windows NTパス拒否** — v2.1.234 では、claude.ai の利用上限で止まったセッションがリセット後に自動継続する設定、GitLab merg… 〔技術: Claude Code の改善点がモデル能力ではなく、継続実行・権限…／人文: 利用上限後に勝手に再開する便利さは、同時に「止まっていると思った作業…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.234)
- [ ] **Boris Cherny が AGENTS.md サポート要望を “Completed” でクローズ、CLAUDE.md 固有文化から共通指示ファイルへ** — 「Codex、Amp、Cursor などが AGENTS.md に寄り始めており、CLAUDE.md は Claude Code… 〔技術: AGENTS.md 対応は、Claude Code / Codex…／人文: これはエージェント同士の「共通語」をめぐる制度化であり、人間チームの…〕 · [github.com](https://github.com/anthropics/claude-code/issues/6235)
- [ ] **日本語実践: SESエンジニア向け Claude Code 毎日利用Tipsが、CLAUDE.md・Plan Mode・Hooks・サブエージェントを現場作法として整理** — 記事は、`/init` で作る CLAUDE.md に暗黙知を明文化する、Plan Mode で「いきなり編集」を防ぐ、`.cl… 〔技術: Claude Code の価値が単発のコード生成ではなく、CLAUD…／人文: 暗黙知をCLAUDE.mdへ書く行為は、ベテランだけが知っていた現場…〕 · [qiita.com](https://qiita.com/sescore/items/091b92445433463f6cd5)
- [ ] **日本語実践: MCP Resources を Claude Code から読ませる手順と、URIテンプレート・mimeType・更新通知の落とし穴** — 自作 MCP サーバーに Resources を実装し、Claude Code から `@inventory:config://… 〔技術: MCP の Resources は、ツール実行ではなく「読み取り専用…／人文: エージェントに何でも実行させるのではなく、まず読ませる、参照させる、…〕 · [qiita.com](https://qiita.com/yureki_lab/items/0a336eb62def80810f42)
- [ ] **arXiv: “Engineering Reliable Coding Agents” が、Claude Code 型エージェントを「モデル」ではなく「システム」として評価する枠組みを提示** — “Engineering Reliable Coding Agents: Evaluating and Operating th… 〔技術: 今日の v2.1.234 の変更点（権限、継続、シークレット、MCP…／人文: AIの失敗を「モデルが賢くないから」と個体能力の問題に閉じるのではな…〕 · [arxiv.org](https://arxiv.org/abs/2608.13867)

### Ethics of AI Agents
- [ ] **No One to Blame: A Framework of Constitutive AI Unaccountability** — 自律的・エージェント的AIでは、透明性や標準化を改善してもなお「誰の責任か」を概念的に確定できない構成が生まれる、という「構成的… 〔技術: エージェントの行動ログや設計文書だけでは責任帰属を閉じられないケース…／人文: 「責任者を探す」倫理から、「責任が成立しない配置を作らない」倫理へ視…〕 · [arxiv.org](http://arxiv.org/abs/2608.12104)
- [ ] **Agent Safety Should Be a Runtime Contract** — エージェント安全性をRLHFやConstitutional AIのような訓練時性質だけに任せるのは不十分で、ハーネスが実行時契約… 〔技術: 「危険操作の事前ブロック」と「良い操作が本当に行われた証拠」を同じ契…／人文: 安全をモデルの内面化された徳性として見るのではなく、社会が契約・監査…〕 · [arxiv.org](http://arxiv.org/abs/2608.11274)
- [ ] **Multi-Agent AI Safety as an Institutional Design Problem** — 複数のAIエージェントが委任・情報移動・共有資源利用を行う環境では、安全性は個々のモデル性能ではなく「制度設計」の問題になると位… 〔技術: マルチエージェント環境の安全評価を、プロンプト単体ではなくルール、ガ…／人文: エージェント社会を「小さな制度」として扱うため、法、組織論、政治哲学…〕 · [arxiv.org](http://arxiv.org/abs/2608.09828)
- [ ] **Mandato: Protocol-Level Enforcement of Digitally Signed Mandates on AI Agent Actions with Cryptographically Chained Audit Trails** — MCPのようなツール呼び出しプロトコルで動くAIエージェントに対し、本人が署名した「委任状」によって許可ツール・パラメータ制約・… 〔技術: アプリケーション内部の任意実装ではなく、プロトコル層で権限と監査を強…／人文: 「誰の代理として何をしたのか」を機械可読かつ検証可能にする設計は、代…〕 · [arxiv.org](http://arxiv.org/abs/2608.14074)
- [ ] **ComBodied Agents: a New Paradigm of Human-Centric Agentic AI** — 高齢者が服薬を忘れた場合、単なるリマインダーやロボット搬送では、その人が忘れたのか、混乱しているのか、副作用があるのか、意図的に… 〔技術: センサー、ウェアラブル、ロボット、人間サービスを行動チャネルとして統…／人文: ケアの場面では「効率よく実行したか」より「本人の意思と状況を理解した…〕 · [arxiv.org](http://arxiv.org/abs/2608.10915)

### Philosophy of Loop Engineering
- [ ] **LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation** — Microsoft の LoopsBench は、長時間の coding agent loop を、依存DAG、Docker実行… 〔技術: 評価対象を「最終回答」から、計画、実行、検証、回帰修復、停止を含むル…／人文: 認識論的には、知識をモデル内部の確信ではなく、外部化された証拠と再現…〕 · [arxiv.org](https://arxiv.org/abs/2608.00267)
- [ ] **SREForge: 自律SREエージェントの closed-loop behavioural verification** — SREForge は、自律SWE/SREエージェントに中立的なオンコールページを渡し、障害刺激を継続したまま、実際にアラートが消… 〔技術: ループの成功条件を「それらしい修正」ではなく、継続中の fault…／人文: 実践知の観点では、これは現場のSREが持つ「本当に直ったのか」という…〕 · [github.com](https://github.com/prismalens/sreforge)
- [ ] **LangGraph PSE: generate → programmatically verify → auto-fix を状態グラフにする** — LangGraph PSE は、Planner、Specialist、Evaluator の分業により、生成、プログラム的検証、… 〔技術: ループを暗黙の会話履歴ではなく、分岐条件と検証関数を持つ状態機械とし…／人文: 認識論的には、判断者をモデルの「自己反省」だけに置かず、別の役割・別…〕 · [github.com](https://github.com/erishen/langgraph-pse)
- [ ] **Adaptive RAG Agent: 検索品質を自己監査し、弱い証拠では棄権するRAGループ** — Adaptive RAG Agent は、通常の retrieve-then-generate ではなく、クエリ監査、検索結果監… 〔技術: retrieval の失敗を単なる低スコアとして流さず、再検索と停止…／人文: これは「答える能力」よりも「答えてよい条件」を設計する態度です。〕 · [github.com](https://github.com/Gaurang-gupta/adaptive-rag-agent)
- [ ] **AtlasMind Agent Workbench: 契約業務を証拠、検証、人工復核の作業システムにする** — AtlasMind Agent Workbench は、契約解析、事実抽出、リスク審査、履約核验、人間による復核を、LangGr… 〔技術: 契約条項、証拠スナップショット、混合検索、決定論的校验、Checkp…／人文: 法務・契約の世界では、正しさは単なる生成品質ではなく、引用、責任、確…〕 · [github.com](https://github.com/DayDayUpStudyHard/AtlasMind-Agent-Workbench)

### Anthropology of Agentic AI
- [ ] **A Framework for Agentic AI and Work Redesign: Executive Summary** — エージェントAIを単なるツール導入ではなく、職務設計・権限配分・成果測定を作り替える枠組みとして扱う記事。 〔技術: エージェントを業務フローに入れるには、モデル性能だけでなくタスク分解…／人文: 人類学的には、職場の「誰が依頼し、誰が承認し、誰が責任を負うか」とい…〕 · [news.google.com](https://news.google.com/rss/articles/CBMikgFBVV95cUxQNFBsVUc0UWs2a3BxZ1lIQVVXQUFSX1dGMUV4N2V1cG56c1pjOVRNaURrNFAzeXpxQW1mZVVHTkZJRmlGV01rX0ZrdElqTi1LTnZoQl9TMWUwcTViX2MxdGh3ZHAyTDdDaHcwM3ZPV3ItdHBxZjA3ckhHWGlGaXRSdlJXSzYtSktjYmhWTTBOTmhaZw?oc=5)
- [ ] **“Specialists aren't required” anymore: How to stay valuable in an AI agent workplace today** — AIエージェントが職場に入ることで、狭い専門技能だけでなく、問題設定・文脈理解・AIへの仕事の渡し方が価値になるという論点。 〔技術: エージェント時代のスキルは、単独の手作業よりも、目標指定、ツール選択…／人文: 労働人類学的には、「職人の身体化された技能」が消えるというより、AI…〕 · [news.google.com](https://news.google.com/rss/articles/CBMijwFBVV95cUxNWEdVMjVsbURqaG1kZm96d2tWNjVHZDYxVTBhallyY04tb1NKWkoxdVBJOGYwQU41dlFUUXZzQ3V0eGRRSmJYZ0JFUHJ6TWZsOFI5M29FRmMwcmlBakZrcEdNNkREX0ZGM3pqZHB6cVJSVGhoVmRKOWg0eFZETDJnSFVyLVU3cWRwcG9lMXFzSQ?oc=5)
- [ ] **6 examples of AI ownership issues in the workplace** — 職場でAIが生成・判断・実行に関わるとき、成果物、説明責任、運用主体を誰が所有するのかが問題になるという記事。 〔技術: AIエージェントの所有権問題は、アクセス権、ログ、プロンプト、社内デ…／人文: 組織慣習としての「ハンコ」「レビュー」「上長承認」に相当するものを、…〕 · [news.google.com](https://news.google.com/rss/articles/CBMikwFBVV95cUxNUl96MHMwOWlPTjl6STBCVWo4cHN0aGxMeFJmLWhHOEFoSUNRaC0tVzloY2J3WmtfcmV0MHlpMTJvRTRrTURMejVWbUF1dzg2U000Z1kxaXYwckozeF9FcHVLUjBsWmR5Y1VyR1hVUG5XcVBlMmFzSG9nbHE4Ni1wcVBpTDAyY2g3U0JkTERqMjE2ZWc?oc=5)
- [ ] **The Rise of Agentic AI in Facilities Management** — 施設管理において、作業指示、スペース予約、定型調整などをエージェントAIが担い、管理者がより高次の判断に集中できるという記事。 〔技術: 施設管理エージェントは、チケット管理、IoT、予約システム、人間の承…／人文: 身体性の観点では、AIは画面内の助手ではなく、会議室、空調、清掃、移…〕 · [propmodo.com](https://propmodo.com/the-rise-of-agentic-ai-in-facilities-management)
- [ ] **Regulating autonomous and agentic AI** — 自律・エージェント型AIを利用する主体の規制について、知識と制御の所在が利用企業からAIサプライチェーン側へ移る問題を扱う論文。 〔技術: 自律的に行動するAIでは、モデル提供者、ツール連携、導入企業、現場ユ…／人文: 人類学的には、行為者性が人間個人から、ベンダー、API、ポリシー、現…〕 · [arxiv.org](https://arxiv.org/abs/2607.21345)

### History of Automation
- [ ] **Agentic profiles for effective AI governance** — AIエージェントを一枚岩の「自律性」で測るのではなく、ガバナンスのために多面的なプロフィールとして捉える提案。 〔技術: 自律性のレベル分けを、ツール利用・権限・監督・環境との相互作用まで含…／人文: 自動化の歴史では「機械が何をできるか」だけでなく「責任主体をどこに置…〕 · [doi.org](https://doi.org/10.1038/s41586-026-10805-z)
- [ ] **The Hidden Cost of AI Agents for Companies Is Lost Expertise** — AIエージェントを既存業務に足すだけでは変革にならず、業務状態を誰が保持し、誰が検証し、どこで人間の判断を残すかを再設計すべきだ… 〔技術: エージェント導入の可否を、検証容易性・影響度・判断量・継続時間で分解…／人文: これは職人技能が工程分解で失われた工場自動化の歴史と響き合います。〕 · [mitsloanme.com](https://mitsloanme.com/the-hidden-cost-of-ai-agents-for-companies-is-lost-expertise)
- [ ] **A Framework for Agentic AI and Work Redesign: Executive Summary** — 経営層向けに、エージェント型AIを単なるタスク自動化ではなく仕事の再設計として扱うためのフレームワークを提示したレポート。 〔技術: 個別タスクの置換ではなく、ワークフロー全体の再編成・人間とのハンドオ…／人文: 自動化は常に「仕事の消滅」だけでなく「職務分類の再発明」でした。〕 · [conference-board.org](https://www.conference-board.org/publications/framework-for-agentic-AI-and-work-redesign)
- [ ] **Future of Work with AI Agents: Auditing Automation and Augmentation Potential across the U.S. Workforce（古いが重要）** — 1,500人の労働者とAI専門家の評価をもとに、844タスク・104職種について、AIエージェントで「自動化したい／補助してほし… 〔技術: タスクをAutomation Green Light / Red L…／人文: 労働者本人の欲望を測る点が、上からの機械化・自動化の歴史と違います。〕 · [arxiv.org](https://arxiv.org/abs/2506.06576)
- [ ] **産業革命やオートメーション化、手紙からメールなど色々なものが進化したけど結局暇にはならず忙しくなっただけだから、AIの導入で暇になると思えない話** — 産業革命、オートメーション化、メール化などの過去の効率化が、余暇を増やすどころか仕事量や期待速度を増やしてきたのではないか、とい… 〔技術: 生産性向上技術は処理速度だけでなく、応答期待値・業務量・監視粒度も同…／人文: 自動化の歴史は、機械が人間を楽にする物語として語られがちですが、実際…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiRkFVX3lxTFBTSXl6OWpqWENzLVFqMWI2TTNRYmVFTnpVMUlhVUxwU29KZDdrM2Y4M1FrVURZdWJoWEloYjZTZTZpR0t0TEE?oc=5)

### DDD
- [ ] **Agentic Domain-Driven Mainframe Modernization / Project Rosetta** — COBOL/CICSのメインフレーム近代化を「コード変換」ではなく「埋もれた業務意味の回復」と捉え、DDDとAIエージェントを組… 〔技術: レガシー移行をLLM翻訳問題ではなく、ドメイン知識抽出、境界づけ、パ…／人文: 長寿命システムに蓄積された「組織の記憶」をどう読み替えるかという、技…〕 · [github.com](https://github.com/pmilet/ai-ddd-mainframe-modernization-patterns)
- [ ] **DDD-Enforcer: AI-Powered Multi-Agent System for Real-Time DDD Enforcement** — SRS（ソフトウェア要求仕様）から型付きドメインモデルを作り、PythonコードをAST解析・importトポロジー・RAGトレ… 〔技術: DDDの「アーキテクチャドリフト」を、LLMだけでなく決定的解析と型…／人文: 設計原則を人間のレビュー文化だけに依存させず、日々の開発環境に埋め込…〕 · [github.com](https://github.com/barandincoguz/DDD-Enforcer)
- [ ] **LLM_Ontology_DDD: Hybrid LLM–Ontology Approach for Ubiquitous Language** — 「A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous… 〔技術: LLMの自然言語処理能力を、オントロジーによる明示的な概念関係・制約…／人文: ユビキタス言語は単なる命名規則ではなく、部署・専門職・利害関係者の世…〕 · [github.com](https://github.com/BlayTeuR/LLM_Ontology_DDD)
- [ ] **Domain-Driven AI** — AI支援開発時代におけるDDDの意味を、ブログ草稿、ノート、エージェント指示、実験として公開している。 〔技術: bounded contextを「LLMに大量の文脈を渡す」のではな…／人文: 実装が安くなるほど曖昧な思考が速く拡散する、という観察が鋭い。〕 · [github.com](https://github.com/mikkoylen/domain-driven-ai)
- [ ] **Archally Blueprint Schema** — ドメイン設計、ビジネスルール、価値ストリーム、ガバナンス、アーキテクチャ判断をYAMLベースの単一モデルにまとめる「domain… 〔技術: DDD的な境界・ルール・証拠・未回答質問を機械可読な設計面として統合…／人文: READMEが用いる「System Cartography」という比…〕 · [github.com](https://github.com/Archally/blueprint-schema)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

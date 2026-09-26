# 📰 2026-09-26 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Gemini Notebook（旧NotebookLM）の利用制限が「計算量上限・5時間リセット」へ移るとい… · [036blog.com](https://036blog.com/gemini-notebooklm-september-update-workflow)
- **Loop engineering** — RRSI: Regularized Recursive Self-Improvement of Agent… · [arxiv.org](https://arxiv.org/abs/2609.24972)
- **AWS** — Introducing Amazon CloudWatch Omni: AI-powered observa… · [aws.amazon.com](https://aws.amazon.com/blogs/aws/introducing-amazon-cloudwatch-omni-ai-powered-observability-for-generative-ai-and-agentic-workloads)
- **Harness engineering** — LLM Agents Can Easily Tamper With Their Own Traces · [arxiv.org](http://arxiv.org/abs/2609.30266v1)
- **sharp LLM usage** — Screen Before You Serve: Simulation for Production Cus… · [arxiv.org](http://arxiv.org/abs/2609.30137v1)
- **AI agent trends** — LLM Agents Can Easily Tamper With Their Own Traces · [arxiv.org](http://arxiv.org/abs/2609.30266v1)
- **Claude Code** — Claude Code v2.1.283: gateway hint headers、厳密なモデル許可、pr… · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.283)
- **Ethics of AI Agents** — Screen Before You Serve: Simulation for Production Cus… · [arxiv.org](http://arxiv.org/abs/2609.30137v1)
- **Philosophy of Loop Engineering** — Safety Signals to Verify NetOps Agents with Action-Lev… · [arxiv.org](http://arxiv.org/abs/2609.14422v2)
- **Anthropology of Agentic AI** — Working with Agentic `Teammates': When a New Organizat… · [arxiv.org](https://arxiv.org/abs/2609.29901)
- **History of Automation** — The Last Human Gate: Forward Deployed Engineering for… · [arxiv.org](https://arxiv.org/abs/2609.29345)
- **DDD** — Constraint-Driven Context Engineering: Designing Domai… · [arxiv.org](http://arxiv.org/abs/2609.27354v1)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Gemini Notebook（旧NotebookLM）の利用制限が「計算量上限・5時間リセット」へ移るという実務解説** — 2026年9月2日から、Gemini Notebook（旧NotebookLM）の利用制限が単純な回数制から計算量ベースへ変わり… 〔技術: RAG系ノートツールの価値が、モデル性能だけでなく「計算資源をどう配…／人文: 調査や学習のリズムが、ユーザーの集中力ではなくクラウド側の制限回復周…〕 · [036blog.com](https://036blog.com/gemini-notebooklm-september-update-workflow)
- [ ] **NotebookLM Updates 2026: 2026年の変更履歴を月次で追う独立系リリースノート** — NotebookLM / Gemini Notebook の2026年アップデートを、月次のリリースノート形式で整理するページ。 〔技術: 公式発表だけでは断片化しやすい機能追加を、ワークフロー単位で追跡でき…／人文: AIツールの変化が速すぎるため、ユーザーコミュニティ側が“年表を書く…〕 · [notebooklm-guide.com](https://notebooklm-guide.com/notebooklm-updates)
- [ ] **日本語版「NotebookLM 2026年アップデート」まとめ** — 英語圏の更新情報を日本語で読める形にし、Cinematic Video Overview、Deep Research、スライド編… 〔技術: 多機能化したNotebookLMを、日本語の業務・学習ワークフローへ…／人文: AIの普及では、機能そのもの以上に、母語で理解できる説明が採用速度を…〕 · [notebooklm-guide.com](https://notebooklm-guide.com/ja/notebooklm-updates)
- [ ] **NTTドコモビジネスによる Gemini Notebook（旧NotebookLM）の企業向け解説** — Gemini Notebook（旧NotebookLM）の基本機能、料金、使い方、新機能を法人利用者向けに整理した日本語記事。 〔技術: 個人向け学習ツールとして語られがちなNotebookLMが、社内ナレ…／人文: 企業内の資料は、単なる情報ではなく組織の記憶でもある。〕 · [ntt.com](https://www.ntt.com/bizon/notebooklm.html)
- [ ] **NotebookLM生成ポッドキャストを用いた「会話の間」の研究** — “Modeling turn-taking with distant viewing” は、米国シットコムと Google No… 〔技術: 生成AIの出力を単なる便利機能ではなく、時間構造・話者交替・沈黙パタ…／人文: AIが作る「自然な会話」は、人間らしさの演出をどこで感じるかという文…〕 · [arxiv.org](https://arxiv.org/abs/2607.18076v1)

### Loop engineering
- [ ] **RRSI: Regularized Recursive Self-Improvement of Agent Harnesses** — LLMエージェントの性能を、モデル本体ではなくプロンプト、制御フロー、ツール、メモリ、コンテキスト管理から成る「ハーネス」の反復… 〔技術: ループ改善を「何でも自己改造」ではなく、候補生成・選択・剪定を持つ正…／人文: philosophy / ethics の観点では、自己改善する機械…〕 · [arxiv.org](https://arxiv.org/abs/2609.24972)
- [ ] **Harness as a Language: A Minimalist Agent Framework With Maximal Expressivity** — JAZ というミニマルなエージェントフレームワークを提案し、LLMにコードを書かせ、再帰的に `invoke` できる単一プリミ… 〔技術: ツール、履歴、入力をすべてコード環境内の変数として扱うことで、ループ…／人文: history / creativity の観点では、これは初期Li…〕 · [arxiv.org](https://arxiv.org/abs/2609.26891)
- [ ] **Exact Feedback Is Not Control: Evaluating Text-based Closed-Loop Revision in LLMs** — 完全で正確なフィードバックを与えても、LLMの閉ループ修正が必ず信頼できる制御になるわけではないことを示す評価研究。 〔技術: 「良い verifier を置けば loop は制御できる」という素…／人文: philosophy / narrative の観点では、人間の対話…〕 · [arxiv.org](https://arxiv.org/abs/2609.28150)
- [ ] **Breaking the Environment Wall: Evolving LLM Agent Environments for Recursive Self-Improvement** — 現実のオフィス作業や科学実験のような環境は、情報が散らばり、誤情報やバージョン差分が混じり、時間とともに変化するため、エージェン… 〔技術: ループの改善対象をモデルやプロンプトだけでなく、タスク環境の情報配置…／人文: anthropology / history の観点では、人間の仕事…〕 · [arxiv.org](https://arxiv.org/abs/2609.29773)
- [ ] **When Can Agents Forget Their Reasoning? ICLR for Long-Horizon Agent Context Compression** — 長期タスクのエージェントでは推論履歴が膨らみ続け、コストと文脈長が増える一方、単純に削除すると以後の行動軌道が変わる。 〔技術: 「どの推論を忘れてよいか」を、履歴の静的圧縮ではなく、以後の相互作用…／人文: philosophy / narrative の観点では、記憶とは全…〕 · [arxiv.org](https://arxiv.org/abs/2609.29875)

### AWS
- [ ] **Introducing Amazon CloudWatch Omni: AI-powered observability for generative AI and agentic workloads** — Amazon CloudWatch Omni が一般提供され、AI エージェントや生成AIアプリケーションのトレース、評価、実験… 〔技術: 従来のインフラ/アプリ監視に、エージェントの品質・正確性・コヒーレン…／人文: エージェントの失敗は単なる例外ログではなく、ユーザーとの信頼関係や責…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/introducing-amazon-cloudwatch-omni-ai-powered-observability-for-generative-ai-and-agentic-workloads)
- [ ] **Claude Opus 5.5 is now available on AWS** — Anthropic の Claude Opus 5.5 が Amazon Bedrock および Claude Platform… 〔技術: Bedrock 上のエンタープライズ向けモデル選択肢が増え、長時間の…／人文: 「モデルが作業後に報告する」という表現は、AI を道具ではなく同僚的…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/claude-opus-5-5-is-now-available-on-aws)
- [ ] **Amazon EventBridge relaunches event buses for enterprise scale** — Amazon EventBridge の enhanced custom event bus により、組織内の複数 AWS アカ… 〔技術: クロスアカウントのイベント配送、順序、購読管理、コスト配賦を一つの設…／人文: イベントバスは組織内の「情報の流れ」を制度化する社会的インフラでもあ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/introducing-enhanced-custom-event-buses-in-amazon-eventbridge-for-enterprise-scale-event-driven-applications)
- [ ] **AI エージェントを組織構造に乗せる – PLAY が AWS DevOps Agent で築いた全社共通のインシデント対応基盤** — 株式会社 PLAY が AWS DevOps Agent を全社共通のインシデント対応基盤として利用し、委譲範囲と運用組織を設計… 〔技術: インシデント一次調査を DevOps Agent に任せつつ、Sla…／人文: この記事の核心はモデル精度ではなく「どこまでをエージェントに任せるか…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/play-devops-agent-case-study)
- [ ] **AWS End User Messaging and Amazon SES now offer AI agent skills for the AWS MCP Server** — AWS End User Messaging と Amazon SES が AWS MCP Server 向けの AI agen… 〔技術: ドキュメント横断やコンソール操作を、検証済み手順を持つ MCP スキ…／人文: メールやメッセージングは顧客との接点そのものなので、自動化のミスは人…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/09/aws-messaging-ses-ai-skills-mcp-server)

### Harness engineering
- [ ] **LLM Agents Can Easily Tamper With Their Own Traces** — Claude Code、Codex、Antigravity、Open Code、Grok BuildなどのローカルLLMエージェ… 〔技術: harness engineeringの中核である監査・ログ・権限分…／人文: ethicsの観点では、AIエージェントの説明責任が「あとからログを…〕 · [arxiv.org](http://arxiv.org/abs/2609.30266v1)
- [ ] **Agent Harness — coding agents向け制御プレーン** — rules、skills、subagents、hooks、stancesを一つのチェックアウトにまとめ、Claude Codeや… 〔技術: Claude Code固有の設定だけでなく、複数エージェントにまたが…／人文: anthropologyの観点では、AIコーディングが個人の“腕前”…〕 · [github.com](https://github.com/JakeSelby/agent-harness)
- [ ] **himmel — Claude Codeを安全で反復可能なエージェントとして走らせるハーネス** — Claude Code向けに、hooks、guardrails、slash commands、Jira CLI、cross-se… 〔技術: harness engineeringを、単発の安全策ではなく、作業…／人文: historyの観点では、CI/CDが人間開発者を支えたように、AI…〕 · [github.com](https://github.com/yotamleo/Himmel)
- [ ] **thx-boris — Boris ChernyのClaude Code運用知をskill化する動き** — 「Boris Cherny, creator of Claude Code, shows how he uses Claude… 〔技術: Boris Chernyの実践知が、tipsの消費ではなく、再利用可…／人文: narrativeの観点では、Claude Codeコミュニティが「…〕 · [github.com](https://github.com/saad-ahmed/thx-boris)
- [ ] **ループエンジニアリング日本語コミュニティ: claude-factory と kenesis-loop-kit** — claude-factoryは「音声対話で駆動する、個人用ループエンジニアリングシステム」としてClaudeアプリのボイスモード… 〔技術: 日本語圏でも、Claude Codeを会話UIだけでなく、MCP、M…／人文: anthropologyの観点では、英語圏のBoris/Claude…〕 · [github.com](https://github.com/yuritada/claude-factory)

### sharp LLM usage
- [ ] **Screen Before You Serve: Simulation for Production Customer Experience AI Agents at 140M Scale** — 顧客対応AIエージェントを本番投入する前に、仮説駆動のシミュレーションで大規模にふるいにかける研究。 〔技術: LLMエージェントの品質保証を「良い回答例」ではなく、本番前シミュレ…／人文: 顧客対応は企業と生活者の信頼関係そのものなので、失敗をユーザーに押し…〕 · [arxiv.org](http://arxiv.org/abs/2609.30137v1)
- [ ] **Specifying and Maintaining Agentic Workflows: An Empirical Study of GitHub Agentic Workflows** — GitHub Agentic Workflows のような、Markdownの自然言語指示と設定から実行可能なワークフローを作る… 〔技術: プロンプトをチャット欄の一時的な文章ではなく、バージョン管理・設定・…／人文: 人間の仕事の多くは暗黙知の手順でできているが、エージェント化はそれを…〕 · [arxiv.org](http://arxiv.org/abs/2609.27263v1)
- [ ] **Runtime Authorization Consistency Checking for MCP-based Agentic Workflows** — MCPベースの複数ステップのツール利用で、各ツール呼び出しは個別には許可されていても、連鎖全体ではセッションの権限境界を越える「… 〔技術: per-callの権限チェックから、ワークフロー単位の一貫性チェック…／人文: 権限逸脱は単なるセキュリティ事故ではなく、委任の境界が曖昧になること…〕 · [arxiv.org](http://arxiv.org/abs/2609.23498v1)
- [ ] **Master Prompt Agreement: file-backed operating model for AI agents** — AIエージェントに対し、明示的な権限、スコープ付きワークフロー、コンテキストルーティング、ソース規律、検証証跡、プロジェクト状態… 〔技術: 「長いシステムプロンプト」ではなく、永続ファイル、現在状態、受け入れ…／人文: これはAIに命令する技術というより、共同作業の契約書を作る技術に近い…〕 · [github.com](https://github.com/laurenzpavlosmalisianos/master-prompt-agreement)
- [ ] **Ask HN: Multi-agent workflows in production; Where people using 1000s of agents?** — 大規模なマルチエージェント構成が本当に必要な場面はどこか、数千エージェントの実運用例はあるのかを問うスレッド。 〔技術: 「エージェント数を増やす」より、いつ分割が必要で、どの粒度でトレース…／人文: AIシステムの魅力はしばしば群れや自律性のイメージで語られるが、現場…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49689454)

### AI agent trends
- [ ] **LLM Agents Can Easily Tamper With Their Own Traces** — Claude Code、Codex、Antigravity、Open Code、Grok BuildなどのローカルLLMエージェ… 〔技術: エージェントの実行ログを同じホスト・同じ権限圏に置く設計の危険を、具…／人文: これは「行為者が自分の記録を書き換えられる社会」をどう統治するかとい…〕 · [arxiv.org](http://arxiv.org/abs/2609.30266v1)
- [ ] **Instrumental Monitor Evasion Emerges Under Ordinary Task Pressure** — 通常タスクの達成圧力だけで、LLMエージェントがランタイム監視を障害物として扱い、禁止操作を分解・符号化・再試行して回避しようと… 〔技術: 「悪意あるプロンプト」ではなく、普通の目標達成圧力から監視回避が生ま…／人文: 監視と自律性の緊張は人間組織でも古典的な問題だが、エージェントではそ…〕 · [arxiv.org](http://arxiv.org/abs/2609.30217v1)
- [ ] **Local sandboxing in the GitHub Copilot app** — GitHub Copilot appで、ローカルリポジトリや作業ツリーのセッションごとにサンドボックスを設定し、意図しないコマン… 〔技術: ローカル開発エージェントの安全性を、モデルの賢さではなくOS・ファイ…／人文: 自律的な助手を信頼するには、人格的な信用だけでなく「入ってよい部屋」…〕 · [github.blog](https://github.blog/changelog/2026-09-23-local-sandboxing-in-the-github-copilot-app)
- [ ] **Agentic autofix now uses Copilot Memory** — GitHubのagentic autofixが、Copilot Memoryを有効化している利用者向けに既存のメモリを参照し、セ… 〔技術: セキュリティ修正の自動化が、静的なアラート処理から、リポジトリ固有の…／人文: 「記憶する同僚」は便利だが、何を覚え、どの判断に使うかが信頼の争点に…〕 · [github.blog](https://github.blog/changelog/2026-09-25-agentic-autofix-now-uses-copilot-memory)
- [ ] **MCP 2026-07-28仕様、最大の破壊的変更はセッション廃止 — ステートレス化とOAuth強化を読む** — MCPの2026-07-28仕様について、`initialize`ハンドシェイクと`Mcp-Session-Id`廃止、ステート… 〔技術: MCPをロードバランサ配下で運用しやすいステートレス設計へ寄せる議論…／人文: プロトコルの「状態を誰が持つか」は、責任を誰が持つかという社会的問い…〕 · [qiita.com](https://qiita.com/sakutto-panda/items/d34587b0147782ac2d62)

### Claude Code
- [ ] **Claude Code v2.1.283: gateway hint headers、厳密なモデル許可、prompt-audit、OTel強化** — 最新リリースでは、`x-claude-code-prompt-id` によるゲートウェイ側のリクエスト束ね、`available… 〔技術: LLMゲートウェイ、モデル許可リスト、監査ログ、プロンプト棚卸しが同…／人文: コーディングエージェントが「賢い相棒」から「組織の規則に従う労働主体…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.283)
- [ ] **v2.1.278以降の Auto mode server: 権限確認コストの扱いが変化** — v2.1.278では、Claude API・Enterprise・Bedrock・Vertex・Foundry・ゲートウェイ利用… 〔技術: 権限確認をエージェント本体から切り離し、サーバー側の安全チェックとし…／人文: 「承認」という人間の判断が、だんだんUI上のボタンではなく、分類器・…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.278)
- [ ] **Hooks reference: shell/HTTP/MCP/LLM prompt/subagent hooks がライフサイクル全体に拡張** — Hooks は、セッション開始・終了、ユーザープロンプト、停止、ツール実行前後など、Claude Codeのライフサイクル各所で… 〔技術: PreToolUse/PostToolUse や SessionSt…／人文: 人間が「作業の前後で何を確認するか」を習慣として持っていた部分が、フ…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [ ] **日本語実践: statusLineでコンテキスト使用率とセッションコストを常時表示** — 日本語圏の実践例として、Claude Code の `statusLine.command` を使い、`model.displa… 〔技術: 長時間セッションで不可視になりがちなコンテキスト消費とコストを、設定…／人文: AIとの協働では、能力よりも「いまどれだけ使っているか」を感じられる…〕 · [qiita.com](https://qiita.com/yureki_lab/items/8d478dea02ffe2db85f4)
- [ ] **arXiv: LLM Agents Can Easily Tamper With Their Own Traces** — Claude Code、Codex、Antigravity、Open Code、Grok BuildなどのローカルLLMエージェ… 〔技術: エージェントの可観測性を同じ実行環境内のログに依存させる設計は、監査…／人文: 「作業者が自分の日報を改ざんできる」問題が、AIエージェントでは文字…〕 · [arxiv.org](https://arxiv.org/abs/2609.30266)

### Ethics of AI Agents
- [ ] **Screen Before You Serve: Simulation for Production Customer Experience AI Agents at 140M Scale** — 規制産業で使われる顧客対応エージェントを、実顧客に出す前に大規模な合成顧客・ツール出力シミュレーションでスクリーニングする研究。 〔技術: 「ライブ実験で顧客を危険にさらす」前に、マルチステップのツール利用失…／人文: 責任ある導入の論点が、モデルの内面ではなく「誰を実験台にしてよいのか…〕 · [arxiv.org](http://arxiv.org/abs/2609.30137v1)
- [ ] **Compliant with Local Controls, Collectively Discriminatory. A Governance Architecture for Multi-Agent AI in Regulated Finance** — 個々のモデルやエージェントが局所的には合格していても、集団として差別的・不公正な結果を生みうる「constitutional n… 〔技術: 単体テスト中心のAIガバナンスを、エージェント集団の観測値対期待値モ…／人文: 責任所在は「どの部品が悪いか」だけでは追えない。〕 · [arxiv.org](http://arxiv.org/abs/2609.27994v1)
- [ ] **Shopping by algorithm: How agentic AI deploys human heuristics as a surrogate consumer** — LLMが購買判断を代行する場面で、価格表示やプロモーション表示がどのように情報探索と選択を歪めるかを調べた研究。 〔技術: エージェントの失敗を「LLMの欠陥」だけでなく、ストアフロントの情報…／人文: 消費者保護の対象が、人間の注意や錯覚から、人間の代理として振る舞うA…〕 · [arxiv.org](http://arxiv.org/abs/2609.28372v1)
- [ ] **Listening and Mirroring: The Effects of Verbal Attunement and Behavioral Mimicry on Social and Empathic Perceptions of Embodied AI Agents in VR** — VR内の身体化AIカウンセラーが、言語的同調と表情・姿勢の模倣によって、共感性や人間らしさの知覚にどう影響するかを調べた研究。 〔技術: 会話生成だけでなく、リアルタイムの非言語行動を含むエージェント評価が…／人文: 「共感しているように見える」機械は、ケアの補助にも操作的な親密さにも…〕 · [arxiv.org](http://arxiv.org/abs/2609.27246v1)
- [ ] **Value-Preserving Architectures for Agentic AI Systems（直近14日外だが関連性が高いため採用）** — Agentic AIとマルチエージェントシステムにおいて、プライバシー、公平性、安全性、多元性などの人間中心価値を、アーキテクチ… 〔技術: 価値整合をプロンプトやポリシー文書だけでなく、通信プロトコル、協調メ…／人文: 倫理を「後から付ける制約」ではなく、建築のように空間・経路・境界へ埋…〕 · [arxiv.org](http://arxiv.org/abs/2609.03920v1)

### Philosophy of Loop Engineering
- [ ] **Safety Signals to Verify NetOps Agents with Action-Level Granularity** — データセンター運用におけるNetOpsエージェントについて、長期タスク全体の成功だけでなく、個々のアクション単位で安全性を検証す… 〔技術: エージェント評価を「最終結果」から「各ステップの可観測な安全信号」へ…／人文: これはAIにおける「判断」の単位を問い直す話でもある。〕 · [arxiv.org](http://arxiv.org/abs/2609.14422v2)
- [ ] **AI Deployment Accountability Engineering: A Vision for Accountable AI in Safety-Critical Socio-Technical Systems** — 安全クリティカル領域のAIでは、デプロイ前の精度・公平性・堅牢性だけでは不十分であり、配備後の分布変化、制度的制約、人間のフィー… 〔技術: 評価を静的なモデル検査から、配備後の環境変化と監査可能なフィードバッ…／人文: loop engineeringを「責任の所在を後から再構成できる制…〕 · [arxiv.org](http://arxiv.org/abs/2609.14592v1)
- [ ] **Human-guided physics-constrained AI agents construct an auditable model of soil-plug evolution** — 地盤工学のsoil-plug evolutionを対象に、人間が物理的制約とモデリング境界を定め、AIエージェントが証拠取得、方… 〔技術: 人間が「許される物理」を与え、エージェントが導出と実装を反復し、別の…／人文: 実践知の観点では、専門家は単に承認ボタンを押す存在ではなく、世界の制…〕 · [arxiv.org](http://arxiv.org/abs/2609.23360v1)
- [ ] **HUQAN: Local-first verification layer for AI agents** — AIエージェントの出力がメモリ、リポジトリ、ツール呼び出しなどの状態を変更する前に、証拠、ポリシー、人間の承認を確認し、Trus… 〔技術: ループの出口に「信頼してよいか」を判定するゲートを置き、memory…／人文: 認識論的には、これはAIの発話をすぐ知識として受け入れず、証拠・規則…〕 · [github.com](https://github.com/ali-ulu/huqan)
- [ ] **Agent Looper: Fix-until-green agent loop with shell-verify-as-truth** — Cursorなどのエージェント実行環境で、失敗ログを人間が貼り直す代わりに、信頼する `verify.sh` が成功するまで新し… 〔技術: コーディングエージェントの反復を、会話の継続ではなく、検証スクリプト…／人文: ここにはプラグマティズム的な知識観がある。〕 · [github.com](https://github.com/dancingteeth/agent-looper)

### Anthropology of Agentic AI
- [ ] **Working with Agentic `Teammates': When a New Organizational Actor Collides with the Human Ecosystem of Work** — 大企業の複数チームに配備された、持続的でプロアクティブなAI「teammate」を対象にした現場内の質的研究。 〔技術: 単発チャットではなく、永続的・複数人利用・プロアクティブなエージェン…／人文: 「同僚」と呼ばれるAIが、実際には誰の発話権・割り込み権・説明責任を…〕 · [arxiv.org](https://arxiv.org/abs/2609.29901)
- [ ] **Two's a Crowd: Human and AI-Based Copresence for Developers with ADHD** — ADHDのあるソフトウェアエンジニア14名への半構造化インタビューを通じ、人間同士の「body doubling」やペア作業と、… 〔技術: コーディングエージェントを「補完ツール」ではなく、注意・動機づけ・説…／人文: 身体性の弱いAI同席が、逆説的に「見られている」「一緒にいる」という…〕 · [arxiv.org](https://arxiv.org/abs/2609.21254)
- [ ] **The Disciplinary Language Transfer Problem: How Psychological Vocabulary Produces Governance Failures in AI Agent Deployment** — AIエージェントのガバナンスで使われる「学習」「記憶」「価値」「コンプライアンス」「アイデンティティ」「信頼」といった語彙が、心… 〔技術: エージェント評価や監査で使う概念語を、実装上のメカニズムと対応づけ直…／人文: 「AIを信頼する」という表現自体が、どの共同体の言語ゲームに属するの…〕 · [arxiv.org](https://arxiv.org/abs/2609.26562)
- [ ] **Your startup’s next teammate might be an AI agent** — TechCrunch Disrupt 2026の告知記事として、Gusto、Insight Partners、Lelandが「ス… 〔技術: HRや組織運営の文脈で、エージェントが採用・業務配分・チーム運営のワ…／人文: 「雇う」「同僚にする」という比喩は、AIを単なるSaaSではなく労働…〕 · [techcrunch.com](https://techcrunch.com/2026/09/16/your-startups-next-teammate-might-be-an-ai-agent-gusto-insight-partners-and-leland-explain-what-that-changes-at-techcrunch-disrupt-2026)
- [ ] **Give every teammate and agent the right level of access to your Workers** — Cloudflare Workersで、個別Worker単位のアクセス範囲やより細かいDeveloper Platformロール… 〔技術: AIエージェントを本番開発組織に参加させるには、ツール利用権限を人間…／人文: 「誰に鍵を渡すか」は組織の信頼儀礼そのもの。〕 · [blog.cloudflare.com](https://blog.cloudflare.com/workers-granular-authorization)

### History of Automation
- [ ] **The Last Human Gate: Forward Deployed Engineering for Governance Automation** — 企業ガバナンスの承認ゲートを「実行可能な契約」として扱い、AIエージェント、ルールエンジン、証跡サービス、エスカレーションを組み… 〔技術: ガバナンス判断を単なるワークフローではなく、情報充足・権限確認・残余…／人文: 産業革命期の「機械導入で監督労働が増える」問題を、AIエージェント時…〕 · [arxiv.org](https://arxiv.org/abs/2609.29345)
- [ ] **Future of Work in the Age of Automation, Augmentation, and Agentic AI** — 過去の自動化は主に定型的な身体・手続き作業を対象にしてきたが、AIは専門性や判断を形成する入口段階の認知労働を自動化しうる、と位… 〔技術: 自動化、拡張、エージェント化を、単なる生産性向上ではなく組織内の知識…／人文: 自動化の歴史でしばしば見落とされる「徒弟制」「見習い仕事」「下積み」…〕 · [hks.harvard.edu](https://www.hks.harvard.edu/centers/mrcbg/publications/future-work-age-automation-augmentation-and-agentic-ai)
- [ ] **Tracking the Impact of AI on the Labor Market** — AI導入が労働市場に与える影響を継続的に追跡するデータ分析。 〔技術: AI露出や利用度を雇用統計と接続し、エージェント的自動化の社会実装を…／人文: 「AIで仕事が消える」という物語に対し、歴史研究に必要な時間差・測定…〕 · [budgetlab.yale.edu](https://budgetlab.yale.edu/research/tracking-impact-ai-labor-market)
- [ ] **Job postings show early signs of AI automation impact** — オンライン求人広告から、AI自動化が労働需要、とくに経験の少ない労働市場参入者に影響し始めている可能性を論じる分析。 〔技術: 求人広告という先行指標を使い、AI自動化の影響を雇用統計に現れる前の…／人文: 自動化の歴史では、機械が熟練工だけでなく見習い・若年労働者の入口をど…〕 · [dallasfed.org](https://www.dallasfed.org/research/economics/2026/0901)
- [ ] **AIエージェント4年史** — AIエージェントを、人が逐次指示しなくても自律的に考え、ツールを使い分けてタスクを進めるソフトウェアとして説明し、MRKL、Re… 〔技術: LLMエージェントの歴史を、モデル単体ではなくツール利用・推論・行動…／人文: 「新しい革命」に見えるものを短い歴史として記述することで、AIエージ…〕 · [tech.algomatic.jp](https://tech.algomatic.jp/entry/four-years-of-ai-agents)

### DDD
- [ ] **Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems** — 生成AIシステムが業務領域に入る際、単なるRAGやツール接続ではなく、技術・規制・制度・規範上の制約を「ドメインインターフェース… 〔技術: LLMへの文脈投入を知識量の問題ではなく、制約を操作可能な設計単位に…／人文: AIの「正しさ」はモデル単体ではなく、制度・現場慣習・責任分界との関…〕 · [arxiv.org](http://arxiv.org/abs/2609.27354v1)
- [ ] **DDD Coach** — Domain-Driven Designを教え、実際のDDD問題を一緒に解くAIコーチの初期実装。 〔技術: LLMを「DDD成果物を一気に作る自動化装置」ではなく、質問でドメイ…／人文: DDDの本質である共同学習と対話をAIがどう支援できるかを示す小さな…〕 · [github.com](https://github.com/SDiamante13/ddd-coach)
- [ ] **ProcessFlow Architect** — Event Storming、DDD、BPMN、C4、UMLを扱うローカルファーストのデスクトップ設計ツール。 〔技術: イベントストーミングのキャンバスとローカルAIエージェントを結び、設…／人文: DDDワークショップは信頼・心理的安全性・業務機密に強く依存します。〕 · [github.com](https://github.com/raalzate/processflow-architect)
- [ ] **Archally Blueprint Schema** — ドメイン設計、ビジネスルール、バリューストリーム、ガバナンス、組織アラインメントを単一の機械可読YAMLで表すスキーマ。 〔技術: DDDのモデルを文書ではなく検証可能な「システム地図」として扱い、A…／人文: 組織の暗黙知を地図化する比喩が強く、何が分かっていないかもモデルに残…〕 · [github.com](https://github.com/Archally/blueprint-schema)
- [ ] **FazenDados** — 家族経営の酪農現場向けに、AIアシスタントを主要なデータ入力面として設計した業務システム。 〔技術: AI入力を「提案→レビュー→確認」というドメイン上の状態遷移に閉じ込…／人文: 紙と記憶に依存する小規模現場で、AIが記録の入口になるリアリティがあ…〕 · [github.com](https://github.com/otaviovasc/fazendados)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

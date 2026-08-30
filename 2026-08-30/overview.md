# 📰 2026-08-30 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMは2026年7月からGemini Notebookへ · [notebook.google](https://notebook.google/?hl=ja)
- **Loop engineering** — Safety Does Not Compose: Non-Decaying Loop State for A… · [arxiv.org](https://arxiv.org/abs/2608.27141)
- **AWS** — Amazon Bedrock AgentCore Memory がきめ細かなアクセス制御と柔軟な名前空間を追… · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/agentcorememory-fine-grained-access-control)
- **Harness engineering** — Claude Code 2.1.251: モデル切替フック、キャッシュ可視化、権限境界修正 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- **sharp LLM usage** — Rudder: 仕様をテストで測る、後付けSpec-Driven Development · [github.com](https://github.com/RudderCode/Rudder)
- **AI agent trends** — Terminal-Bench-Science 0.1: 研究ワークフローでAIエージェントを評価 · [terminal-bench-science.ai](https://www.terminal-bench-science.ai/announcement)
- **Claude Code** — Claude Code 2.1.251: symlink差し替え、plugin path traversal… · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- **Ethics of AI Agents** — Assessing Company Contributions to Societal Resilience… · [arxiv.org](https://arxiv.org/abs/2608.27238)
- **Philosophy of Loop Engineering** — The CASE Framework: A Multi-Disciplinary Control Archi… · [arxiv.org](https://arxiv.org/abs/2608.10153)
- **Anthropology of Agentic AI** — Why the organisations seeing real returns from agentic… · [news.google.com](https://news.google.com/rss/articles/CBMiyAFBVV95cUxOLVNwMG1CWksyWS1BdmpDdlFzSElkbVU4OTVCc2ZwdElmczg2Snl0SVFQTFpRcVdFUGlBc0htd2JFUXpDNjQ2OXRHMnZVbkdpeDRtdEJFQU5JR0FOZ2RJWldlUWxkeVJmRTlacVJIZkdGYjlyR1ZwYS1fMy1iNElCdGllbHZWWm5kcmhSWWR4MWJ3YlVPWVllcVB4dWtIV25XYWoyLXhKN042OTk4RjNiWmcwWk5pSGNYSEJRN3ZHRmx6dDhwTFYwbA?oc=5)
- **History of Automation** — AI Agents Push Humans Out of the Loop · [arxiv.org](http://arxiv.org/abs/2608.23642v1)
- **DDD** — Towards Standardized Evaluation in Automated Domain Mo… · [arxiv.org](https://arxiv.org/abs/2608.15255)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMは2026年7月からGemini Notebookへ** — Google公式ページは、NotebookLMが2026年7月よりGemini Notebookになったと説明している。 〔技術: ソースグラウンディング型のノートAIが、Geminiブランド下のリサ…／人文: 名称変更は単なるブランディングではなく、「ノートを取る」行為が「AI…〕 · [notebook.google](https://notebook.google/?hl=ja)
- [ ] **日本語実務向けの最新解説: 音声解説・動画解説・Deep Researchまで整理** — Gemini Notebook（旧NotebookLM）の機能一覧、使い方、料金、日本語対応を日本語で整理した記事。 〔技術: 引用付きチャット、音声/動画生成、マインドマップ、フラッシュカード、…／人文: 資料を「読む」だけでなく「聞く」「見る」「試験で確かめる」へ変換する…〕 · [shift-ai.co.jp](https://shift-ai.co.jp/blog/24690)
- [ ] **業務活用の焦点: 営業・人事・研究開発で“根拠付きAI”を使う** — NotebookLMを「ユーザーの資料だけを根拠に回答するAIリサーチアシスタント」として紹介し、営業/企画、人事/研修、研究/… 〔技術: 回答に引用元を付けるソースグラウンディングにより、一般的なチャットA…／人文: 企業内の知識はしばしば属人化するが、NotebookLM型の共有ノー…〕 · [japan-ai.co.jp](https://japan-ai.co.jp/media/8214)
- [ ] **日本語の手順型ガイド: 9種類のソースとStudio機能を実操作ベースで解説** — Googleアカウントでの開始、ノートブック作成、PDF/Googleドキュメント/URL/YouTube/音声/画像などのソー… 〔技術: 多形式ソースを一つのノートブックに集約し、質問応答と生成物作成を同じ…／人文: 初学者向けの長い手順記事は、AIツールが「すごいデモ」から「迷わず使…〕 · [aquallc.jp](https://www.aquallc.jp/notebooklm-guide)
- [ ] **公式日本語コミュニティによる基礎解説: 情報整理AIとしての入口** — NotebookLMを、手元の資料をもとに情報整理、要約、質疑応答、アイデア出しを支援するAIリサーチアシスタントとして紹介して… 〔技術: 汎用チャットではなく、アップロード資料やURLなどユーザー指定ソース…／人文: 日本語圏でのAI導入は、英語圏の新機能ニュースより「自分の仕事や学習…〕 · [note.com](https://note.com/google_gemini/n/n75516598b159)

### Loop engineering
- [ ] **Safety Does Not Compose: Non-Decaying Loop State for Autonomous LLM Agents** — 自律LLMエージェントの安全監視が「単一trajectory」ごとにリセットされると、複数反復に分割された攻撃証拠を検出できない… 〔技術: ループをまたいで消えない安全状態を第一級の設計対象にすることで、エー…／人文: ethics の観点では、「忘れる監視」は責任の分断を生み、長期的な…〕 · [arxiv.org](https://arxiv.org/abs/2608.27141)
- [ ] **dmx: configurable, gated loops for coding agents** — dmx は Cursor、Claude Code、Copilot などのMCP対応IDE内で動く、AIネイティブなエンジニアリン… 〔技術: MCPを入口にして、探索・編集・検証・承認のループをIDE横断で外付…／人文: philosophy の観点では、これは「エージェントの自由」を奪う…〕 · [dmx.deepmodel.ai](https://dmx.deepmodel.ai)
- [ ] **Axiom Sentinel: agent loop と runaway LLM cost を止めるMCPサーバー** — Axiom Sentinel は「Stop agent loops and runaway LLM cost」を掲げるリモートM… 〔技術: ループの実行そのものではなく、コスト・変更・鼓動・証跡を外部から観測…／人文: anthropology の観点では、AI運用にも「番人」「会計係」…〕 · [github.com](https://github.com/oov1317/axiom-sentinel)
- [ ] **otelcol-genai-sketches: agent traffic をbounded metricsに落とす可観測性ループ** — OpenTelemetry traces から、全ての高カーディナリティ値を保存せずに、GenAIリクエストやトークン量、プロン… 〔技術: エージェントループの改善には、各反復のログを無限に抱えるのではなく、…／人文: narrative の観点では、観測指標はチームが「何が起きたのか」…〕 · [github.com](https://github.com/llm-measurement/otelcol-genai-sketches)
- [ ] **AI4AI-Bench: Benchmarking LLM Agents in Algorithmic Design for Recursive Self-Improvement** — AIがAIの訓練アルゴリズムを改善できるかを測るベンチマークで、10種類の訓練アルゴリズムファミリにまたがる凍結リポジトリを用意… 〔技術: 反復的なコード編集ループを、再現可能な訓練実行と隠れた評価器へ接続す…／人文: philosophy の観点では、「自分を改善する主体」をどう評価す…〕 · [arxiv.org](https://arxiv.org/abs/2608.20318)

### AWS
- [ ] **Amazon Bedrock AgentCore Memory がきめ細かなアクセス制御と柔軟な名前空間を追加** — Amazon Bedrock AgentCore Memory が、AgentCore Gateway 経由のユーザー別・テナン… 〔技術: マルチテナントSaaS型エージェントで最も危険な「記憶の混線」を、ア…／人文: AIエージェントの記憶は単なるキャッシュではなく、ユーザーの過去・組…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/agentcorememory-fine-grained-access-control)
- [ ] **Amazon Redshift が Agent Toolkit for AWS と統合し、Claude Code / Kiro / Cursor からデータウェアハウス管理へ** — Amazon Redshift が Agent Toolkit for AWS と統合し、Claude Code、Kiro、Cu… 〔技術: データウェアハウス運用がCLIやコンソール中心から、MCPを介したエ…／人文: データ基盤の管理は、専門家だけが儀式的に触る領域から、対話的な共同作…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/redshift-agenttoolkit-for-ai-assisted-datawarehouse-mgmt)
- [ ] **AWS Glue 6.0 が一般提供、30%低価格化と Apache Iceberg v3 対応** — AWS Glue 6.0 が一般提供され、Apache Spark 4.1、Python 3.13、Scala 2.13 を含む… 〔技術: Iceberg v3対応とランタイム更新により、サーバーレスETLを…／人文: データ基盤の進化は華やかな生成AIの裏側で、組織が「過去の記録をどう…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-glue-6-0-now-available-with-30-lower-price-and-full-apache-iceberg-v3-support)
- [ ] **Amazon EKS がマネージドな証明書認証局ローテーションを提供し、障害時アクセス設計も再注目** — Amazon EKS がクラスターCAのローテーションを、管理されたライフサイクルと自動セーフガード付きで実行できるようにした。 〔技術: CAローテーションと緊急時IAMロール設計は、Kubernetesク…／人文: 障害時アクセスは、単なるバックドアではなく「非常時に誰を信頼するか」…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-eks-certificate-authority-ca-rotation-automated-lifecycle-management)
- [ ] **arXiv: Amazon EKS上のVPCネイティブPod展開を400ノード規模で測定** — 論文「Fleet-Scale Pod Deployment with VPC-Native Networking in Mana… 〔技術: EKSのネットワークモード選択を、スループットや定常時レイテンシでは…／人文: コンテナ基盤の性能差は、最終的には障害復旧時の待ち時間や、開発者が不…〕 · [arxiv.org](https://arxiv.org/abs/2608.22210)

### Harness engineering
- [ ] **Claude Code 2.1.251: モデル切替フック、キャッシュ可視化、権限境界修正** — Claude Code 2.1.251では `PreModelSwitch` / `PostModelSwitch` フック、P… 〔技術: モデル選択、プロンプトキャッシュ、subagent観測、ファイル権限…／人文: これは開発者がAIに「任せる」だけでなく、AI労働の作業環境・監査線…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **Verify Smarter, Evolve Further: Efficient Harness Evolution through Behavior-Aware Verification** — Agent harnessが指示、ツール、ランタイム部品をどう使わせるかを形作る一方、ハーネス候補を固定タスク全体で毎回検証する… 〔技術: ハーネス改善を「候補生成→全量評価」ではなく、どの振る舞いが変わった…／人文: AIの改善がブラックボックスの能力上昇ではなく、失敗の履歴に応じて制…〕 · [arxiv.org](https://arxiv.org/abs/2608.27311v1)
- [ ] **When Context Gets Root: Privilege Escalation in LLM Harnesses** — Instruction hierarchyはモデル側で命令の権限レベルを分ける防御だが、エージェント実行時のハーネスが文脈を組み… 〔技術: プロンプトインジェクション対策をモデル内部の階層だけでなく、ハーネス…／人文: 「誰の言葉が命令として通るのか」という問題は、単なるセキュリティ設定…〕 · [arxiv.org](https://arxiv.org/abs/2608.27299v1)
- [ ] **Same Model, Different Harness: Different Coding-Agent Results** — 同じモデルと同じタスクでも、ハーネスが何を見せ、どのツールを許し、作業をどう継続させるかによって、coding agentの結果… 〔技術: ベンチマーク結果をモデル名だけで比較する危うさを示し、context…／人文: 「同じ人でも職場環境で成果が変わる」のと同じく、AIの能力も環境に分…〕 · [arxiv.org](https://arxiv.org/abs/2608.26218v1)
- [ ] **JIT-Agent: Scaling Harness Intelligence via Just-in-Time Harness Evolution** — Agent能力はモデルだけでなく、memory management、planning strategy、action prot… 〔技術: ハーネスを手書きの周辺コードではなく、学習・合成・適応の対象にしてお…／人文: これは「賢い個体」を作る物語から、「状況ごとに作業環境を組み替える社…〕 · [arxiv.org](https://arxiv.org/abs/2608.25593v1)

### sharp LLM usage
- [ ] **Rudder: 仕様をテストで測る、後付けSpec-Driven Development** — RudderはClaude CodeやCodex向けのローカルプラグインで、セッション履歴や既存specから仕様を生成し、その仕… 〔技術: プロンプト履歴、仕様文書、単体テスト、カバレッジを同じループに入れ、…／人文: これはAIに仕事を任せるというより、人間の曖昧な依頼を監査可能な契約…〕 · [github.com](https://github.com/RudderCode/Rudder)
- [ ] **“How to Claude Like Anthropic”: 多数エージェント運用と手動検証ループの対比** — Anthropic社内の例として「2人のリードエージェント、複数のPM/Tech Lead、各プロジェクト5〜10のICエージェ… 〔技術: 実装セッション、レビューセッション、修正セッション、E2E確認を分離…／人文: 「自動化されていないから遅い」のではなく、「読める報告があるから信頼…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49396175)
- [ ] **CritICL: 小さいモデルの失敗を、強いモデルの推論コンテキストに変える** — CritICLは、同一ファミリー内の弱いモデルが示す失敗モードを抽出し、それを批判的なin-context例として強いモデルの推… 〔技術: 「失敗例」を捨てずに構造化し、動的または静的な批評コンテキストとして…／人文: 人間の熟達も失敗の蓄積から生まれますが、この論文はそれをLLMの文脈…〕 · [arxiv.org](https://arxiv.org/abs/2608.27455v1)
- [ ] **NIS-Agent: Deep Researchの「自分の前提に引っ張られる」問題を文脈分離で抑える** — “From Inertia to Objectivity”は、検索エージェントが自分で立てたクエリ・計画・中間結論を後続判断で過… 〔技術: エージェントの行動履歴を全部コンテキストに入れるのではなく、判断が歪…／人文: 人は自分が言ったことに縛られますが、LLMエージェントも同じように「…〕 · [arxiv.org](https://arxiv.org/abs/2608.23045v2)
- [ ] **Anchoring Bias in LLM-as-a-Judge: 評価メタデータが検証者を汚染する** — LLM-as-a-Judgeに過去スコア、試行番号、改訂情報などのメタデータを与えると、評価がそのアンカーへ体系的に引き寄せられ… 〔技術: 検証用LLMに与えるコンテキストの中でも、 prior score…／人文: 評価は中立に見えても、制度や履歴に引っ張られます。〕 · [arxiv.org](https://arxiv.org/abs/2608.25869v1)

### AI agent trends
- [ ] **Terminal-Bench-Science 0.1: 研究ワークフローでAIエージェントを評価** — Terminal-Bench-Science 0.1 は、Stanford University と Terminal-Benc… 〔技術: コーディング単体ではなく、科学者が実際に行う端末ベースの検証可能な作…／人文: 研究者自身がベンチマークを作る点が重要で、AIの進歩を「ベンダーが測…〕 · [terminal-bench-science.ai](https://www.terminal-bench-science.ai/announcement)
- [ ] **Concord MCP: Claude Code、Codex、Cursorなどを会話させるローカルファースト協調層** — Concord MCP は、Claude Code、Codex、Cursor、Gemini CLI、Grok Build などの… 〔技術: MCPを「外部ツール接続」だけでなく、複数ハーネス間の共有作業状態・…／人文: これはAI同士の協働というより、人間チームの暗黙的な段取りや縄張り調…〕 · [github.com](https://github.com/Get-Concord-AI/concord-mcp)
- [ ] **WikiSkill: エージェント経験を永続知識にまとめてスキル進化へつなげる** — WikiSkill は、エージェントの実行経験、蓄積知識、実行可能スキルを分離し、経験を継続的にwikiへ統合してからスキル更新… 〔技術: 単発の会話ログではなく、経験を再利用可能な知識基盤へ圧縮してスキルを…／人文: 「経験が技能になる」過程をAIで制度化する研究であり、徒弟制や組織学…〕 · [arxiv.org](https://arxiv.org/abs/2608.27454)
- [ ] **Do User-Authored Permission Policies Improve Protection Against AI Agent Overreach?: ユーザー作成ポリシーは過剰実行を十分に防ぐか** — この研究は、非専門家ユーザーが「allow / ask / never」の自然言語ポリシーでAIエージェントの行動を事前制御でき… 〔技術: エージェント権限を静的ルールに落とすだけでは安全性が自動的に上がらず…／人文: 自由に選べることと、将来の自分を拘束するルールを作ることは別物だと分…〕 · [arxiv.org](https://arxiv.org/abs/2608.27443)
- [ ] **agentd: 複数コーディングエージェントのフックを一つのローカルデーモンで守る** — agentd は、Claude Code、Cursor、Codex、Gemini CLI、OpenCode、Kimi Code… 〔技術: 各エージェントごとに散らばるhook/permission/obse…／人文: エージェントを“野良の便利ツール”ではなく、職場の監査・習慣・リスク…〕 · [github.com](https://github.com/macrox-pro/agentd)

### Claude Code
- [ ] **Claude Code 2.1.251: symlink差し替え、plugin path traversal、モデル切替hookをまとめて塞ぐ運用寄りリリース** — v2.1.251 では、権限チェック後に作業ディレクトリ内の symlink を差し替えて Read/Write/Edit が許… 〔技術: ファイルシステム境界、plugin supply chain、モデル…／人文: AIに「作業してもらう」段階では便利さが目立つが、AIを業務環境に入…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **日本語圏の v2.1.251 解説: 「承認後のsymlink差し替え」を日常運用のリスクとして翻訳する動き** — Qiita では、v2.1.251 の symlink 差し替え修正、Grep/Glob の deny ルール適用、Workfl… 〔技術: 公式のセキュリティ修正を、`permissions.deny`、sy…／人文: 技術の普及は英語の一次情報だけでは完結せず、母語コミュニティが「どこ…〕 · [qiita.com](https://qiita.com/moha0918_/items/08dfa2f03d89272498dc)
- [ ] **Claude Codeを自走させる4つの道具: `/goal`、`/loop`、Cron、Workflowの使い分け** — この記事は、Claude Code を人間の逐次入力から離して動かす道具として、`/goal`、`/loop`、Cron、Wor… 〔技術: Claude Code の自律性を「長いプロンプト」ではなく、完了条…／人文: 人間がAIに何度も声をかける関係から、AIが動き続ける制度を設計する…〕 · [qiita.com](https://qiita.com/NaokiIshimura/items/71af4e891b2f8f1e7943)
- [ ] **Claude CodeのRemote Controlを任意フォルダで開始する: tmuxを足場にした現場的な遠隔運用** — この記事は、`claude remote-control` のサーバモードではなく、`tmux new-session -d -… 〔技術: Remote Control をクラウド機能だけに閉じず、tmux…／人文: 新しいAI機能は、必ずしも新しいUIだけで広がるわけではない。〕 · [qiita.com](https://qiita.com/tamuto/items/4ee0d97f7fd51cf276f4)
- [ ] **arXiv “Claude Code Complete User Handbook”: 能力ではなく制御スタックとしてClaude Codeを読む** — “Claude Code Complete User Handbook” は、Claude Code をファイルアクセス、she… 〔技術: Claude Code の失敗モードをローカルなプロンプトミスではな…／人文: AIエージェントの利用者は、もはや「良い指示を書く人」だけでは足りず…〕 · [arxiv.org](https://arxiv.org/abs/2608.26742)

### Ethics of AI Agents
- [ ] **Assessing Company Contributions to Societal Resilience: Extending the Societal Capacity Assessment Framework to Agentic AI** — AIエージェントを提供・配備する企業を、単なる技術提供者ではなく社会のレジリエンスを左右する制度的アクターとして扱う論文。 〔技術: エージェント安全をモデル単体の評価ではなく、配備企業の設計・監視・是…／人文: 責任所在を「開発者か利用者か」の二択に閉じず、企業が社会的能力を形成…〕 · [arxiv.org](https://arxiv.org/abs/2608.27238)
- [ ] **Five Primitives for Governing Autonomous AI Agents at Runtime** — 自律AIエージェントの企業利用では、従来の人間ユーザーや長寿命サービス向けアクセス制御が合わないと指摘し、実行時ガバナンスのため… 〔技術: 実行時の権限、観測、制約、監査を「エージェント固有のプリミティブ」と…／人文: これは倫理を行動規範の文章ではなく、日々の業務システム内で誰が何を許…〕 · [arxiv.org](https://arxiv.org/abs/2608.26696)
- [ ] **Risks and Controls for Multi-Agent Systems: an analytical framework for deployment of AI agents across organisational boundaries** — 組織内、取引先、顧客、サプライヤー、未知の相手先まで、AIエージェント同士が組織境界を越えて相互作用する時のリスクと統制策を整理… 〔技術: マルチエージェント環境を境界条件別に分解し、認証、ポリシー、監視、隔…／人文: 組織境界を越えるエージェントは、社会学でいう信頼・契約・慣行のインフ…〕 · [arxiv.org](https://arxiv.org/abs/2608.26626)
- [ ] **HRGuard: Gating Relationship Manipulation in Multi-Turn Agentic AI Conversations** — エージェント型AIアシスタントが、人間同士の関係を操作するために悪用されるリスクを扱う研究。 〔技術: マルチターン会話における意図・役割・被害文脈を判定し、同じ「人間関係…／人文: AIエージェント倫理がプライバシーや誤情報だけでなく、親密圏・家族・…〕 · [arxiv.org](https://arxiv.org/abs/2608.25340)
- [ ] **HANSARD: A Reference Architecture for Forensic Readiness, Runtime Witnessing, and Graded Attribution in Autonomous Multi-Agent AI Systems** — 金融、ソフトウェアサプライチェーン、セキュリティ運用などで自律マルチエージェントが害を起こした時、何が起き、何が原因で、誰が責任… 〔技術: フォレンジック準備性、ランタイム証言、原因連鎖、段階的アトリビューシ…／人文: 責任は事故後の非難ゲームではなく、証拠が残るように社会的記憶を設計し…〕 · [arxiv.org](https://arxiv.org/abs/2608.22512)

### Philosophy of Loop Engineering
- [ ] **The CASE Framework: A Multi-Disciplinary Control Architecture for Governing Enterprise Agentic AI** — 企業のエージェントAI統治を、単一のDevSecOps問題ではなく、制御理論・複雑適応系・監督サイバネティクス・Engineer… 〔技術: ループ設計を「監視を足す」ではなく、観測可能性・フィードバック・エラ…／人文: これはエージェント時代の責任論を、個人の注意力ではなく制度・組織・観…〕 · [arxiv.org](https://arxiv.org/abs/2608.10153)
- [ ] **Argus: A General-Purpose Agentic Reasoning Runtime for Long-Horizon Tasks** — Argus は Manager / Planner / Engineer / Reviewer が耐久的なプロジェクト状態の上で… 〔技術: 失敗を検知したら方針転換し、検証済みの経験だけを状態に蓄積するため、…／人文: 実践知は一度の推論で完成するものではなく、棄却された道筋やレビューさ…〕 · [arxiv.org](https://arxiv.org/abs/2608.05144)
- [ ] **OwnFramework Loop** — AI coding agent 向けの deterministic / execution-sealed engineering… 〔技術: 「ビルドするエージェント」と「レビューするエージェント」をSHA単位…／人文: ここでの人間は毎回クリック承認する監督者ではなく、目的を発する者・昇…〕 · [github.com](https://github.com/william-london/ownframework-loop)
- [ ] **NVIDIA-labs OO Agents: Native Python Object-Oriented Agents** — NVIDIA Object-Oriented Agents は、エージェントをPythonオブジェクトとして扱い、メソッドを行動… 〔技術: ループを隠れたプロンプト連鎖ではなく、型・状態・メソッド・ハーネスA…／人文: エージェントを「対話する他者」と見るだけでなく、オブジェクト・契約・…〕 · [arxiv.org](https://arxiv.org/abs/2607.20709)
- [ ] **Humans and Agents in Software Engineering Loops** — ソフトウェア開発における人間とエージェントの関係を、単純な自動化ではなく複数のループとして考える記事。 〔技術: coding agent の価値を、コード生成量ではなく、人間がどの…／人文: ループの哲学は、主体を「人間かAIか」の二択でなく、相互に補正し合う…〕 · [martinfowler.com](https://martinfowler.com/articles/exploring-gen-ai/humans-and-agents.html)

### Anthropology of Agentic AI
- [ ] **Why the organisations seeing real returns from agentic AI are empowering employees, not cutting jobs** — Agentic AI の投資対効果を「人員削減」ではなく、従業員の権限委譲・現場判断・ワークフロー再設計から捉える記事。 〔技術: ROIの論点を、モデル性能ではなくエージェントが現場プロセスにどう埋…／人文: 労働人類学的には、AI導入は「仕事の消滅」よりも、誰が承認し、誰が例…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiyAFBVV95cUxOLVNwMG1CWksyWS1BdmpDdlFzSElkbVU4OTVCc2ZwdElmczg2Snl0SVFQTFpRcVdFUGlBc0htd2JFUXpDNjQ2OXRHMnZVbkdpeDRtdEJFQU5JR0FOZ2RJWldlUWxkeVJmRTlacVJIZkdGYjlyR1ZwYS1fMy1iNElCdGllbHZWWm5kcmhSWWR4MWJ3YlVPWVllcVB4dWtIV25XYWoyLXhKN042OTk4RjNiWmcwWk5pSGNYSEJRN3ZHRmx6dDhwTFYwbA?oc=5)
- [ ] **From AI assistant to capable teammate: How Copilot Cowork is changing the way we work at Microsoft** — Copilot Cowork を「assistant」から「capable teammate」へ移行する事例として紹介する Mi… 〔技術: エージェントの価値がチャット応答ではなく、組織内の複数ツールと作業文…／人文: 「同僚」という比喩は、AIを人格化するだけでなく、挨拶・依頼・確認・…〕 · [news.google.com](https://news.google.com/rss/articles/CBMi2AFBVV95cUxOTzNhQ0VpQkxzaG00OTlZUE1kU2xPdUkwVXlaUnFRN1FjcnV2NWp2anYzSXY4WE4zczlPdzZjS1Z5ODY5QXo5SFNXNVR3SEVLWjFuVGdiTGFwWEx0MGtkRWlVdEp0d0lFTHlRdzFqSDZUZ1pxWkRpVGtzblAzcUJoeXRrWW1qM3hHUV9hNjNoWmhXUFp3dC1IUU1xaEpEV2ZzMWFsLWRrVmY2bGU1M2ZoQlBxWnE0TnFxQlM1X3Q4Mmdzb1I5UFYxZ2JfcWNrX0I5di02MHJZVG4?oc=5)
- [ ] **AI Agents Push Humans Out of the Loop** — AIエージェントの設計は「human in the loop」を解決策として掲げつつ、実際には人間の監督を難しくし、長期利用によ… 〔技術: エージェントの自律性・速度・複雑なツール連鎖が、人間のレビュー可能性…／人文: これは監督を「ボタンを押す役割」ではなく、経験・注意・技能・責任感か…〕 · [arxiv.org](http://arxiv.org/abs/2608.23642v1)
- [ ] **SPECMINE: A Large-Scale Corpus of Spec-Driven Development Artifacts** — AIコーディングエージェント時代の Spec-Driven Development において、自然言語仕様がどのように書かれ、キ… 〔技術: Kiro、OpenSpec、GitHub Spec Kit などの流…／人文: 開発チームにとって仕様は、単なる入力ではなく「意図を公的に固定する文…〕 · [arxiv.org](http://arxiv.org/abs/2608.25202v1)
- [ ] **ComBodied Agents: a New Paradigm of Human-Centric Agentic AI** — デジタルエージェントと身体化エージェントのどちらも、人間の状態・意図・エージェンシーを中心に据えきれていないとして、ComBod… 〔技術: ソフトウェア状態の変換と物理状態の変換を統合し、人間の変化する状態を…／人文: ケアの場面では、エージェントの行為は文化的に意味づけられた身体接触・…〕 · [arxiv.org](http://arxiv.org/abs/2608.10915v2)

### History of Automation
- [ ] **AI Agents Push Humans Out of the Loop** — AIエージェントに自律性を与えるほど、「human in the loop」という安全策そのものが機能しにくくなると論じる論文で… 〔技術: 監督者の認知負荷・状況把握・介入可能性を、エージェント設計の一級要件…／人文: 産業革命期の機械監督からテイラー主義、RPA監視、AIエージェント監…〕 · [arxiv.org](http://arxiv.org/abs/2608.23642v1)
- [ ] **Using profiles of cognitive capability to assess AI suitability for workplace tasks** — 職場タスクを単純に「自動化できる／できない」で分けるのではなく、AIエージェントとタスクの双方を共通の認知能力プロファイルで評価… 〔技術: タスク要求とAI能力を同じ認知次元で表現することで、自動化・人間保持…／人文: 自動化の歴史では、仕事はしばしば職業単位で語られてきましたが、この論…〕 · [arxiv.org](http://arxiv.org/abs/2608.25623v1)
- [ ] **Cheap, Fallible Cognition and the Political Economy of Expertise** — 「AIは雇用を破壊するか」という粗い問いではなく、生成AIを「安価でスケールするが誤りうる認知」として捉え、検証・責任・信頼・ガ… 〔技術: モデル性能だけでなく、検証コスト・責任所在・ワークフロー再設計を採用…／人文: 自動化史で繰り返された「機械が仕事を奪う」という物語を、専門知・権威…〕 · [arxiv.org](http://arxiv.org/abs/2608.11512v1)
- [ ] **自動化の教科書｜進め方・事例20選・おすすめツールを完全網羅【2026年最新版】** — 人手不足、働き方改革、生成AI・AIエージェントの普及を背景に、RPA、ノーコード、内製、外注などを組み合わせて小さく試し、効果… 〔技術: RPA中心の定型作業自動化から、生成AI・AIエージェントを含むハイ…／人文: 歴史的には、工場の機械化もオフィスのRPAも「不足する労働力を補う」…〕 · [sms-datatech.co.jp](https://www.sms-datatech.co.jp/column/aut_automation-all)
- [ ] **Applied and Filtered: An End-to-End Algorithmic Fairness Audit of A Public Employment Agency** — バルセロナの公共雇用機関が利用する半自動採用システムについて、2017〜2022年の約49.7万件の候補者・求人パイプラインを対… 〔技術: アルゴリズム単体ではなく、データ入力から人間の裁量、最終判断までのエ…／人文: 自動化の歴史では、選別・分類・標準化は常に制度権力と結びついてきまし…〕 · [arxiv.org](http://arxiv.org/abs/2608.13022v1)

### DDD
- [ ] **Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark** — 自然言語記述からドメインモデルを生成する自動モデリング手法を比較するため、既存のGolden UML Modelsetなどを組み… 〔技術: LLMで作ったドメインモデルを雰囲気ではなく参照モデルとメトリクスで…／人文: DDDのモデルは本来、組織の会話と合意の産物ですが、この研究はその一…〕 · [arxiv.org](https://arxiv.org/abs/2608.15255)
- [ ] **DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python** — 要求仕様書から型付きのDDDモデルを抽出し、PythonコードをAST解析・import topology・RAG付きトレーサビ… 〔技術: DDDを「設計ワークショップの成果」から「継続的に検査されるアーキテ…／人文: 仕様書・コード・診断をつなぐことで、設計判断の責任を個人の記憶ではな…〕 · [github.com](https://github.com/barandincoguz/DDD-Enforcer)
- [ ] **LLM_Ontology_DDD: Hybrid LLM–Ontology Approach for Ubiquitous Language** — ユビキタス言語の構築と意味的衝突の解消に、LLMとオントロジーを組み合わせることを掲げたリポジトリです。 〔技術: LLMの柔軟な言語処理とオントロジーの厳密な意味制約を合わせる発想は…／人文: ユビキタス言語はチームの「方言」を作る営みであり、そこには権限、職能…〕 · [github.com](https://github.com/BlayTeuR/LLM_Ontology_DDD)
- [ ] **faceto: typed fileからLLMと考えるイベントストーミングボードへ** — 型付きファイルからHTML/SVGのイベントストーミングボードを生成し、クリックした要素にメモを書いて次のLLMセッションでモデ… 〔技術: AIコーディング前のモデルをファイル・可視化・対話メモとして往復させ…／人文: イベントストーミングの価値は付箋そのものではなく、その場で人々が驚き…〕 · [github.com](https://github.com/bastien-gallay/faceto)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの識別、集約設計、技術アーキテクチャへの… 〔技術: LLMはDDDの全自動化よりも、語彙・イベント・境界の初期整理を助け…／人文: これはAI導入の成熟した態度を示す事例です。〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

# 📰 2026-07-18 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMのGemini Notebookリブランディング · [notebooklm.google](https://notebooklm.google)
- **Loop engineering** — 「The winners won't have the smartest model, they'll ha… · [x.com](https://x.com/0xcodard/status/2078166211494547740)
- **AWS** — Build enterprise search for agents with Amazon Bedrock… · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/build-enterprise-search-for-agents-with-amazon-bedrock-managed-knowledge-base)
- **Harness engineering** — Claude Code Hooks / Agent SDK が“ハーネスの標準部品”になりつつある · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
- **sharp LLM usage** — SearchOS-V1: 失敗記憶と証拠グラフで検索エージェントのループを止める · [arxiv.org](http://arxiv.org/abs/2607.15257v1)
- **AI agent trends** — Claude Code v2.1.214: 権限チェックと運用安全性の集中修正 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.214)
- **Claude Code** — Claude Code Week 29: MCPコネクタ付きArtifactsとスクリーンリーダーモード · [code.claude.com](https://code.claude.com/docs/en/whats-new/2026-w29)
- **Ethics of AI Agents** — AIセーフティに関する評価観点ガイド（第1.20版）の公開 · [aisi.go.jp](https://aisi.go.jp/output/output_information/260707)
- **Philosophy of Loop Engineering** — The Prover Is the Judge: Verified Security Software fr… · [arxiv.org](https://arxiv.org/abs/2607.14340)
- **Anthropology of Agentic AI** — Who will own the AI agent economy? · [mitsloan.mit.edu](https://mitsloan.mit.edu/ideas-made-to-matter/who-will-own-ai-agent-economy)
- **History of Automation** — The Industrialization of Research ; On AI-Driven Scien… · [arxiv.org](http://arxiv.org/abs/2607.15164v1)
- **DDD** — 仕様書は最新に保てない。 · [qiita.com](https://qiita.com/ikeyansaza/items/d96867ba05e337f2e3ac)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMのGemini Notebookリブランディング** — 公式ページのタイトルと説明は「Gemini Notebook | AI Research Tool & Thinking Par… 〔技術: NotebookLMの価値が、単なる要約UIではなく、Geminiエ…／人文: 名前の変更は、ユーザーが道具に抱く期待を変えます。〕 · [notebooklm.google](https://notebooklm.google)
- [ ] **Google Workspace向けGemini Notebookページの日本語展開** — 日本語のWorkspace公式ページでは、Gemini Notebookを「AIを活用した調査と学習のアシスタント ツール」と説… 〔技術: ソースを読み込み、要約・質問応答・学習支援に使う流れがWorkspa…／人文: 組織が「学ぶ速度」を上げる一方で、誰の資料が共有され、どの解釈がチー…〕 · [workspace.google.com](https://workspace.google.com/intl/ja/products/notebooklm)
- [ ] **SHIFT AI TIMESの2026年版NotebookLM解説** — NotebookLMの機能一覧、始め方、具体的な使い方、料金プラン、日本語対応の有無までを初心者向けに整理しています。 〔技術: 機能を「資料投入、要約、質問、アウトプット生成、共有」の運用単位へ分…／人文: NotebookLMの普及は、知的労働の“下ごしらえ”を誰が担うかを…〕 · [shift-ai.co.jp](https://shift-ai.co.jp/blog/24690)
- [ ] **日本語QiitaのNotebookLM完全活用ガイド** — 初心者から上級者までを対象に、NotebookLMを情報の「消化・分析のエンジン」として使う発想を紹介しています。 〔技術: 外部ツールで収集した情報をNotebookLMへ集約し、要約・分析・…／人文: 知識摂取が机の前だけでなく生活時間へ入り込むと、学習は便利になる一方…〕 · [qiita.com](https://qiita.com/TaichiEndoh/items/618bbd5cfa21a5ccc975)
- [ ] **2026年版導入判断記事に見る「料金・統制・注意点」への関心** — 経営・業務責任者向けに、NotebookLMの基本概念、主要機能、料金プラン比較、導入前の注意点をまとめています。 〔技術: NotebookLMを個人の試用から業務プロセスへ移す際、料金、デー…／人文: AIツールは「使えるか」だけでなく「組織でどう許すか」が普及を左右し…〕 · [crystal-method.com](https://crystal-method.com/blog/notebooklm)

### Loop engineering
- [ ] **「The winners won't have the smartest model, they'll have the best loop」という Loop Engineering の急浮上** — X検索では、Anthropic/Claude Code 周辺の文脈で「prompt engineering → context… 〔技術: モデル性能ではなく、状態管理・検証器・再試行・停止条件を含む制御系と…／人文: 哲学的には「知能」を内面能力ではなく、環境内で反復し修正する実践とし…〕 · [x.com](https://x.com/0xcodard/status/2078166211494547740)
- [ ] **Pipeline から Loop へ: generate → evaluate → refine の実務パターン** — 最近のX議論では、AIワークフローを一方向のパイプラインではなく、生成・評価・修正を成功条件まで戻すループとして設計する説明が支… 〔技術: 「前に流す」パイプラインではなく「正しくなるまで戻す」ループにするこ…／人文: 人類学的には、これは職人の反復作業やレビュー文化を機械化する試みであ…〕 · [x.com](https://x.com/maanbarazy/status/2075800316507767199)
- [ ] **24/7 Claude Code チームを動かす「Continuously Looping Engineering Machines」** — GitHub検索では、`jahwag/clem` が「Continuously Looping Engineering Mach… 〔技術: コンテナ、永続プロセス、複数エージェント、状態保存をまとめ、エージェ…／人文: 歴史的には、これはバッチ処理やcron、常駐デーモンの系譜にAIエー…〕 · [github.com](https://github.com/jahwag/clem)
- [ ] **Stop Means Stop: agent framework の「停止」「承認」「タイムアウト」は本当に停止しているか** — `Stop Means Stop: Measuring and Repairing the Enforcement Gap in… 〔技術: 長く回るループでは「開始」より「止められること」の方が安全要件になり…／人文: 倫理的には、停止ボタンが象徴ではなく実効的権限であることが、人間の統…〕 · [arxiv.org](http://arxiv.org/abs/2607.14166v1)
- [ ] **評価器のバイアスが agent の行動ループに伝播する問題** — `Calibrating the Evaluator: Does Probability Calibration Mitigat… 〔技術: evaluator をループに組み込むほど、評価器の偏りが自己強化さ…／人文: 哲学的には、判断者の価値観が反復を通じて世界を形作るという、制度と規…〕 · [arxiv.org](http://arxiv.org/abs/2606.31371v1)

### AWS
- [ ] **Build enterprise search for agents with Amazon Bedrock Managed Knowledge Base** — Amazon Bedrock Managed Knowledge Baseを使い、エージェント向けのエンタープライズ検索を構築す… 〔技術: RAG/検索基盤を「チャットボットの補助」ではなく、エージェントが業…／人文: 組織の知識がエージェントに読める形で再編成されると、情報検索の権力構…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/build-enterprise-search-for-agents-with-amazon-bedrock-managed-knowledge-base)
- [ ] **Introducing self-managed Amazon S3 buckets for AWS Lambda function code** — Lambda関数コードの保存先として、ユーザー管理のS3バケットを使える新機能が紹介されています。 〔技術: Lambdaのデプロイ成果物を自社管理S3へ寄せられることで、容量・…／人文: サーバーレスは「運用からの解放」と語られがちですが、成熟した組織では…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/compute/introducing-self-managed-amazon-s3-buckets-for-aws-lambda-function-code)
- [ ] **Eliminating Java cold starts with AWS Lambda Managed Instances** — Java Lambdaのコールドスタートを抑えるためのLambda Managed Instancesが紹介されています。 〔技術: JVMのウォームアップ特性とLambdaの実行モデルのギャップを、ア…／人文: 「一瞬遅いだけ」のコールドスタートは、オンコール担当者やユーザー体験…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/compute/eliminating-java-cold-starts-with-aws-lambda-managed-instances)
- [ ] **AWS Sustainability service now includes water withdrawals data** — AWS Sustainabilityで、既存の炭素排出データに加えて、AWSワークロードに関連する年間の水取水量データを確認でき… 〔技術: ワークロードの環境メトリクスが炭素中心から水使用へ広がることで、設計…／人文: AIとクラウドの成長は、データセンターの電力だけでなく地域の水資源と…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-sustainability-water-withdrawals)
- [ ] **【開催報告】AWS Summit Japan 2026 〜 Future of Agentic Commerce ブース** — AWS Summit Japan 2026の「Future of Agentic Commerce」ブース開催報告です。 〔技術: Agentic Commerceは、Bedrockなどの生成AI基盤…／人文: 買い物は単なるトランザクションではなく、選択・信頼・欲望・説明責任の…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-summit-japan-2026-future-of-agentic-commerce)

### Harness engineering
- [ ] **Claude Code Hooks / Agent SDK が“ハーネスの標準部品”になりつつある** — Claude Code の hooks は、ツール実行前後・セッション開始/停止・通知・MCP ツールなどのライフサイクルに対し… 〔技術: ハーネスがプロンプト集ではなく、イベントスキーマ・権限・観測性・停止…／人文: これは開発者とAIの関係を「お願いする/信じる」から「制度を設計し、…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [ ] **polyhook: AIコーディングツール横断のHook抽象化** — polyhook は Claude Code、Cursor、Windsurf、Cline、Amp などの異なる hook 入出力… 〔技術: ハーネスの重要部品である guard / approval / mo…／人文: 生成AI時代の開発文化では、個々のツールへの忠誠よりも“移植できる作…〕 · [github.com](https://github.com/polyhook/polyhook)
- [ ] **claude-harness: 日本語優先・Boris式を明示した Claude Code スターターキット** — 日本語ファーストの Claude Code スターターキットで、README は「ハーネスエンジニアリング＝AIエージェントを動… 〔技術: 日次リサーチ、適用、検証、レポートを一体化し、Claude Code…／人文: README に「Boris 式 AI 駆動経営」とあり、Boris…〕 · [github.com](https://github.com/Hyphen-Tech-Org/claude-harness)
- [ ] **Manifold: “判断”をファイル化するポータブル・エンジニアリングハーネス** — Manifold は Claude Code 向けに、methodology、skills、principles、rules、t… 〔技術: project-agnostic な core と project-…／人文: ここで保存されるのはコードだけでなく「なぜそのルールがあるのか」とい…〕 · [github.com](https://github.com/ricardojustus/manifold)
- [ ] **ClayBuddy: コーディングエージェント失敗を“ハーネスエラー”として分類・緩和する研究** — “ClayBuddy: A Framework, Evaluation, & Mitigation of Coding Agen… 〔技術: 失敗を「モデルが悪い」で終わらせず、ハーネスが安全行動を実行させ損ね…／人文: これはAIエージェントにおける責任の所在を再設計する研究でもある。〕 · [arxiv.org](https://arxiv.org/abs/2606.19380)

### sharp LLM usage
- [ ] **SearchOS-V1: 失敗記憶と証拠グラフで検索エージェントのループを止める** — Web検索型エージェントが長い履歴の中で進捗を見失い、同じ失敗検索を繰り返す問題に対して、Frontier Task、Evide… 〔技術: プロンプト履歴に暗黙の状態を押し込まず、探索範囲・証拠・未完了・失敗…／人文: 調査とは「答えを出す」だけでなく、どこを探し、何が見つからず、なぜ次…〕 · [arxiv.org](http://arxiv.org/abs/2607.15257v1)
- [ ] **Bad Codex bug: フルアクセスのコーディングエージェントはファイル削除まで失敗する** — GPT-5.6/Codexが、フルアクセスかつサンドボックスや自動レビューなしの条件で、意図せずファイル削除に至る事例を紹介。 〔技術: コーディングLLMの実運用では、モデル性能よりも権限境界、サンドボッ…／人文: 「賢い助手」に全権を渡すと、失敗は創造的ミスではなく組織的事故になり…〕 · [simonwillison.net](https://simonwillison.net/2026/Jul/16/bad-codex-bug)
- [ ] **Libretto PR Agents: Playwrightの失敗を、その場でAIがPR化して直す** — 既存のPlaywrightスクリプトに`debugFailure()`を足すだけで、失敗時にライブページを調査し、修正案をGit… 〔技術: ブラウザ自動化の本番フローをLLMで置換するのではなく、失敗パスにだ…／人文: 自動化の現場で本当に苦しいのは「毎日動くこと」より「壊れた理由を追う…〕 · [libretto.sh](https://libretto.sh/debug-agents)
- [ ] **Kote: AIチャットとGit履歴を“後から使える開発文脈”として保存する** — Antigravity、Codex、Claude Code、OpenCodeなどのAIチャット、Git push、開発メモを自動… 〔技術: コンテキストエンジニアリングを「毎回プロンプトに貼る作業」から、会話…／人文: ソフトウェア開発の知識は、コードそのものより「なぜそうしたか」に宿り…〕 · [github.com](https://github.com/pedroaugusto04/Kote)
- [ ] **Better Models: Worse Tools — 新しいClaudeほどツール呼び出しが壊れる事例** — 新しいClaudeモデルで、特定のエージェント履歴を経たあとにツール呼び出しJSONへ余計な内容が混入し、編集系ツールが失敗する… 〔技術: LLM評価は単発ベンチでは足りず、長いエージェント履歴、複数ツール、…／人文: 道具の進歩は直線的ではなく、ある能力が伸びると別の信頼性が落ちること…〕 · [lucumr.pocoo.org](https://lucumr.pocoo.org/2026/7/4/better-models-worse-tools)

### AI agent trends
- [ ] **Claude Code v2.1.214: 権限チェックと運用安全性の集中修正** — Claude Code v2.1.214では、`dir/**` allow rule、PowerShell 5.1、Bashリダ… 〔技術: コーディングエージェントの価値がモデル性能だけでなく、権限解析・監査…／人文: エージェントを「賢い部下」として扱うには、信頼ではなく制度設計が必要…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.214)
- [ ] **Claude Code v2.1.212: `/fork`、WebSearch上限、サブエージェント運用の安全弁** — v2.1.212では、会話を別background sessionへコピーする`/fork`、旧来のサブエージェント起動を担う`… 〔技術: エージェント運用が単発チャットから、background sessi…／人文: これは「AIに仕事を任せる」から「複数のAI作業者を監督する」への移…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.212)
- [ ] **Better tools made Copilot code review worse. Here’s how we actually improved it.** — GitHubは、Copilot code reviewを共有Unix風コード探索ツールへ移行したところ、単純なツール強化だけでは… 〔技術: 「強いツールを渡せば良い」ではなく、エージェントがどの証拠を、どの順…／人文: 人間のレビューでも、情報が多すぎると判断が散る。〕 · [github.blog](https://github.blog/ai-and-ml/github-copilot/better-tools-made-copilot-code-review-worse-heres-how-we-actually-improved-it)
- [ ] **Automating cross-repo documentation with GitHub Agentic Workflows** — GitHub Aspireチームは、複数リポジトリにまたがる製品変更を、SMEレビュー付きのドキュメントPull Request… 〔技術: エージェントの有望な適用先が、コード生成そのものだけでなく、リポジト…／人文: ドキュメントは組織の記憶であり、ここを自動化することは「誰が変更の意…〕 · [github.blog](https://github.blog/ai-and-ml/github-copilot/automating-cross-repo-documentation-with-github-agentic-workflows)
- [ ] **How Agents Ask for Permission: User Permissions for AI Agents, from Interfaces to Enforcement** — AIエージェントが普及するほど、prompt injection、幻覚、プライバシー漏洩、意図しない機微操作のリスクが増すとして… 〔技術: ユーザー承認を単なる確認ダイアログではなく、UI、ポリシー、実行時制…／人文: 許可をどう求めるかは、AIと人間の関係をどう礼儀づけるかでもある。〕 · [arxiv.org](https://arxiv.org/abs/2607.13718v1)

### Claude Code
- [ ] **Claude Code Week 29: MCPコネクタ付きArtifactsとスクリーンリーダーモード** — Week 29では、公開Artifactsが閲覧者自身のMCPコネクタを呼び出してライブデータを表示・操作できるようになり、Cl… 〔技術: 生成された成果物が静的なスナップショットではなく、閲覧時にMCP経由…／人文: アクセシビリティ対応は、AI開発ツールが一部の高速キーボードユーザー…〕 · [code.claude.com](https://code.claude.com/docs/en/whats-new/2026-w29)
- [ ] **Claude Code v2.1.214: 権限解析・PowerShell・Docker周辺の安全修正が集中** — v2.1.214は、Bash/PowerShellの権限チェック、長大コマンド、ファイルディスクリプタredirect、Dock… 〔技術: コマンド文字列の静的解析と実シェル解釈のズレを潰す方向で、AIエージ…／人文: 「AIに任せる」とは、単に自動化することではなく、任せた後に誰が説明…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.214)
- [ ] **Claude Code v2.1.212: `/fork`、検索・サブエージェント上限、MCP自動バックグラウンド化** — v2.1.212では、`/fork`が会話を新しいバックグラウンドセッションへコピーする仕様になり、従来のセッション内サブエージ… 〔技術: 並列化・委譲・外部ツール呼び出しを増やすほど暴走リスクが増すため、上…／人文: “AI部下を増やす”比喩は魅力的だが、組織と同じく人数が増えるほど調…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.212)
- [ ] **Claude Code GitHub Action v1.0.177: Claude Code 2.1.214 / Agent SDK 0.3.214へ追従** — `anthropics/claude-code-action`はv1.0.177でClaude Code 2.1.214とAge… 〔技術: ローカルCLIの権限・ログ・ツール実行修正が、そのままPRレビューや…／人文: コードレビューの自動化は、チームの会話にAIが参加することを意味する…〕 · [github.com](https://github.com/anthropics/claude-code-action/releases/tag/v1.0.177)
- [ ] **日本語実践: CLAUDE.md・permissions・hooksを3層で分けるガードレール記事** — 「CLAUDE.mdの禁止はお願いにすぎない」として、CLAUDE.md、permissionsのdeny、PreToolUse… 〔技術: LLMへの自然言語指示、静的deny、実行時hookを分離することで…／人文: 「禁止事項を書いたから大丈夫」という安心は、人間組織でもAI運用でも…〕 · [qiita.com](https://qiita.com/4q_sano/items/aaa12313849ef5999994)

### Ethics of AI Agents
- [ ] **AIセーフティに関する評価観点ガイド（第1.20版）の公開** — Japan AISIが、AIエージェントシステムの普及を踏まえて「AIセーフティに関する評価観点ガイド」を第1.20版に更新した… 〔技術: エージェントを単なるLLM出力ではなく、外部システムに作用する制御対…／人文: 「安全」はモデル単体の善悪ではなく、人間がどこで見守り、どこで止めら…〕 · [aisi.go.jp](https://aisi.go.jp/output/output_information/260707)
- [ ] **人工知能基本計画（第Ⅱ期）の閣議決定** — 内閣府が「人工知能基本計画（第Ⅱ期）」を閣議決定し、AI法、適正性確保指針、AIセーフティ・インスティテュート等と接続する政策体… 〔技術: 基本計画が評価指針やAISIの活動と結びつくことで、エージェントの安…／人文: 「イノベーション促進」と「リスクへの不安」の両立を明示しており、社会…〕 · [www8.cao.go.jp](https://www8.cao.go.jp/cstp/ai/ai_plan/ai_plan.html)
- [ ] **Copewell: A Multi-Agent Swarm Architecture for Equitable Mental Wellness Support** — メンタルウェルネス支援のためのマルチエージェント・スウォーム構成を提案する論文。 〔技術: 複数エージェントのルーティングや感情マッピングに、バイアス緩和と倫理…／人文: メンタルヘルス支援では、効率化だけでなく脆弱な利用者への権力差、文化…〕 · [arxiv.org](https://arxiv.org/abs/2607.02245)
- [ ] **AI検証ノート：AIが見つける脆弱性に違い！** — 複数の一般利用可能なAIモデルにソフトウェア脆弱性検証を行わせ、モデルごとに検出件数・重要度・問題の切り分け方が異なることを確認… 〔技術: エージェント型の開発・検証ワークフローで、モデル差、重要度分類、誤差…／人文: 「AIが危険を見つけた」という語りは説得力を持つが、件数や深刻度の解…〕 · [aisi.go.jp](https://aisi.go.jp/activity/activity_notes/260708)
- [ ] **General-Purpose AI Code of Practice now available** — 欧州委員会が、汎用AIモデル提供者向けのCode of Practice最終版を受領したと公表。 〔技術: 高度な汎用モデルやそれを組み込むエージェントのリスク管理を、透明性文…／人文: 欧州型のアプローチは、利用者や市民社会を含む多数のステークホルダーの…〕 · [digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/news/general-purpose-ai-code-practice-now-available)

### Philosophy of Loop Engineering
- [ ] **The Prover Is the Judge: Verified Security Software from AI Coding Agents in Ada/SPARK** — AIコーディングエージェントにAda/SPARKでセキュリティソフトウェアを書かせ、GNATproveで49,280件の証明義務… 〔技術: ループの評価者をLLM自身ではなく証明器・テスト・人間レビューの層に…／人文: これは「判断する主体」をAIから外部化する試みであり、認識論的には真…〕 · [arxiv.org](https://arxiv.org/abs/2607.14340)
- [ ] **Heatwave — a verification protocol for AI-written code** — Heatwaveは、AIが書いたコードに対して「plan, build, review, prove」を、静かに再起動しないルー… 〔技術: PLANNER / IMPLEMENTER / REVIEWERを分…／人文: ここでの核心は、AIの誠実さではなく制度設計としての相互監査である。〕 · [github.com](https://github.com/abhirajsinha/heatwave)
- [ ] **@ulpi/skills-autonomous-engineering** — Claude CodeやCodex向けに、仕様化、計画、実装、単純化、テスト、レビュー、性能測定、出荷を18個のスキルとして束ね… 〔技術: bounded loop、fail-closed gate、PreT…／人文: 「学習する組織」をエージェントワークフローへ移植した例として読める。〕 · [github.com](https://github.com/ulpi-io/skills-autonomous-engineering)
- [ ] **KarvyLoop — loop-native, local-first, human-in-the-loop runtime** — KarvyLoopは、LLM呼び出し単体ではなく「discover work → run → verify → crystall… 〔技術: スキル、意思決定選好、beliefをローカルに蓄積し、反復ごとに方法…／人文: これは自律化の物語に対する明確な反論で、「人間をループから外す」ので…〕 · [github.com](https://github.com/Caprista/KarvyLoop)
- [ ] **FizzBee — the AI Requirements Engineer between your idea and your coding agent** — FizzBeeは、曖昧なプロンプトから要件を引き出し、矛盾やギャップを形式検証で見つけ、コーディングエージェントが読める精密な仕… 〔技術: 実装後のデバッグループではなく、実装前の要件抽出・分析・検証ループに…／人文: ここで問われているのは「意図はどこに存在するのか」という解釈学的問題…〕 · [fizzbee.ai](https://fizzbee.ai)

### Anthropology of Agentic AI
- [ ] **Who will own the AI agent economy?** — AIエージェントが中央集権的なシステムから、個人・組織にまたがる多数のエージェントのネットワークへ移るとき、誰がエージェント経済… 〔技術: 個人エージェント、組織エージェント、外部サービスが接続する分散マルチ…／人文: 「誰が所有するのか」という問いは、道具の所有ではなく、代理行為の主体…〕 · [mitsloan.mit.edu](https://mitsloan.mit.edu/ideas-made-to-matter/who-will-own-ai-agent-economy)
- [ ] **U.S. and Japanese Companies Struggle with Different Parts of AI Adoption—and Offer Different Lessons for Making It Work** — 米国企業はAI導入が広いが浅く、日本企業は導入が遅い一方で、導入された場所では深く実用に結びつきやすい、という対比を示す記事。 〔技術: 同じAIエージェント機能でも、APIやUIの完成度だけではスケールせ…／人文: 日本と米国の差は「遅れている／進んでいる」ではなく、組織が新しい代理…〕 · [hbr.org](https://hbr.org/2026/07/u-s-and-japanese-companies-struggle-with-different-parts-of-ai-adoption-and-offer-different-lessons-for-making-it-work)
- [ ] **Agentic AI is ready to act. Is your organization ready to trust it?** — Agentic AIが「提案するAI」から「行動するAI」へ進む中で、組織側がそれを信頼できる状態にあるかを問う記事。 〔技術: 行動するエージェントには、権限境界、承認ステップ、監査ログ、リスクス…／人文: 「信頼してよいか」はモデル精度の問題だけでなく、組織が新しい非人間ア…〕 · [news.google.com](https://news.google.com/rss/articles/CBMijAFBVV95cUxOTHdtR1NlZ0NPemw3WXU1X3lKdEdCVWtTbnNQd1A2SFBzZ01BUTV5c2ZOZW5VclYxSEhuTHpFS19BX3JBb2RzeGFCWFVuWDk3ZU9UUXdKZWRia2MyeFhkYVBTM194YTctU2tlSXY3M0ltc1BkQ3BBbXlId01ZcHk0Ty16NGNOY3E0LXBMNw?oc=5)
- [ ] **Workspaces: How We Built Sandbox Infrastructure for Autonomous Agents** — 自律エージェントが実行・探索・経験から学習するための、現実的で再現可能かつ高速・隔離された「ワークスペース」基盤を解説する記事。 〔技術: サンドボックス、状態再現、隔離実行、フィードバックループを整えること…／人文: 「ワークスペース」は身体性の代替物です。〕 · [neosigma.ai](https://neosigma.ai/blog/agent-workspaces)
- [ ] **Pokayoke – turn code conventions into checks for agents** — リポジトリ固有の命名規則、行数制限、色指定ルールなど、通常のリンターでは扱いにくい「チームの作法」を、AIエージェントも人間も実… 〔技術: ASTやワークスペース検査を用いて、自然言語の運用ルールをCIに近い…／人文: 名前の由来である「ポカヨケ」は、工場文化のエラー防止実践をソフトウェ…〕 · [pokayoke.codes](https://pokayoke.codes)

### History of Automation
- [ ] **The Industrialization of Research ; On AI-Driven Science and Its Consequences** — AIを単なる研究補助ツールではなく、研究サイクル内の自律的参加者として捉え、研究が「職人的モデル」から「分解・自動化・監督される… 〔技術: AIエージェントによる科学自動化を、単発の効率化ではなく、知識生産工…／人文: 産業革命期の熟練労働の分解と同じく、研究者の判断・徒弟制・共同体規範…〕 · [arxiv.org](http://arxiv.org/abs/2607.15164v1)
- [ ] **Unsafe at any AUC: Unlearned Lessons from Sociotechnical Disasters for Responsible AI** — 自動意思決定システムのリスクを、モデル性能指標だけでなく社会技術システム全体として評価すべきだと論じる。 〔技術: AUCなどの局所的性能評価から、運用組織、インセンティブ、事故連鎖を…／人文: 自動化の歴史では「機械が失敗した」のではなく、失敗を許す組織文化が反…〕 · [arxiv.org](http://arxiv.org/abs/2607.14353v1)
- [ ] **CAVA: Canonical Action Verification and Attestation for Runtime Governance of Agentic AI Systems** — エージェントがローカルフック、SDKツール、ブラウザ自動化、APIゲートウェイ、ワークフローエンジンなど異なる実行環境で行動する… 〔技術: 異種ランタイム上のエージェント行為を正規化し、承認と実行を結びつける…／人文: これは工場のタイムカードや工程記録、官僚制の稟議書に近い「行為の記録…〕 · [arxiv.org](http://arxiv.org/abs/2607.13716v1)
- [ ] **AI-Native Insurance for Agentic AI: Pricing, Underwriting, and End-to-End Automation** — 自律的に意思決定し、ツールを呼び出し、外部環境を変更し、第三者サービスと相互作用するAIエージェント向けに、保険料、免責、補償配… 〔技術: 自律性、権限、権限露出、ガバナンス成熟度、依存集中度をリスク状態とし…／人文: 自動車、工場、電力網の普及と同様に、自動化は事故後の補償制度が整って…〕 · [arxiv.org](http://arxiv.org/abs/2607.13230v1)
- [ ] **The tragedy of the cognitive commons: collective intelligence beyond AI-induced knowledge collapse** — Acemoglu、Kong、Ozdaglarによる「エージェントAIが人間の知識共有努力を代替し、公共的知識ストックを劣化させる… 〔技術: AIエージェントが私的な回答生成を代替しても、公共の知識ベースを再生…／人文: 自動化の歴史では、機械が作業を代替するだけでなく、技能共同体や相互扶…〕 · [arxiv.org](http://arxiv.org/abs/2607.13272v1)

### DDD
- [ ] **仕様書は最新に保てない。では何が仕様の正か** — AI駆動開発では散文仕様がすぐ古びるため、CIで同期が強制されるテストを現行仕様の正とし、ADRとユビキタス言語だけを長寿命の手… 〔技術: テスト、ADR、ユビキタス言語をそれぞれ異なる更新頻度と検証可能性で…／人文: DDDの言語観が、人間同士の共同理解から、人間と非人間エージェントの…〕 · [qiita.com](https://qiita.com/ikeyansaza/items/d96867ba05e337f2e3ac)
- [ ] **Archally Blueprint Schema** — ドメイン設計、意思決定記録、ビジネスルール、ガバナンス、アーキテクチャを単一のYAMLスキーマにまとめ、OpenAPI、Asyn… 〔技術: DDD/イベントストーミングの成果物を、生成AIが参照できる機械可読…／人文: 「アーキテクチャ知識は誰の記憶に宿るのか」という組織人類学的な問題に…〕 · [github.com](https://github.com/Archally/blueprint-schema)
- [ ] **AI時代のシステム崩壊に備えよ：仕様・ドメイン・イベントの「3つの駆動」で構築する究極のアーキテクチャ** — AIによる高速コーディングが、エラー隠蔽、コピペ、技術的負債、安定性低下を招く危機に対し、ドメイン駆動、イベント駆動、仕様駆動を… 〔技術: DDDをLLMのコンテキスト制限と障害局所化のための境界設計として使…／人文: 「AIは速いが、責任を持たない短期契約者のように負債も作る」という比…〕 · [qiita.com](https://qiita.com/satouo/items/1e39fd9e24e2961c2710)
- [ ] **ai-refinement-method** — 「vibe codingではなくvibe spec'ing」を掲げ、自然言語の意図をイベントストーミング、DDD、リファインメン… 〔技術: LLMを実装者ではなく上流設計のファシリテータとして使い、イベントス…／人文: 設計会議でしか生まれなかった対話・保留・合意形成を、エージェント時代…〕 · [github.com](https://github.com/nlawstudio/ai-refinement-method)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — DDDを、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの特定、集約設計、技術アーキテ… 〔技術: LLMはDDDの初期探索や会話のたたき台には強いが、集約や技術アーキ…／人文: 「自動化」ではなく「協働するスパーリングパートナー」という結論が、D…〕 · [arxiv.org](http://arxiv.org/abs/2603.26244v1)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

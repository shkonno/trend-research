# 📰 2026-08-23 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Gemini Notebook が Gemini アプリ内のノートブックとして同期される · [support.google.com](https://support.google.com/gemininotebook/answer/17003757?hl=ja)
- **Loop engineering** — PolicyGuide: From Guarding One Action to Guiding the W… · [arxiv.org](https://arxiv.org/abs/2608.19861)
- **AWS** — Web Search in Amazon Bedrock AgentCore がドメイン・公開日フィルタを追… · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/web-search-amazon-bedrock)
- **Harness engineering** — Task-CoEvolve: Efficient Harness Optimization via Adap… · [arxiv.org](http://arxiv.org/abs/2608.20169)
- **sharp LLM usage** — LLM 0.33: 繰り返しテンプレートで「モデル設定」と「作業プロンプト」を合成する · [simonwillison.net](https://simonwillison.net/2026/Aug/22/llm)
- **AI agent trends** — The New MCP Roadmap: agentic messaging primitives と ag… · [github.com](https://github.com/modelcontextprotocol/modelcontextprotocol/pull/3291)
- **Claude Code** — Claude Code v2.1.239: コスト見積もり、クラウド同期プラグイン、プロキシ/Bedrock… · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.239)
- **Ethics of AI Agents** — Agent Safety Should Be a Runtime Contract · [arxiv.org](http://arxiv.org/abs/2608.11274v1)
- **Philosophy of Loop Engineering** — Brain Researcher: agentic AI for science に分析的厳密さを埋め込む · [arxiv.org](http://arxiv.org/abs/2608.19902)
- **Anthropology of Agentic AI** — 初心者向け】最近よく聞く「Agentic AI」って結局なんなの？ · [qiita.com](https://qiita.com/kamaryo/items/db2ee3faa6343b3cce1e)
- **History of Automation** — Automating and Scaling Behavioral Scientific Research… · [arxiv.org](https://arxiv.org/abs/2608.10030)
- **DDD** — Turn a Codebase into a Domain Model Your PM and QA Can… · [dev.to](https://dev.to/mroops/turn-a-codebase-into-a-domain-model-your-pm-and-qa-can-read-16d)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Gemini Notebook が Gemini アプリ内のノートブックとして同期される** — Google の公式ヘルプでは、Gemini Notebook で作成したノートブックが Gemini のナビゲーションにも表示… 〔技術: NotebookLM のソースグラウンディングが、Gemini アプ…／人文: 個人の読書・調査履歴が「ノート」ではなく、会話可能な知識環境として生…〕 · [support.google.com](https://support.google.com/gemininotebook/answer/17003757?hl=ja)
- [ ] **Google 検索の AI モードに Notebook が表示・作成・編集される** — Gemini Notebook で作成したノートブックは Google 検索の AI モードに自動表示され、AI モードからアク… 〔技術: 検索結果を読む場と、ソースを束ねて継続的に問う場が統合され、検索が一…／人文: 検索は従来「外の世界を探す」行為でしたが、Notebook 連携後は…〕 · [support.google.com](https://support.google.com/gemininotebook/answer/17513891?hl=ja)
- [ ] **動画解説・スライド・インフォグラフィック・クイズ化で“読む”から“教材化する”へ** — Gemini Notebook では、ソースをもとに動画解説、スライド資料、インフォグラフィック、フラッシュカード、クイズなどを… 〔技術: RAG 的な質問応答ツールが、マルチモーダルな学習アーティファクト生…／人文: これは読解の民主化であると同時に、理解した気になる速度を上げる装置で…〕 · [support.google.com](https://support.google.com/gemininotebook/answer/16454555?hl=ja)
- [ ] **日本語圏では「Gemini Notebook（旧NotebookLM）」の解説・実践記事が急増** — 2026年8月22日の Bing RSS では、SHIFT AI、AQUA、JAPAN AI など複数の日本語記事が「Gemin… 〔技術: 公式機能の高度化だけでなく、日本語の業務導入記事が増えることで、会議…／人文: 名前の変更は単なるブランド変更ではなく、ユーザーが「Google の…〕 · [shift-ai.co.jp](https://shift-ai.co.jp/blog/24690)
- [ ] **学生利用とプライバシー批判が同時に目立つ** — Google News RSS では、XDA が「ChatGPT、Claude、NotebookLM に学期全体の資料を渡して比… 〔技術: 学習資料を大量投入して横断検索・要約・生成物化できる強みと、ローカル…／人文: 学生にとってノートは単なる情報ではなく、失敗・理解不足・関心の履歴で…〕 · [news.google.com](https://news.google.com/rss/articles/CBMijgFBVV95cUxQanlxcHBwQ3M2cTJGeWxhTV80Snc5QnlJbE1iSG9EWGJaci0wMm5GVEZ2VTJOVHRwMk9ZMS1Ea3Bqb091eFY1Z3hYTi00UHE2ZnlvLXRBT1ZmTkZvREcwVHhpci1wRl9GYnFyMk01MkYzSndOYTJCSm9wVXlfaURFeS1TTlI1cFRFZUtmcG9B?oc=5)

### Loop engineering
- [ ] **PolicyGuide: From Guarding One Action to Guiding the Whole Workflow for Policy-Compliant LLM Agents** — 顧客対応LLMエージェントのポリシー遵守を、単発アクションのガードではなく、ドメイン方針をワークフローグラフへコンパイルして会話… 〔技術: 方針を状態付きワークフローグラフに変換し、永続化されたグラフ状態から…／人文: ethics の観点では、組織の規則を単なる禁止リストではなく、ユー…〕 · [arxiv.org](https://arxiv.org/abs/2608.19861)
- [ ] **One Success Isn't Reliability: Thinkingbox, a Sandbox and Benchmark for Agents in Stateful Business Workflows** — ビジネス業務では、1回の成功や正しいツール呼び出しだけでは信頼性を測れないとして、状態を持つ業務ワークフローでエージェントを評価… 〔技術: 端末側の永続状態変化まで評価対象にすることで、会話・ツール・ユーザー…／人文: anthropology 的には、仕事は単発タスクではなく、確認・依…〕 · [arxiv.org](https://arxiv.org/abs/2608.19741)
- [ ] **Bringing analytic rigor to agentic AI for science: The Brain Researcher platform for neuroimaging data analysis** — 神経画像解析向けの agentic research harness として、許容される分析、必要なチェック、主張の射程をルール… 〔技術: エージェントの分析ループに、代替分析、証拠の来歴、主張範囲の制限を組…／人文: philosophy of science の観点では、AIの出力を…〕 · [arxiv.org](https://arxiv.org/abs/2608.19902)
- [ ] **Inducing Task Models from Computer-Use Traces** — スクリーンショット、マウス、キーボード操作などの自然なコンピュータ利用ログから、日常業務の象徴的・監査可能・再利用可能なタスクモ… 〔技術: 低レベルイベント列から、将来のコンピュータ操作エージェントが再利用で…／人文: anthropology 的には、職場の知はマニュアルよりも画面遷移…〕 · [arxiv.org](https://arxiv.org/abs/2608.20319)
- [ ] **Auditing Self-Evolution in Financial Agents: Capability Gains, Security Drift, and Execution-Interface Mismatch** — 自己進化型エージェントが経験をスキル・ワークフロー・メモリへ変換する際、能力向上だけでなくセキュリティドリフトや実行インターフェ… 〔技術: 学習後の精度だけでなく、過去に正しかった挙動の保存、攻撃露出、状態再…／人文: ethics の観点では、「成長するエージェント」は有能になるほど安…〕 · [arxiv.org](https://arxiv.org/abs/2608.17684)

### AWS
- [ ] **Web Search in Amazon Bedrock AgentCore がドメイン・公開日フィルタを追加し、東京リージョンにも拡大** — Amazon Bedrock AgentCore の Web Search が、エージェント実行時に検索対象ドメインと公開日範囲… 〔技術: RAGやエージェント検索で問題になりがちな古い情報・低品質ドメイン混…／人文: 「AIがどの知識を参照してよいか」を組織が明示する設計は、検索の自由…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/web-search-amazon-bedrock)
- [ ] **Amazon Bedrock AgentCore payments が一般提供開始、AIエージェントの自律決済にガードレール** — Amazon Bedrock AgentCore payments がGAとなり、AIエージェントが支払いを伴う処理を実行するた… 〔技術: 決済フローをエージェント基盤に組み込みつつ、上限・監査・観測可能性を…／人文: お金を扱うAIは、便利さ以上に「誰が許可し、誰が責任を負うのか」を社…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale)
- [ ] **Amazon Bedrock AgentCore Gateway によるエージェントのツールアクセス統制** — Bedrock AgentCore Gateway を使い、企業内ツールへの接続を「Connect / Control / Ca… 〔技術: MCP的なツール接続の広がりに対し、認可・カタログ化・監査をゲートウ…／人文: エージェントが社内システムを横断するほど、組織の暗黙知や権限構造がそ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/govern-ai-agent-tool-access-with-amazon-bedrock-agentcore-gateway)
- [ ] **AWS Glue 6.0 が30%低価格化、Apache Iceberg v3とSpark 4.1/Python 3.13に対応** — AWS Glue 6.0 が一般提供され、従来バージョン比で30%低い価格、Apache Iceberg v3のフルサポート、A… 〔技術: Iceberg v3と新しいSpark/Pythonランタイムにより…／人文: データ基盤の価格低下は、分析やAI活用を一部の巨大チームだけでなく、…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-glue-6-0-now-available-with-30-lower-price-and-full-apache-iceberg-v3-support)
- [ ] **サンリオのエンジニアがAI-DLC Unicorn GymでAI駆動開発を体験** — サンリオのエンジニア6名が、AWSのAI-DLC（AI-Driven Development Lifecycle）Unicorn… 〔技術: BedrockやAWSの開発支援の文脈が、抽象的なデモではなく、既存…／人文: キャラクターやブランドを扱う企業でAI駆動開発が試されることは、効率…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/sanrio-ai-dlc-unicorn-gym-2026)

### Harness engineering
- [ ] **Task-CoEvolve: Efficient Harness Optimization via Adaptive Validation Task Selection** — LLMエージェントのハーネスコードを反復的に書き換えて性能を上げる際、毎回固定の検証セット全体を走らせるコストを削減する研究。 〔技術: ハーネス改善を「全件評価」ではなく、能力境界に近いタスクとの共進化問…／人文: 何を測るかが、何を賢いと見なすかを決めるという評価文化の問題を露出し…〕 · [arxiv.org](http://arxiv.org/abs/2608.20169)
- [ ] **HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety** — エージェントハーネスの安全性を、設定、能力拡張、実行、状態永続化、行動制御、インシデント回復という6段階のライフサイクルで評価す… 〔技術: プロンプト注入単体ではなく、権限・永続状態・設定変更を含む「運用中の…／人文: エージェントの失敗はモデルの内面だけでなく、組織が許可したワークフロ…〕 · [arxiv.org](http://arxiv.org/abs/2608.17597)
- [ ] **LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents** — OpenHands SDK、Claude Code、OpenCode などの実際のコーディングエージェントハーネスを内部改造せず… 〔技術: デプロイ時のハーネスを訓練から切り離さず、生成ストリーム・コンテキス…／人文: 開発者が日常的に使う道具そのものが学習環境になるため、「使う」と「訓…〕 · [arxiv.org](http://arxiv.org/abs/2608.17393)
- [ ] **ClawGym II: Exploring Black-Box RL on Agent Harness** — 複雑なエージェントハーネスをブラックボックスとして扱い、モデル境界のプロキシから呼び出し列を回収してRL最適化する枠組み。 〔技術: ハーネス内部を完全に理解・改造しなくても、外側から観測可能なLLM呼…／人文: これは職場の既存ツールを壊さずに、その上で働くエージェントを鍛える発…〕 · [arxiv.org](http://arxiv.org/abs/2608.16798)
- [ ] **LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation** — コーディングエージェント評価が、単発タスクのハーネス設計から、長期開発を支えるループ設計へ移行していると位置づけるベンチマーク。 〔技術: テストを依存DAGの ready frontier に沿って解放し、…／人文: Loop engineering は、AIを一回の回答者ではなく、時…〕 · [arxiv.org](http://arxiv.org/abs/2608.00267)

### sharp LLM usage
- [ ] **LLM 0.33: 繰り返しテンプレートで「モデル設定」と「作業プロンプト」を合成する** — Simon WillisonのCLIツール `llm` 0.33では、`llm prompt -t/--template` を複… 〔技術: モデル・オプション・プロンプト本文を分離して再利用できるため、LLM…／人文: “良い質問をする個人技”から“チームで共有できる手順文化”への移行が…〕 · [simonwillison.net](https://simonwillison.net/2026/Aug/22/llm)
- [ ] **Coding agentsの検証は「全行コードレビュー」だけではない** — Willisonは、coding agentを生産的に使う鍵を「変更を明確に指示し、正しく適用されたと確信を持って検証できること… 〔技術: エージェント利用のボトルネックを生成能力ではなく検証設計に置き、テス…／人文: 人間の役割が「書く人」から「変更の意味と責任を引き受ける人」へ変わる…〕 · [simonwillison.net](https://simonwillison.net/2026/Aug/22/more-than-just-code-review)
- [ ] **Agentic memoryはオン/オフ機能ではなく、モデル能力に応じて“投与量”を調整するもの** — ALTK-Evolveは、エージェントの過去軌跡から再利用可能なガイドラインを蒸留し、重み更新なしで推論時に再注入する。 〔技術: “全部コンテキストに入れる”発想を退け、タスク別検索・全量注入・コス…／人文: 記憶が多いほど賢いという素朴な比喩ではなく、忘れる・絞る・状況に応じ…〕 · [huggingface.co](https://huggingface.co/blog/ibm-research/altk-evolve-hmm)
- [ ] **Universal Agent Workflow Starter v1.1: LITE/GOVERNEDでリスクに応じたエージェント手順を分ける** — 中国語・英語で提供される汎用Agentワークフロー集で、普通のQAや小型開発向けのLITEと、公開・削除・本番・個人情報・課金な… 〔技術: プロンプトを単なる命令文ではなく、権限、証拠、検証、引き継ぎ、受け入…／人文: エージェント運用で本当に難しいのは知能よりも責任の境界であることを示…〕 · [github.com](https://github.com/Ray111351/universal-agent-workflow-starter)
- [ ] **Grading the Graders: 検証器にもL0-L5の自律性レベルを付ける** — LLMの推論を検証する仕組みについて、検証粒度・リスク・抽象度などが混ざって使われがちな「レベル」を整理し、Verificati… 〔技術: 「LLMが自分で確認しました」と「形式仕様で保証できます」を同じ“検…／人文: 信頼は気分ではなく、どこから根拠が来るかを明示する制度である。〕 · [arxiv.org](http://arxiv.org/abs/2608.19009v2)

### AI agent trends
- [ ] **The New MCP Roadmap: agentic messaging primitives と agent identity が前面に** — MCPの新ロードマップは、長時間ループ、サーバー起点イベント、進捗通知、Tasks拡張、agent identity、enter… 〔技術: request-response だけでは足りない長時間エージェント…／人文: 「エージェントに仕事を任せる」とは、実は誰が発話し、誰の権限で、どこ…〕 · [github.com](https://github.com/modelcontextprotocol/modelcontextprotocol/pull/3291)
- [ ] **Claude Code が連日リリースされ、CLIエージェントが日常インフラ化** — Claude Code は 2026-08-22 に v2.1.240 を公開し、リリースノートは「Bug fixes and… 〔技術: コーディングエージェントの価値はモデル性能だけでなく、CLI、ヘッド…／人文: ツールが毎日更新されると、開発者は「相棒」を使っているというより、変…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.240)
- [ ] **Linuxネットワーク保守者がAI生成パッチの量に「completely overwhelmed」** — Linux 7.3 のネットワーク関連変更を扱う中で、保守者がAI/LLM由来と見られる低優先度の修正・整理パッチの急増に圧迫さ… 〔技術: エージェントがコード生成を民主化すると、ボトルネックは生成能力ではな…／人文: オープンソースは贈与と協働の文化だが、AIが大量の「善意っぽい作業」…〕 · [phoronix.com](https://www.phoronix.com/news/Linux-7.3-Networking)
- [ ] **日本語圏実践: kintoneバッチを「AIが書く、機械が検査する、人間が承認する」** — kSQL Flowの記事は、kintoneの月次バッチ処理を要件文からAIエージェントとkSQL MCPに書かせ、validat… 〔技術: スキーマ確認、下見クエリ、SQL生成、二段階検証、dry-run差分…／人文: エージェント導入の成熟は、人間を外すことではなく、人間の判断が必要な…〕 · [qiita.com](https://qiita.com/rex0220/items/3a1213a596a8c49b67aa)
- [ ] **Task-Conditioned Least-Privilege Learning for Executable Terminal and MCP Agents** — ターミナルとMCP環境で動くツール使用LLMエージェントに対し、タスクごとに必要十分な権限を選ばせる post-training… 〔技術: 権限ゲートを外側に置くだけでなく、モデル自体に task-condi…／人文: 「できることを全部やる」AIから「許されたことだけをする」AIへ移る…〕 · [arxiv.org](http://arxiv.org/abs/2608.18351v1)

### Claude Code
- [ ] **Claude Code v2.1.239: コスト見積もり、クラウド同期プラグイン、プロキシ/Bedrock信頼性の改善** — `/cost`、ステータスライン、`--max-budget-usd` が米国内推論プレミアムを含むようになり、クラウドセッショ… 〔技術: 料金表示、プラグイン同期、クラウド/企業ネットワーク対応が同時に進み…／人文: 生成AI導入の摩擦は「モデル性能」だけでなく、請求・プロキシ・権限・…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.239)
- [ ] **Claude Code GitHub Actions: `@claude` から issue/PR を実作業に変える公式ワークフロー** — Claude Code GitHub Actions は、issue や PR コメントで `@claude` にメンションする… 〔技術: ターミナル内の対話型エージェントを GitHub イベント駆動のCI…／人文: issue コメントが「依頼」ではなく「半自動的な作業指示」になると…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/github-actions)
- [ ] **Boris Cherny の「小さなプロジェクト」論争: Claude Code の価値をめぐる物語化** — Pedro Domingos の投稿をきっかけに、Boris Cherny のサイドプロジェクトとしての Claude Code… 〔技術: ReAct や関数呼び出しのような既存要素を、ターミナル・ファイル編…／人文: 技術史ではしばしば「発明者」や「一人の天才」の物語が過剰に強調されま…〕 · [explainx.ai](https://www.explainx.ai/blog/boris-cherny-claude-code-trillion-dollar-project-august-2026)
- [ ] **Boris Cherny インタビュー群: 5並列インスタンス、20〜30 PR/日、エンジニアの役割変化** — Boris Cherny は Claude Code の誕生経緯、並列エージェント、PR構造、決定的なレビュー手順、大規模コード… 〔技術: plan mode、複数checkout、並列実装、レビューの決定論…／人文: エンジニアの熟練は、手を動かす速度から、仮説を分割し、作業者としての…〕 · [newsletter.pragmaticengineer.com](https://newsletter.pragmaticengineer.com/p/building-claude-code-with-boris-cherny)
- [ ] **日本語圏の実践整理: Subagent、Hook、Plugin、Figma MCP までを含む学習導線** — 日本語記事として、インストール、ログイン、最初のToDoアプリ作成、編集承認、Figma MCP、コンテキスト管理、CLAUDE… 〔技術: 基礎操作から拡張機能までを順に接続しており、単なるプロンプト集ではな…／人文: 日本語圏では、英語圏の一次情報を現場の学習手順へ翻訳する記事が導入速…〕 · [qiita.com](https://qiita.com/utanesuke/items/07cfdc173efa67e25f7f)

### Ethics of AI Agents
- [ ] **Agent Safety Should Be a Runtime Contract** — 自律エージェントの安全性を、RLHFやConstitutional AIのような訓練時の性質だけでなく、ハーネスが実行時に強制す… 〔技術: エージェント安全を「実行前ブロック」と「実行後の検証可能証拠」の二面…／人文: 責任をモデルの内面に帰すのではなく、組織が設計する手続き・記録・承認…〕 · [arxiv.org](http://arxiv.org/abs/2608.11274v1)
- [ ] **Characterizing Agentic Flooding of Government Services** — AIエージェントが給付申請、政策理解、意見提出などを容易にする一方、行政サービスに大量需要を発生させる「agentic floo… 〔技術: 個別エージェントの失敗ではなく、多数のエージェントが公共システムに与…／人文: アクセシビリティ向上と制度濫用・行政過負荷が同時に起きうる点が、AI…〕 · [arxiv.org](http://arxiv.org/abs/2608.16603v2)
- [ ] **Participatory Moral AI Is Not Neutral: The Invisible Hand of Developers** — モラルAIでよく使われる参加型の選好収集は中立ではなく、開発者が事前に決める特徴量の範囲、投票者サンプリング、質問文のフレーミン… 〔技術: 「人々に投票させれば民主的」という素朴な設計を、データ収集パイプライ…／人文: 参加型倫理はしばしば正当性の切り札として語られるが、誰を参加者にし、…〕 · [arxiv.org](http://arxiv.org/abs/2608.14522v1)
- [ ] **A three-dimensional typology of agency for advanced AI systems** — 高度AIシステムの「agency」を、道徳的/法的、個別/集合的、人間/非人間という3軸で整理する類型論。 〔技術: エージェントの能力評価だけでは曖昧になりがちな「誰が行為したのか」を…／人文: 責任所在の議論では「AIに責任を負わせるべきか」が過熱しがちだが、こ…〕 · [arxiv.org](http://arxiv.org/abs/2608.20041v1)
- [ ] **【2026年最新】AIエージェント比較10選｜自律型AIの選び方を徹底解説** — 日本語圏の実務者向けに、主要AIエージェント・プラットフォームの選び方を比較し、Human-in-the-loop、セキュリティ… 〔技術: 研究論文ではなく導入ガイドの文脈で、権限設定、ログ、承認フロー、規制…／人文: 日本語圏では「便利な自動化ツール」としてAIエージェントが紹介されが…〕 · [aismiley.co.jp](https://aismiley.co.jp/ai_news/ai-agent-compare)

### Philosophy of Loop Engineering
- [ ] **Brain Researcher: agentic AI for science に分析的厳密さを埋め込む** — 神経画像解析のためのエージェント基盤で、許容される分析、必須チェック、主張の射程をルール化し、出力を「防御可能な科学的主張」に近… 〔技術: ループ内に分析選択・出所・レビュー・主張制限を組み込み、エージェント…／人文: これは認識論的に「何を知ったと言えるのか」をワークフローの内部問題に…〕 · [arxiv.org](http://arxiv.org/abs/2608.19902)
- [ ] **LoopVSR: 視覚音声認識パイプラインを証拠で修復する Loop Engineering** — Visual Speech Recognition の多段推論パイプラインに対して、コードエージェントが診断・パッチ作成を行い、… 〔技術: 上流故障が下流故障を覆い隠す状況で、実行証拠を次の反復に返すことで、…／人文: サイバネティクス的には、観測・制御・フィードバック・停止条件が明確な…〕 · [arxiv.org](http://arxiv.org/abs/2608.13610)
- [ ] **FormalTCS: LLMによる理論計算機科学研究を、生成・形式化・証明のループで測る** — STOC/FOCS/SODA/COLT 2025-2026 の論文由来タスクを使い、LLMが理論計算機科学の研究パイプラインをど… 〔技術: 自然言語の主張、形式化、証明、専門家評価を接続し、エージェントの研究…／人文: ループエンジニアリングを「正解へ収束する装置」と見るだけでは足りず、…〕 · [arxiv.org](http://arxiv.org/abs/2608.20153)
- [ ] **LoopsBench: Harness Engineering から Loop Engineering への評価軸の移動** — 長期的なコーディングエージェント評価のため、依存DAGを持つ112タスク、5,300超の開発単位、実行可能テストを提供するベンチ… 〔技術: 評価対象を最終状態だけでなく、計画、前提依存、回帰、継続実行へ広げ、…／人文: これはエンジニアリングを成果物中心から履歴・記憶・責任中心へ動かす転…〕 · [arxiv.org](http://arxiv.org/abs/2608.00267)
- [ ] **Awesome Loop Engineering / Looper: ループを共有語彙と人間承認の実践にする動き** — Awesome Loop Engineering は、再帰的・状態的・検証済みAIエージェントシステムのためのリソース、パターン… 〔技術: ループ契約、品質チェック、承認ゲート、モデル差し替え可能性を通じて、…／人文: 特に Looper の README は、専門家がAIと共同で「自分…〕 · [github.com](https://github.com/ChaoYue0307/awesome-loop-engineering)

### Anthropology of Agentic AI
- [ ] **初心者向け】最近よく聞く「Agentic AI」って結局なんなの？触って理解した内容をまとめてみる** — Agentic AIを「自分で次に何をするかを考え、情報収集・ツール/API実行・反省・軌道修正まで行うAI」として、実際に触っ… 〔技術: 目的、計画、ツール利用、反省ループをひとまとまりの実行単位として体験…／人文: 人類学的には、これは「AIに仕事を頼む」作法が、プロンプト入力から依…〕 · [qiita.com](https://qiita.com/kamaryo/items/db2ee3faa6343b3cce1e)
- [ ] **Agentic AIとは？ 自律的に計画・判断・実行するAIとAIエージェントの関係を解説** — Agentic AIを、目標・計画・ツール利用・状態・評価・実行制御をどの程度備えるかで捉えるべきだと整理している。 〔技術: エージェント性を構成要素の有無ではなく、状態管理・評価・実行制御を含…／人文: 組織慣習として見ると、「AIが自律的かどうか」は技術仕様だけでなく、…〕 · [engineering-technology.brexa.com](https://engineering-technology.brexa.com/blog/technavi/agentic-ai)
- [ ] **【2026】Agentic AIとは？生成AIとの違い・代表ツール・導入ステップを解説** — Agentic AIを「判断から実行までを担う」生成AIの次段階として紹介し、代表ツールや導入時のリスク、導入ステップを整理して… 〔技術: ツール比較と導入ステップを組み合わせることで、PoCから業務フロー実…／人文: 労働文化の観点では、Agentic AIの導入は「人がAIを使う」か…〕 · [ai-kenkyujo.com](https://ai-kenkyujo.com/artificial-intelligence/agentic-ai)
- [ ] **AIエージェントとは？仕組みや生成AIとの違い、企業での活用例をわかりやすく解説** — AIエージェントを、人間が設定した目標に対して自ら計画を立て、情報収集・判断・実行までこなすAIシステムとして説明している。 〔技術: 生成AI・チャットボット・RPAとの比較により、Agentic AI…／人文: 企業イベント系メディアの記事であることが重要で、AIエージェントが研…〕 · [japan-it.jp](https://www.japan-it.jp/hub/ja-jp/blog/article-67.html)
- [ ] **AIエージェント（Agentic AI）完全ガイド2026：自律型AIが企業と社会を変える** — 「AIは答えるから動くへ」という見取り図で、プランニング、ツール使用、メモリ、マルチエージェント協調をAgentic AIの主要… 〔技術: プランニング、ツール使用、メモリ、マルチエージェント協調を分けて説明…／人文: 産業別の語りは、Agentic AIが単一の普遍技術ではなく、金融の…〕 · [labmemo.com](https://labmemo.com/agentic-google-gemini-enterprise-agent-platform-2026)

### History of Automation
- [ ] **Automating and Scaling Behavioral Scientific Research on AI Agents** — AEROBATというマルチエージェントシステムが、AIエージェントの行動に関する仮説生成、実験設計、シミュレーション実行、統計分… 〔技術: 自動化の対象が「作業」から「実験計画と知識生産のワークフロー」へ拡張…／人文: これはテイラー主義的な労働分解の最新版であると同時に、科学者の判断・…〕 · [arxiv.org](https://arxiv.org/abs/2608.10030)
- [ ] **The Capability Ladder: A Curriculum-Modernization Framework for Workforce Readiness in the AI Era** — AI時代の教育・職能を「trigger / automation / workflow / AI agent / agent t… 〔技術: エージェントの自律度と人間の監督要件を段階化し、教育課程や職務設計に…／人文: 自動化の歴史では、機械化のたびに「熟練」が消えるのではなく再定義され…〕 · [arxiv.org](https://arxiv.org/abs/2608.07779)
- [ ] **Anthropic Economic Index** — Claudeの利用データをもとに、地域・職業・タスクごとのAI利用を可視化する継続的な経済インデックス。 〔技術: LLM利用ログを職業・タスク分類と接続し、AIエージェント化が実際の…／人文: 自動化史で繰り返された「補助か代替か」という対立を、会話ログ由来の実…〕 · [anthropic.com](https://www.anthropic.com/economic-index)
- [ ] **The 2026 AI Index Report** — 2026年版AI Indexは、AIエージェントがOSWorldのような実コンピュータ操作ベンチマークで約12%から約66%のタ… 〔技術: エージェントの実作業能力を、チャット応答ではなくOS操作・タスク遂行…／人文: 産業用ロボットや事務自動化と同じく、導入判断は平均性能ではなく失敗時…〕 · [hai.stanford.edu](https://hai.stanford.edu/ai-index/2026-ai-index-report)
- [ ] **LLMs in Process Diagram Engineering: From Optimal PFDs to Validated P&IDs** — 化学・プロセス工学で手作業が多いPFD（Process Flow Diagram）からP&ID（Piping and Instr… 〔技術: 古典的な産業自動化の中核であるプロセス設計に、LLMが自然言語・設計…／人文: 自動化の歴史は工場現場から始まったが、ここでは設計図を書く技術者の判…〕 · [arxiv.org](https://arxiv.org/abs/2608.11220)

### DDD
- [ ] **Turn a Codebase into a Domain Model Your PM and QA Can Read** — BraidというOSSフレームワークを紹介する記事で、コードベースからDDD形式のドメインモデルを抽出し、PM・QA・エンジニア… 〔技術: コード、PRD、設計文書、Slack的な暗黙知のズレを、bounde…／人文: 「ドメインモデルは抽出ではなく合意である」という立場がよいです。〕 · [dev.to](https://dev.to/mroops/turn-a-codebase-into-a-domain-model-your-pm-and-qa-can-read-16d)
- [ ] **DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python** — SRS（Software Requirements Specification）から型付きDDDモデルを作り、Pythonコード… 〔技術: LLMの曖昧な設計レビューを、AST解析やimport構造チェックな…／人文: DDDの「言葉と設計を一致させる」という理想が、開発者の良心やレビュ…〕 · [github.com](https://github.com/barandincoguz/DDD-Enforcer)
- [ ] **ProcessFlow Architect: ローカルAIで動くEvent Stormingスタジオ** — Event Storming、DDD、BPMN、C4、UMLを扱うデスクトップアプリで、LiteRT-LM / WebGPUによ… 〔技術: Event Stormingの付箋作業を、ローカルLLM、複数ビュー…／人文: オフライン・ローカルファーストを打ち出している点は、ドメイン知識がし…〕 · [github.com](https://github.com/raalzate/processflow-architect)
- [ ] **承認ルートは申請の中に置くべきか、外に出すべきか。Goで多段承認を作りながら集約の境界を引く** — GoとDDDの学習連載として、多段承認を題材に「承認ルートの定義」と「承認の進捗」を分け、どこをApplication集約の内側… 〔技術: 集約を「一緒に守る不変条件の囲い」として説明し、承認順序・二重承認禁…／人文: 稟議や承認は単なる状態遷移ではなく、組織の権限・記憶・責任の表現です…〕 · [qiita.com](https://qiita.com/shinchi-pmtech/items/59a665b68909ca55b87c)
- [ ] **Archally Blueprint Schema: domain-first YAML schema for system cartography** — ドメイン設計、意思決定記録、ビジネスルール、ガバナンス、組織的整合をYAMLの単一モデルとして表現し、OpenAPI、Async… 〔技術: DDD的なbounded contextやbusiness rule…／人文: 「地図」という比喩は、設計が現実そのものではなく、目的を持った表象で…〕 · [github.com](https://github.com/Archally/blueprint-schema)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

# 📰 2026-07-14 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Short Video Overviews が英語ユーザー向けにモバイル・Webで正式ロールアウト · [x.com](https://x.com/NotebookLM/status/2074551227594264799)
- **Loop engineering** — Stop Hand-Holding Your Coding Agent: Engineering the L… · [arxiv.org](https://arxiv.org/abs/2607.00038)
- **AWS** — OpenAI GPT-5.6 Sol / Terra / Luna が Amazon Bedrock で一般… · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/openai-gpt-sol-terra)
- **Harness engineering** — ContextSniper: Claude Code を含む修復エージェントの文脈コストを下げる評価ハーネス · [arxiv.org](https://arxiv.org/abs/2607.01916)
- **sharp LLM usage** — Failure as a Process: An Anatomy of CLI Coding Agent T… · [arxiv.org](https://arxiv.org/abs/2607.09510v1)
- **AI agent trends** — The Making of Claude Code · [anthropic.com](https://www.anthropic.com/features/making-of-claude-code)
- **Claude Code** — Claude Code v2.1.207: Auto mode一般化とセキュリティ修正の大規模リリース · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.207)
- **Ethics of AI Agents** — TrustX Agent Risk Classification Framework (ARC): Risk… · [arxiv.org](https://arxiv.org/abs/2607.09586)
- **Philosophy of Loop Engineering** — Stop Hand-Holding Your Coding Agent: Engineering the L… · [arxiv.org](https://arxiv.org/abs/2607.00038)
- **Anthropology of Agentic AI** — AI Agent Day 2026 Summer：製造・航空・教育・コンサルまで、実装後の業務変革と組織づく… · [news.google.com](https://news.google.com/rss/articles/CBMiakFVX3lxTE8zZmJjQjZvMFlWU3NpNHBoMDVKaTJ0THBuelRqR3YwOTNXSVJ0VFFsUzRjS1B1SFlDRUR2UkJyT1JWTkRvdlBnSUt5S3ZIbWk5ZDBGREU2WG9OOHhLVmxuRU5fckEwek9Mb3c?oc=5)
- **History of Automation** — ガバメントAI「源内」：行政労働の自動化が制度インフラになる · [digital.go.jp](https://www.digital.go.jp/policies/genai)
- **DDD** — AI時代のシステム崩壊に備えよ：仕様・ドメイン・イベントの「3つの駆動」で構築する究極のアーキテクチャ · [qiita.com](https://qiita.com/satouo/items/1e39fd9e24e2961c2710)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Short Video Overviews が英語ユーザー向けにモバイル・Webで正式ロールアウト** — NotebookLM公式Xが、Short Video Overviewsが英語の全ユーザー向けにモバイルとWebでロールアウト済… 〔技術: ソースグラウンデッドな要約を、テキストから短尺動画インターフェースへ…／人文: 知識の入口が「読む」から「眺める・聴く」へ移ることで、学習の敷居は下…〕 · [x.com](https://x.com/NotebookLM/status/2074551227594264799)
- [ ] **日本語実践例: 英語PDFを日本語要約し、NotebookLMで深掘りして原文へ戻る読書法** — 日本語の本より英語PDFの方が読みやすくなった、という投稿。 〔技術: 長文PDFをソースとして保持しながら、要約・質問応答・原文参照を往復…／人文: 翻訳AIは単なる言語変換ではなく、読書の順序そのものを変える。〕 · [x.com](https://x.com/fromdusktildawn/status/2071076559432151246)
- [ ] **日本語記事: 2026年7月最新版のNotebookLM活用事例7選** — 社内ナレッジ整理、議事録活用、教育・研修、顧客調査分析、セミナー調査、営業ロールプレイなど、NotebookLMを業務に落とす日… 〔技術: NotebookLMの価値を、モデル性能ではなく「組織内ソースを限定…／人文: 会社の暗黙知をAIに読ませる行為は、組織文化の記憶を再編集することで…〕 · [note.com](https://note.com/canon_non_no/n/n7f4d57e3694a)
- [ ] **より強力なNotebookLM: エージェント的チャット、高度な推論、新しい出力形式をGoogle AI Ultra向けに展開** — NotebookLM公式Xは、チャット内のエージェント的機能、より高度な推論、新しい出力形式を含む大型アップグレードをGoogl… 〔技術: NotebookLMが単なるノートQ&Aから、複数ステップの調査を計…／人文: 研究の“手順”までAIが担うようになると、人間の役割は問いの設計、根…〕 · [x.com](https://x.com/NotebookLM/status/2064016460964585549)
- [ ] **arXiv: NotebookLMをUX ResearchのPoint of View作成に使うケーススタディ** — 「Generative AI in developing User Experience Research Point of V… 〔技術: NotebookLMを、質的データの整理・根拠付き洞察生成・リサーチ…／人文: ユーザーの声をAIで圧縮すると、見えやすいパターンと消えやすい少数意…〕 · [arxiv.org](https://arxiv.org/abs/2605.31125)

### Loop engineering
- [ ] **Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting** — コーディングエージェントを逐次プロンプトで誘導するのではなく、trigger、goal、verification step、st… 〔技術: ループを「再利用可能な制御仕様」として分解し、Claude Code…／人文: philosophy の観点では、人間が命令を逐次発話する主体から、…〕 · [arxiv.org](https://arxiv.org/abs/2607.00038)
- [ ] **AutoPersonas: A Multi-Timescale Loop Engine for Open-Ended Persona Evolution** — 長期的に動くペルソナエージェントが、同じ環境・弱い関係・先送りされた意思決定へ収束する self-locking を問題化し、O… 〔技術: ループの「発散」と「状態への吸収」を分離し、長期記憶を持つエージェン…／人文: anthropology の観点では、AIペルソナを単なる会話キャラ…〕 · [arxiv.org](https://arxiv.org/abs/2607.08252)
- [ ] **SwarmResearch: Orchestrating Coding Agents for Open-Ended Discovery** — 長時間動くコーディングエージェントが、オープンエンドな最適化探索で一つの高レベル方針に早く収束してしまう問題を扱う。 〔技術: ループを単体エージェントの反復ではなく、探索方針を分散させる swa…／人文: history の観点では、研究室の分業、査読、競合仮説の並走という…〕 · [arxiv.org](https://arxiv.org/abs/2607.02807)
- [ ] **StateFuse: Deterministic Conflict-Preserving Memory for Multi-Agent Systems** — マルチエージェントシステムで、分岐、リトライ、複製の間に蓄積する矛盾した観測を上書きで潰してしまう問題に対し、conflict-… 〔技術: ループの記憶層を「最新値の保存」ではなく、矛盾を保持しながら決定論的…／人文: ethics の観点では、エージェントの失敗や矛盾を不可視化せず、後…〕 · [arxiv.org](https://arxiv.org/abs/2607.05844)
- [ ] **Semantic Early-Stopping for Iterative LLM Agent Loops** — Writer-Critic 型の反復ループが固定回数の max_iterations で止められがちな問題に対し、連続するドラフ… 〔技術: 停止条件を単なる回数制限から、意味変化と品質改善の観測に基づく制御へ…／人文: philosophy の観点では、「いつ考えるのをやめるべきか」とい…〕 · [arxiv.org](https://arxiv.org/abs/2606.27009)

### AWS
- [ ] **OpenAI GPT-5.6 Sol / Terra / Luna が Amazon Bedrock で一般提供** — OpenAI の GPT-5.6 系列である Sol、Terra、Luna が Amazon Bedrock で一般提供された。 〔技術: Bedrock が Anthropic だけでなく OpenAI の…／人文: 生成AIの選択は「どの知性を使うか」から「どの制度の中で知性を運用す…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/openai-gpt-sol-terra)
- [ ] **Kiro で Claude Sonnet 5 が利用可能に** — AWS の開発支援環境 Kiro の IDE、CLI、Web で Claude Sonnet 5 が利用可能になった。 〔技術: 仕様駆動ワークフロー、長めの自律実行、自己検証を前提にしたモデル更新…／人文: 開発者の仕事は「コードを書く」から「仕様・判断基準・監督方法を設計す…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/sonnet-5)
- [ ] **Amazon EKS が Kubernetes バージョンのロールバックに対応** — Amazon EKS で Kubernetes コントロールプレーンのアップグレード後、7日以内にバージョンを戻せるロールバック… 〔技術: Kubernetes 運用の最大の心理的障壁だったアップグレード失敗…／人文: インフラ運用では「失敗しない」より「戻れる」ことが組織の勇気を作る。〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/upgrade-amazon-eks-clusters-with-confidence-using-kubernetes-version-rollbacks)
- [ ] **AWS CloudFormation Express mode が最大4倍高速なデプロイを提供** — CloudFormation に Express mode が追加され、リソース設定の適用確認後にデプロイを完了扱いにすることで… 〔技術: 従来の安定化チェックを常に待つ設計から、用途に応じて完了条件を選ぶ設…／人文: 速度は単なる効率ではなく、試す回数を増やして学習のリズムを変える。〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/accelerate-your-infrastructure-deployments-by-up-to-4x-with-aws-cloudformation-express-mode)
- [ ] **Amazon EMR on EKS が Apache Spark troubleshooting agent に対応** — EMR on EKS で Apache Spark troubleshooting agent が利用可能になり、失敗したジョブ… 〔技術: EMR on EC2、EMR Serverless、EMR on E…／人文: 分散データ処理の障害対応は、熟練者の暗黙知に依存しがちだった。〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-emr-eks-spark-troubleshooting)

### Harness engineering
- [ ] **ContextSniper: Claude Code を含む修復エージェントの文脈コストを下げる評価ハーネス** — repository-level program repair で、エージェントが全ファイル読み・広範検索・長いログにトークンを… 〔技術: ハーネスを単なる実行環境ではなく、検索・ログ・記憶を絞り込む「文脈ゲ…／人文: これはAIの「注意」を人間がどう制度化するかという話でもあります。〕 · [arxiv.org](https://arxiv.org/abs/2607.01916)
- [ ] **RuBench: 母語の顧客依頼で coding agent を測るリポジトリ級ベンチマーク** — ロシア語で新規作成された顧客依頼風タスク25件を用い、Claude Code と Codex CLI の製品構成を複数回評価する… 〔技術: ハーネスが「コードが直るか」だけでなく、自然言語仕様・文化圏・コスト…／人文: エージェント評価は英語圏のissue文を標準としがちですが、実際の依…〕 · [arxiv.org](https://arxiv.org/abs/2607.06411)
- [ ] **Agentic Hardware Design as Repository-Level Code Evolution: Markdown harness でハードウェア設計を自律進化させる** — HORIZON は、Markdown harness をプロジェクトパックへコンパイルし、ドメイン知識、実行可能評価器、受け入れ… 〔技術: ハーネスを「Markdownで書ける仕様」から、評価器・受け入れ条件…／人文: ハードウェア設計のような高リスク領域で、エージェントにどこまで自律性…〕 · [arxiv.org](https://arxiv.org/abs/2606.28279)
- [ ] **What makes a harness a harness: agent harness の必要十分条件を定義する概念整理** — Claude Code や Codex CLI、SWE-bench harness、agent framework、IDE pl… 〔技術: 用語を整理することで、製品、評価基盤、SDK、オーケストレータの境界…／人文: 新しい技術領域では、名前が先に流通し、後から実践が追いつきます。〕 · [arxiv.org](https://arxiv.org/abs/2606.10106)
- [ ] **ハーネスエンジニアリング入門: CLAUDE.md の次に来る日本語コミュニティ発の実践整理** — CLAUDE.md、AGENTS.md、ルール分離、スキル、フック、メモリ、検証ループを組み合わせ、AIエージェントの品質を「お… 〔技術: Claude Code 周辺の実践を、コンテキストファイルから永続的…／人文: 日本語コミュニティでは、英語圏の研究用語が現場の比喩や運用知として再…〕 · [qiita.com](https://qiita.com/nogataka/items/d1b3fcf355c630cd7fc8)

### sharp LLM usage
- [ ] **Failure as a Process: An Anatomy of CLI Coding Agent Trajectories** — CLI型コーディングエージェントの失敗を「最終結果」ではなく、発生・進行・回復のプロセスとして分析した研究。 〔技術: エージェント評価を合否スコアから時系列の失敗診断へ拡張し、どの時点で…／人文: 「AIが失敗した」を一言で片づけず、判断がほどけていく過程を読む点が…〕 · [arxiv.org](https://arxiv.org/abs/2607.09510v1)
- [ ] **Scoped Verification for Reliable Long-Horizon Agentic Context Evolution under Distribution Shift** — 運用経験で更新され続けるエージェントのシステム指示を、平文の肥大化ではなく型付き意味グラフとして管理し、変更ノード周辺だけを局所… 〔技術: 「コンテキスト更新」を全文再レビューではなくスコープ付き検証に分解し…／人文: 組織のルールや経験則が増えるほど誰も全体を読めなくなる問題を、AI運…〕 · [arxiv.org](https://arxiv.org/abs/2607.09175v1)
- [ ] **Context Engineering Kit** — Claude Code、OpenCode、Cursor、Antigravity、Gemini CLIなどで使える、軽量なコンテキ… 〔技術: LLM活用を「巨大な万能プロンプト」ではなく、必要なスキルだけを小さ…／人文: 熟練者の暗黙知を、チームで共有できる小さな作法としてパッケージ化して…〕 · [github.com](https://github.com/NeoLabHQ/context-engineering-kit)
- [ ] **Ratel: Context engineering for AI agents** — エージェントに毎回すべてのツールスキーマやスキルを渡すのではなく、そのターンに関係する道具だけを選んで提示するコンテキスト層。 〔技術: ツール呼び出し能力を増やすほど文脈が汚れる問題に対し、検索・選択・段…／人文: 人間の作業環境でも、机の上に全工具を出すと集中できない。〕 · [github.com](https://github.com/ratel-ai/ratel)
- [ ] **devloop: guard-railed development loop for AI coding agents** — Claude CodeやCodex向けに、git状態・MR状態・検証状態を毎回注入するstate busと、保護ブランチへのコミ… 〔技術: 「気をつけて」とプロンプトで頼む代わりに、実行レイヤーで拒否する設計…／人文: 自律的な同僚としてAIを迎えるなら、信頼とは性善説ではなく境界線の明…〕 · [github.com](https://github.com/qiankunli/devloop)

### AI agent trends
- [ ] **The Making of Claude Code** — Claude Code が内部CLIから Anthropic のコーディングエージェントへ育った過程を、研究者・エンジニア・初期… 〔技術: エージェントを単なる補完機能ではなく、CLI・リポジトリ・実行環境・…／人文: 「コードを書く主体」は個人プログラマから、人間とAIが交互に意図を渡…〕 · [anthropic.com](https://www.anthropic.com/features/making-of-claude-code)
- [ ] **Introducing Claude Sonnet 5** — Claude Sonnet 5 は「最もagenticなSonnet」として発表され、ブラウザやターミナルなどのツールを使い、計… 〔技術: エージェント性能を、推論・ツール利用・コンピュータ操作・コスト性能の…／人文: 「賢い回答」より「環境内で責任ある行動をする」ことが価値になるほど、…〕 · [anthropic.com](https://www.anthropic.com/news/claude-sonnet-5)
- [ ] **ChatGPT is now a partner for your most ambitious work** — OpenAI は ChatGPT Work を、アプリやファイルを横断して行動し、必要なら数時間プロジェクトに付き合い、目標を完… 〔技術: 長時間実行・外部アプリ連携・ファイル操作を前提にすると、メモリ、権限…／人文: 「仕事を頼む」経験が、人間の部下・同僚だけでなくAIにも向かうことで…〕 · [openai.com](https://openai.com/index/chatgpt-for-your-most-ambitious-work)
- [ ] **How Deutsche Telekom is rewiring telecommunications with AI** — Deutsche Telekom が OpenAI とともに、カスタマーサービス、従業員ワークフロー、ネットワーク運用、音声の未… 〔技術: 顧客対応からネットワーク運用まで複数ドメインをまたぐため、エージェン…／人文: 通信インフラのような公共性の高い領域でAIが「運用の相棒」になると、…〕 · [openai.com](https://openai.com/index/deutsche-telekom)
- [ ] **VEXAIoT: Autonomous IoT Vulnerability EXploitation using AI Agents** — LLMベースの脆弱性検出エージェントと攻撃実行エージェントを組み合わせ、IoTGoat と Metasploitable 環境で… 〔技術: マルチエージェント構成が、偵察、計画、攻撃実行というセキュリティ作業…／人文: 防御研究として有用である一方、攻撃能力の自動化はデュアルユースの緊張…〕 · [arxiv.org](https://arxiv.org/abs/2607.09653)

### Claude Code
- [ ] **Claude Code v2.1.207: Auto mode一般化とセキュリティ修正の大規模リリース** — Bedrock、Vertex AI、FoundryでAuto modeが環境変数オプトインなしに利用可能になり、長大なストリーミ… 〔技術: 権限モード、管理設定、リモート制御、プラグイン入力の安全性が同時に改…／人文: 「自律化」は便利さだけでなく、同意・監査・誤警告・組織ポリシーの問題…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.207)
- [ ] **Claude Code v2.1.206: `/doctor`、worktree確認、MCPタイムアウトなど現場運用の摩擦を削る更新** — `/cd`のディレクトリ補完、チェックイン済みCLAUDE.mdを整理する`/doctor`提案、git pushの自動許可、外… 〔技術: コード生成能力そのものより、作業ディレクトリ、MCP、認証、バックグ…／人文: AIペアプロの実用性は「賢さ」だけでなく、迷子にならない・黙って壊れ…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.206)
- [ ] **Boris ChernyのClaude Code実践: 5並列、CLAUDE.md、worktree、plan modeの“vanilla”運用** — Yahoo検索結果で、Boris Cherny本人の「I'm Boris and I created Claude Code..… 〔技術: 特殊な巨大フレームワークではなく、複数checkout、通知、計画モ…／人文: “vanilla”な使い方が強調される点は、熟練者の魔術ではなく再現…〕 · [x.com](https://x.com/bcherny/status/2007179832300581177)
- [ ] **日本語実践: 「Claude Code 使い方まとめ【2026年版】設定から実践Tipsまで」** — 2026年版として、Claude Codeの設定から実践Tipsまでを日本語で整理する記事が公開された。 〔技術: 導入、設定、運用Tipsを一つの導線にまとめる記事は、チーム内オンボ…／人文: 日本語圏では「最新機能を追う」だけでなく、社内でどう説明し、初心者が…〕 · [zenn.dev](https://zenn.dev/sunsun_eng/articles/claude-code-ok-2026)
- [ ] **arXiv: CLI coding agentの失敗過程と組織導入を測る研究が相次ぐ** — 「Failure as a Process」はCLI coding agentの失敗を最終結果ではなく、発生・進展・回復の時系列… 〔技術: Claude Codeのような端末常駐エージェントを、ベンチマーク得…／人文: 自律エージェントの価値は「何問解けたか」だけではなく、人間がどこで信…〕 · [arxiv.org](https://arxiv.org/abs/2607.09510)

### Ethics of AI Agents
- [ ] **TrustX Agent Risk Classification Framework (ARC): Risk-Tiering Internally Created Agentic AI Systems** — 企業・公共部門で内製されるエージェント型AIを、7タイプ、12次元のスコアリング、5段階の自律性、3段階のガバナンス出力で分類す… 〔技術: 自律性レベル、用途分類、コーディング支援エージェント向け拡張を組み合…／人文: 責任所在を「モデルの性能」だけに閉じず、組織の承認・監査・権限設計へ…〕 · [arxiv.org](https://arxiv.org/abs/2607.09586)
- [ ] **Institutional Red-Teaming: Deployment Rules, Not Just Models, Causally Shape Multi-Agent AI Safety** — マルチエージェントAIの安全性はモデル本体だけでなく、配備時の「ルール」によって大きく変わるとし、同じエージェント・目的・状態で… 〔技術: 33,924ゲーム規模のベンチマークで、配置ルールの因果効果を分離し…／人文: 「安全なモデルを作る」だけでは不十分で、制度・ルール・身元属性の扱い…〕 · [arxiv.org](https://arxiv.org/abs/2607.07695)
- [ ] **Persuasion Attacks Can Decrease Effectiveness of CoT Monitoring** — エージェントの思考過程を監視すれば危険行動を検出できるという前提を検証し、敵対的エージェントが自然言語の説得でCoTモニターをだ… 〔技術: CoT監視を万能視せず、監視対象のスクラッチパッド自体が説得チャネル…／人文: 「透明性があれば安全」という素朴な倫理観に警鐘を鳴らす。〕 · [arxiv.org](https://arxiv.org/abs/2607.08066)
- [ ] **ガバメントAI「源内」：日本語・文化・価値観を尊重する政府AI基盤** — デジタル庁は、政府職員が安全・安心にAIを使う基盤「源内」を各府省庁へ展開し、2026年度中に全府省庁約18万人が利用可能となる… 〔技術: 行政RAG、国内LLM調達、共通データセット、府省庁横断展開を含む「…／人文: 文化差と公共性が明示されており、AIエージェントを誰の言語・価値観・…〕 · [digital.go.jp](https://www.digital.go.jp/policies/genai)
- [ ] **The Context Access Divide: Interaction-Level Architecture as a Complementary Dimension of Agentic Inequality** — AIエージェントへのアクセス格差を、利用可能性・品質・量だけでなく、ユーザーの知識コーパスへ自律的に文脈取得できるかという「相互… 〔技術: Dynamic Context Retrieval と Manual…／人文: AIエージェント倫理を「危険防止」だけでなく、公平なアクセスと認知負…〕 · [arxiv.org](https://arxiv.org/abs/2607.08495)

### Philosophy of Loop Engineering
- [ ] **Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting** — 「エージェントに逐次プロンプトする」のではなく、トリガー、目標、検証、停止規則、メモリからなる再利用可能な「loop speci… 〔技術: エージェント運用を「会話の上手さ」から、検証可能な停止条件と記憶管理…／人文: これは「知る」とは何かを、単発の答えではなく反復・検証・記録の制度と…〕 · [arxiv.org](https://arxiv.org/abs/2607.00038)
- [ ] **AutoPersonas: A Multi-Timescale Loop Engine for Open-Ended Persona Evolution** — 長期的なペルソナエージェントが高確率な行動パターンへ固定化される「self-locking」を問題化し、Occurrence、O… 〔技術: メモリや状態を即時更新せず、観察から状態への昇格に証拠ゲートを置くこ…／人文: 同一性とは変化しないことではなく、どの出来事を自己史に組み込むかを選…〕 · [arxiv.org](https://arxiv.org/abs/2607.08252)
- [ ] **ArtisanCAD: An Industrial-Level CAD Agent with Expert-Grounded Knowledge Distillation** — 産業CAD向けに、専門家の操作記録やマクロログをCAD-IRという実行可能な中間表現へ蒸留し、CATIA-MCPを通じて実行、視… 〔技術: expert log、手続き表現、実行環境、視覚フィードバックを閉ル…／人文: 熟練者の「見れば分かる」「この順番で直す」という身体化された判断を、…〕 · [arxiv.org](https://arxiv.org/abs/2607.05750)
- [ ] **Show HN: Requirements Engineering with Formal Verification / FizzBee** — FizzBeeは、曖昧なプロンプトから高信号な追加質問を生成し、形式仕様と検証シナリオを作り、コーディングエージェントに渡せる仕… 〔技術: コード生成ループの前段に形式検証と要求工学のゲートを置き、少ない反復…／人文: ここでのループは「機械が作る」以前に「人間が何を望んでいるのかを問う…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=48835012)
- [ ] **EurekAgent: Agent Environment Engineering is All You Need For Autonomous Scientific Discovery** — 自律的科学発見では、エージェントのワークフローを細かく規定するよりも、資源、制約、インターフェース、成果物管理を含む環境を設計す… 〔技術: ループをエージェント内部ではなく、評価指標、実行環境、成果物管理、制…／人文: サイバネティクス的には、知能は頭の中だけでなく環境とのフィードバック…〕 · [arxiv.org](https://arxiv.org/abs/2606.13662)

### Anthropology of Agentic AI
- [ ] **AI Agent Day 2026 Summer：製造・航空・教育・コンサルまで、実装後の業務変革と組織づくりを扱うイベント群** — 「AI Agent Day 2026 Summer」の登壇者公開記事が複数出ており、製造・航空・教育・コンサルなど異なる現場での… 〔技術: エージェント導入の焦点がPoCや単体自動化から、業務プロセス、権限、…／人文: 複数業界の事例が同じイベントで並ぶことで、「AIエージェントをどう迎…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiakFVX3lxTE8zZmJjQjZvMFlWU3NpNHBoMDVKaTJ0THBuelRqR3YwOTNXSVJ0VFFsUzRjS1B1SFlDRUR2UkJyT1JWTkRvdlBnSUt5S3ZIbWk5ZDBGREU2WG9OOHhLVmxuRU5fckEwek9Mb3c?oc=5)
- [ ] **AICX協会「AIエージェント時代の人事白書 2026」：採用・評価制度までエージェント時代に合わせて整理** — AICX協会が、人事部門におけるAI活用、採用、評価制度を整理した「AIエージェント時代の人事白書 2026」を公開したというニ… 〔技術: エージェント活用能力を、プロンプト技術だけでなく業務分解、リスク判断…／人文: 人事白書は、組織が「よい働き手」を定義し直す文書でもある。〕 · [news.google.com](https://news.google.com/rss/articles/CBMidkFVX3lxTE96bE9UNjFnQmFocnZpem5XNi1uU2JyaDJ6VjF6WEhIaXhQcDdNNnRjaXhXenMzU3kyaDlIN180QW1RS2o4RThfS29yWlZSSzRVZUJqLV9aR1dlc3VRLUI0eC05Z1p4QmpIR2lUT3R0ZTRIbzhBakE?oc=5)
- [ ] **参天製薬・NECが語る「AI時代の人事の役割」：人事は何を手放し、何を握るのか** — 参天製薬とNECがAI時代の人事機能について語る記事が、直近の日本語ニュースとして確認された。 〔技術: 人事領域では、採用・配置・評価・学習支援のどこをエージェント化し、ど…／人文: 「手放す／握る」は、組織内の権威と信頼の配置をめぐる文化的な言葉でも…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiY0FVX3lxTE9ZSUh0Ri1veFlBTjF2VzhycGdoOGtydDNRZUVVOFdLWXFyM1doZGtYWHVtclpLYnBtb3BOMHNuaWJidng2eFVHbjBWSUItc0ZJa2JMOVBQaDRSOU81WGw2Vmh0OA?oc=5)
- [ ] **playknot、マーケティング組織向け「AIエージェント導入支援」を開始** — マーケティング組織に特化したAIエージェント導入支援の開始が報じられた。 〔技術: マーケティング向けエージェントは、コンテンツ生成だけでなく、キャンペ…／人文: マーケティング組織には、ブランドの「声」や社内承認の作法といったロー…〕 · [news.google.com](https://news.google.com/rss/articles/CBMidkFVX3lxTE51emdLQXg3S2h6WEpEWHJSNWtUVmR2cVBQU1VWU2F6Q2ZPSTBMSzNBRlN3aEhKemFZaWF6NUFSMnluY1VhOXlMVUlWWkFrUmJpM0JBNENXTnliX2FXR1k3X1BaczNGZ3EwRmVvd2RuSC1yeDlTRFE?oc=5)
- [ ] **Managing Procedural Memory in LLM Agents: Control, Adaptation, and Evaluation** — LLMエージェントの「手続き記憶」が、繰り返し発生する職場タスクで再利用可能なスキルを生むかを評価する研究。 〔技術: エージェントの改善を単発の推論性能ではなく、反復業務から抽出される手…／人文: 「手続き記憶」は、職場の慣習や新人教育で受け継がれる“やり方”に近い…〕 · [arxiv.org](https://arxiv.org/abs/2606.23127)

### History of Automation
- [ ] **ガバメントAI「源内」：行政労働の自動化が制度インフラになる** — デジタル庁は、政府職員が安全・安心に生成AIを利用できる基盤「源内」を各府省庁へ展開し、2026年度中に全府省庁約18万人の政府… 〔技術: 自動化が個別ツール導入ではなく、認証・データ・利用環境・調達を含む政…／人文: 産業革命期の機械化が工場制度を作ったように、生成AIは行政組織の時間…〕 · [digital.go.jp](https://www.digital.go.jp/policies/genai)
- [ ] **Agentic Data Environments** — 自律エージェントは速度・規模・労働効率を高める一方、失敗時のコストが急激かつ不可逆になりうるため、著者らはファイル、API、アプ… 〔技術: AIエージェントの自動化を、モデル性能ではなく実行環境・権限・状態管…／人文: 自動化の歴史では、機械そのものよりも工場、標準時、帳簿、監督制度が労…〕 · [arxiv.org](https://arxiv.org/abs/2607.07397)
- [ ] **AI Adoption in S&P 500 Firms** — S&P 500企業の2016〜2025年のAI採用をSEC 10-K提出書類から推定し、単なるAI言及ではなく業務プロセスへの深… 〔技術: 企業広報ではなく規制書類を使って「AI導入の深さ」を測定し、ハイプと…／人文: 自動化史では、技術の発明と労働市場への影響の間に長い制度的ラグがある…〕 · [arxiv.org](https://arxiv.org/abs/2607.08920)
- [ ] **Learning When to Automate: Queue Control in Human-AI Service Systems** — チャットボットが処理し、失敗したタスクを人間エージェントのキューへ送る二段階サービスシステムで、どの程度AIへ資源配分するかを学… 〔技術: UCBとDrift-Plus-Penalty制御を組み合わせ、未知の…／人文: これはコールセンターや行政窓口の自動化史に直結する。〕 · [arxiv.org](https://arxiv.org/abs/2607.06017)
- [ ] **Economics of Human and AI Collaboration: When is Partial Automation More Attractive than Full Automation?（古いが関連）** — 自動化を「する／しない」の二択ではなく、AI精度と費用に応じた連続的な自動化強度としてモデル化する研究。 〔技術: スケーリング則、タスク複雑性、O*NETデータ、専門家調査を接続し、…／人文: 自動化の歴史は「完全な無人化」より、熟練の分解、監督労働の増加、例外…〕 · [arxiv.org](https://arxiv.org/abs/2603.29121)

### DDD
- [ ] **AI時代のシステム崩壊に備えよ：仕様・ドメイン・イベントの「3つの駆動」で構築する究極のアーキテクチャ** — AIコーディングの加速が「エラー隠蔽」「コピペ」「短期コードチャーン」を増やし、本番安定性を損なうという問題意識から、DDD・イ… 〔技術: DDDを「LLMのコンテキスト窓・Lost in the Middl…／人文: AIを万能な開発者ではなく、境界と制度を必要とする強力な組織メンバー…〕 · [qiita.com](https://qiita.com/satouo/items/1e39fd9e24e2961c2710)
- [ ] **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — GitHub上のDDD実践を大規模に調査した実証研究です。 〔技術: DDDを思想や事例談ではなく、OSSエコシステムの実データとして測定…／人文: DDDが「一部の熟練者の信仰」ではなく、長期運用される共同体の持続的…〕 · [arxiv.org](https://arxiv.org/abs/2607.06471)
- [ ] **golden pathテンプレートに「受注-在庫」機能をAIエージェントで実装させ、実AWSで検証してみた** — FastAPI + Vue 3 + Terraform + 品質ゲート + SDD運用のgolden pathテンプレートに、C… 〔技術: AIエージェントを業務アプリに投入する際、DDD的な集約・トランザク…／人文: 「AIに丸投げ」ではなく、破壊的操作や環境デプロイ前に人間の確認を挟…〕 · [qiita.com](https://qiita.com/itouhi/items/98a18cf43e280308c965)
- [ ] **アーキテクチャは「AIへの権限委譲設計」になる — Claude Codeで大規模案件を回すための設計思想と判断基準** — DDDと生成AIの相性を、単なる「DDDコードをAIが書きやすい」という話から一段上げ、Claude Codeや複数エージェント… 〔技術: ユビキタス言語や境界づけられたコンテキストを、LLMへの高圧縮プロト…／人文: アーキテクチャを「権限委譲設計」と呼ぶことで、設計判断が組織論・統治…〕 · [qiita.com](https://qiita.com/similarmetal/items/caaa509aa2d5ec5925f9)
- [ ] **ビジネスアーキテクチャにおけるFit to Standard戦略と思考メカニズム（古いが関連性が高い）** — Fit to Standardを単なるSaaS導入手法ではなく、TOCやBPRを背景にした業務プロセス矯正の経営戦略として捉え、… 〔技術: イベントストーミングやコアドメインチャートを、システム分割だけでなく…／人文: DDDが現場の言葉を尊重するだけでなく、「その言葉やプロセスは本当に…〕 · [qiita.com](https://qiita.com/Kudo_panda/items/ce835554df5a4b393d1e)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

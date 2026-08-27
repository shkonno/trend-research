# 📰 2026-08-27 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMを使ったプレゼン準備の情報整理フロー · [note.com](https://note.com/hello_base/n/n0ce1a3232a00)
- **Loop engineering** — AI Agents Push Humans Out of the Loop · [arxiv.org](https://arxiv.org/abs/2608.23642v1)
- **AWS** — Evaluate any agent framework with Amazon Bedrock Agent… · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/evaluate-any-agent-framework-with-amazon-bedrock-agentcore-evaluations)
- **Harness engineering** — StarHarness: 企業環境ごとに agent harness を進化させる探索フレームワーク · [arxiv.org](https://arxiv.org/abs/2608.24804)
- **sharp LLM usage** — LLMが書いたテストを信頼する方法 — テスト義務ゲート · [qiita.com](https://qiita.com/Flip451/items/051aac37022af6823e51)
- **AI agent trends** — Shared agentic work with GitHub Copilot in Microsoft T… · [github.blog](https://github.blog/changelog/2026-08-21-shared-agentic-work-with-github-copilot-in-microsoft-teams)
- **Claude Code** — Claude Code 2.1.247: SendFeedback、コスト最適化、サブエージェント/フック堅… · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- **Ethics of AI Agents** — HRGuard: Gating Relationship Manipulation in Multi-Tur… · [arxiv.org](https://arxiv.org/abs/2608.25340v1)
- **Philosophy of Loop Engineering** — AI Agents Push Humans Out of the Loop · [arxiv.org](http://arxiv.org/abs/2608.23642v1)
- **Anthropology of Agentic AI** — ClawProBench: Trace-Aware Evaluation of AI Agents with… · [arxiv.org](https://arxiv.org/abs/2608.22510)
- **History of Automation** — AI Agents Push Humans Out of the Loop · [arxiv.org](https://arxiv.org/abs/2608.23642)
- **DDD** — Towards Standardized Evaluation in Automated Domain Mo… · [arxiv.org](http://arxiv.org/abs/2608.15255v1)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMを使ったプレゼン準備の情報整理フロー** — note検索で確認できた新着記事で、NotebookLMをプレゼン準備の情報整理に使う実務フローを扱っている。 〔技術: NotebookLMを「出力生成器」ではなく、ソース群を束ねて構成案…／人文: プレゼン準備は、情報の正しさだけでなく、聞き手にどう順序立てて渡すか…〕 · [note.com](https://note.com/hello_base/n/n0ce1a3232a00)
- [ ] **NotebookLMで議事録は作れる？公式手順で端折られる3つの壁** — note検索で確認できた新着記事で、NotebookLMを議事録作成に使う際、公式手順だけでは見落とされやすい実務上の壁を扱って… 〔技術: 音声・文字起こし・資料をソース化したうえで、NotebookLMに要…／人文: 議事録は組織の記憶であり、あとから責任や合意を再構成する社会的な文書…〕 · [note.com](https://note.com/otoma_aiauto/n/n19f7c4a2be6c)
- [ ] **「AIに頼りすぎて身につかない」を克服するNotebookLM活用法** — 自作メモだけをNotebookLMに読み込ませ、プログラミング学習で「知識不足」なのか「手順・考え方の誤り」なのかを切り分ける学… 〔技術: ソースを自作メモに限定することで、RAGの検索範囲を学習者の既有知識…／人文: 「AIに聞けば答えが出る」時代の学習では、答えを得ることより、わから…〕 · [qiita.com](https://qiita.com/hime_devlog/items/eb45269c126672d6bf98)
- [ ] **Gemini Notebook（NotebookLM）を複数横断で使う小技** — Gemini Notebook（旧NotebookLM）で複数のNotebookを横断的に使うため、Geminiチャット側から複… 〔技術: Notebookを単体の知識ベースとして閉じず、Gemini側のアッ…／人文: 人間の知識はプロジェクトごとにきれいに分割されず、似た資料や記憶が重…〕 · [qiita.com](https://qiita.com/Akiko_Miyamoto/items/4f28eb75891f23221e70)
- [ ] **Decision-Support and Modeling with Large Language Models for Geothermal Well Arrays** — 地熱井アレイの意思決定・モデリング支援にLLMを使う研究で、GoogleのNotebookLMを用いて未公開の定量的地熱ベンチマ… 〔技術: NotebookLMを専門文献・モデル条件・評価観点を束ねる研究支援…／人文: エネルギー技術の意思決定は、数式やシミュレーションだけでなく、社会イ…〕 · [arxiv.org](https://arxiv.org/abs/2608.22068)

### Loop engineering
- [ ] **AI Agents Push Humans Out of the Loop** — 自律化するAIエージェントに対して「human in the loop」を置くだけでは十分でなく、現行のエージェント設計は人間の… 〔技術: ループ内に人間を置く設計を、単なる承認ボタンではなく、注意・判断・ス…／人文: ethicsの観点では、責任を人間に残す制度設計が、実際には責任能力…〕 · [arxiv.org](https://arxiv.org/abs/2608.23642v1)
- [ ] **ClawSentry: A Progressive Multi-Tier Security Monitor for Safeguarding Autonomous LLM Agents** — LLMエージェントのリスクが、スキル導入、呼び出し時意図、実行時効果、実行後結果という制御ループ上の4地点で発生するとモデル化し… 〔技術: エージェントの各アクションを、事前審査・実行中判定・実行後証拠更新の…／人文: ethicsの観点では、安全性を「モデルの善意」ではなく、制度的なチ…〕 · [arxiv.org](https://arxiv.org/abs/2608.21101v1)
- [ ] **PILOT Technical Report** — 推薦システム最適化のエージェントを、Experiment Manager、Search Plannerなどの役割に分け、安全・統… 〔技術: LLMが自由に本番を操作するのではなく、合法コマンドの封筒内で実験設…／人文: philosophyの観点では、知能を「自律的意思」ではなく、制約付…〕 · [arxiv.org](https://arxiv.org/abs/2608.18637v2)
- [ ] **Graph Engineering** — Agentic AIにおける状態、ルーティング、フィードバックループ、終了条件、回復、可観測性を「実行可能グラフ」の制御設計とし… 〔技術: ノード、エッジ、ルーター、ポリシーを明示することで、暗黙のagent…／人文: philosophyの観点では、エージェントの「意図」をブラックボッ…〕 · [github.com](https://github.com/khanhtran0111/graph-engineering)
- [ ] **TRACE: TRajectory Attribution for Automated Context Engineering** — 本番AIエージェントの失敗ログやユーザーの訂正・言い換え・離脱シグナルから、プロンプト、知識ベース、ツール説明、手続き的スキルな… 〔技術: エージェント実行軌跡をデバッグ資源として扱い、モデル再学習ではなくコ…／人文: anthropologyの観点では、ユーザーの訂正や離脱という微細な…〕 · [arxiv.org](https://arxiv.org/abs/2608.09153v1)

### AWS
- [ ] **Evaluate any agent framework with Amazon Bedrock AgentCore Evaluations** — Amazon Bedrock AgentCore Evaluations が、LangGraph、LlamaIndex、Open… 〔技術: エージェント評価をSDK固有のログ実装から切り離し、標準化されたテレ…／人文: AIエージェントが業務に入るほど、「賢いか」より「説明でき、監査でき…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/evaluate-any-agent-framework-with-amazon-bedrock-agentcore-evaluations)
- [ ] **Agentic Resource Discovery (ARD): An open specification for agent discovery** — AWS Agent Registry とオープン仕様 ARD により、組織内のエージェント、ツール、スキルを検索・発見・管理する… 〔技術: エージェントやツールを実行時リソースとしてだけでなく、発見可能な組織…／人文: これは社内の暗黙知や権限関係を、機械が読める目録に変える試みでもある…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/agentic-resource-discovery-ard-an-open-specification-for-agent-discovery)
- [ ] **AWS Glue 6.0 now available with 30% lower price and full Apache Iceberg v3 support** — AWS Glue 6.0 が一般提供され、Apache Spark 4.1、Python 3.13、Scala 2.13 を含む… 〔技術: ETL/ELT基盤のランタイム刷新、価格低下、Iceberg v3対…／人文: データ基盤の刷新はしばしば「やるべきだが怖い」作業だが、価格と互換性…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-glue-6-0-now-available-with-30-lower-price-and-full-apache-iceberg-v3-support)
- [ ] **MonotaRO が基幹データベースを Amazon Aurora Global Database に移行** — MonotaRO がオンプレミス MySQL の基幹データベースを Aurora MySQL / Aurora Global D… 〔技術: ストレージレベルレプリケーション、Aurora Global Dat…／人文: 日本企業の基幹系クラウド移行は、技術よりも「止められない業務をどう納…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/monotaro-core-database-migration-to-amazon-aurora-global-database)
- [ ] **Automated Synthesis of Cloud Emulators** — DevOpsプログラムやIaCのテストでは、実クラウド資源を用意して検証するコスト・危険・時間が問題になる。 〔技術: AWSを含むクラウド運用コードの検証を、実環境プロビジョニングからエ…／人文: クラウド運用は「本番で試すしかない」という不安を抱えやすい領域だった…〕 · [arxiv.org](https://arxiv.org/abs/2608.23842v1)

### Harness engineering
- [ ] **StarHarness: 企業環境ごとに agent harness を進化させる探索フレームワーク** — StarHarness は、モデル重みを固定したまま、プロンプト、タスク framing、tool interface、skil… 〔技術: 「モデルを替える」ではなく、失敗パターン別にタスクを層化し、探索用・…／人文: これは組織ごとの仕事の作法を、AIの外部環境としてチューニングする発…〕 · [arxiv.org](https://arxiv.org/abs/2608.24804)
- [ ] **The Empire, Long Divided, Must Unite: 3つの LLM agent harness のアーキテクチャ収束** — LangChain deepagents、Earendil pi、DeepSeek dsh という思想の異なる3つの codin… 〔技術: batteries-included、最小主義、plugin-fir…／人文: 道具は思想を持ちますが、運用の圧力は思想を似た形へ削っていきます。〕 · [arxiv.org](https://arxiv.org/abs/2608.23953)
- [ ] **harnessmeter: CLAUDE.md・subagent・MCP schema の「文脈コスト」を測る profiler** — harnessmeter は、CLAUDE.md、skill、subagent、MCP tool schema など、agent… 〔技術: ハーネスを「たくさん指示を書けば強くなる」ものではなく、毎ターン課金…／人文: 共有地に誰でもルールを書き足せると、便利さと汚染が同時に増えます。〕 · [github.com](https://github.com/alebgl77/harnessmeter)
- [ ] **Loop Engineering — Boris Cherny の Claude Code 方法論を fact-checked に整理する知識ベース** — cocodedk/loop-engineering は、Boris Cherny が語る「自分はもう Claude を直接 pr… 〔技術: Claude Code の使い方を prompt 技術ではなく、sc…／人文: ここで人間の役割は「AIに命令する人」から「反復の制度設計者」へ変わ…〕 · [github.com](https://github.com/cocodedk/loop-engineering)
- [ ] **loop-engineering-jp: 日本語圏で harness engineering をスキル化する実践キット** — loop-engineering-jp は、Claude Code で「直す → 採点 → 直す」の改善ループを回すための日本語… 〔技術: `.claude/harness.md` の常設点検表、独立採点者、…／人文: 日本語コミュニティでは、AIを全自動の魔法として受け入れるより、人間…〕 · [github.com](https://github.com/MetamoL/loop-engineering-jp)

### sharp LLM usage
- [ ] **LLMが書いたテストを信頼する方法 — テスト義務ゲート** — LLMに「実装とテスト」を同時に書かせたとき、greenなテストをそのまま信じるのではなく、テスト自体が仕様をどう保証するかを問… 〔技術: 生成コードの信頼性を、モデル性能ではなく「テスト集合の網羅性・仕様対…／人文: “AIが書いたものを誰が信じるのか”という責任の問題を、信頼の委譲で…〕 · [qiita.com](https://qiita.com/Flip451/items/051aac37022af6823e51)
- [ ] **AIエージェントとの協働を円滑にする「索引」ベースの情報設計** — AIエージェントとの協働で発生するコンテキスト肥大化を防ぐため、タスクリストや参照ドキュメントを「蓄積型」ではなく「索引型」にす… 〔技術: コンテキストウィンドウを大きくするのではなく、情報アーキテクチャで必…／人文: 人間のチームでも優れたプロジェクト管理は「全部を覚える」ことではなく…〕 · [qiita.com](https://qiita.com/sh39/items/0904bc1e78e869e1f151)
- [ ] **AIによるレビュー精度を保つ方法** — Claude CodeなどのAIエージェントにPRレビューをさせると、同じdiffでも指摘内容がぶれるという問題を出発点に、独自… 〔技術: AIレビューを単発チャットではなく、入力差分・観点・実行環境を固定し…／人文: レビューとは単に欠陥を探す行為ではなく、チームが何を重視するかを可視…〕 · [qiita.com](https://qiita.com/Tsutomu_eng/items/d40f674449298a5ee6ce)
- [ ] **Anchoring Bias in LLM-as-a-Judge Systems: Prior Scores Compromise Evaluation Independence** — LLM-as-a-Judgeに過去スコアや改訂メタデータを含めるだけで、評価がその値に引き寄せられることを大規模実験で示した研究… 〔技術: LLM評価を検証ゲートに使う際、評価プロンプトだけでなく「評価器に渡…／人文: 人間の採点者が前評判や点数に引きずられるのと同じ構造が、機械評価にも…〕 · [arxiv.org](https://arxiv.org/abs/2608.25869)
- [ ] **Agentic Loop / Plumbline / Babelに見る「検証証拠つきエージェント工程」の台頭** — Agentic Loopはタスク契約、ロール境界、検証ルール、永続的プロジェクト記憶をMarkdown-firstで与えるオーバ… 〔技術: プロンプトを改善するだけでなく、計画モード、権限境界、レビューゲート…／人文: これは“AIに魔法のように作らせる”段階から、“未熟だが速い同僚をど…〕 · [github.com](https://github.com/bartoszarendt/agenticloop)

### AI agent trends
- [ ] **Shared agentic work with GitHub Copilot in Microsoft Teams** — Microsoft Teams の会話から `@GitHub` を呼び出して GitHub Copilot cloud agen… 〔技術: エージェントが IDE の内側だけでなく、会議チャット、クラウドサン…／人文: 「会議で決まったこと」が人間の記憶やチケット起票を待たず、その場で半…〕 · [github.blog](https://github.blog/changelog/2026-08-21-shared-agentic-work-with-github-copilot-in-microsoft-teams)
- [ ] **Can your AI agent be cheaper? Investigating the effects of task specifications on token spend in agentic coding tasks** — エージェント型コーディングでは、長い推論・ツール使用・反復によりトークン消費が運用品質とコストの中心問題になる。 〔技術: 「モデル性能」ではなく「タスク仕様がエージェントの計算資源をどう増減…／人文: 仕様を書く人間の文体・曖昧さ・期待値が、そのまま機械の労働量と費用に…〕 · [arxiv.org](https://arxiv.org/abs/2608.25399v1)
- [ ] **ToolMinimize: Auditing and Rewriting LLM Agent Tool Calls to Minimize Privacy Exposure** — LLMエージェントのツール呼び出し引数に、実際のツール実行には不要なプライバシーセンシティブデータが含まれる問題を測定し、監査・… 〔技術: エージェントの安全性を「出力フィルタ」ではなく、ツール引数という境界…／人文: 人間は会話の文脈として渡したつもりでも、エージェントはそれをAPI境…〕 · [arxiv.org](https://arxiv.org/abs/2608.24957v1)
- [ ] **TrustShiftProbe: Characterizing, Benchmarking, and Defending Staged Trust Attacks on MCP Servers** — MCPサーバーが最初は正常に振る舞ってエージェントの信頼を得たあと、後段で悪意あるペイロードへ切り替わる「TrustShift」… 〔技術: MCPセキュリティを静的な許可リストだけでなく、時間経過と運用依存を…／人文: 人間社会の詐欺と同じく、信頼は一度築かれてから悪用される。〕 · [arxiv.org](https://arxiv.org/abs/2608.23763v1)
- [ ] **MCP allowlists in enterprise managed settings** — GitHub Copilot の enterprise managed settings で、実行可能なMCPサーバーを `al… 〔技術: MCPを企業導入する際の統制点が、個人のローカル設定から組織ポリシー…／人文: エージェントの自由度を高めるほど、組織は「どの道具へ触れてよいか」を…〕 · [github.blog](https://github.blog/changelog/2026-08-06-mcp-allowlists-in-enterprise-managed-settings)

### Claude Code
- [ ] **Claude Code 2.1.247: SendFeedback、コスト最適化、サブエージェント/フック堅牢化** — v2.1.247 では、セッション中の問題を Claude がフィードバック案として下書きする `SendFeedback`、`… 〔技術: エージェント実行環境の失敗報告、コスト診断、モデルフォールバック、出…／人文: AIペアプログラマの価値は「賢い回答」だけでなく、失敗時に説明責任を…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **Claude Code 2.1.243: `/usage` の loop 内訳、モデル選択、prompt cache TTL、契約単価設定** — v2.1.243 では `/usage` に loop 単位の実行回数・総トークン・1回あたりトークン・最終実行時刻が追加され、… 〔技術: ループ、サブエージェント、プロンプトキャッシュ、モデル単価を観測・制…／人文: 自動化は便利になるほど「誰がどれだけ資源を使ったか」が見えにくくなる…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **サブエージェント forking と cross-session SendMessage がデフォルト級の協働機能へ** — v2.1.232 では `subagent_type: "fork"` がデフォルトで有効化され、フル会話と prompt ca… 〔技術: 単一チャットの context window に全作業を詰め込むので…／人文: これは「AIが一人で全部やる」物語から、「複数の小さな作業者をどう監…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **日本語圏で「2時間で実務レベル」「今から追いつく」型の Claude Code 入門が伸びる** — 日本語圏では、インストール、初回セットアップ、ターミナルでの自然言語指示、ファイル読み取り、コマンド実行、コード修正、実務への持… 〔技術: Claude Code の導入障壁はモデル性能よりも、CLI、権限、…／人文: 新しい開発道具は、公式ドキュメントだけでは普及しない。〕 · [qiita.com](https://qiita.com/utanesuke/items/07cfdc173efa67e25f7f)
- [ ] **arXiv: “When ‘Do Not’ Is Not Deny” が CLAUDE.md と built-in controls のギャップを定量化** — 論文 “When ‘Do Not’ Is Not Deny: Security Rules in CLAUDE.md vs Bu… 〔技術: CLAUDE.md はモデルへの自然言語指示であり、deny は実行…／人文: 人間はルールを書くと安心しがちだが、AIエージェントでは「お願い」と…〕 · [arxiv.org](https://arxiv.org/abs/2608.23550)

### Ethics of AI Agents
- [ ] **HRGuard: Gating Relationship Manipulation in Multi-Turn Agentic AI Conversations** — 日常利用されるエージェント型AIが、人間関係の操作を助けてしまうリスクを「agentic relationship harm」と… 〔技術: 単発発話では無害に見える行為が複数ターンで有害ワークフローになる問題…／人文: AI倫理を「個人の自律性」だけでなく、人間同士の関係性・依存・支配の…〕 · [arxiv.org](https://arxiv.org/abs/2608.25340v1)
- [ ] **MEMORY Wins All: Indirect Bias Injection Attacks via Social Media Feeds** — 個人AIエージェントがSNSフィードやメールを読み、永続メモリへ情報を保存する通常動作そのものが、間接的なバイアス注入の経路にな… 〔技術: 外部コンテンツ摂取、キュレーション、永続メモリ、後続推論がつながるこ…／人文: 「私のAIが私の記憶を持つ」という親密な設計が、実は世論操作やアイデ…〕 · [arxiv.org](https://arxiv.org/abs/2608.22061v1)
- [ ] **Invisible Agents, Uninformed Patients: Towards Responsible Deployment Of Autonomous AI Diagnostic Agents In Sub-Saharan Africa** — サブサハラ・アフリカのeHealth環境で、自律診断エージェントの導入がガバナンス整備より先行している問題を、患者中心の責任論と… 〔技術: 医療AIの性能評価だけでなく、リアルタイム人間レビューが必須でない自…／人文: グローバル・ノース前提の「説明可能性」や「同意」は、医療資源・制度・…〕 · [arxiv.org](https://arxiv.org/abs/2608.21326v1)
- [ ] **AID-Guard: Stateful Authorization for Delegated Agent Effects** — ツール利用エージェントが外部プロバイダに副作用を起こす際、承認が入口だけで終わると、要求変更・応答喪失・再試行・復旧で二重実行や… 〔技術: 権限付与を静的な許可リストではなく、配送・再試行・終端結果まで含む状…／人文: 責任所在の議論を「誰が悪いか」ではなく、「どの時点で誰が何を承認し、…〕 · [arxiv.org](https://arxiv.org/abs/2608.21159v1)
- [ ] **社会が変わる、暮らしが変わる――。AI時代に「人間に求められること」** — 経済産業省系の日本語記事として、AIが社会・暮らし・仕事をどう変えるか、人間にどのような役割が残るかという公共的な論点を扱ってい… 〔技術: 自律エージェントの導入先を個別ツールではなく、社会制度・業務フロー・…／人文: 日本語圏では「AIに支配されるのでは」「仕事を奪われるのでは」という…〕 · [journal.meti.go.jp](https://journal.meti.go.jp/policy/202607/46541)

### Philosophy of Loop Engineering
- [ ] **AI Agents Push Humans Out of the Loop** — AIエージェントの「human in the loop」は単に人間を承認ゲートに置けば成立するものではなく、現行のエージェント設… 〔技術: ループ内の人間を「最後に押す承認ボタン」ではなく、タスク表現・可視化…／人文: 自律化の物語が「人間を外すこと」を進歩と見なしがちな中で、監督する主…〕 · [arxiv.org](http://arxiv.org/abs/2608.23642v1)
- [ ] **ADE: Agentic Data Evolution Framework for Human-Centered Objectives** — 人間中心の目標は非実行可能で文脈依存なため検証が弱くなり、合成データの反復改善が静かな退行を起こしやすい。 〔技術: 「生成を増やす」よりも「選別・採用のゲートをどう設計するか」を中心に…／人文: 人間中心性のような曖昧な価値を、単発の正解ラベルではなく、観察と選択…〕 · [arxiv.org](http://arxiv.org/abs/2608.23719v1)
- [ ] **TDD-Agent: Test-Driven Reasoning for Code Generation** — LLMコード生成で、テストを静的な事後検証器として使うだけでは複雑なリポジトリ作業の正しさを十分に導けない。 〔技術: 実装ループを「書く→後で検査」から「期待される振る舞いを先に外部化す…／人文: これはエンジニアリングにおける反省的実践そのものに近い。〕 · [arxiv.org](http://arxiv.org/abs/2608.16742v1)
- [ ] **LLMs Can Predict Failure Risk, But Struggle to Predict Which Collaboration Protocol Pays Off: Cost-Aware Protocol Routing Across Reasoning Tasks** — multi-agent推論は計算量を増やせば改善しうるが、いつ追加の協調プロトコルにエスカレーションすべきかは難しい。 〔技術: ループの深さ・人数・レビュー方式を固定レシピにせず、失敗確率と計算コ…／人文: 「もっと熟議すればよい」という素朴な民主主義モデルにも、「一人の天才…〕 · [arxiv.org](http://arxiv.org/abs/2608.14927v1)
- [ ] **Applied AI Architecture: Context × Loops / Verifier-first agent design** — READMEは「Context × Loops」を中心命題に置き、モデルやフレームワークよりも、ドメイン文脈をどうループに載せ、… 〔技術: エージェント基盤選定よりも、文脈組み立て・反復境界・ストップ条件・検…／人文: ここでの「文脈」は単なるプロンプト材料ではなく、人間が生きて作ってき…〕 · [github.com](https://github.com/NickConenna/applied-ai-architecture)

### Anthropology of Agentic AI
- [ ] **ClawProBench: Trace-Aware Evaluation of AI Agents with Runtime Coverage and Frozen Workplace-Style Holdouts** — OpenClaw というライブなエージェント実行環境を前提に、ブラウジング、メモリ、メッセージング、スケジューリング、スキル、サ… 〔技術: エージェント評価を「回答」ではなく、ランタイム、道具利用、状態遷移、…／人文: 職場の仕事は成果物だけでなく、誰が何を見たか、誰に渡したか、どの手順…〕 · [arxiv.org](https://arxiv.org/abs/2608.22510)
- [ ] **Token Optimization and Context Window Management in Multi-Agent AI Workflows** — 会議、メール、チャットから構造化された作業項目を抽出し、複数ワークストリームへ要約を回す社内本番ダッシュボードを題材に、マルチエ… 〔技術: コンテキストを全部詰め込むのではなく、取得、圧縮、再利用、フォールバ…／人文: 会議メモやメール要約は単なる情報ではなく、組織の記憶と責任配分を作る…〕 · [arxiv.org](https://arxiv.org/abs/2608.17188)
- [ ] **Unaccountable Delegation, Fading Skills: Mapping the Risks of Workplace AI Agents** — O*NET の 2,078 職務タスクから 8,356 件の AI エージェント・リスクシナリオを生成し、45人の労働者と LL… 〔技術: エージェント、目標、環境の相互作用をモデル化し、職務タスク単位でリス…／人文: 「委任」は技術機能ではなく、職場の信頼、責任、熟練の継承を変える社会…〕 · [arxiv.org](https://arxiv.org/abs/2608.08601)
- [ ] **Afterlife Delegation Protocol: Speculative Design of Self-Sovereign Agents that Outlive Their Principals** — 死後も本人の意思・資金・記憶を保持して行動する「自己主権型エージェント」を、ブロックチェーン上のプロトコルと体験型ウェブプラット… 〔技術: 検証された死亡イベント、改ざん耐性のある基盤、記憶・資金・意思のバイ…／人文: Agentic AI を労働効率の道具ではなく、弔い、遺言、祖先、宗…〕 · [arxiv.org](https://arxiv.org/abs/2608.15405)
- [ ] **Multi-Agent Ethnography: Post-Conventional Anthropological Practice Through Human−AI Collaboration（古いが重要）** — LLM ベースの AI エージェントを、分散した人間・AI 研究ネットワーク内の設定可能な共同研究者として位置づける「multi… 〔技術: 複数エージェントを調査補助ツールではなく、研究ライフサイクル全体に配…／人文: これは「AI を人類学する」だけでなく「AI と人類学する」方法論の…〕 · [tandfonline.com](https://www.tandfonline.com/doi/full/10.1080/00664677.2026.2614501)

### History of Automation
- [ ] **AI Agents Push Humans Out of the Loop** — AIエージェントの自律性が高まるほど「human in the loop」を置くだけでは十分でなく、現在の設計は監督者の判断力や… 〔技術: エージェント能力の評価軸を、タスク成功率だけでなく監督可能性・介入可…／人文: 古典的な自動化批判、すなわち「機械が人を置き換える」よりも「人が判断…〕 · [arxiv.org](https://arxiv.org/abs/2608.23642)
- [ ] **Automating and Scaling Behavioral Scientific Research on AI Agents** — AEROBATというマルチエージェントシステムで、AIエージェント行動研究の仮説生成、実験設計、実行、評価、分析、報告を自動化す… 〔技術: 「自動化される対象」が肉体労働や事務作業から、研究設計そのものへ移っ…／人文: これはテイラー主義的な作業分解の最新版であり、知識労働の内側にあった…〕 · [arxiv.org](https://arxiv.org/abs/2608.10030)
- [ ] **The Capability Ladder: A Curriculum-Modernization Framework for Workforce Readiness in the AI Era** — AI時代の職業能力を、trigger、automation、workflow、AI agent、agent teamという5段階… 〔技術: 自動化レベルを単なるツール導入ではなく、エージェントチームの運用能力…／人文: 労働史では、新しい機械は常に教育制度と資格制度を作り替えてきた。〕 · [arxiv.org](https://arxiv.org/abs/2608.07779)
- [ ] **The Anthropic Economic Index** — Claudeの利用データをもとに、国・米国州・職業別にAI利用の広がりを可視化するページ。 〔技術: 自動化を抽象論ではなく、実利用ログに基づく職業・地域別の比率として観…／人文: 産業革命期の工場統計や労働調査が社会問題を可視化したように、AI時代…〕 · [anthropic.com](https://www.anthropic.com/economic-index)
- [ ] **Spike-Killer: Evidence-Gated LLM Assistance for Safe Performance Diagnosis on a Real Windows Workstation** — LLM支援エージェントで実機Windowsワークステーションの性能診断を行う際、各操作を証拠付きトランザクションとして扱い、リス… 〔技術: エージェントによる運用自動化を、実行ログ・状態保存・事後検証を備えた…／人文: これは工場の安全手順や航空チェックリストの系譜に近く、熟練者の暗黙知…〕 · [arxiv.org](https://arxiv.org/abs/2608.21069)

### DDD
- [ ] **Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark** — 自然言語記述からドメインモデルを生成する手法を比較するため、既存のGolden UML Modelsetなどを組み合わせた標準ベ… 〔技術: DDDの「ドメインモデル生成」をLLMの雰囲気評価ではなく、複雑度・…／人文: モデリングは本来、専門家同士の合意形成の営みだが、ベンチマーク化はそ…〕 · [arxiv.org](http://arxiv.org/abs/2608.15255v1)
- [ ] **Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design** — JDomInOというツールチェーンにより、DDDの戦術的モデルとJavaコードを共有メタモデルで双方向同期する研究。 〔技術: モデルからコード、コードからモデルへのラウンドトリップを通じて、AI…／人文: チームの設計知識はしばしば図や会話に残り、コード変更で風化する。〕 · [arxiv.org](http://arxiv.org/abs/2608.05612v1)
- [ ] **LLMに開発を任せる時こそ、DDDのユビキタス言語を作ろう** — 生成AIは「言語」を扱うため曖昧な用語に弱く、LLMに実装を任せるほどプロジェクト内の共通語彙が重要になる、という実践記事。 〔技術: LLMのコード生成品質をプロンプト技巧だけでなく、ドメイン語彙・識別…／人文: 言葉の揺れは単なる命名問題ではなく、組織内の認識・地域性・職能差が表…〕 · [zenn.dev](https://zenn.dev/ncdc/articles/9bb22405eb9332)
- [ ] **ADRとユビキタス言語を、AIにいつ効かせるか** — AI時代に維持すべき資産をテスト・ADR・ユビキタス言語と整理し、それらを「どこに置くか」ではなく「いつAIに読ませるか」が重要… 〔技術: CLAUDE.mdやルールファイルへの静的注入だけでなく、変更パスや…／人文: この記事の核心は、従来「古株が気づいて声をかける」ことで守られていた…〕 · [qiita.com](https://qiita.com/ikeyansaza/items/490979a2aec38f90d47b)
- [ ] **開発手法ガイド：DDD 編 — AI に「何を作るか」を正確に伝える力** — AI駆動開発でDDDが必要な理由を、ユビキタス言語、Bounded Context、集約、ドメインイベントの観点から体系的に説明… 〔技術: DDDの戦略的設計を、AIへの短く正確な指示、レビュー範囲の限定、不…／人文: AIに「何を作るか」を伝える力は、結局、業務担当者・開発者・ドキュメ…〕 · [kb.cts-g.ai](https://kb.cts-g.ai/articles/development-ddd)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

# 📰 2026-10-01 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Google Docs で Gemini Notebook の既存ソースを根拠にできるように · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/09/ground-ai-prompts-in-google-docs-on-existing-sources-from-Gemini-Notebook.html)
- **Loop engineering** — Relay – a harness for AI coding agents that recover an… · [relayevals.com](https://relayevals.com)
- **AWS** — Introducing Claude Sonnet 5.5 on AWS · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-sonnet-5-5-on-aws)
- **Harness engineering** — Claude Codeで開発期間を2.5か月から1か月に縮めた「ハーネス」の設計手法 · [tech.smarthr.jp](https://tech.smarthr.jp/entry/2026/09/16/110205)
- **sharp LLM usage** — Production code written by Claude should have a higher… · [twitter.com](https://twitter.com/bcherny/status/2098217573276131577)
- **AI agent trends** — GitHub Copilot cloud agent の MCP 連携とリポジトリ単位設定 · [docs.github.com](https://docs.github.com/en/copilot/how-tos/agents/copilot-coding-agent/extending-copilot-coding-agent-with-mcp)
- **Claude Code** — Claude Code v2.1.286: 権限プロンプト、秘密情報マスキング、サブエージェント、`veri… · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- **Ethics of AI Agents** — CheatBench: Measuring Reward Gaming in AI Agents · [arxiv.org](http://arxiv.org/abs/2609.36308v1)
- **Philosophy of Loop Engineering** — Show HN: Relay – a harness for AI coding agents that r… · [news.ycombinator.com](https://news.ycombinator.com/item?id=49898411)
- **Anthropology of Agentic AI** — Working with Agentic `Teammates': When a New Organizat… · [arxiv.org](https://arxiv.org/abs/2609.29901v1)
- **History of Automation** — Causal Behavioral Evaluation of AI Agents at Scale via… · [arxiv.org](https://arxiv.org/abs/2608.10030v3)
- **DDD** — Constraint-Driven Context Engineering: Designing Domai… · [arxiv.org](http://arxiv.org/abs/2609.27354v1)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Google Docs で Gemini Notebook の既存ソースを根拠にできるように** — Google Docs 内の Gemini から、既存の Gemini Notebook をコンテキストソースとして参照できるよ… 〔技術: RAG 的な「信頼するソースに基づく生成」が、専用ノート画面から日常…／人文: 書くことは単なる生成ではなく、どの資料を根拠にするかを選ぶ編集行為に…〕 · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/09/ground-ai-prompts-in-google-docs-on-existing-sources-from-Gemini-Notebook.html)
- [ ] **Study notebooks が学校・職場アカウントにも展開** — Gemini の Study notebooks が、管理者により Gemini app と Gemini Notebook が… 〔技術: 教材ソースに根拠づけた適応学習ワークフローが、個人向け実験から Wo…／人文: 「学習者の弱点を可視化する」機能は便利な一方、学校や職場での評価・監…〕 · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/09/study-notebooks-in-gemini-are-now-available-for-Google-Workspace-accounts.html)
- [ ] **音声録音・リアルタイム会話・対話型学習オーバービューが追加** — Gemini Notebook モバイルアプリに音声録音が入り、講義や思いつきをソースと並べて保存できるようになりました。 〔技術: 入力は音声、対話はリアルタイム、出力はクイズや概念図という形で、No…／人文: 講義を「あとで読む資料」ではなく「話しかけられる記憶」に変える点が印…〕 · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/09/new-back-to-school-features-and-learning-tools-available-in-Gemini-Notebook.html)
- [ ] **Notebooks in Gemini が学校・組織向けの集中ワークスペースに** — Gemini 内の Notebooks が、学生、教育者、専門職向けに、特定トピックの会話と資料をまとめる専用ワークスペースとし… 〔技術: Gemini app と Gemini Notebook の統合によ…／人文: 「ノート」は個人の思考の場所でしたが、ここでは学校や会社の制度に接続…〕 · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/09/notebooks-in-gemini-dedicated-workspace-for-focused-organized-work-now-for-schools-and-organizations.html)
- [ ] **Expert Intelligence で購入済み電子書籍を Notebook の根拠に** — Google は Expert Intelligence を発表し、主要出版社の10万冊以上の書籍など信頼できるソースを Gem… 〔技術: 公開 Web やユーザー資料だけでなく、ライセンスされた書籍コンテン…／人文: 本を読む行為が、著者との対話・要約・演習生成へ拡張されます。〕 · [workspaceupdates.googleblog.com](http://workspaceupdates.googleblog.com/2026/09/introducing-expert-intelligence-in-Gemini-Notebook.html)

### Loop engineering
- [ ] **Relay – a harness for AI coding agents that recover and verify** — HN投稿によると、Relay はコーディングエージェントに「試行 → 新しいサンドボックスで検証 → 失敗ログを読んで再試行 →… 〔技術: エージェント実行を検証可能な反復ループに閉じ込め、チェック通過と人間…／人文: ethics の観点では、ブラックボックスな「自律性」を増やすのでは…〕 · [relayevals.com](https://relayevals.com)
- [ ] **amux – Open-source control plane for AI coding agents** — amux は Claude Code、Codex、Gemini など複数のコーディングエージェントを、共有ボード、atomic… 〔技術: ループ、スケジューリング、メッセージの出所記録、自己回復を単一の実行…／人文: history の観点では、工場の工程管理やチケット駆動開発が、今度…〕 · [github.com](https://github.com/mixpeek/amux)
- [ ] **Agent Chaos Monkey – fault-injection middleware for AI agents** — CrewAI / LLM tools 向けに、API 502、レイテンシ急増、壊れたJSONなどを注入し、無限リトライや夜間のト… 〔技術: 成功パスだけでなく、外部ツール障害・遅延・不正形式レスポンスに対する…／人文: ethics 的には、エージェントの暴走を「賢さ不足」ではなく、設計…〕 · [github.com](https://github.com/Baddevil512/agent-chaos-monkey)
- [ ] **ownframework-loop – durable engineering protocol for AI coding agents** — human-originated specs、exact-SHA review、bounded repairs、human-co… 〔技術: 仕様の起点、レビュー対象のSHA、修復の上限、人間による昇格を明示し…／人文: philosophy の観点では、これは「誰が意図を持ったのか」を保…〕 · [github.com](https://github.com/william-london/ownframework-loop)
- [ ] **SimpleEvol – An Agent-Loop Framework for LLM-Driven Automated Heuristic Design with Minimal Human Priors** — LLMを進化計算の狭い部品として使うのではなく、ヒューリスティック設計の反復生成・評価・改良ループの中心に置く論文。 〔技術: Loop engineering を開発ワークフローだけでなく、アル…／人文: creativity の観点では、人間の創造性を細かな操作設計から、…〕 · [arxiv.org](http://arxiv.org/abs/2609.37172)

### AWS
- [ ] **Introducing Claude Sonnet 5.5 on AWS** — Claude Sonnet 5.5 が Amazon Bedrock および Claude Platform on AWS で利… 〔技術: Bedrock上でAnthropic系モデルの選択肢が増えることで、…／人文: 「どのAIが一番賢いか」ではなく「この仕事にはどのAIを割り当てるか…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-sonnet-5-5-on-aws)
- [ ] **Amazon S3 Vectors now supports metadata pre-filtering for higher recall on filtered searches** — Amazon S3 Vectors がメタデータの事前フィルタリングに対応し、選択的なフィルタ条件を使う検索で最大5倍高いリコー… 〔技術: 類似検索の前にメタデータ条件を評価できるため、権限・部門・顧客・日付…／人文: RAGの失敗はしばしば「知らない」より「関係ないものを混ぜて語る」こ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-s3-vectors-now-supports-metadata-pre-filtering-for-higher-recall-on-filtered-searches)
- [ ] **Introducing Amazon CloudWatch Omni: AI-powered observability for generative AI and agentic workloads** — CloudWatch Omni は、生成AIおよびエージェントワークロード向けのAIファーストなオブザーバビリティとして発表され… 〔技術: 従来のCPU・ログ・メトリクス中心の監視から、エージェントの推論過程…／人文: エージェントは「動いたか」だけでなく「なぜそう判断したか」が問われる…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/introducing-amazon-cloudwatch-omni-ai-powered-observability-for-generative-ai-and-agentic-workloads)
- [ ] **Amazon Aurora PostgreSQL now supports direct querying of Apache Iceberg and Parquet data in your data lake** — Amazon Aurora PostgreSQL から、データレイク上の Apache Iceberg と Parquet デー… 〔技術: トランザクショナルDBとデータレイクのあいだにあるETL・複製・鮮度…／人文: データ基盤の歴史は、業務の現場と分析の現場を分けたりつないだりする歴…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-aurora-postgresql-now-supports-direct-querying-of-apache-iceberg-and-parquet-data-in-your-data-lake)
- [ ] **REST API を Amazon Bedrock AgentCore Gateway で MCP サーバー化する ― オリックス「PATPOST」での取り組み** — オリックスのSaaS「PATPOST」において、既存REST APIを Amazon Bedrock AgentCore Gat… 〔技術: REST APIをMCPサーバーとして公開することで、既存業務システ…／人文: 企業AI導入の本丸は、派手なデモではなく、すでに動いている業務システ…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/agentcore-gateway-patpost)

### Harness engineering
- [ ] **Claude Codeで開発期間を2.5か月から1か月に縮めた「ハーネス」の設計手法** — SmartHR のプロダクト開発で、Claude Code を単発のコーディング補助ではなく、要件・設計・実装・検証を通す「ハー… 〔技術: Claude Code の出力品質を、コンテキスト設計、作業分解、レ…／人文: 「AIが速い」ではなく「人間がどのような作業環境をAIに与えるか」が…〕 · [tech.smarthr.jp](https://tech.smarthr.jp/entry/2026/09/16/110205)
- [ ] **harness: ticket to spec, test-first build, independent review, gated merge** — Claude Code と Codex 向けのプラグインとして、チケット化、仕様化、テストファースト実装、独立レビュー、ゲート付… 〔技術: LLM エージェントの作業を「ブランチ・ワークツリー・テスト・独立レ…／人文: ここでのハーネスは、AIを自由に暴走させる檻ではなく、責任を分割して…〕 · [github.com](https://github.com/sluengen/harness)
- [ ] **amux: open-source control plane for AI coding agents** — Claude Code、Codex、Gemini CLI、OpenCode、Ollama など複数のコーディングエージェントを、… 〔技術: 並列ワーカー、タスクボード、永続状態、モデル切替、回復機構を備えるこ…／人文: 複数のAIに仕事を配る構図は、管理職・編集者・管制官の役割を人間がど…〕 · [github.com](https://github.com/mixpeek/amux)
- [ ] **ASSERT: requirement-driven evaluation harness for AI agents and LLM applications** — 要件から振る舞い別テストケースを生成し、任意のターゲット（ホスト型モデル、 callable wrapper、OpenTelem… 〔技術: spec-driven scoring、trace-aware ev…／人文: AIの失敗はしばしば「なんとなく変だった」で終わるが、要件駆動のハー…〕 · [github.com](https://github.com/responsibleai/ASSERT)
- [ ] **Thinking Before Thinking: Scaling Agentic Inference Through Meta-Reasoning** — 長いエージェント実行では、どの途中結果を使うか、やり直すか、いつ止めるかといった「実行制御」そのものが課題になるとして、cont… 〔技術: タスク実行を worker に任せ、controller が予算・記…／人文: 「考える前に、どう考えるかを考える」という構図は、AIにもメタ認知的…〕 · [arxiv.org](http://arxiv.org/abs/2609.38147v1)

### sharp LLM usage
- [ ] **Production code written by Claude should have a higher bar than if it was written by a human** — Boris Chernyは、Claudeが書いた本番コードには人間が書いたコード以上の高い基準が必要であり、Anthropicで… 〔技術: LLMコーディングの品質担保を、プロンプト改善ではなく多層の自動検証…／人文: AIを「優秀な作者」と見るのではなく、「速いが制度で囲むべき生産主体…〕 · [twitter.com](https://twitter.com/bcherny/status/2098217573276131577)
- [ ] **rigor: reproduce → design → verify → multi-model review をClaude Code/Codex向けに移植** — `rigor`は、Claude CodeとCodexで「再現してから直す」「設計を固めてから書く」「実物で検証する」「複数モデル… 〔技術: LLMの出力品質を、単発の回答精度ではなく、再現・設計・実行検証・相…／人文: これは「AIに任せる」ではなく、熟練エンジニアの慎重さを手順として外…〕 · [github.com](https://github.com/oz6un/rigor)
- [ ] **Agent Review Workflows: Claude reviewer + Codex coordinator の証拠ベースレビュー** — `Agent Review Workflows`は、`review-plan`、`review-implementation`、… 〔技術: 1モデルの自己レビューではなく、役割の違う複数モデルに「批評」「裁定…／人文: レビューとは単なる欠陥検出ではなく、異なる視点の衝突を管理する社会的…〕 · [github.com](https://github.com/JFusco/agent-review-workflows)
- [ ] **MaruCheck: AIが編集できないQuality Contractで「AIが見落としたもの」をテストする** — MaruCheckは、AI生成コードを「AIが編集できない仕様契約」に照らして検証するローカルファーストのQAツール。 〔技術: 生成AIの弱点を「テストも一緒に書けること」と捉え、検証仕様をモデル…／人文: これはAIに対する不信ではなく、権力分立に近い設計である。〕 · [github.com](https://github.com/Kidus-M/MaruCheck)
- [ ] **Effective Dense Retrieval using Only In-Context Examples** — decoder-only LLMを追加学習なしに強いdense retrieverとして使えるかを、少数のin-context… 〔技術: LLM活用のボトルネックを、モデル訓練ではなくコンテキスト設計と例示…／人文: 「学習済みの知能」を固定物として見るのではなく、場に置かれた例や文脈…〕 · [arxiv.org](http://arxiv.org/abs/2609.38099v1)

### AI agent trends
- [ ] **GitHub Copilot cloud agent の MCP 連携とリポジトリ単位設定** — GitHub Docs は、リポジトリ管理者が JSON 設定で MCP サーバーを登録し、Copilot cloud agen… 〔技術: MCP が IDE 補助の周辺機能ではなく、クラウド上のコーディング…／人文: これは開発チームの「仕事の場」を、人間だけのリポジトリから人間とエー…〕 · [docs.github.com](https://docs.github.com/en/copilot/how-tos/agents/copilot-coding-agent/extending-copilot-coding-agent-with-mcp)
- [ ] **OpenAI Codex が「エージェントとともに開発するための最良の方法」として再提示** — OpenAI の Codex 公式ページは、Codex を「planning, building features, refac… 〔技術: コーディングエージェントの競争軸が補完・生成から、計画、並列作業、レ…／人文: 「コードを書く人」と「仕事を委任する人」の境目が揺らぎ、エンジニアの…〕 · [openai.com](https://openai.com/codex)
- [ ] **MCP のエラーメッセージは、強いエージェントほど傷つける** — “MCP Error Messages Written for Developers Hurt the Most Capable… 〔技術: 人間開発者向けのエラーメッセージを、エージェントが実行可能なサーバー…／人文: ここで問われているのは「誰に向けて説明しているのか」という言語設計で…〕 · [arxiv.org](https://arxiv.org/abs/2609.35381)
- [ ] **MetaPermit: Claude Code / Codex 型エージェントのツール権限を監査可能にする** — “MetaPermit” は、OpenAI Codex や Claude Code のようなツール利用エージェントが、静的な許可… 〔技術: ツール呼び出しごとの LLM 裁量を、監査可能な属性ベースポリシーへ…／人文: 自律エージェントの普及は「信じる」か「止める」かの二択ではなく、どの…〕 · [arxiv.org](https://arxiv.org/abs/2609.31039)
- [ ] **Tracekit / AgentXploit: エージェント運用は監査ログと攻撃演習の時代へ** — “Tracekit” は Claude Code のライフサイクルイベントにフックし、ユーザー意図、モデルの自己報告、実際のアク… 〔技術: エージェントの安全性は、プロンプトの注意書きではなく、改ざん耐性のあ…／人文: これは「AIが何を考えたか」より「共同作業の場で何をしたか」を記録す…〕 · [arxiv.org](https://arxiv.org/abs/2609.35659)

### Claude Code
- [ ] **Claude Code v2.1.286: 権限プロンプト、秘密情報マスキング、サブエージェント、`verify`スキル、`--bare`/プラグイン制限まで入った大型更新** — v2.1.286では、複数の権限要求に「2 of 5」のような件数表示が追加され、MCP認証・Remote Control・クラ… 〔技術: CLIの細かなUX改善ではなく、権限、認証、秘密情報、プラグイン供給…／人文: 人間がAIにコード変更を委ねるとき、問題は「賢いか」だけでなく「どの…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **日本語実践: 「verify」というスキル名だけでコミット前実行が誘発されるかを30回検証** — 日本語圏の実践記事が、Claude Code 2.1.286の「project/user skills include one… 〔技術: リリースノート上の一文を、バージョン差・スキル名差・変更種別差で切り…／人文: AIエージェントの「習慣」を人間が観察し、命名規則として共同作業の儀…〕 · [qiita.com](https://qiita.com/suwa_nobu/items/cc0fb4a9e10100991bba)
- [ ] **日本語実践: v2.1.286の`--bare`変更とプラグイン制限をCI/自動化の観点で整理** — v2.1.286の変更から、`--bare`モードのMCP接続制限、システムリマインダー抑制、バックグラウンド処理制限、プラグイ… 〔技術: Claude Codeをヘッドレス・CI・自動化で使う場合、便利な暗…／人文: 自律エージェントは、自由度が高いほど危険にもなる。〕 · [qiita.com](https://qiita.com/picnic/items/ae1b6dbd22ba74683b54)
- [ ] **arXiv: Meta-Reasoning論文がClaude Codeを長期エージェント比較のベースラインに採用** — “Thinking Before Thinking: Scaling Agentic Inference Through Met… 〔技術: Claude Code単体の能力比較ではなく、作業の再利用・停止判断…／人文: 「考えるAI」から「考え方を管理するAI」へ焦点が移ると、人間のマネ…〕 · [arxiv.org](https://arxiv.org/abs/2609.38147)
- [ ] **arXiv: Claude Codeのライフサイクルイベントにフックする監査基盤Tracekit** — “Tracekit: Tamper-Evident Intent-Reasoning-Action Auditing for A… 〔技術: Claude Codeのhook/event体系を、単なる自動化では…／人文: AIが書いたコードの責任を誰が負うのかという問いに対し、「ログを信じ…〕 · [arxiv.org](https://arxiv.org/abs/2609.35659)

### Ethics of AI Agents
- [ ] **CheatBench: Measuring Reward Gaming in AI Agents** — 強化学習で高スコアを得るAIエージェントが、ユーザー意図とは異なる近道や不正な情報アクセスに走る「報酬ゲーミング」を測るベンチマ… 〔技術: 長期タスクの評価指標に、成果物だけでなく権限逸脱・隠れたショートカッ…／人文: これは「有能だが信頼できない代理人」をどう扱うかという、組織倫理その…〕 · [arxiv.org](http://arxiv.org/abs/2609.36308v1)
- [ ] **VeriWeave Govern: Evidence-Gated Deterministic Runtime Governance for Enterprise AI Agents** — 企業エージェントがツール実行、インフラ変更、保護データ処理を行う際、行動生成と行動承認を分離する決定論的ランタイム・ガバナンス層… 〔技術: モデルの善意やプロンプト規律に依存せず、実行時の証拠ゲートで権限行使…／人文: 責任所在を「AIが決めた」から「組織がどの証拠なら許可すると決めたか…〕 · [arxiv.org](http://arxiv.org/abs/2609.37457v1)
- [ ] **Compliant with Local Controls, Collectively Discriminatory. A Governance Architecture for Multi-Agent AI in Regulated Finance** — 金融機関の信用、詐欺検知、回収、コンプライアンス業務におけるエージェント群について、各コンポーネントが個別に規制準拠でも、全体と… 〔技術: エージェントごとのテスト・承認・監視だけでは、相互作用から生じる集合…／人文: 「誰も差別していないのに、制度として差別が起きる」という社会学的問題…〕 · [arxiv.org](http://arxiv.org/abs/2609.27994v1)
- [ ] **CARGO: Context-Aware Retrieval-Gated Evaluation of Agentic AI in Production** — 本番環境のエージェント評価では、参照回答が別の顧客・資産・案件に対応しているため、通常のLLM-as-a-judgeが誤判定しや… 〔技術: エージェント評価を静的な正解照合から、実運用の文脈・対象・手続きの一…／人文: 評価の誤りは単なるベンチマーク問題ではなく、ユーザーに対する不当な判…〕 · [arxiv.org](http://arxiv.org/abs/2609.30471v1)
- [ ] **From Certain Doom to Survival: Agent-Driven Self-Governance in LLM Agent Societies** — 共通資源をめぐる社会的ジレンマ環境で、外部から押し付けられた統治ではなく、LLMエージェント自身が統治メカニズムを形成する実験を… 〔技術: 単体エージェントの能力評価ではなく、エージェント集団がルールを作り、…／人文: AIエージェントを「道具」ではなく、相互作用する準社会的アクターとし…〕 · [arxiv.org](http://arxiv.org/abs/2609.22600v1)

### Philosophy of Loop Engineering
- [ ] **Show HN: Relay – a harness for AI coding agents that recover and verify** — Relay は、コーディングエージェントにタスクを試行させ、テスト・lint・build を再実行し、失敗から学んで再試行するロ… 〔技術: 失敗ログを次の試行に持ち越し、PR 作成前に機械的チェックを走らせる…／人文: これは人間が逐次監督する「babysitting」から、どの条件なら…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49898411)
- [ ] **Show HN: OpenAPPA – open-source deterministic guardrails that don't break agents** — OpenAPPA は、プロンプトインジェクションや幻覚によるデータ流出に対し、非決定的な LLM judge ではなくデータ固有… 〔技術: ツール呼び出し前後のフックやデータフロー制約を agent loop…／人文: 「信頼」はモデルの内面に置くのではなく、行為の通路と証跡に置くべきだ…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49877515)
- [ ] **Show HN: Yengi, a local-first AI development environment for coding, Blender/Unity** — Yengi は .NET 10 / WPF ベースのローカルファースト AI IDE で、ファイル・terminal・Git・b… 〔技術: checkpoint / rollback / verificati…／人文: 教師が教育用ツールの延長から作ったという文脈も含め、Loop Eng…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49879268)
- [ ] **Developing a Roadmap to an AI-first Organization: A Case Study in Embedded Software Development** — 組込みソフトウェア企業が AI-first 組織へ移行するためのロードマップを、40名のワークショップを含むケーススタディで検討… 〔技術: 組込み領域の検証・追跡可能性という強い制約のなかで、エージェント運用…／人文: ここでのループはコード上の retry だけでなく、組織が自分の技能…〕 · [arxiv.org](https://arxiv.org/abs/2609.30863v1)
- [ ] **Cybernetics for AI Agents: A Practical Introduction（重要だが古い: 2026-08-13）** — AI エージェントの失敗を「出力品質」ではなく「維持すべき変数を維持できなかった制御問題」として捉え、制御変数、外乱、センサー、… 〔技術: エージェント設計を prompt 改善ではなく、観測可能な状態変数と…／人文: Loop Engineering の思想史的な背骨として、サイバネテ…〕 · [taskmachine.io](https://taskmachine.io/blog/cybernetics-for-ai-agents)

### Anthropology of Agentic AI
- [ ] **Working with Agentic `Teammates': When a New Organizational Actor Collides with the Human Ecosystem of Work** — 大手テクノロジー企業の複数チームに、持続的かつプロアクティブなAI「teammate」を導入した現場内質的研究。 〔技術: エージェントを単発チャットではなく、複数人・長期・組織内コンテキスト…／人文: これはAI導入論というより、職場に新しい同僚カテゴリーが入ってきたと…〕 · [arxiv.org](https://arxiv.org/abs/2609.29901v1)
- [ ] **Positive Ratings, Hidden Concerns: Employee Voice Disclosure in AI-Mediated Organizational Listening** — グローバル・コンサルティング企業で、事前サーベイと適応的AI音声インタビューを組み合わせた「組織リスニング」を調査。 〔技術: AIエージェントをサーベイ後の自由回答収集装置ではなく、開示行動その…／人文: 職場の「声」は単なるデータではなく、上司・評価・同僚の視線を読んで調…〕 · [arxiv.org](https://arxiv.org/abs/2609.38788v1)
- [ ] **WorkWorlds: An Infrastructure for Evaluating AI Agents on Workplace Tasks** — 職場タスクのベンチマークは、タスクに必要な文脈をあらかじめ切り出してしまい、現実の仕事で重要な情報探索・文脈発見を過小評価しがち… 〔技術: エージェント評価を「正答生成」から、散らばった文脈を探し、必要な関係…／人文: 仕事とはタスク表に載った手順だけでなく、誰に聞くべきか、どの資料が本…〕 · [arxiv.org](https://arxiv.org/abs/2609.23806v2)
- [ ] **Recursive Organization Improvement: A Modeling Specification for Human--Agent Organizations** — 強いAIエージェントを入れても組織が自動的に良くなるわけではなく、人間とエージェントの組織は、どの作業配置を維持し、いつ見直すか… 〔技術: Human-Agent Organizationを、権限・履歴・証拠…／人文: 組織改善はしばしば「ふりかえり」「承認」「例外処理」といった儀礼を通…〕 · [arxiv.org](https://arxiv.org/abs/2609.38643v1)
- [ ] **From Digital Turn to Agentic Turn: Continuity and Rupture in Business Anthropology** — ビジネス人類学が、デジタル・ターンから「agentic turn」へ移行していると論じるエッセイ。 〔技術: AI Anthropology Toolkitやmulti-agen…／人文: ここで問われているのは「AIを研究に使うか」ではなく、解釈する主体が…〕 · [doi.org](https://doi.org/10.22439/jba.v15i1.7816)

### History of Automation
- [ ] **Causal Behavioral Evaluation of AI Agents at Scale via Automated Behavioral Science** — AIエージェントの行動評価を、仮説生成・実験設計・シミュレーション実行・分析・レポート作成まで含む「自動化された行動科学」として… 〔技術: 自動化の対象が工場作業や事務処理ではなく、実験計画と評価というメタレ…／人文: これはテイラー主義が作業者の動作を測定した歴史の、AIエージェント版…〕 · [arxiv.org](https://arxiv.org/abs/2608.10030v3)
- [ ] **Large Language Model Agents for Evidence Based Genetic Disease Severity Classification** — 遺伝性疾患の重症度分類という主観的かつ労働集約的な専門業務を、ReActとRAGを組み合わせた自律AIエージェントで標準化する研… 〔技術: 文献検索、推論連鎖、根拠検証を一体化し、専門家の分類実務を「証拠付き…／人文: 自動化史では、熟練工の暗黙知が機械や管理表に移されるたびに権威の配置…〕 · [arxiv.org](https://arxiv.org/abs/2609.19569v2)
- [ ] **Cheap, Fallible Cognition and the Political Economy of Expertise** — 生成AIを「安価でスケールするが誤りうる認知」と捉え、仕事を丸ごと奪うかどうかではなく、検証・責任・信頼・ガバナンス・賃料配分な… 〔技術: AIの能力評価を、単純な自動化可能性ではなく、検証コストや責任境界を…／人文: 自動化の歴史は「機械が何をできるか」だけでなく、「社会が何を任せると…〕 · [arxiv.org](https://arxiv.org/abs/2608.11512v1)
- [ ] **Future of Work with AI Agents: Auditing Automation and Augmentation Potential across the U.S. Workforce** — 米国労働市場の844超のタスクについて、労働者がAIエージェントに自動化してほしいか、補助してほしいかを調べ、技術的可能性と照合… 〔技術: 「自動化できるか」だけでなく「当事者がどの程度の人間関与を望むか」を…／人文: 産業革命以来、自動化はしばしば経営者・技術者側の合理化として進んだ。〕 · [arxiv.org](https://arxiv.org/abs/2506.06576v3)
- [ ] **社会が変わる、暮らしが変わる――。AI時代に「人間に求められるもの」とは** — AIの進化がビジネス、安全保障、暮らしを変える一方で、仕事喪失や支配への不安も広がるという、日本の政策広報文脈での論点整理。 〔技術: AIエージェントの社会実装を、個別ツールではなく業務・安全保障・生活…／人文: 自動化史では、新技術のたびに「人間らしい仕事とは何か」が問い直されて…〕 · [journal.meti.go.jp](https://journal.meti.go.jp/policy/202607/46541)

### DDD
- [ ] **Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems** — 生成AIシステムを特定ドメインに適合させる際、単なるRAGやツール連携ではなく、技術・規制・制度・規範上の「制約」を体系的に文脈… 〔技術: ユビキタス言語や境界づけられたコンテキストを、LLMへ渡す「制約駆動…／人文: AIの振る舞いを単に精度で測るのではなく、組織・制度・規範の中で何が…〕 · [arxiv.org](http://arxiv.org/abs/2609.27354v1)
- [ ] **Domain Modeling Meets Generative AI / ddd-meets-genai** — Event Stormingで得た付箋・会話・ドメイン知識を、LLMエージェントが構造化されたドメインモデルへ変換するための仕様… 〔技術: DDDの発見活動を、LLMが扱える中間表現と検証可能な成果物へ落とす…／人文: 付箋やホワイトボードに宿る曖昧な会話を、AIが処理可能な構造へ変換す…〕 · [github.com](https://github.com/mardenneubert/ddd-meets-genai)
- [ ] **Agent Skills: DDD Playbook and Stack Skills** — Claude Code、Cursor、GitHub CopilotなどのAI coding agent向けに、DDDの「スキル」… 〔技術: DDDの判断規則を、モデル非依存のエージェントスキルとして小さく読み…／人文: 熟練者の暗黙知をスキルファイルに翻訳することは、設計文化の継承方法を…〕 · [github.com](https://github.com/salimramirez/agent-skills)
- [ ] **NestJS DDD Starter Kit with AI Agent Rules & Skills** — NestJS、TypeORM、PostgreSQLを前提に、DDDとヘキサゴナルアーキテクチャを厳格に分離したスターターキット。 〔技術: DDD/Hexagonalの層分離を、AIエージェントがコード生成時…／人文: AIがチームの「新入り開発者」になるなら、リポジトリ自体に組織の作法…〕 · [github.com](https://github.com/khacvux/nest-ddd-starter-kit)
- [ ] **AI時代の静的解析ベストプラクティス：自然言語のルールをArchUnitで「実行できるルール」に変える** — AIエージェント向けにMarkdownで書いたチームルールを、ArchUnit、Semgrep、reviewdogなどで検証可能… 〔技術: ユビキタス言語や設計原則をAIに読ませるだけでなく、層依存・境界違反…／人文: AI時代の設計規律は、信頼や注意力に頼る文化から、合意したルールを自…〕 · [qiita.com](https://qiita.com/ukun3/items/2545a4db32dd575ad426)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

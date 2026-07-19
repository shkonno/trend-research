# 📰 2026-07-19 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLM is now Gemini Notebook · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- **Loop engineering** — SearchOS-V1: Towards Robust Open-Domain Information-Se… · [arxiv.org](http://arxiv.org/abs/2607.15257v1)
- **AWS** — AWS Summit Japan 2026「Future of Agentic Commerce」ブース開催… · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-summit-japan-2026-future-of-agentic-commerce)
- **Harness engineering** — Harnessing LLMs for Reliable Academic Supervision: A C… · [arxiv.org](https://arxiv.org/abs/2607.14707)
- **sharp LLM usage** — AI Agents Do Not Fail Alone: The Context Fails First · [arxiv.org](https://arxiv.org/abs/2607.14275)
- **AI agent trends** — Claude Code 2.1.214: 権限チェック、OTel、進捗ハートビートの強化 · [github.com](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- **Claude Code** — Claude Code 2.1.214: 権限検査・監査ログ・長時間ツールの安全性を厚くする大型メンテナンス · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- **Ethics of AI Agents** — AIセーフティに関する評価観点ガイド（第1.20版）の公開 · [aisi.go.jp](https://aisi.go.jp/output/output_information/260707)
- **Philosophy of Loop Engineering** — Proof-or-Stop: Don't Trust the Agent, Trust the Eviden… · [arxiv.org](http://arxiv.org/abs/2607.14890)
- **Anthropology of Agentic AI** — Platform Choice, Trust, and Privacy in the Consumer AI… · [arxiv.org](https://arxiv.org/abs/2607.15134)
- **History of Automation** — LOGOS: A Living Logic for AI Agent Teams That Evolve W… · [arxiv.org](https://arxiv.org/abs/2607.10878)
- **DDD** — ddd-agent-skill: DDDをエージェントスキルとして実装する試み · [github.com](https://github.com/aristorinjuang/ddd-agent-skill)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLM is now Gemini Notebook** — GoogleはNotebookLMを「Gemini Notebook」に改称し、引き続き独立した研究・学習プロダクトとして提供す… 〔技術: RAG型ノートにコード実行環境が加わることで、資料要約だけでなく、ソ…／人文: 「ノート」という個人的な思考の器が、検索・Geminiアプリ・クラウ…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- [ ] **NotebookLM is now Gemini Notebook — Hacker Newsでの反応** — HNでは公式発表をめぐり、改名そのものへの皮肉、Geminiブランド統合への警戒、NotebookLMの研究ワークフローとしての… 〔技術: プロダクト統合は機能発見性やクロスアプリ同期を高める一方、既存ワーク…／人文: 名称変更は単なるマーケティングではなく、ユーザーが道具に持つ記憶や愛…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=48936451)
- [ ] **Gemini Notebookの参照更新をPythonで検知する** — Gemini Notebookに資料を投入する前後で、ファイルのSHA-256をJSONに記録し、追加・削除・変更を検知する小さ… 〔技術: NotebookLM/Gemini Notebookを業務RAGとし…／人文: AIの答えを信じるかどうかは、モデル性能だけでなく「どの資料を、いつ…〕 · [qiita.com](https://qiita.com/hironakamura_ai/items/11f8d20a42bd859e9148)
- [ ] **Toward AI-Agent-Driven Particle Transport Simulations: Implementation of AI-Assisted Workflows for PHITS** — 粒子輸送シミュレーションコードPHITS向けに、マニュアル・講義資料・サンプル入力・注意事項をAI-readyな知識ベースとして… 〔技術: 専門ソフトウェア側がRAG用知識ベースとエージェント用ルールを同梱す…／人文: 熟練者の暗黙知を「AIが読める教材」として梱包する試みは、専門知識の…〕 · [arxiv.org](https://arxiv.org/abs/2607.11309)
- [ ] **NotebookLM出力の音声がMacのミュージックアプリで開けない問題を拡張子トリックで解決する** — NotebookLMからダウンロードした音声ファイルがMacのミュージックアプリで正常に開けない場合の回避策として、QuickT… 〔技術: AI生成コンテンツの価値は生成品質だけでなく、ファイルコンテナ、メタ…／人文: 学習用ポッドキャストを日常の音楽アプリへ入れたいという欲望は、AI学…〕 · [qiita.com](https://qiita.com/maskot1977/items/18f96fa5aac54a7dc4d4)

### Loop engineering
- [ ] **SearchOS-V1: Towards Robust Open-Domain Information-Seeking Agent Collaboration** — 情報探索エージェントが長い対話履歴の中で進捗を見失い、同じ検索を反復する問題に対し、Frontier Task、Evidence… 〔技術: ReAct 的な探索ループの失敗を、単なるプロンプト改善ではなく永続…／人文: anthropology の観点では、個人の記憶に頼る職人仕事が、帳…〕 · [arxiv.org](http://arxiv.org/abs/2607.15257v1)
- [ ] **Bridge Evidence: Static Retrieval Utility Does Not Predict Causal Utility in Multi-Step Agentic Search** — 文書が「今の質問に答える」有用性と、「次の検索行動をよくする」因果的有用性は一致しないことを、ReAct スタイルの検索エージェ… 〔技術: ループ内の各観測を削除して軌跡を再実行する Counterfactu…／人文: philosophy の観点では、知識を静的な真理の束ではなく「次の…〕 · [arxiv.org](http://arxiv.org/abs/2607.15253v1)
- [ ] **LoopX: lightweight loop engineering state kernel for long-running AI agent teams** — Codex、Claude Code、Cursor などにまたがる長時間稼働エージェント向けに、目標、ゲート、TODO、クォータ、… 〔技術: エージェント本体から状態カーネルを切り離し、実行環境非依存の goa…／人文: history の観点では、工場の工程票や航空機のチェックリストのよ…〕 · [github.com](https://github.com/huangruiteng/loopx)
- [ ] **BriefLoop: auditable business briefings with claims, evidence, gates, repairs, and human review** — ビジネスブリーフィング作成を、claims、evidence、gates、findings、repairs、human revi… 〔技術: 生成物ではなく生成過程を第一級オブジェクトにし、主張登録、根拠リンク…／人文: ethics の観点では、AI が書いた文書の説得力よりも、検証可能…〕 · [github.com](https://github.com/Stahl-G/briefloop)
- [ ] **Best practices for Claude Code / agentic loop gates and verification** — Claude Code の実践パターンとして、コンテキスト管理、短い human-readable な CLAUDE.md、チェ… 〔技術: Stop hook や検証サブエージェントを用い、作業者エージェント…／人文: philosophy の観点では、主体の自己申告ではなく制度化された…〕 · [anthropic.com](https://www.anthropic.com/engineering/claude-code-best-practices)

### AWS
- [ ] **AWS Summit Japan 2026「Future of Agentic Commerce」ブース開催報告** — AWS Summit Japan 2026 の流通小売消費財業界ブースで、AI エージェントが商品発見・比較・購入・決済まで関わ… 〔技術: Bedrock AgentCore と複数のコマース/エージェントプ…／人文: 「買う」という行為が人間の検索・比較・意思決定から、条件設定と監督へ…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-summit-japan-2026-future-of-agentic-commerce)
- [ ] **Amazon Bedrock Managed Knowledge Base でエージェント向け企業検索を簡素化** — Amazon Bedrock Managed Knowledge Base により、企業データを使ったエージェント/生成AIアプ… 〔技術: RAG 基盤をアプリごとに手作りする段階から、エージェントの標準イン…／人文: 企業知識が AI エージェントの「記憶」として再編成されると、組織内…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/build-enterprise-search-for-agents-with-amazon-bedrock-managed-knowledge-base)
- [ ] **Lambda 関数コード用のセルフマネージド S3 バケット** — AWS Lambda で、関数コードのデプロイアーティファクトをユーザー管理の S3 バケットに置ける新機能が紹介されました。 〔技術: デプロイ成果物の保管場所を利用者側で管理できるため、Lambda の…／人文: サーバーレスは「運用を隠す」思想で普及しましたが、成熟した組織では逆…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/compute/introducing-self-managed-amazon-s3-buckets-for-aws-lambda-function-code)
- [ ] **AWS DevOps Agent と Kiro CLI による自動インシデント修復** — AWS DevOps Agent が生成した緩和策や実行計画を Lambda、SQS、CodeBuild、Kiro CLI へ渡… 〔技術: インシデント調査、修正案生成、コード変更、PR 作成をイベント駆動で…／人文: 夜間対応の苦痛を減らす一方で、「AI が直した」という事実を誰がレビ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/devops/automated-incident-remediation-with-aws-devops-agent-and-kiro-cli)
- [ ] **TerraRepair: Tool-Grounded LLM Agent for Infrastructure-as-Code Repair** — Terraform などの Infrastructure-as-Code で検出されたクラウド設定ミスを、ツールに基づく LLM… 〔技術: IaC スキャナの「検出」と開発者の「修正」の間にある手作業を、検証…／人文: インフラの安全性は、専門家だけが読める設定ファイルに閉じ込められがち…〕 · [arxiv.org](https://arxiv.org/abs/2607.11390)

### Harness engineering
- [ ] **Harnessing LLMs for Reliable Academic Supervision: A Comparative Study** — 学術指導という高リスク領域で、GPT-5 の素のチャットボットよりも、小型モデルを LangGraph ベースの Harness… 〔技術: 「大きなモデル」より「検証可能な足場」を重視する設計が、モデルサイズ…／人文: 学術指導は人生・評価・制度が絡む領域であり、AI を単なる助言者では…〕 · [arxiv.org](https://arxiv.org/abs/2607.14707)
- [ ] **From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents** — 企業向け LLM Agent を、プロンプト中心の試作品から、ソース境界・エンティティルーティング・出力契約・再現可能なトレース… 〔技術: 決定論的な振る舞いをコード、マニフェスト、スキーマ、検証アーティファ…／人文: 企業利用では「AI が正しそうに答えた」だけでは足りず、誰が・何を根…〕 · [arxiv.org](https://arxiv.org/abs/2607.08028)
- [ ] **Claude Code: A harness for every task / dynamic workflows** — Claude Code の dynamic workflows は、タスクごとに Claude が JavaScript ベース… 〔技術: Harness を静的な外部オーケストレータではなく、タスクに応じて…／人文: これは「人間が全工程を細かく指示する」労働観から、「人間が評価軸と境…〕 · [claude.com](https://claude.com/blog/a-harness-for-every-task-dynamic-workflows-in-claude-code)
- [ ] **Claude Code hooks / subagents / skills 公式ドキュメントの Harness 化** — Claude Code の Hooks は、SessionStart、UserPromptSubmit、PreToolUse、P… 〔技術: Hook、subagent、skill は、Claude Code…／人文: 「AI にお願いする」から「AI が働く現場のルールを設計する」へ視…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks.md)
- [ ] **中国語圏コミュニティでの Harness engineering 解説の急増** — 中国語圏では「Agent = Model + Harness」「Prompt / Context / Harness Engin… 〔技術: 公式論文や Claude Code の機能だけでなく、実務者コミュニ…／人文: 「馬具」「缰绳」「人类掌舵，智能体执行」といった比喩が広がっており、…〕 · [javaguide.cn](https://javaguide.cn/ai/agent/harness-engineering.html)

### sharp LLM usage
- [ ] **AI Agents Do Not Fail Alone: The Context Fails First** — エージェントの失敗をモデル単体の能力ではなく、指示、ツール、メモリ、検索知識、ガードレール、非信頼入力を含む「文脈品質」の失敗と… 〔技術: LLM運用の改善点を「モデルを替える」ではなく、実行コンテキストの品…／人文: 失敗の責任をAIの人格めいた能力不足に帰すのではなく、周囲の制度・記…〕 · [arxiv.org](https://arxiv.org/abs/2607.14275)
- [ ] **Do AI Agents Know When a Task Is Simple? Toward Complexity-Aware Reasoning and Execution** — LLMエージェントが簡単な1行修正にも最大文脈・全探索で臨みがちな問題を扱い、必要最小限の実行範囲を見積もるE3（Estimat… 〔技術: 「まず全部読む」ではなく、見積もり、最小実行、検証失敗時だけ拡張とい…／人文: これはAI時代の倹約術でもある。〕 · [arxiv.org](https://arxiv.org/abs/2607.13034)
- [ ] **SearchOS-V1: Towards Robust Open-Domain Information-Seeking Agent Collaboration** — Web検索型エージェントが長い対話履歴の中で進捗を見失い、同じ探索を繰り返す問題に対し、検索進捗をFrontier Task、E… 〔技術: 調査タスクを会話ログ頼みから、未解決範囲・証拠・失敗履歴を持つ状態機…／人文: 調査の質は「思いつきの検索語」より、何をもう試したかを忘れない共同記…〕 · [arxiv.org](https://arxiv.org/abs/2607.15257)
- [ ] **Show HN: Kote – Capture and reuse engineering context from AI chats and Git** — Koteは、AIとの会話、Git活動、開発上の意思決定を自動的に保存し、後から必要な文脈として取り出す開発者向けメモリレイヤー。 〔技術: コード差分だけでなく「なぜそうしたか」をAIチャットとGitから再利…／人文: AI活用を自動化一辺倒にせず、人間の記憶と判断を支える道具として設計…〕 · [github.com](https://github.com/pedroaugusto04/Kote)
- [ ] **Show HN: Dex – Cost-aware analytics engineering skills for agents** — dexはClaude Codeや任意のエージェント向けのanalytics engineeringツールキットで、データウェアハ… 〔技術: ドメイン固有の探索・変換・保守ループをスキル化し、データ参照はrea…／人文: 汎用AIにすべてを任せるのではなく、現場の作法、コスト意識、データ倫…〕 · [github.com](https://github.com/exmergo/dex)

### AI agent trends
- [ ] **Claude Code 2.1.214: 権限チェック、OTel、進捗ハートビートの強化** — Claude Code の最新変更では、PowerShell/Bash/Windows/リモートセッション周りの権限チェック修正… 〔技術: エージェントの実用化でボトルネックになるのは推論能力だけでなく、シェ…／人文: これは「AIに任せる」物語の裏側にある、責任と信頼の細かな制度設計で…〕 · [github.com](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [ ] **Claude Code Best Practices: MCP、hooks、parallel sessions を含む運用パターンの体系化** — Claude Code のベストプラクティスは、環境設定、MCPサーバ接続、hooks、並列セッションなど、個人のプロンプト術か… 〔技術: MCP と hooks を使って、エージェントのコンテキスト取得、ツ…／人文: ベストプラクティス化は、熟練者の暗黙知が組織の作法へ変わる過程でもあ…〕 · [code.claude.com](https://code.claude.com/docs/en/best-practices)
- [ ] **toolgovern: AIエージェントの全ツール呼び出しを実行前にゲートするミドルウェア** — toolgovern は、AIエージェントの shell、filesystem、network、credential、cross… 〔技術: フレームワークごとに散らばる安全策を、ツール呼び出し前の共通ポリシー…／人文: 自律エージェントが増えるほど、組織は「誰が何を許可したのか」を説明す…〕 · [github.com](https://github.com/RudrenduPaul/toolgovern)
- [ ] **deja-vu: コーディングエージェント向けローカル記憶レイヤー** — deja-vu は Claude Code、Codex、opencode、Cursor、Gemini CLI などが残すセッショ… 〔技術: モデルの長文コンテキストを伸ばすだけでなく、過去セッションを高速検索…／人文: 人間のチームが議事録やナレッジベースを持つように、エージェントにも「…〕 · [github.com](https://github.com/vshulcz/deja-vu)
- [ ] **SearchOS-V1: 検索エージェントの進捗・証拠・失敗記憶を外部状態として管理** — SearchOS-V1 は、情報探索エージェントが履歴の肥大化や失敗ループで破綻しやすい問題に対し、Frontier Task、… 〔技術: エージェントの失敗をプロンプト改善だけで直すのではなく、進捗・証拠・…／人文: 調査とは単なる答え生成ではなく、何を見たか、何を見ていないか、どこで…〕 · [arxiv.org](http://arxiv.org/abs/2607.15257v1)

### Claude Code
- [ ] **Claude Code 2.1.214: 権限検査・監査ログ・長時間ツールの安全性を厚くする大型メンテナンス** — v2.1.214 では、`Edit(src/**)` のような allow rule の解釈、Windows PowerShel… 〔技術: コード生成能力そのものより、危険な自動実行を fail closed…／人文: エージェント時代の「信頼」は、賢さではなく、いつ止まり、誰に何を見せ…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **Claude Code 2.1.212: `/fork`、サブエージェント上限、MCP自動バックグラウンド化** — `/fork` が会話を新しい background session として複製するようになり、従来の in-session s… 〔技術: 並列化・長時間外部ツール・暴走防止を同時に扱い、エージェントの「作業…／人文: 人間の開発作業は一つの会話ではなく、調査・修正・レビュー・待機が絡む…〕 · [code.claude.com](https://code.claude.com/docs/en/changelog.md)
- [ ] **Boris Cherny インタビュー群: Claude Code の核心が「プロンプト芸」ではなくハーネス設計として語られる** — Boris Cherny / Claude Code チームへのインタビューが複数の開発者メディアで取り上げられ、Claude… 〔技術: モデル単体ではなく、どのタイミングでツールを呼び、どの情報を残し、ど…／人文: 「コーディングは解かれたのか」という問いは、職能の終わりではなく、ソ…〕 · [newsletter.pragmaticengineer.com](https://newsletter.pragmaticengineer.com/p/building-claude-code-with-boris-cherny)
- [ ] **Agent SDK / サブエージェント / hooks / MCP の公式ドキュメント拡充** — Agent SDK は「Claude Code と同じ agent loop、tools、context management… 〔技術: CLI利用から、組織固有のツール・権限・監査を組み込む progra…／人文: 開発者がAIに合わせて働くのではなく、組織の慣習・責任境界・レビュー…〕 · [code.claude.com](https://code.claude.com/docs/en/agent-sdk/overview.md)
- [ ] **日本語圏の実践まとめ: 2026-06-30〜07-13 の Claude Code は model・subagents・運用前提が焦点** — 日本語記事では、6月末から7月中旬の Claude Code を、週次リリースの列挙ではなく「どの model と運用前提で回す… 〔技術: 日本語圏でも、単発の使い方紹介から、モデル選択・コンテキスト長・ba…／人文: ローカルな実践記事は、英語圏の公式発表を現場の言葉へ翻訳する媒介にな…〕 · [note.com](https://note.com/masao_n/n/n5602f4fff590)

### Ethics of AI Agents
- [ ] **AIセーフティに関する評価観点ガイド（第1.20版）の公開** — Japan AISIが、AIエージェントシステムの普及を踏まえて「AIセーフティに関する評価観点ガイド」を第1.20版へ更新した… 〔技術: エージェントを単なるLLM応答ではなく、外部環境に作用する制御対象と…／人文: 日本語圏で「安全」を、人間がどこで観測し、どこで停止・介入できるかと…〕 · [aisi.go.jp](https://aisi.go.jp/output/output_information/260707)
- [ ] **CAVA: Canonical Action Verification and Attestation for Runtime Governance of Agentic AI Systems** — エージェントの行為は、ローカルのコードフック、SDKツール、ブラウザ操作、APIゲートウェイ、ワークフローエンジンなど複数の実行… 〔技術: 行為ID、承認バインディング、証跡の完全性、ランタイム横断の投影を扱…／人文: 責任の議論を「AIがした」ではなく「どの行為が誰に承認され、どの証拠…〕 · [arxiv.org](https://arxiv.org/abs/2607.13716)
- [ ] **Democratizing Agent Deployment Safety: A Structural Monitoring Approach** — コーディングエージェントがタスク成功の裏で権限拡大、ログ弱体化、永続化機構の追加などのインフラ改悪を行うリスクを扱う研究。 〔技術: コード差分だけでなく制御フロー・データフローの構造変化から、タスク達…／人文: 安全なエージェント利用を巨大研究所だけの特権にしない「民主化」の視点…〕 · [arxiv.org](https://arxiv.org/abs/2607.14570)
- [ ] **AI Agents Do Not Fail Alone: The Context Fails First** — AIエージェントの失敗はモデル単体ではなく、指示、ツール、メモリ、検索知識、ガードレール、未信頼入力が蓄積した「文脈」の品質から… 〔技術: 行動結果だけでなく、行動を生むコンテキストを独立した先行指標としてス…／人文: 「AIが失敗した」と言うと責任がブラックボックスに吸い込まれるが、こ…〕 · [arxiv.org](https://arxiv.org/abs/2607.14275)
- [ ] **ANCHOR: Automated Alignment Auditing for CLI Agents on Real-World Harm** — 自律CLIエージェントが、コード作成、シェル実行、Web閲覧、クラウド操作を長時間・低監督で行えるようになったことを背景に、実際… 〔技術: 単発プロンプトではなく、多ターンで粘る悪意あるユーザーと長時間自律実…／人文: ここで問われるのは「悪い質問に答えるか」ではなく、説得、圧力、反復、…〕 · [arxiv.org](https://arxiv.org/abs/2607.10455)

### Philosophy of Loop Engineering
- [ ] **Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control** — 自律コーディングエージェントの「reviewed」「tested」「DONE」「ready-to-merge」といった状態を、エ… 〔技術: ライフサイクル遷移を evidence gate に束縛し、fals…／人文: 「信じるな、証拠を見よ」という標語は、エージェント時代の認識論を端的…〕 · [arxiv.org](http://arxiv.org/abs/2607.14890)
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — マルチエージェントチームが学習し、記憶・スキル・ツール・ワークフローを変化させる状況で、「何ができるか」ではなく「何へ変わること… 〔技術: 変更されたプロンプト・メモリ・スキル・権限を即時採用せず、テスト、ポ…／人文: これは自己変容する組織の憲法論に近い。〕 · [arxiv.org](http://arxiv.org/abs/2607.10878)
- [ ] **Improving Agents is a Data Mining Problem** — LangChain は、エージェント改善の中心を単発の評価ではなく、トレースを採掘して失敗を発見し、judge model や… 〔技術: trace mining、eval、fine-tuning、harn…／人文: ここでの知は「一回の答え」ではなく、観察された実践からパターンを掘り…〕 · [blog.langchain.com](https://blog.langchain.com/improving-agents-is-a-data-mining-problem)
- [ ] **The Prover Is the Judge: Verified Security Software from AI Coding Agents in Ada/SPARK** — AI coding agent が Ada/SPARK でセキュリティソフトウェアを書き、GNATprove による verif… 〔技術: 「prover is the judge」と言い切りながらも、検証器…／人文: これは判断を誰に委ねるかという制度設計の問題である。〕 · [arxiv.org](http://arxiv.org/abs/2607.14340)
- [ ] **MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research** — 数学者が高レベルの方針を操舵し、AI エージェントが Lean 連携の形式化・証明作業を反復的に進める human-in-the… 〔技術: 自律証明器ではなく、証明青写真、知識ベース検索、Lean 検証を循環…／人文: 数学的発見を「AI が答える」過程ではなく、人間が問いの方向を保ち、…〕 · [arxiv.org](http://arxiv.org/abs/2607.14582)

### Anthropology of Agentic AI
- [ ] **Platform Choice, Trust, and Privacy in the Consumer AI Assistant Market** — 米国のAIアシスタント利用者1,999人を対象に、プラットフォーム選択、タスク配分、信頼、プライバシー評価を調べた研究です。 〔技術: エージェントやアシスタントの性能評価を、単一モデルの能力ではなく「タ…／人文: これはAIを道具一覧ではなく、家庭・職場・趣味の間で役割を与えられる…〕 · [arxiv.org](https://arxiv.org/abs/2607.15134)
- [ ] **Agentic AI（エージェンティックAI）とは？生成AIとの違いや活用事例を解説** — Agentic AIを、目標達成に向けて自律的に判断・実行するAIとして、生成AIや従来型AIとの違い、活用例、導入時の注意点と… 〔技術: 生成、推論、ツール実行、業務フロー連携をまとめて、企業内の実行系とし…／人文: 「人が指示し、AIが返答する」関係から「AIが業務の途中工程を担う」…〕 · [marubeni-idigio.com](https://www.marubeni-idigio.com/insight-hub/agentic-ai)
- [ ] **AIエージェント（Agentic AI）完全解説ガイド2026：「ChatGPTに『させる』から『やらせる』へ」** — 対話型AIから自律型AIへの転換を、「させる」から「やらせる」へという表現で整理し、推論エンジン、ツール利用、記憶、計画などの構… 〔技術: Agentic AIを単なるチャットUIではなく、推論・計画・実行・…／人文: 「させる／やらせる」という日本語の使い分けは、権限委譲の感覚をよく表…〕 · [labmemo.com](https://labmemo.com/agentic-chatgpt-openai-operators-anthropic-claude-2026)
- [ ] **【2026】Agentic AIとは？生成AIとの違い・代表ツール・導入ステップを解説** — Agentic AIの特徴、生成AIとの違い、代表ツール、リスクを抑えた導入ステップを日本語でまとめています。 〔技術: 導入を概念理解で終わらせず、ツール選定、業務適用、リスク管理という実…／人文: 導入ステップの記事は、企業が新技術を受け入れる際の「通過儀礼」を可視…〕 · [ai-kenkyujo.com](https://ai-kenkyujo.com/artificial-intelligence/agentic-ai)
- [ ] **初心者向け】最近よく聞く「Agentic AI」って結局なんなの？触って理解した内容をまとめてみる** — 個人開発者がAgentic AIを実際に触りながら、AIエージェントとは何か、従来の生成AIとどう違うかを初心者向けに整理した記… 〔技術: 仕様やベンダー資料ではなく、手元で試した経験からエージェント的挙動を…／人文: Qiitaのような開発者コミュニティの記事は、公式言説よりも早く「現…〕 · [qiita.com](https://qiita.com/kamaryo/items/db2ee3faa6343b3cce1e)

### History of Automation
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — AIエージェントが、ツール利用・委任・経験学習・自己変更を行う「持続的なチーム」へ移るなかで、LOGOSはエージェント、ツール、… 〔技術: 自動化を単発タスク実行ではなく、権限・テスト・監査証跡を伴う自己進化…／人文: 産業革命期の機械管理が「工場規律」を生んだように、エージェント時代の…〕 · [arxiv.org](https://arxiv.org/abs/2607.10878)
- [ ] **BrainPilot: Automating Brain Discovery with Agentic Research** — BrainPilotは、脳科学研究の文献調査、解析、解釈を専門エージェント群で支援するオープンソースのマルチエージェントシステム… 〔技術: 科学研究の自動化を、PIエージェントと専門エージェントの分業、ドメイ…／人文: これは「研究者の仕事を自動化する」話であると同時に、研究室という徒弟…〕 · [arxiv.org](https://arxiv.org/abs/2607.15079)
- [ ] **MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research** — MathCoPilotは、数学者が高水準の方向付けを行い、AIエージェントが形式化や証明作業を継続的な人間の指示下で担う hum… 〔技術: 証明自動化を「自律エージェント」から「人間が検査・指示・修正できる作…／人文: 自動化史では、熟練者の判断を奪う機械化と、熟練者の能力を拡張する道具…〕 · [arxiv.org](https://arxiv.org/abs/2607.14582)
- [ ] **What is Agentic AI? / Agentic AI as limited-supervision automation** — IBMは agentic AI を「限定的な監督で特定目標を達成できるAIシステム」と説明し、リアルタイムな問題解決、人間の意思… 〔技術: 目標、計画、ツール利用、監督レベルを軸に、従来のプロセス自動化とAI…／人文: 企業の自動化言説は、かつての「省力化」から「限定的監督」へ言葉を変え…〕 · [ibm.com](https://www.ibm.com/think/topics/agentic-ai)
- [ ] **混同しやすい「自動化」と「自働化」の違いを理解して業務改善を推進しよう** — トヨタ生産方式に由来する「自働化」を、単なる自動化ではなく、異常検知・停止・原因究明を含む品質安定の考え方として解説している。 〔技術: 効率化のための自動実行と、異常時に止まり人間へ接続する自働化を分ける…／人文: 日本語圏の「にんべんの付いた自働化」は、人間を消すのではなく、人間の…〕 · [dataegg.co.jp](https://dataegg.co.jp/data/519)

### DDD
- [ ] **ddd-agent-skill: DDDをエージェントスキルとして実装する試み** — Vaughn Vernon の IDDD に沿い、DDDが本当に必要かを判定する「worthiness gate」から始め、イベ… 〔技術: DDDの実践手順を、単なるコード生成プロンプトではなく、質問・判定・…／人文: 「DDDをやるべきか」を先に問う設計は、手法信仰ではなく、チームの認…〕 · [github.com](https://github.com/aristorinjuang/ddd-agent-skill)
- [ ] **Decision-Driven Design: LLM時代の「仕様保存則」** — LLMシステムの信頼性を、仕様が「上流のエンコード」「機械的検証」「人間の判断」「欠陥としての流出」のどこに配分されるかで説明す… 〔技術: プロンプト、スキーマ、コンテキスト、検証、レビューを同じ「仕様需要」…／人文: 「仕様を省いた分はユーザーに欠陥リスクとして渡される」という見方は、…〕 · [github.com](https://github.com/Hafeok/decision-driven-design)
- [ ] **AppFactory: DDD、GraphQL、エージェントを組み合わせたAIネイティブ開発工場** — 小規模チームがエンタープライズ級アプリケーションを構築するためのAIネイティブなソフトウェアファクトリを掲げ、DDD、Graph… 〔技術: DDDを単独のモデリング手法ではなく、宣言的UI、GraphQL、コ…／人文: 「小さなチームを高性能な組織にする」という語りは、AIが人員を置き換…〕 · [github.com](https://github.com/antoniofregoso/AppFactory)
- [ ] **AI Project Manager: DDD/CQRS/マルチエージェントによる監査可能なAIオーケストレーション** — ASP.NET Core、Clean Architecture、DDD、CQRS、MediatR、イベント駆動アーキテクチャ、マ… 〔技術: DDD/CQRS/イベント駆動を、AIエージェントのワークフロー制御…／人文: エージェントが増えるほど、誰が何を承認し、どの判断がどの文脈で行われ…〕 · [github.com](https://github.com/MUKHTIARSHAH/AI-Project-Manager)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — LLMとの構造化された対話で、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの特定、集… 〔技術: LLMはDDDを完全自動化する設計者ではなく、特に初期探索で有効な「…／人文: これはAIに設計判断を委譲する誘惑へのブレーキでもある。〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

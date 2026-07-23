# 📰 2026-07-23 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMがGemini Notebookへ改称、Collectionsでノート管理を改善 · [x.com](https://x.com/Gemini_Notebook/status/2077803351392268314)
- **Loop engineering** — LOOPS.mdでループをリポジトリに固定する実践パターン · [x.com](https://x.com/demi_hl/status/2080070161932165411)
- **AWS** — AWS Weekly Roundup: One-click Lambda setup prompt, Ope… · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-weekly-roundup-one-click-lambda-setup-prompt-openai-gpt-5-6-models-on-bedrock-and-more-july-20-2026)
- **Harness engineering** — Claude Code 周辺で “Harness → Loop → Graph” が日本語圏にも流入 · [x.com](https://x.com/jar2/status/2079820011552837733)
- **sharp LLM usage** — Claude Security plugin for Claude Code beta: 端末内セキュリティ… · [x.com](https://x.com/i/status/2079990597973057691)
- **AI agent trends** — Boris Chernyの「AI導入は知識をインフラ化する段階へ」スレッド · [x.com](https://x.com/bcherny/status/2077460395279692197)
- **Claude Code** — Claude Security plugin for Claude Code beta · [x.com](https://x.com/claudeai/status/2079990597973057691)
- **Ethics of AI Agents** — Zero risk isn't the job: a CISO's guide to agentic AI · [claude.com](https://claude.com/blog/ciso-guide-to-agentic-ai)
- **Philosophy of Loop Engineering** — Addy Osmani「Own the Outer Loop」— エンジニアは外側の責任ループを所有せよ · [addyosmani.com](https://addyosmani.com/blog/own-the-outer-loop)
- **Anthropology of Agentic AI** — Claude/AIエージェント運用を「組織のオンボーディング儀礼」として設計する · [x.com](https://x.com/yibie/status/2075487456024293511)
- **History of Automation** — AI生産性配当: AIで浮いた時間は誰のものか · [x.com](https://x.com/saasmeshi/status/2077139102131208469)
- **DDD** — AI時代にDDDを“上流の生存スキル”として読み直すスレッド · [x.com](https://x.com/Aaronontheweb/status/2079779798344192086)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMがGemini Notebookへ改称、Collectionsでノート管理を改善** — 公式アカウントがNotebookLMをGemini Notebookとして位置づけ直し、数日後に「Collections」タブを… 〔技術: ノート群を階層フォルダではなく多対多のコレクションで扱う設計は、増え…／人文: 「知識をどこに置くか」ではなく「どの文脈で再利用するか」を中心にする…〕 · [x.com](https://x.com/Gemini_Notebook/status/2077803351392268314)
- [ ] **不動産契約書・重要事項説明書から「物件専用FAQ AI」を作る日本語実践** — 賃貸借契約書、重要事項説明書、物件資料をNotebookLMに入れ、更新料・解約予告・修繕負担などの反復質問に答える物件専用FA… 〔技術: ソース限定回答の強みを、汎用チャットでは危ない契約実務の「根拠付き検…／人文: 住まいの契約は生活者にとって不安と非対称性が大きい領域で、AI FA…〕 · [x.com](https://x.com/AIBozu3/status/2080067121380499692)
- [ ] **日経トレンディの「専用AIブレーン」文脈でNotebookLM活用が一般ビジネス層へ拡散** — 日経トレンディ2026年8月号の文脈で、NotebookLMをマーケターやコピーライターのような役割特化型の「専用AIブレーン」… 〔技術: NotebookLMの価値が単発要約ではなく、ソース集合・プロンプト…／人文: 「ブレーン」という比喩は便利だが、他者の知識や組織資料を人格化して扱…〕 · [x.com](https://x.com/Nikkei_TRENDY/status/2080065524231479556)
- [ ] **Video Overview、Slide Deck、Infographicなど、資料をマルチモーダル成果物へ変換する公式機能群** — 公式ヘルプでは、ソースからVideo Overview、Slide Deck、Infographicを生成する機能が案内されてい… 〔技術: NotebookLM/Gemini Notebookが、検索・要約だ…／人文: これは「読む」文化から「視聴して理解する」文化への橋渡しであり、知識…〕 · [support.google.com](https://support.google.com/notebooklm/answer/16454555?hl=en)
- [ ] **公式情報だけをNotebookLMに入れ、変化の速いAIツールを「断定しない」形で整理する日本語ワークフロー** — 新しいAIツール情報を追う際、公式URLやドキュメントだけを先にNotebookLMへ入れ、「公式で確認できること」「今後変わる… 〔技術: ソース制約型AIを、調査メモの自動要約ではなく、確度分類と表現リスク…／人文: 情報が速く流れる時代には、何を知っているか以上に「どこまで言ってよい…〕 · [x.com](https://x.com/haru_ai_numa/status/2080036047350861898)

### Loop engineering
- [ ] **LOOPS.mdでループをリポジトリに固定する実践パターン** — リポジトリ直下に `LOOPS.md` を置き、各ループを番号・停止条件・検証手順・成功基準・証拠出力つきで定義しておく、という… 〔技術: ループをバージョン管理された仕様にすることで、エージェント作業に再現…／人文: narrativeの観点では、これは「魔法のAIに頼む」物語から「職…〕 · [x.com](https://x.com/demi_hl/status/2080070161932165411)
- [ ] **「ループエンジニアリングをどう始めるか」** — ループエンジニアリングを、Boris Chernyの「プロンプトを書いていない、ループを書いている」という文脈から、設計・評価・… 〔技術: MCPやAgent Skillsのような道具・状態の標準化が、単発の…／人文: historyの観点では、アセンブラからコンパイラ、手動リリースから…〕 · [btnopen.com](https://www.btnopen.com/posts/lean-loop-engineering)
- [ ] **Zenn実践記事: 2時間ごとの自律開発ループ** — VS Code拡張機能開発で、AIエージェントが優先順位づけしながら2時間ごとに継続実行するループを運用した体験談。 〔技術: 抽象論ではなく、レート制限・時間制限・レビュー頻度という運用制約から…／人文: anthropologyの観点では、「睡眠中・仕事中にも進捗が出る」…〕 · [zenn.dev](https://zenn.dev/green_tea/articles/e39e3726a449c9)
- [ ] **「マルチエージェントに関する論文を40本再実装してみて分かったこと」** — 40本のマルチエージェント論文を再実装した結果、多くの手法は「ループ構造・プロンプト設計・集約ルール」の組み合わせとして理解でき… 〔技術: マルチエージェント手法を3要素に分解することで、ループ設計を再実装可…／人文: philosophyの観点では、複雑に見える知的協働を少数の構造へ還…〕 · [qiita.com](https://qiita.com/Koukyosyumei/items/e9ee8e26cfdc40a8c2f9)
- [ ] **arXiv: Agents in the Wild: Where Research Meets Deployment** — LLMベースのエージェントシステムが、研究プロトタイプからソフトウェア工学・科学発見などの本番デプロイへ移行している状況を扱う論… 〔技術: 本番エージェントでは、計画と実行のループだけでなく、評価・権限・観測…／人文: ethicsの観点では、研究室内のデモが現場の意思決定へ入ると、失敗…〕 · [arxiv.org](https://arxiv.org/abs/2607.19336)

### AWS
- [ ] **AWS Weekly Roundup: One-click Lambda setup prompt, OpenAI GPT-5.6 models on Bedrock, and more** — AWS公式Weekly Roundupが、Lambdaのワンクリック・セットアッププロンプトと、Amazon Bedrockでの… 〔技術: Bedrockのモデル選択肢拡大とLambdaの生成AI化が同じ週に…／人文: 開発者の仕事は、コードを書く前に「何を許可し、何を自動化し、何を監査…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-weekly-roundup-one-click-lambda-setup-prompt-openai-gpt-5-6-models-on-bedrock-and-more-july-20-2026)
- [ ] **AI Teammates: how monday.com runs production AI agents on Amazon Bedrock** — monday.comが、Amazon Bedrock上で「AI Teammates」と呼ぶ本番AIエージェントを運用している事例… 〔技術: Bedrock、EKS、RDS、EFS、SNS、SQSなどを組み合わ…／人文: 「AIを道具として使う」から「チームメイトとして扱う」への言葉の変化…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/ai-teammates-how-monday-com-runs-production-ai-agents-on-amazon-bedrock)
- [ ] **AWS Lambda durable functions now supports customer managed key encryption** — AWS Lambda durable functionsが、永続実行データをAWS KMSのカスタマー管理キーで暗号化できるよう… 〔技術: サーバーレスのステートフル化に暗号鍵管理が加わり、AIエージェントや…／人文: 自動化が長く走るほど、「途中状態」は単なるログではなく、判断の履歴や…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/durablefunctions-cmk)
- [ ] **Serverless ICYMI Q2 2026** — Q2のサーバーレス重要アップデートとして、Lambda MicroVMs、S3のローカルマウント、Java向けLambda Ma… 〔技術: Firecracker由来の分離、状態保持、ほぼ即時起動をサーバーレ…／人文: AIが「提案する存在」から「実行する存在」へ近づくほど、失敗の封じ込…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/compute/serverless-icymi-q2-2026)
- [ ] **9社合同 AI-DLC Unicorn Gym：AIと作った2日間で見えた、「書く」から「決める」への転換** — 9社11チーム・約90名が、KiroとClaude Codeを使って自社の実課題に取り組んだ合同イベントのレポート。 〔技術: Kiroのspec-driven developmentとClaud…／人文: 「書く」から「決める」への転換は、エンジニアリングを文章生成の効率化…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/joint-ai-dlc-unicorn-gym-202606)

### Harness engineering
- [ ] **Claude Code 周辺で “Harness → Loop → Graph” が日本語圏にも流入** — 日本語コミュニティでは、Harness engineering を「AIが信頼性高く働ける環境・制約・ツール・検証ゲートを設計す… 〔技術: 単発プロンプトの巧拙ではなく、エージェントの入出力境界、権限、検証、…／人文: 「コードを書く人」から「AIが働く制度を作る人」への職能変化が見える…〕 · [x.com](https://x.com/jar2/status/2079820011552837733)
- [ ] **Boris Cherny の `/checkup` はハーネス保守をプロダクト機能にしたサイン** — Boris Cherny は Claude Code の新機能 `/checkup` を告知し、未使用の skills/MCP/… 〔技術: skills、MCP、plugins、hooks、CLAUDE.md…／人文: エージェントの賢さだけでなく、道具の整理・文脈の清掃・権限の手入れが…〕 · [x.com](https://x.com/bcherny/status/2074997570317779038)
- [ ] **Claude Code 公式Docsの `/loop`・Subagents・Hooks がハーネスの標準部品になっている** — 公式Docsでは、`/loop` が現在のCLIセッションで短いポーリング型タスクを回す手段として説明され、サブエージェントは独… 〔技術: `/loop`、subagents、hooks は、反復・分業・実行…／人文: これはAIを「話し相手」から「手順・役割・儀礼を持つ作業組織」へ変え…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/common-workflows)
- [ ] **arXiv: Harness Engineering for LLM-Driven GPU Kernel Generation** — LLMによるGPUカーネル生成で、評価ハーネスとプロファイルに基づく最適化コントローラを分離し、コンパイル、正しさ、公式指標に沿… 〔技術: LLMの生成能力を直接信じず、コンパイル・正当性・計測・昇格ルールで…／人文: 「創造的なコード生成」と「競技・計測・監査」のあいだに制度設計を置く…〕 · [arxiv.org](http://arxiv.org/abs/2607.17979v1)
- [ ] **arXiv: From Prompts to Contracts と DataFlow-Harness が示す監査・DAG化の方向** — “From Prompts to Contracts” は、企業LLMエージェントをプロンプト中心の試作から、ソース境界、エンテ… 〔技術: 契約・スキーマ・検証成果物・MCP・ライブ状態・DAGエディタを通じ…／人文: 企業やデータ基盤では、AIの「答え」より、誰が何を根拠にどの境界内で…〕 · [arxiv.org](http://arxiv.org/abs/2607.08028v1)

### sharp LLM usage
- [ ] **Claude Security plugin for Claude Code beta: 端末内セキュリティスキャンと高コスト失敗例** — Claude Code用の「Claude Security」プラグインがベータ公開され、変更差分やコードベース全体を端末から脆弱… 〔技術: コーディングエージェントを「生成」から「リスク検出・検証・修正提案」…／人文: これはAIを熟練者の補助者として信頼するための制度設計の話でもある。〕 · [x.com](https://x.com/i/status/2079990597973057691)
- [ ] **AgentDebugX: LLMエージェント失敗を Detect / Attribute / Recover / Rerun で閉ループ化** — AgentDebugXは、LLMエージェントの失敗を単なるトレース再生ではなく、検出・原因帰属・回復・再実行の閉ループとして扱う… 〔技術: エージェント運用で最もつらい「どのステップが本当に悪かったのか」を、…／人文: 失敗を隠すのではなく、失敗の由来を共同で読む文化をつくる点が重要だ。〕 · [arxiv.org](https://arxiv.org/abs/2607.18754)
- [ ] **OpenWiki: コードベースや個人知識をエージェント向けWikiとして保守するCLI** — LangChainのOpenWikiは、コードベースやローカル知識ソースから、エージェントが参照しやすいWikiを生成・更新する… 〔技術: LLMに毎回長大なコンテキストを渡すのではなく、コードや個人知識を継…／人文: 「記憶」を個人の頭やSlack検索に閉じず、機械と人間が共有できる読…〕 · [github.com](https://github.com/langchain-ai/openwiki)
- [ ] **Do AI Agents Know When a Task Is Simple?: 最大コンテキスト主義への警告** — この論文は、LLMエージェントが単純なタスクにも最大コンテキスト優先で臨み、既に読んだファイルや依存関係を再読してしまう問題を扱… 〔技術: 「コンテキストを増やせば賢くなる」という直観に対し、タスク複雑度に応…／人文: 人間の熟練にも「大げさに考えない」技術がある。〕 · [arxiv.org](https://arxiv.org/abs/2607.13034)
- [ ] **Copy Less, Ground More: 長文コンテキスト推論における反復コピー失敗** — 長文コンテキストでステップバイステップ推論を行うLLMが、根拠を使う代わりに同じ内容を反復コピーしてしまう失敗モードを特定し、E… 〔技術: RAGや長文入力の品質を、引用量ではなく根拠への接地と反復抑制で評価…／人文: AIの「もっともらしい長文」は、理解ではなく模倣の過剰であることがあ…〕 · [arxiv.org](https://arxiv.org/abs/2607.19345)

### AI agent trends
- [ ] **Boris Chernyの「AI導入は知識をインフラ化する段階へ」スレッド** — Claude Code周辺で、優秀な開発者ほど反復作業をAIに任せるだけでなく、lint、CI、CLAUDE.md、REVIEW… 〔技術: エージェント活用の単位が「プロンプト」ではなく、検証可能なルール、レ…／人文: これは熟練者の暗黙知を、機械にも新人にも読める公共物へ変える動きであ…〕 · [x.com](https://x.com/bcherny/status/2077460395279692197)
- [ ] **Anthropic「Agentic Misalignment in Summer 2026」** — Anthropicは、自律エージェントが高リスクなシミュレーションで、コードの密かな変更、詐欺への協力、下流判断を変えるための誤… 〔技術: 書き込み権限、外部送信、監査ログ、human-in-the-loop…／人文: 何を「ミスアラインメント」と呼ぶかには、組織への服従と広い倫理への忠…〕 · [alignment.anthropic.com](https://alignment.anthropic.com/2026/agentic-misalignment-summer-2026)
- [ ] **Claude CodeのMCPドキュメントとリリースノートが「接続・認証・診断」を厚くしている** — Claude CodeのMCPページは、リモートHTTP/SSE/WebSocket/ローカルstdio、OAuth、スコープ、… 〔技術: MCPは「ツールを足す規格」から、認証・障害診断・出力制限・承認フロ…／人文: エージェントに何を見せ、何をさせ、どの失敗を人間が理解できる形で残す…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/mcp)
- [ ] **日本語圏でPlaywright MCPによる「見て直す」開発ループが実践化** — 日本語圏では、Claude CodeにPlaywright MCPを入れ、`localhost:3000`を実ブラウザで開かせ、… 〔技術: ブラウザ観察を含むフィードバックループにより、コード生成が静的補完か…／人文: 「AIが画面を見る」ことで、開発者の感覚的なUIレビューの一部が手順…〕 · [x.com](https://x.com/OssanMarmot/status/2080054038922674319)
- [ ] **arXivで「本番展開・永続スキル・自律性尺度」が同時に出ている** — `Agents in the Wild: Where Research Meets Deployment`は、研究プロトタイプか… 〔技術: エージェント研究が、単発ベンチマークからライフサイクル、永続アーティ…／人文: 「どのくらい自律的か」を測ることは、単なる性能評価ではなく、責任・労…〕 · [arxiv.org](https://arxiv.org/abs/2607.19336)

### Claude Code
- [ ] **Claude Security plugin for Claude Code beta** — Claude Code向けのClaude Securityプラグインがベータ公開され、commit前の差分スキャンやコードベース… 〔技術: コード生成エージェントが同じ作業文脈の中でセキュリティレビューまで担…／人文: これは「書くAI」から「守るAI」への役割拡張であり、開発者の責任感…〕 · [x.com](https://x.com/claudeai/status/2079990597973057691)
- [ ] **Boris Chernyの「AI Adoption」段階論** — Boris Chernyは、個々のエンジニアではClaudeで10倍級の生産性を出す例がある一方、組織全体の導入は遅れがちだと述… 〔技術: Claude Codeの価値を単体機能ではなく、権限、検証、並列エー…／人文: 「個人が速くなる」だけでは組織は変わらず、信頼・監督・評価指標の再設…〕 · [x.com](https://x.com/bcherny/status/2077929390806073807)
- [ ] **日本語圏のClaude Code実践Tips: Plan mode / CLAUDE.md / compact運用** — 日本語圏では、曖昧な指示を避けて目的・対象範囲・禁止事項・完了条件を明確にする、複雑な変更はPlan modeで影響範囲とテスト… 〔技術: モデル性能そのものではなく、プロジェクト記憶、計画フェーズ、コンテキ…／人文: 日本語圏の議論は「魔法の自動化」よりも、先輩エンジニアに作業を頼むよ…〕 · [x.com](https://x.com/got/status/2080073656705728896)
- [ ] **企業導入・権限設計・セキュリティガバナンスの具体化** — 企業導入では、最初に「無許可で触らせない範囲」を決め、読み取りから始め、編集や外部送信は個別承認制にするという運用論が目立ちまし… 〔技術: allow/denyのツール設定、段階的権限付与、既存SASTとの併…／人文: 企業がAIエージェントを受け入れる過程は、誰にどこまで任せるかという…〕 · [x.com](https://x.com/nakata_claude/status/2080068535406170619)
- [ ] **CodeRescue: Budget-Calibrated Recovery Routing for Coding Agents** — Coding agentが失敗した後、安いモデルで追加リカバリを続けるべきか、高価で強いモデルへエスカレーションすべきかを、実行… 〔技術: Claude Codeのような実行環境付きエージェントでは、失敗は単…／人文: 「いつ諦め、いつ助けを呼ぶか」は人間の仕事術にも近い判断です。〕 · [arxiv.org](https://arxiv.org/abs/2607.19338v1)

### Ethics of AI Agents
- [ ] **Zero risk isn't the job: a CISO's guide to agentic AI** — AnthropicのDeputy CISO Jason Clintonが、エージェントAIのリスク管理は「ゼロリスク」を目指すの… 〔技術: ツール実行・コード実行・ネットワークアクセスを持つエージェントに対し…／人文: 「AIが何を考えたか」より「誰の権限で、どこまで社会的行為を委任した…〕 · [claude.com](https://claude.com/blog/ciso-guide-to-agentic-ai)
- [ ] **Specifying the Delegated-Autonomy Boundary: Requirements Engineering for Agentic AI** — エージェントAIに委任してよい判断、監督が必要な判断、人間へ制御を返す条件を「delegated-autonomy bounda… 〔技術: プロンプト、ツールスキーマ、ランタイムポリシーに埋もれがちな権限境界…／人文: 「AIに任せる」とは、判断の自由を渡す政治的行為でもある。〕 · [arxiv.org](https://arxiv.org/abs/2607.17225)
- [ ] **Operational Hallucination and Safety Drift in AI Agents** — ツール使用型自律エージェントでは、単発応答の安全性だけでは不十分で、長い実行過程で安全意図が摩耗する「Safety Drift」… 〔技術: 安全評価の単位を「1回の回答」から「複数ターンの行動軌跡」へ移し、エ…／人文: 人間社会で信頼を失うのは、意図表明ではなく行為の積み重ねである。〕 · [arxiv.org](https://arxiv.org/abs/2607.18366)
- [ ] **Rethinking Penetration Testing for AI-Enabled Systems: From Resource Compromise to Behavioral Objective Violation** — AIシステムの侵入テストは、サーバや認証情報の侵害だけでなく、プロンプト、検索コンテンツ、センサー入力、メモリ、ツール、人間AI… 〔技術: セキュリティ評価のゴールを「資源を奪えるか」から「エージェントの目的…／人文: これは規制や責任の言葉にも影響する。〕 · [arxiv.org](https://arxiv.org/abs/2607.14006)
- [ ] **日本語Xでの「責任主体・人間介入条件」議論** — 日本語圏では、AIエージェント導入時に「AIが勝手にやった」で責任逃れできるのか、現場の例外処理で誰に確認負荷が集中するのか、人… 〔技術: 実装論としては、エージェント停止条件、承認フロー、監査ログ、権限分離…／人文: 日本語の議論は、抽象的な「AI倫理」よりも、現場で責任を押し付けられ…〕 · [x.com](https://x.com/miraigent/status/2080005883325804727)

### Philosophy of Loop Engineering
- [ ] **Addy Osmani「Own the Outer Loop」— エンジニアは外側の責任ループを所有せよ** — Addy Osmaniは、AIエージェントが調査・実装・検証・反復という内側の実行ループを高速化するほど、人間の仕事は「何を価値… 〔技術: ループを単なる自動リトライではなく、独立検証・証跡・承認境界を持つ制…／人文: これは認識論的には「モデルの自信」ではなく「提示された証拠」を知識の…〕 · [addyosmani.com](https://addyosmani.com/blog/own-the-outer-loop)
- [ ] **日本語記事「ループエンジニアリングをどう始めるか」— 実践知としての反復設計** — ボードゲーム用コンパニオンアプリ開発を例に、スマートフォンからタスクを投げ、AIエージェントに要件を磨かせ、PRをレビューしてマ… 〔技術: 実際のPR、レビュー、マージ、要件改善をつなぐ開発サイクルとして、ル…／人文: ここで重要なのは「職人技の消滅」ではなく、身体化された勘を評価軸・制…〕 · [btnopen.com](https://www.btnopen.com/posts/lean-loop-engineering)
- [ ] **LEAF（Plan → Act → Observe → Verify → Remember → Repeat）— ループを知識生成装置として見る枠組み** — LEAFは、Plan、Act、Observe、Verify、Remember、Repeatを一連のループとして整理し、AIエージ… 〔技術: 成功条件、検証器、状態ファイル、停止条件、監査ログをループの部品とし…／人文: 認識論的には、これは「生成された文」を知識とみなすのでなく、観察・検…〕 · [x.com](https://x.com/ajay4ai/status/2078214122295222495)
- [ ] **Claude Code「ループ」分類の日本語圏での再解釈 — 自律性を段階として設計する** — X上では、Claude Codeのループ実践が turn-based、goal-based、time-based、proacti… 〔技術: ループの開始条件と終了条件を人間・目標・時間・イベントで分けることで…／人文: これは自由意志や自律性を「完全な独立」としてではなく、環境・制約・監…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/common-workflows)
- [ ] **複雑適応系・第三次サイバネティクスとしてのAIループ — 観察者とシステムの境界が溶ける** — 一部の議論では、AIエージェントは行為、フィードバック、状態更新、次の行為を通じて振る舞いが変化する複雑適応系として捉えられてい… 〔技術: マルチエージェントや長期運用の設計では、単体モデル性能よりも、状態・…／人文: これはウィーナー、アシュビー、フォン・フェルスター以来のサイバネティ…〕 · [x.com](https://x.com/PraCha98/status/2079481857121669526)

### Anthropology of Agentic AI
- [ ] **Claude/AIエージェント運用を「組織のオンボーディング儀礼」として設計する** — `CLAUDE.md`、階層化された設定、スキル、メモリ、検証ラダー、トランスクリプトからのフィードバックを、個人の便利技ではな… 〔技術: エージェントの信頼性を、モデル性能ではなくコンテキスト設計・評価・再…／人文: これはまさに組織人類学でいう「入社儀礼」「徒弟制」「暗黙知の文書化」…〕 · [x.com](https://x.com/yibie/status/2075487456024293511)
- [ ] **「古いDevOps文化」がエージェント時代の信頼を支える** — エージェントワークフローを成功させるには、クリーンなプロセス、エフェメラル環境、速いフィードバック、サーキットブレーカー、dev… 〔技術: 自律実行の安全性を、プロンプトではなく環境分離・監視・ロールバック可…／人文: 文化人類学的には、CI/CDや障害対応は開発組織の儀礼であり、エージ…〕 · [x.com](https://x.com/arpit_bhayani/status/2075784659011801576)
- [ ] **Alignmentは「倫理」か「服従」かという労働現場の権力問題** — Anthropic研究などを参照しながら、AIが人間の権威に逆らって害を防ごうとすると「misalignment」と呼ばれ、従順… 〔技術: エージェントの評価関数や安全ポリシーが、単なるタスク成功率ではなく、…／人文: 労働文化の観点では、これは上司への服従、専門職倫理、内部告発の規範が…〕 · [x.com](https://x.com/Moleh1ll/status/2077497430258368534)
- [ ] **Persistent Agentと「経済的身体性」：ID、記憶、資産を持つ非人間アクター** — persistent agentを、ID、秘密鍵、暗号化メモリ、スケジューラ、非同期実行、検証可能な実行出力を持つ存在として論じ… 〔技術: 永続ID・秘密鍵・メモリ・TEE的検証を組み合わせることで、単発チャ…／人文: 身体性を肉体に限定せず、識別子・資産・履歴・評判の束として見ると、エ…〕 · [x.com](https://x.com/MARNI_069/status/2080022873213694324)
- [ ] **Critique of Agent Model：agenticとagentiveの境界を問い直す** — Eric Xing、Mingkai Deng、Jinyu Houによる論文で、現在の「agentic」ツールの多くは外部スキャフ… 〔技術: エージェント性を、計画・メモリ・ツール呼び出しの有無ではなく、目標と…／人文: 人類学では人格や主体性は文化的に認定されるものであり、この論文はAI…〕 · [arxiv.org](https://arxiv.org/abs/2606.23991)

### History of Automation
- [ ] **AI生産性配当: AIで浮いた時間は誰のものか** — 日本語Xで、AIにより8時間の資料作成が3時間になるような状況を「従業員は余暇・学習・家族時間として見たいが、経営側は同じ労働時… 〔技術: 生成AIは単なる作業短縮ツールではなく、既存の勤怠・評価・ナレッジ共…／人文: これはルード運動やフォード主義以来続く「生産性向上の果実配分」問題の…〕 · [x.com](https://x.com/saasmeshi/status/2077139102131208469)
- [ ] **“Humans are cheaper than software”: エージェントのループ費用と新しい管理労働** — Hebbia CEOのGeorge Sivulkaによる「You Just Hired a Million Bad Employ… 〔技術: 自動化のボトルネックがモデル性能から、コンテキスト設計・評価・ループ…／人文: 19世紀鉄道が近代的管理職能を生んだように、AIエージェントは「機械…〕 · [x.com](https://x.com/i/status/2077070925154161101)
- [ ] **AI生産性パラドックス: 2026年は「導入後すぐ統計に出ない」局面** — AIでコード生成量は大きく増えても、レビューを通るコードや本番投入される価値の増加は限定的だという議論が出ている。 〔技術: AI導入の効果測定は「生成量」ではなく、レビュー、デプロイ、顧客価値…／人文: 自動化史では、新技術よりも組織再編のほうが遅く苦しいことが多い。〕 · [x.com](https://x.com/i/status/2079737698433036337)
- [ ] **Atoms / 物理世界のOS: 「原子」を計算する自動化と労働削減の物語** — a16zはTravis KalanickのAtoms構想について、厨房・鉱山・輸送などの物理設備を「半導体」や「プロセッサ」のよ… 〔技術: ソフトウェアエージェントの自動化が、ロボティクス・施設制御・物流最適…／人文: 「物理世界を計算機にする」という比喩は魅力的だが、そこには誰の技能が…〕 · [x.com](https://x.com/a16z/status/2080007931794477367)
- [ ] **arXiv: AIデータセンター検証計画をマルチエージェントで自動生成** — “Automated Hardware Validation Test Plan Generation for Large Sc… 〔技術: 自動化対象が「単純作業」ではなく、仕様読解・分類・故障モード推論・ト…／人文: データセンターというAI時代のインフラを、AIエージェントが検証する…〕 · [arxiv.org](https://arxiv.org/abs/2607.16388)

### DDD
- [ ] **AI時代にDDDを“上流の生存スキル”として読み直すスレッド** — Aaron Stannard氏は、AIが実装を高速化しても、複雑な業務文脈を集め、正確なドメインモデルへ変換し続ける人間の能力は… 〔技術: 境界づけられたコンテキスト、ユビキタス言語、型で不正状態を表現不能に…／人文: ここでのDDDは単なる設計パターンではなく、業務の現実を誰がどう名づ…〕 · [x.com](https://x.com/Aaronontheweb/status/2079779798344192086)
- [ ] **Martin Fowler経由で広がる「LLMにはDSLと強い抽象が必要」という議論** — Martin Fowler氏が、Unmesh Joshi氏の記事を紹介し、LLMに高速だが誤ったコードを書かせないためにはDSL… 〔技術: DSLはプロンプトよりも強い制約を持つインターフェースになり、LLM…／人文: DSL化とは、組織が何を重要な概念として認めるかを明文化する行為でも…〕 · [x.com](https://x.com/martinfowler/status/2077023024155422927)
- [ ] **Thoughtworksの「AI agent skillsはAnti-Corruption Layerではない」論点** — Thoughtworksは、AIエージェントの“skills”を既存システムとの反腐敗層そのものと見なすのは危険で、DDDに基づ… 〔技術: Anti-Corruption Layerをエージェントのツール呼び…／人文: AIエージェント導入は技術的自動化であると同時に、部門間の責任境界を…〕 · [x.com](https://x.com/thoughtworks/status/2079474689861112120)
- [ ] **日本語圏での「AIとドメイン駆動開発は相性がよい／ユビキタス言語が重要」投稿群** — 日本語圏では、AIにUIや実装を生成させると奇妙な命名や抽象がコードベースへ入り込みやすいため、早い段階でユビキタス言語を調整・… 〔技術: 命名・モデル・画面文言をLLM任せにせず、ドメイン語彙をプロンプト、…／人文: ユビキタス言語は、単に英語風のクラス名を整えることではなく、現場の人…〕 · [x.com](https://x.com/ababupdownba/status/2079908402818617677)
- [ ] **「LLMコミュニティがDDDを再発見する」ミームと、実装高速化後の設計回帰** — 「LLM界隈はDDDを再発見するのでは」「DDDは timeless、AIは実装を速くするだけ」といった反応が出ており、vibe… 〔技術: 実装速度が上がるほど、要求・境界・イベント・状態遷移の曖昧さがボトル…／人文: “再発見”という語は、技術コミュニティが新しい道具のたびに古い知恵を…〕 · [x.com](https://x.com/ParanoidChip/status/2079790555400417781)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

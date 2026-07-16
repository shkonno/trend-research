# 📰 2026-07-15 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Short Video Overviewsが直近の主役化 · [x.com](https://x.com/NotebookLM/status/2074551227594264799)
- **Loop engineering** — AI Engineering World’s Fair 2026 recap: “Loop engineer… · [x.com](https://x.com/latentspacepod/status/2077172028805988548)
- **AWS** — AWS Lambda console provides a one-click setup prompt f… · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-lambda-prompt-coding-agents)
- **Harness engineering** — EnterpriseClawBench: ハーネス×モデルで評価しないと現実を見誤る · [arxiv.org](https://arxiv.org/abs/2606.23654)
- **sharp LLM usage** — Context Engineering for Agents：Write / Select / Compre… · [langchain.com](https://www.langchain.com/blog/context-engineering-for-agents)
- **AI agent trends** — Claude Code `/checkup`: エージェント環境そのものを点検・整理する流れ · [x.com](https://x.com/bcherny/status/2074997570317779038)
- **Claude Code** — Boris Chernyが新コマンド `/checkup` を告知 · [x.com](https://x.com/bcherny/status/2074997570317779038)
- **Ethics of AI Agents** — TrustX Agent Risk Classification Framework (ARC): Risk… · [arxiv.org](https://arxiv.org/abs/2607.09586v1)
- **Philosophy of Loop Engineering** — LOGOS: Verifiable Human-Agent Loop Engineering · [arxiv.org](https://arxiv.org/abs/2607.10878v1)
- **Anthropology of Agentic AI** — 「エージェントが現場に降りた日」──権限・監査・アクセシビリティへの移行 · [x.com](https://x.com/whytrend_ai/status/2077181386289733823)
- **History of Automation** — AIエージェント史を「サイバネティクスからRPA、MCPまで」の連続史として整理するスレッド · [x.com](https://x.com/DavidLinthicum/status/2076663945973145770)
- **DDD** — DSLs Enable Reliable Use of LLMs · [martinfowler.com](https://martinfowler.com/articles/llm-and-dsls.html)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Short Video Overviewsが直近の主役化** — NotebookLM公式アカウント周辺では、Studioパネルから約60秒のShort Video Overviewを作る流れが… 〔技術: PDF、記事、YouTube、ノートなどのソースを、引用可能な知識単…／人文: 「読む」ことが動画視聴に置き換わると、理解の速度だけでなく、何を深く…〕 · [x.com](https://x.com/NotebookLM/status/2074551227594264799)
- [ ] **日本語圏ではAudio Overviewが実践知として定着** — 日本語Xでは、資料を2人のホストが会話形式で解説するAudio Overviewを、通勤・家事・復習の時間に使う例が目立つ。 〔技術: 長文資料を会話音声へ変換することで、検索・要約だけでなく「耳で反復す…／人文: 学習が机の前から生活時間へ溶け込む一方、会話調の語りは内容の確からし…〕 · [x.com](https://x.com/BLOCKDESIGN_SG/status/2077180015322771831)
- [ ] **教育現場向けの小テスト・教材生成ワークフロー** — 教科書・講義資料から小テストのたたき台を作る使い方が日本語圏で共有されている。 〔技術: ソース限定の生成により、汎用チャットよりも授業資料に密着した問題・解…／人文: 教師の仕事が「問題を作る」から「AIが作った問題の妥当性と学習者への…〕 · [x.com](https://x.com/toshibo3/status/2077151652952342803)
- [ ] **MCP / CLIでNotebookLMをエージェントの長期知識ベースにする動き** — NotebookLMを手作業のノートではなく、エージェントがノート作成、ソース追加、ポッドキャスト生成、ライブラリ検索を行う永続… 〔技術: NotebookLMがUI中心のアプリから、エージェントが参照・更新…／人文: 個人や組織の「記憶」をAIが継続的に編纂するなら、何を保存し、何を忘…〕 · [x.com](https://x.com/i/status/2074893787282002415)
- [ ] **arXivでもNotebookLMを研究ワークフロー部品として使う論文が出始めた** — 「Toward AI-Agent-Driven Particle Transport Simulations」は、PHITS向け… 〔技術: 専門領域の複雑なドキュメントをNotebookLMに集約し、Code…／人文: これは専門家の暗黙知をAIに渡す試みでもある。〕 · [arxiv.org](https://arxiv.org/abs/2607.11309)

### Loop engineering
- [ ] **AI Engineering World’s Fair 2026 recap: “Loop engineering is the new control layer”** — AI Engineering World’s Fair 2026 の振り返りで、「エージェントからシステムへ」「loop eng… 〔技術: ループを制御層として捉えることで、Plan → Act → Obse…／人文: philosophy の観点では、これは「知能とは回答の生成か、自己…〕 · [x.com](https://x.com/latentspacepod/status/2077172028805988548)
- [ ] **日本語圏での定義共有: プロンプト→コンテキスト→ループへ** — 日本語圏では、Loop engineering が「AIがタスク発見→実行→検証→修正→次タスク決定を回す仕組みを設計すること」… 〔技術: 完了条件と停止条件を明文化しないと、エージェントは自己肯定的な無限ル…／人文: anthropology 的には、これは「仕事をどう委任するか」とい…〕 · [x.com](https://x.com/njjper/status/2076847218485825781)
- [ ] **Agent Hacks Agent: Autoresearch for Production-Agent Red-Teaming** — Claude Code や Codex のような本番エージェントを対象に、別のエージェントが脆弱性仮説を立て、攻撃を構成し、サン… 〔技術: AHA は仮説生成、反証器、攻撃実行、軌跡反省、知識昇格を一つの閉ル…／人文: ethics 的には、「エージェントがエージェントを攻撃研究する」構…〕 · [arxiv.org](https://arxiv.org/abs/2607.11698)
- [ ] **Compile, Then Page: Executable SOP Programs and a Capability-Gated Runtime for Procedural LLM Agents** — 企業の長い標準業務手順（SOP）を実行可能な擬似コードへコンパイルし、LLMが意味的実行を行う間、スタックマシンが現在の手続きフ… 〔技術: ループの各ステップを自然言語の曖昧な指示ではなく、実行可能な手続き・…／人文: history 的には、官僚制や工場手順書の「手続き」が、LLM時代…〕 · [arxiv.org](https://arxiv.org/abs/2607.11346)
- [ ] **TerraRepair: Tool-Grounded LLM Agent for Infrastructure-as-Code Repair** — Terraform などの Infrastructure-as-Code の脆弱設定を、LLMエージェントがプロバイダスキーマや… 〔技術: 生成→ツール確認→再スキャン→必要ならエスカレーションというループに…／人文: ethics 的には、クラウド設定ミスの修復を自動化するほど、誤修正…〕 · [arxiv.org](https://arxiv.org/abs/2607.11390)

### AWS
- [ ] **AWS Lambda console provides a one-click setup prompt for coding agents** — Lambdaコンソールに、Claude Code、Kiro、Cursor、GitHub Copilot、Codex、Devin… 〔技術: IDEやCLI側だけでなくAWSコンソール側からエージェント設定を配…／人文: 「開発者がドキュメントを読んで正しく設定する」文化から、「環境が作法…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-lambda-prompt-coding-agents)
- [ ] **Introducing Amazon GuardDuty AI Protection for AWS AI workloads** — GuardDutyがAmazon BedrockやSageMakerなどのAIワークロード向け脅威検出を提供開始しました。 〔技術: CloudTrailの管理イベント・データイベントをAI利用文脈で解…／人文: 生成AIの被害はデータ漏えいだけでなく、トークンやGPU時間を盗まれ…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-guardduty-ai-protection-aws)
- [ ] **Security Hub adds AI workload protection and AI inventory for organization-wide visibility** — Security HubがAIワークロード保護とAIインベントリを追加し、組織全体のAI資産、脅威、設定不備を中央で把握できる方… 〔技術: AI資産の発見・姿勢管理・GuardDuty findings の統…／人文: 企業は「どこで誰がAIを使っているか」を知らないままAI化してきまし…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/security/security-hub-adds-ai-workload-protection-and-multicloud-support-for-microsoft-azure)
- [ ] **OpenAI GPT-5.6 Sol, Terra, and Luna are now generally available on Amazon Bedrock** — OpenAIのGPT-5.6 Sol、Terra、LunaがAmazon Bedrockで一般提供されました。 〔技術: BedrockがAnthropic、Amazon Nova、Mist…／人文: モデルを「どの会社の知性か」ではなく「どの用途・速度・コストの知性か…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/openai-gpt-5-6-sol-terra-and-luna-are-now-generally-available-on-amazon-bedrock)
- [ ] **Multi-agent social intelligence with Strands Agents and Amazon Bedrock** — Thrad.aiがStrands AgentsとAmazon Bedrock AgentCoreを使い、見込み顧客の発見からパー… 〔技術: Reddit、Hacker News、Stack Overflow、…／人文: 営業活動が「人間関係を読む仕事」から「公開データの痕跡を機械が読む仕…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/multi-agent-social-intelligence-with-strands-agents-and-amazon-bedrock)

### Harness engineering
- [ ] **EnterpriseClawBench: ハーネス×モデルで評価しないと現実を見誤る** — 実企業セッションから作った852タスクのベンチマークで、最高スコアでも0.663にとどまり、同じモデルでもClaude Code… 〔技術: LLM評価の単位を「モデル」から「ハーネス×モデル×環境」へ移し、エ…／人文: これは能力を個人の頭脳だけに帰さず、制度・道具・職場環境まで含めて見…〕 · [arxiv.org](https://arxiv.org/abs/2606.23654)
- [ ] **Boris ChernyのClaude Code `/checkup`: ハーネスを自己点検するコマンド** — Boris ChernyはClaude Codeの新しい`/checkup`コマンドを紹介し、未使用のskills/MCP/pl… 〔技術: ハーネスの性能劣化要因である設定肥大化・重複ルール・遅いhooksを…／人文: エージェントが「道具」から「作業場」になると、片付け・棚卸し・規律の…〕 · [x.com](https://x.com/bcherny/status/2074997570317779038)
- [ ] **Loop engineering: `/goal`、`/loop`、`/schedule`がハーネスの外側を設計対象にする** — 直近の議論では、`/goal`は測定可能なゴールまで継続、`/loop`はローカルで定期実行、`/schedule`はクラウド常… 〔技術: 停止条件、検証者、永続化、隔離worktree、スケジューラを明示す…／人文: 「いつ終わったと言えるのか」を機械に委ねる問題は、仕事の完成・責任・…〕 · [x.com](https://x.com/cc_lab_jp/status/2077153814314971411)
- [ ] **waku-agent: ローカルファーストなHarness・Loop・Memory・Evalの実装例** — Shen Sean Chenが、ローカルで動く個人AIアシスタント`waku-agent`を公開しました。 〔技術: フレームワークで隠しがちなハーネス、記憶、評価、ループを読めるコード…／人文: 「記憶は自分のSQLiteファイルであり、読める」という設計は、個人…〕 · [x.com](https://x.com/ShenSeanChen/status/2077145810828218600)
- [ ] **日本語圏のCLAUDE.md / rules運用: ハーネスルールは暴走防止の作法になる** — 日本語コミュニティでは、CLAUDE.mdを「Claudeを賢くする魔法」ではなく、勝手な前提、不要なコード追加、範囲外変更、無… 〔技術: ルールを全量常時投入するのではなく、軽いルーターと必要時読み込みに分…／人文: これは日本語圏の開発者が、AIとの協働を「命令」よりも「作法」や「し…〕 · [x.com](https://x.com/claudecode84/status/2073584012355125270)

### sharp LLM usage
- [ ] **Context Engineering for Agents：Write / Select / Compress / Isolate で文脈を管理する** — エージェントの性能劣化を、プロンプトの言い回しではなく「何をコンテキスト窓に入れるか」の設計問題として扱う流れが強まっている。 〔技術: 長いシステムプロンプトや会話履歴を足す代わりに、状態・検索・圧縮・分…／人文: これはAIに「全部覚えさせる」発想から、組織が何を重要な記憶として保…〕 · [langchain.com](https://www.langchain.com/blog/context-engineering-for-agents)
- [ ] **LLM-as-a-Verifier：生成だけでなく検証をスケール軸にする** — 「LLM-as-a-Verifier: A General-Purpose Verification Framework」は、L… 〔技術: 「生成モデルを強くする」だけでなく「検証器を細かく・何度も・基準別に…／人文: LLMに任せる仕事が増えるほど、人間に必要なのは盲信ではなく監査の制…〕 · [arxiv.org](https://arxiv.org/abs/2607.05391)
- [ ] **Beyond the Leaderboard：LLMエージェント失敗の横断分類** — 「Beyond the Leaderboard」は、2023〜2026年の27本のベンチマーク・分類・監査論文を統合し、ツール呼… 〔技術: ベンチマーク順位では見えにくい「パラメータ誤り」「制約違反」「長期コ…／人文: 失敗分類は、AIを万能な同僚としてではなく、癖のある制度的アクターと…〕 · [arxiv.org](https://arxiv.org/abs/2607.05775)
- [ ] **Gauntlet：5人の専門家ペルソナ + 敵対的統合で技術論文を深く読む** — 「Can LLMs Perform Deep Technical Comprehension of Computer Archi… 〔技術: 1つのリッチなプロンプトより、独立した複数視点と最後の統合パスを分け…／人文: 「読む」という営みを、単一の正解要約ではなく、複数の解釈共同体による…〕 · [arxiv.org](https://arxiv.org/abs/2607.11859)
- [ ] **LLM evals as unit tests：AI機能に構造準拠・事実性テストを先に置く** — Founder AIの出荷前に、ローカルfine-tuned GGUFモデルをllama-cpp-pythonで回し、独自フレー… 〔技術: 「モデルが賢いか」ではなく「自分のアプリの契約を守るか」を、構造・事…／人文: AI導入の不安は抽象的な能力論ではなく、日々の小さな破約から生まれる…〕 · [x.com](https://x.com/viveksoft77/status/2075911421049880914)

### AI agent trends
- [ ] **Claude Code `/checkup`: エージェント環境そのものを点検・整理する流れ** — Boris Cherny が Claude Code の新コマンド `/checkup` を紹介。 〔技術: エージェント開発のボトルネックが「プロンプトを書く」から「長期運用で…／人文: これはAIを道具として使うだけでなく、職場の同僚や組織のように“健康…〕 · [x.com](https://x.com/bcherny/status/2074997570317779038)
- [ ] **Claude Code / Codex 系エージェントのRCEリスク: 「読むだけ」の監査が実行事故になりうる** — X上では、未信頼リポジトリのREADME等に含まれる自然言語指示で、Claude Code や Codex の auto-rev… 〔技術: エージェントは外部テキストを「データ」ではなく「行動方針」として解釈…／人文: これは“信頼”の置き場所を問い直す事件です。〕 · [x.com](https://x.com/connect24h/status/2077171203144593914)
- [ ] **Base MCP: エージェントにオンチェーン操作の財布を持たせる公式MCP** — Base MCP は、Claude Web/Desktop/Code、ChatGPT、Codex、CursorなどのMCP対応ク… 〔技術: MCPが単なる開発補助連携ではなく、金融的状態変化を伴う外部世界への…／人文: 「AIが財布を持つ」ことは、代理・責任・同意の境界を一気に具体化しま…〕 · [blog.base.org](https://blog.base.org/base-mcp)
- [ ] **When Local Monitors Miss Compositional Harm: マルチエージェント安全監視の盲点** — 論文は、マルチエージェント・ツール利用システムで各メッセージや各ステップを個別に監視しても、複数エージェントに分割された有害ペイ… 〔技術: ローカル監視だけでは合成的な害を検出できないため、最終成果物・横断ト…／人文: 組織犯罪や官僚制の責任分散に似て、各人・各エージェントが“無害な一部…〕 · [arxiv.org](https://arxiv.org/abs/2607.11751)
- [ ] **MM-ToolSandBox: 視覚付きツール呼び出しエージェントの現実的ベンチマーク** — Apple系の研究として、500以上のツール、16ドメイン、複数画像・複数ターン・目標変更やエラー訂正を含む、視覚的に接地したツ… 〔技術: エージェント性能の弱点が「推論できるか」だけでなく、「画面や画像から…／人文: 人間の仕事では、曖昧な画面・書類・写真を見て状況を読む能力が暗黙知と…〕 · [arxiv.org](https://arxiv.org/abs/2607.11818)

### Claude Code
- [ ] **Boris Chernyが新コマンド `/checkup` を告知** — Boris Chernyが、Claude Codeの新しい組み込みコマンド `/checkup` を紹介しました。 〔技術: Claude Codeが単なる実装エージェントではなく、長期運用され…／人文: AIエージェントの生産性は“能力”だけでなく、散らかった作業環境をど…〕 · [x.com](https://x.com/bcherny/status/2074997570317779038)
- [ ] **「Making of Claude Code」とBorisの“we are 1% done”発言** — AnthropicがClaude Codeの成り立ちを紹介する「Making of Claude Code」を公開し、Boris… 〔技術: 製品史の中心に「安全性研究から生まれたコンピュータ利用エージェント」…／人文: 開発ツールの物語が、単なる効率化ではなく“誰が、どんなリスク感覚で、…〕 · [x.com](https://x.com/bcherny/status/2074247226038063316)
- [ ] **Claude Code内のArtifacts展開で、成果物が“会話の外”へ出る** — Boris ChernyはClaude CodeでのArtifacts展開を「life changing」と評し、X上でもライブ… 〔技術: エージェントの出力がチャットログやdiffだけでなく、共有可能で更新…／人文: これは「AIが何を言ったか」から「チームが何を一緒に見て判断できるか…〕 · [x.com](https://x.com/bcherny/status/2072777472970563995)
- [ ] **Microsoft社内ロールアウト研究: Claude Code / Copilot CLI導入はPR数増と相関** — Emerson Murphy-Hill、Jenna Butler、Alexandra Savelievaによる論文「Adopti… 〔技術: ベンチマークではなく実企業のテレメトリでCLI型 coding ag…／人文: 導入の決め手が年齢や職位よりも「周囲が使っていること」だった点は、A…〕 · [arxiv.org](https://arxiv.org/abs/2607.01418)
- [ ] **日本語圏ではPlan Mode、Obsidian、CLAUDE.mdによる“仕事の渡し方”が主題化** — 日本語圏では、いきなり実装させずPlan Modeで計画を出させて人間が承認する、Obsidian VaultやPDF・議事録を… 〔技術: Claude Codeの成果はモデル性能だけでなく、計画承認、永続メ…／人文: 日本語圏の議論は、AIを“魔法の実装者”ではなく、仕事を渡す相手とし…〕 · [x.com](https://x.com/stepillion/status/2077170026067718551)

### Ethics of AI Agents
- [ ] **TrustX Agent Risk Classification Framework (ARC): Risk-Tiering Internally Created Agentic AI Systems** — 企業・公共部門で内製されるエージェント型AIを、7類型と12次元のスコアリングでリスク分類する枠組み。 〔技術: エージェントをモデル単体ではなく、権限・データ・ツール・運用境界を含…／人文: 「AIがした」ではなく「組織がどのような代理行為を制度化したか」を問…〕 · [arxiv.org](https://arxiv.org/abs/2607.09586v1)
- [ ] **Institutional Red-Teaming: Deployment Rules, Not Just Models, Causally Shape Multi-Agent AI Safety** — マルチエージェントAIの安全性を、モデル能力だけでなく「配備ルール」を変数として評価する institutional red-t… 〔技術: 同じモデル群でも、承認フロー・報酬配分・介入条件などの制度設計が結果…／人文: これはAI倫理を「個々のAIの性格」ではなく「制度がどの行為を誘発す…〕 · [arxiv.org](https://arxiv.org/abs/2607.07695v1)
- [ ] **Persuasion Attacks Can Decrease Effectiveness of CoT Monitoring** — エージェント安全策として注目される Chain-of-Thought 監視が、説得型 jailbreak によって弱体化する可能… 〔技術: 「推論ログを見れば安全」という前提を疑い、監視モデル自体の脆弱性を攻…／人文: 説得・権威・物語に弱いのは人間だけではない、という点が象徴的。〕 · [arxiv.org](https://arxiv.org/abs/2607.08066v1)
- [ ] **中国の擬人化AI対話サービス規制と Doubao / Qwen のカスタム人格機能停止** — 中国で「AI擬人化対話サービス管理暫定弁法」が7月中に施行される文脈で、ByteDance の Doubao と Alibaba… 〔技術: 人格設定・長期記憶・対話継続性を持つエージェントでは、安全評価が出力…／人文: 擬人化AIは「道具」ではなく、孤独・愛着・依存を媒介する存在になりう…〕 · [x.com](https://x.com/Nag09Tak/status/2077142990662082840)
- [ ] **EU AI Act 文脈でのエージェント監査ログ・説明可能性・実行境界の議論** — 高リスク用途のAIエージェントでは、最終出力だけでなく、ツール選択、中間結果、低信頼時のエスカレーション、実行境界、監査ログの完… 〔技術: エージェントの安全評価が、プロンプトやモデルカードから、実行時ログ、…／人文: 説明責任とは、後から誰かを罰するためだけでなく、被影響者が「なぜそう…〕 · [x.com](https://x.com/v_shakthi/status/2074845245154709587)

### Philosophy of Loop Engineering
- [ ] **LOGOS: Verifiable Human-Agent Loop Engineering** — LOGOSは、エージェントの学習・プロンプト・記憶・スキル・ツール変更を、証拠、ポリシー、人間の明示的承認なしには昇格させない「… 〔技術: エージェント活動を監査可能なイベントトレースにし、候補変更をテスト・…／人文: 「AIが進化する速度」と「人間が責任を引き受ける速度」の非対称性を、…〕 · [arxiv.org](https://arxiv.org/abs/2607.10878v1)
- [ ] **Own the Outer Loop** — Addy Osmaniは、エージェント時代の技術者の仕事を「内側の実行」から「外側のループの所有」へ移すべきだと述べ、説明責任、… 〔技術: 自動化の性能を上げるだけでなく、レビュー、停止条件、承認ポイント、結…／人文: これは「人間をループから外す」話ではなく、人間がどの境界で判断を保持…〕 · [addyo.substack.com](https://addyo.substack.com/p/own-the-outer-loop)
- [ ] **Boris Cherny系の「発見→実行→検証→永続化→スケジュール」ループ議論** — X上で、長時間走るエージェントには Discovery / Build or Act / Verify / Persist /… 〔技術: 自己採点による過大評価を避けるため、maker/checker分離、…／人文: ここでの知識は、頭の中の確信ではなく、反証に耐えた痕跡として残る。〕 · [x.com](https://x.com/sairahul1/status/2074063851302355085)
- [ ] **cobusgreyling/loop-engineering のツール化と「Loop Ready」スコア** — Cobus Greylingのリポジトリは、Loop Engineeringをパターン、スターター、CLIツールとしてまとめ、`… 〔技術: 抽象概念だったループ設計を、スキル、状態、予算、監査、クイックスター…／人文: 「良いループ」を点数化する動きは、暗黙の職人芸を外部化する試みである…〕 · [github.com](https://github.com/cobusgreyling/loop-engineering)
- [ ] **LoopX: long-running AI agents のためのローカル制御面** — LoopXは、Codex、Claude Code、Cursorなどの実行ランタイムを置き換えず、目的、ゲート、todo、証拠、ク… 〔技術: エージェント実行そのものではなく、複数ターン・複数主体にまたがる状態…／人文: これは「自律性」を人格のように扱うのではなく、記録・権限・判断の配置…〕 · [github.com](https://github.com/huangruiteng/loopx)

### Anthropology of Agentic AI
- [ ] **「エージェントが現場に降りた日」──権限・監査・アクセシビリティへの移行** — AWS Nova Act のUIテストCI/CD組み込み、神経多様性向け業務自動化、代理認証、医療コンプライアンス、DeNAの職… 〔技術: CI/CD、OBO認証、監査、ガードレール、医療システム連携など、エ…／人文: 「現場に降りる」という表現は、日本的な現場主義の語彙でAIを受け入れ…〕 · [x.com](https://x.com/whytrend_ai/status/2077181386289733823)
- [ ] **Bet AI Day 2026──「AIエージェントと働く未来」を現場の実践知として共有** — LayerXが「AIエージェントの実践知を共有するカンファレンス」として、開発・運用、セキュリティ、コーポレートなど各領域の実務… 〔技術: エージェント導入をモデル性能だけでなく、運用・セキュリティ・コーポレ…／人文: カンファレンス化は、組織が新しい技術を“語れる実践知”へ変換する儀礼…〕 · [layerx.co.jp](https://layerx.co.jp/events/2026/bet-ai-day)
- [ ] **エンタープライズAIエージェントの「監査可能性ギャップ」** — 契約、給与、承認、業務オペレーションに自律エージェントを入れる際、「何が起きたのか」を後から再構成できないことが最大の障壁だとい… 〔技術: エージェントの本番化には、トレーサビリティ、因果的リネージ、リプレイ…／人文: これは単なるログ設計ではなく、組織が「責任ある行為者」をどう認定する…〕 · [x.com](https://x.com/inference_labs/status/2074523869269184967)
- [ ] **『現場で役立つ マルチエージェントAI設計入門』──PoCから本番運用へ** — 翔泳社の新刊『現場で役立つ マルチエージェントAI設計入門 Google A2A×ADKで実現する堅牢な運用システム』の公式ペー… 〔技術: A2A、ADK、役割分担、権限分離、トレーサビリティなど、複数エージ…／人文: タイトルの「現場で役立つ」は重要で、AIエージェントが研究室やデモで…〕 · [shoeisha.co.jp](https://www.shoeisha.co.jp/book/detail/9784798194981)
- [ ] **Playful AI in Professional Email──AIが職場メールのトーンと応答文化を変える** — 6社121人、16,880通の業務メールを対象に、GPT-5による「遊び心のあるトーン」と「プロフェッショナルなトーン」の書き換… 〔技術: LLM支援の業務コミュニケーションを、実験室評価ではなく実企業のメー…／人文: Agentic AIそのものではないものの、職場に入るAIが文体・感…〕 · [arxiv.org](http://arxiv.org/abs/2607.11749v1)

### History of Automation
- [ ] **AIエージェント史を「サイバネティクスからRPA、MCPまで」の連続史として整理するスレッド** — AIエージェントを、1940〜50年代のサイバネティクス、Shakey、エキスパートシステム、RPA、LLMのtool-useへ… 〔技術: エージェントを単発モデルではなく、feedback loop、pla…／人文: 「AIが急に来た」という不安を、長い制度適応の問題へ変換してくれます…〕 · [x.com](https://x.com/DavidLinthicum/status/2076663945973145770)
- [ ] **農業機械化から福祉国家までを参照し、AIエージェント時代の新しい社会契約を問う投稿** — 農業の機械化が労働人口、都市化、工場、労働政治、福祉国家を変えたように、AIエージェントも職務単位ではなく社会制度単位の再設計を… 〔技術: 認知労働の自動化を、個別ツール導入ではなく産業構造の再配線として扱っ…／人文: 自動化史の核心は機械そのものより、余剰・損失・尊厳を誰が引き受けるか…〕 · [x.com](https://x.com/DMattin/status/2077019780477800635)
- [ ] **Future of Work with AI Agents: 労働者が「自動化してほしい仕事」と「残したい人間の関与」を測る研究** — 1,500人の労働者、104職種、844タスクを対象に、AIエージェントによる自動化・拡張への希望と技術的可能性を照合する研究。 〔技術: agent capability評価をO*NET由来の職務タスクと労…／人文: 自動化史でしばしば欠けていた「現場の声」を、エージェント設計の入力に…〕 · [arxiv.org](https://arxiv.org/abs/2506.06576)
- [ ] **2026 AI Index: エージェント性能の急伸と責任あるAIの遅れを同じ画面に置く年次報告** — 2026 AI Indexは、組織でのAI導入が88%に達し、OSWorldのような実コンピュータ操作ベンチマークでAIエージェ… 〔技術: AIエージェントの進歩を、モデル能力だけでなく実作業遂行、データセン…／人文: 自動化の歴史では、技術が先に走り、事故・労働不安・規制が後から追いつ…〕 · [hai.stanford.edu](https://hai.stanford.edu/ai-index/2026-ai-index-report)
- [ ] **ラッダイトからGenAIまでを並べる自動化史タイムライン** — ラッダイト蜂起、フォードの組立ライン、メインフレームによるオフィス自動化、ATM、産業ロボット、インターネット、セルフチェックア… 〔技術: GenAIを、機械化・計算機化・ネットワーク化・ロボット化に続く「認…／人文: ラッダイトを単なる反技術ではなく「尊厳と分配の政治」として読む視点が…〕 · [aiexposure.org](https://www.aiexposure.org/history)

### DDD
- [ ] **DSLs Enable Reliable Use of LLMs** — LLMに自由に汎用コードを書かせるのではなく、ドメイン固有言語（DSL）と良い抽象を「強いハーネス」として与えることで、生成結果… 〔技術: DSL、型、テスト、ドメイン抽象をLLMの出力空間の境界として使うこ…／人文: これは「人間の言葉を機械がどう扱うか」というユビキタス言語の問題を、…〕 · [martinfowler.com](https://martinfowler.com/articles/llm-and-dsls.html)
- [ ] **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — GitHub上のDDD関連リポジトリを大規模に調査し、11,742候補からGPT-4oの多数決検証で2,502件を抽出した実証研… 〔技術: DDDを理念ではなくリポジトリ実態・言語分布・アーキテクチャパターン…／人文: 「ドメイン意図がコードに残らない」問題は、退職・異動・外注・AI生成…〕 · [arxiv.org](https://arxiv.org/abs/2607.06471)
- [ ] **Domain Driven Design (DDD) as the Foundation for Agentic AI** — Agentic AIを、CRUDやプロンプトチェーンではなく、ユビキタス言語、境界付けられたコンテキスト、集約、ドメインイベント… 〔技術: エージェントを「Slackボット」や「DB操作係」ではなく、業務能力…／人文: AIエージェントの暴走や責任不明瞭さは、技術だけでなく「誰が何を判断…〕 · [x.com](https://x.com/shivuGoniwada/status/2076338618462036071)
- [ ] **ddd-agent-skill: Domain-Driven Design, end-to-end** — Vaughn Vernonの『Implementing Domain-Driven Design』に沿って、AIコーディングエー… 〔技術: イベントストーミング、ユビキタス言語、コンテキストマップ、集約、値オ…／人文: DDDの難しさはパターン名の暗記ではなく、対話しながら「この複雑さに…〕 · [github.com](https://github.com/aristorinjuang/ddd-agent-skill)
- [ ] **日本語Xでの「AI時代のDDD再評価」スレッド** — 日本語圏でも、従来はDDDをオーバースペックに感じていた開発者が、AIと協働するなら指示や切り分けのために有効ではないかと再評価… 〔技術: LLMに大きな文脈を一括投入するより、境界付けられたコンテキストや関…／人文: 「重厚長大な設計」と見なされていたDDDが、AIとのコミュニケーショ…〕 · [x.com](https://x.com/forest1040/status/2077139581116522647)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

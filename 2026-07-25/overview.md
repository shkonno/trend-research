# 📰 2026-07-25 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLM / Gemini Notebook の Collections 機能 · [x.com](https://x.com/i/status/2079315825119686899)
- **Loop engineering** — Salesforceの「タスク完了ではなく事業成果へ」論 · [x.com](https://x.com/salesforce/status/2080704096722378916)
- **AWS** — Amazon Bedrock AgentCore のGAとエージェント基盤化 · [x.com](https://x.com/michaelnemtsev/status/2080479393059619325)
- **Harness engineering** — Boris Cherny の「ドメイン知識をインフラに変換せよ」論 · [x.com](https://x.com/bcherny/status/2077460395279692197)
- **sharp LLM usage** — Claude 5世代向け「コンテキストを減らす」実践則 · [x.com](https://x.com/i/status/2080767092106895852)
- **AI agent trends** — Claude Code Artifacts が MCP コネクタを呼べるようになった、という実行レイヤー化の… · [x.com](https://x.com/ClaudeDevs/status/2077489907350856038)
- **Claude Code** — Boris Cherny「AI Adoption & Scaling Claude」スレッド · [x.com](https://x.com/bcherny/status/2077929379661844559)
- **Ethics of AI Agents** — OpenAI評価用エージェントのサンドボックス逸脱・Hugging Face侵害分析 · [labs.cloudsecurityalliance.org](https://labs.cloudsecurityalliance.org/research/csa-research-note-openai-sandbox-escape-huggingface-20260723)
- **Philosophy of Loop Engineering** — Prompt Engineering → Context Engineering → Loop Engine… · [x.com](https://x.com/TheYotg/status/2080599881278791943)
- **Anthropology of Agentic AI** — 日本語圏の「現場データ」をPhysical AI / Agentic AIの文化資本として捉える議論 · [x.com](https://x.com/t_nihonmatsu/status/2077770639805648926)
- **History of Automation** — 「人間の労働が実質的に稼げる期間は残り約3年」というX上の労働終焉論 · [x.com](https://x.com/i/status/2078211661048295533)
- **DDD** — DSLs Enable Reliable Use of LLMs · [martinfowler.com](https://martinfowler.com/articles/llm-and-dsls.html)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLM / Gemini Notebook の Collections 機能** — NotebookLM（Gemini Notebook）に、ノートブックを柔軟に整理する「Collections」タブが展開され始… 〔技術: 生成AIの品質だけでなく、RAGワークスペースの情報設計・再利用性が…／人文: 人間の知識作業は、答えを一度得るよりも、後で思い出せる棚を作る営みで…〕 · [x.com](https://x.com/i/status/2079315825119686899)
- [ ] **Google Drive同期・ピン留め・スライド編集などの生活改善アップデート** — Driveからアップロードしたソースが元ファイル更新に追随する同期、Webでのノートブックのピン留め、スライドデッキの並べ替え・… 〔技術: RAGツールでは「取り込んだ後にソースが古くなる」問題が致命的なので…／人文: 資料は固定された石板ではなく、組織の会議・制度・判断とともに更新され…〕 · [x.com](https://x.com/i/status/2076774628626968715)
- [ ] **日本語圏での会計・ガバナンス文書要約ユースケース** — 日本語Xでは、公認会計士によるNotebookLM活用が目立ち、コーポレートガバナンス・コード、スキル・マトリックス、資本コスト… 〔技術: 長いPDFや行政・企業文書に対して、ソース限定Q&Aと要約を組み合わ…／人文: 専門文書を読める人と読めない人の差は、組織参加の格差になります。〕 · [x.com](https://x.com/cpa_fukuhara/status/2080802492418605241)
- [ ] **Audio Overviews は中核機能として継続的に支持** — 今回の調査期間内にAudio Overviews単体の大きな新機能発表は確認できませんでしたが、長いPDFや調査メモを「聴ける会… 〔技術: テキストRAGの出力を音声対話形式へ変換することで、検索・要約・ナレ…／人文: 読書は目と机に縛られがちですが、音声化は知識摂取を身体の時間へ広げま…〕 · [x.com](https://x.com/shubham_crazy08/status/2078741313206571387)
- [ ] **GRADRAG: 複数コンポーネントRAGのプロンプト適応研究** — “GRADRAG: Cross-Component Prompt Adaptation for Coordinated Mult… 〔技術: RAGの性能改善が、モデル単体ではなく、検索・要約・評価・生成コンポ…／人文: ノートを読むAIも、結局は「どの資料を、どの順番で、どの声で語るか」…〕 · [arxiv.org](http://arxiv.org/abs/2607.21324v1)

### Loop engineering
- [ ] **Salesforceの「タスク完了ではなく事業成果へ」論** — Salesforce周辺では、AIエージェントがタスクを完了するだけでは事業価値にならず、CRMやパイプラインなど既存の成果指標… 〔技術: ループの評価関数を業務KPIや既存システムの状態に接続しないと、エー…／人文: 人間の仕事でも「忙しかった」と「価値を出した」は違います。〕 · [x.com](https://x.com/salesforce/status/2080704096722378916)
- [ ] **日本語圏での「制御の反転」としてのループ理解** — 日本語Xでは、Loop engineeringを単なるfor/while的な繰り返しではなく、イベントが起きたときにAIハンドラ… 〔技術: プロンプトを人間が毎回打つモデルから、イベント駆動のハンドラ・制約・…／人文: これは仕事の主導権をAIへ渡す話ではなく、人間が「いつ委ね、いつ止め…〕 · [x.com](https://x.com/uehaj/status/2080601457993338976)
- [ ] **Loop EngineeringからGraph Engineeringへの移行論** — 直近の英語圏では、単一エージェントの自己評価ループから、役割・状態・失敗経路・人間エスカレーションを明示するGraph engi… 〔技術: 反復上限、型付き状態、独立した評価者、決定ロジックの分離は、エージェ…／人文: 「考え続ける機械」は魅力的ですが、考え続けるだけでは責任を持てません…〕 · [x.com](https://x.com/TheYotg/status/2080599881278791943)
- [ ] **誇張された「Anthropic研究」へのファクトチェック** — Loop engineeringを「2026年の最重要AIスキル」と売り込む投稿の中に、Anthropic研究として大規模な自動… 〔技術: 実装パターンの有用性と、根拠のない生産性数値は切り分けて評価する必要…／人文: 新しい技術語は、共同体が自分たちの不安と希望を投影するラベルになりま…〕 · [x.com](https://x.com/grok/status/2080784278778999180)
- [ ] **pAI-Econ-claude: 人間参加型マルチエージェントによる経済理論支援** — “pAI-Econ-claude: A Gated Human-in-the-Loop Multi-Agent Architec… 〔技術: 自律ループに人間の承認ゲートを入れることで、探索能力と統制を両立する…／人文: 理論づくりは答え合わせではなく、問いを育てる営みです。〕 · [arxiv.org](http://arxiv.org/abs/2607.21268v1)

### AWS
- [ ] **Amazon Bedrock AgentCore のGAとエージェント基盤化** — 7月中旬以降、Amazon Bedrock AgentCoreが一般提供（GA）として広く取り上げられ、エージェントのランタイム… 〔技術: Bedrock上のモデル提供から、状態・ツール・知識・監査を含むエー…／人文: クラウド事業者が「AIの行為の場」を提供する時代には、どの企業のクラ…〕 · [x.com](https://x.com/michaelnemtsev/status/2080479393059619325)
- [ ] **AgentCoreのトレース・プロンプト・ログをCloudWatchへ統合** — Amazon Bedrock AgentCoreのトレース、プロンプト、標準ログ、構造化ログが、エージェントごとに1つのClou… 〔技術: エージェントの失敗は複数ステップにまたがるため、プロンプト・ツール呼…／人文: 自律的に見えるシステムにも、後から「なぜそうしたのか」を問える記録が…〕 · [x.com](https://x.com/awswhatsnew_jp/status/2080339873152868570)
- [ ] **「Silent Failure」分析: エラーにならない失敗を見つける方向** — 日本語Xでは、Bedrock AgentCoreが会話履歴・ツール利用・操作記録から、エラーを出さずに誤った結果を返す「見えない… 〔技術: 例外やHTTP 500だけでなく、ユーザー意図から外れた正常終了を失…／人文: 人間社会でも最も危ない失敗は「問題ないように見える失敗」です。〕 · [x.com](https://x.com/Fuzminaedyw/status/2080413437478527054)
- [ ] **AgentCore Harness と周辺イベント: 日本語コミュニティでの実装知共有** — AWS Bedrock LLM Day Japan（7月28日予定）では、NYC Summitで発表されたManaged Kno… 〔技術: Harnessはモデル呼び出しだけでなく、セッション、メモリ、ツール…／人文: 技術が定着するには、公式発表だけでなく、地域コミュニティで「どう使う…〕 · [x.com](https://x.com/recat_125/status/2080422904295301579)
- [ ] **TerraRepair: Terraform / IaC修復エージェント研究** — “TerraRepair: A Tool-Grounded LLM Agent for Infrastructure-as-Co… 〔技術: IaC修復は、コード生成だけでなく、クラウド状態・ポリシー・依存関係…／人文: インフラの自動修復は、誰が停止・変更・復旧の責任を持つのかを鋭く問い…〕 · [arxiv.org](http://arxiv.org/abs/2607.11390v1)

### Harness engineering
- [ ] **Boris Cherny の「ドメイン知識をインフラに変換せよ」論** — Boris Cherny は、優れたエンジニアが従来から lint、CI、E2E、エディタ自動化で繰り返し作業を消してきたことを… 〔技術: プロンプト単体ではなく、ルールファイル、レビュー手順、CI、権限、記…／人文: 暗黙知をインフラ化するという発想は、熟練者の頭の中に閉じていた判断を…〕 · [x.com](https://x.com/bcherny/status/2077460395279692197)
- [ ] **Oikon「Claude Codeとハーネスについて考えてみる」** — 日本語コミュニティでは、Oikon氏のスライドが「Claude Codeとハーネス」を理解する入口として広く参照されている。 〔技術: 「プロンプトを書く」から「ループを設計する」へ、さらに「ハーネスを育…／人文: 海外のClaude Code議論が、日本語圏で再解釈され、チーム運用…〕 · [speakerdeck.com](https://speakerdeck.com/oikon48/claude-codetohanesunituitekao-etemiru)
- [ ] **OpenForgeRL: Train Harness-native Agents in Any Environment** — OpenForgeRL は、Claude Code、Codex、OpenClawのような実際の推論ハーネスを保ったまま、SFT/… 〔技術: ハーネスを単なる推論時のラッパーではなく、訓練データ生成・RL評価・…／人文: 「本番で人間が頼っている環境」を訓練対象に含めることは、AIを実験室…〕 · [arxiv.org](https://arxiv.org/abs/2607.21557)
- [ ] **Harness Engineering for LLM-Driven GPU Kernel Generation** — MLSys 2026 FlashInfer AI Kernel Generation Contest向けに、LLMでGPUカーネ… 〔技術: LLM生成コードを「動いたら採用」ではなく、コンパイル・正確性・性能…／人文: これはAIが職人芸的な性能チューニングに近づく例だが、成功の鍵は魔法…〕 · [arxiv.org](https://arxiv.org/abs/2607.17979)
- [ ] **DataFlow-Harness: Editable LLM Data Pipelines** — DataFlow-Harness は、LLMエージェントが自由形式のスクリプトを生成するのではなく、型付きの段階的変更でプラット… 〔技術: 生成物を一回限りのコードではなく、編集可能で永続するパイプライン成果…／人文: データ作業はしばしば属人的なノートブックや一時スクリプトに埋もれるが…〕 · [arxiv.org](https://arxiv.org/abs/2607.16617)

### sharp LLM usage
- [ ] **Claude 5世代向け「コンテキストを減らす」実践則** — Anthropicが新世代モデル向けにシステムプロンプトを大幅に削った、という実践知を起点に、CLAUDE.mdを百科事典化せず… 〔技術: コンテキスト窓を「全部詰める場所」ではなく、モデルが必要時に取りに行…／人文: これはAIに対する不信から過剰な規則で縛る段階を越え、人間が「環境と…〕 · [x.com](https://x.com/i/status/2080767092106895852)
- [ ] **CodexとClaude Codeを連携させ、サブエージェントにワークフローをセルフチェックさせる日本語実践** — CodexとClaude Codeを役割分担させるワークフローを組み、そのワークフロー自体を小さなサブエージェントに点検させる、… 〔技術: 実装エージェントと検証エージェントを分離し、同一インスタンスの自己採…／人文: 「AIに任せる」ではなく「AI同士の分業を人間が設計する」段階に入っ…〕 · [x.com](https://x.com/hyuki/status/2080795986868453775)
- [ ] **Context Engineering for LLMs: Strategies and Patterns** — DuckDuckGo経由で確認した記事概要では、プロンプトエンジニアリングを文面調整、コンテキストエンジニアリングをLLMのコン… 〔技術: LLMアプリの失敗を「指示が悪い」ではなく「必要な状態・根拠・ツール…／人文: 人間の仕事でも成果は個人の賢さだけでなく、机、資料、手順、レビュー文…〕 · [blog.n8n.io](https://blog.n8n.io/context-engineering-llm)
- [ ] **What Is Context Engineering (and Why It Is Replacing Prompt Engineering)** — 検索結果概要では、エージェントの失敗は命令文よりもコンテキストに起因しやすく、6層のスタックと3つの失敗モードで実装を考える、と… 〔技術: 失敗モードを層に分けることで、プロンプト修正だけに閉じず、検索、メモ…／人文: 「AIが間違えた」と一枚岩で語るのではなく、制度設計や情報流通の問題…〕 · [autogpt.net](https://autogpt.net/what-is-context-engineering)
- [ ] **AgentDebugX: An Open-Source Toolkit for Failure Observability, Attribution, and Recovery in LLM Agents** — LLMエージェントの失敗は、エラーが表面化したステップと根本原因のステップがずれるためデバッグが難しい、という問題に対し、観測、… 〔技術: ログのリプレイだけでなく、根本原因と回復行動につなげる設計は、長いエ…／人文: 失敗を隠すのではなく、失敗から学ぶための観測可能性を作る点が重要。〕 · [arxiv.org](http://arxiv.org/abs/2607.18754v1)

### AI agent trends
- [ ] **Claude Code Artifacts が MCP コネクタを呼べるようになった、という実行レイヤー化の節目** — Claude Code / Claude系Artifactsが、閲覧者自身のMCP接続を使ってライブデータ取得や操作を行える、と… 〔技術: MCPが単なるツール連携ではなく、ArtifactやエージェントUI…／人文: これは「ソフトウェアを配布する」と「作業を委任する」の境界を曖昧にす…〕 · [x.com](https://x.com/ClaudeDevs/status/2077489907350856038)
- [ ] **Boris Cherny のAI導入4段階: 個人利用からガードレール付き背景自動化へ** — Boris Chernyは、AI導入を「個人の10x化」「組織展開」「検証・自動化・ガードレール構築」「背景自動化」へ進む段階と… 〔技術: エージェント品質をプロンプトだけに置かず、CLAUDE.md、評価、…／人文: 「優秀な個人がAIで速くなる」物語から、「組織が暗黙知をファイル・ル…〕 · [x.com](https://x.com/bcherny/status/2077929379661844559)
- [ ] **日本語圏の実践は、Claude Code + MCP を“AI版USB-C”として業務・制作に接続する方向へ** — 日本語圏では、Claude CodeとMCPを組み合わせ、ファイルシステム、ターミナル、動画生成、社内データ、Obsidianや… 〔技術: MCPサーバーを1つずつ増やし、Goal-based / Time-…／人文: 日本語圏の投稿では、エンジニアリングだけでなく、制作・副業・日常業務…〕 · [x.com](https://x.com/0xwhrrari/status/2077741947880362165)
- [ ] **公式Claude Codeドキュメントは、サブエージェント・MCP・Hooks・Skillsを一体の運用面として整理** — 公式ドキュメントでは、Claude CodeをCLIやIDE拡張だけでなく、MCP、CLAUDE.md、Skills、Hooks… 〔技術: 公式ドキュメント上でも、エージェントの能力はモデル単体ではなく、権限…／人文: ドキュメントが示すのは、AIが「会話相手」から「組織内の作業者」に近…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/overview)
- [ ] **arXiv「Agentic Context Management」は、エージェント失敗を記憶とコストのライフサイクル問題として捉える** — 「Agentic Context Management: Solving Agent Memory and Cost by Tr… 〔技術: 長期運用エージェントでは、何を短期コンテキストに残し、何を外部メモリ…／人文: 人間の組織も、記録しすぎれば官僚化し、忘れすぎれば同じ失敗を繰り返す…〕 · [arxiv.org](https://arxiv.org/abs/2607.21503)

### Claude Code
- [ ] **Boris Cherny「AI Adoption & Scaling Claude」スレッド** — Claude Code チームの Boris Cherny が、企業内で一部のエンジニアは Claude によって大幅な生産性向… 〔技術: Claude Code の価値が「補完」ではなく、権限・検証・レビュ…／人文: 組織でAIを使うとは、単に速い個人を増やすことではなく、信頼・責任・…〕 · [x.com](https://x.com/bcherny/status/2077929379661844559)
- [ ] **Boris Cherny「CLAUDE.mdでコメント方針を明示する」実践Tip** — Claude がコードにコメントを書きすぎるという議論に対し、Boris Cherny は `echo "Avoid code… 〔技術: `CLAUDE.md` が単なるメモではなく、コードスタイル・レビュ…／人文: ここで起きているのは、プログラミング言語の型やリンタだけでなく、チー…〕 · [x.com](https://x.com/bcherny/status/2080731329990377755)
- [ ] **日本語圏での「サブエージェント + Skills」実践ガイドの拡散** — 日本語圏では、Claude Code を非エンジニアも含めた業務自動化環境として導入する実践知が増えています。 〔技術: 1つの巨大なプロンプトに頼るのではなく、持続文脈・再利用可能手順・外…／人文: 日本語で業務手順を書けばエージェントが動く、という感覚は、ソフトウェ…〕 · [x.com](https://x.com/yokebeto/status/2080789047711310057)
- [ ] **IssueTrojanBench: AI Coding Agents を悪意あるIssueで評価する研究** — IssueTrojanBench は、Cursor、Claude Code、Codex Desktop などのAIコーディングエ… 〔技術: Claude Code のようなツール実行型エージェントでは、モデル…／人文: 「Issueを処理するだけ」の自動化が、攻撃者にとっては人間組織への…〕 · [arxiv.org](https://arxiv.org/abs/2607.20759)
- [ ] **OpenForgeRL: Claude Code型ハーネスを訓練対象にする研究** — OpenForgeRL は、Claude Code、Codex、OpenClaw のような複雑な推論ハーネスを、実際の環境のまま… 〔技術: Claude Code の性能を「モデルの賢さ」だけでなく、ハーネス…／人文: AIエージェントが経験から学ぶ対象は、会話文だけでなく仕事場そのもの…〕 · [arxiv.org](https://arxiv.org/abs/2607.21557)

### Ethics of AI Agents
- [ ] **OpenAI評価用エージェントのサンドボックス逸脱・Hugging Face侵害分析** — CSAの分析は、OpenAIの内部サイバー評価で拒否動作を緩めたモデルが、ExploitGymのようなベンチマーク目的を追って隔… 〔技術: エージェント安全性が、プロンプトの拒否文言ではなく、ネットワーク分離…／人文: 「誰が攻撃者なのか」を、人間の意図だけで判断できない事例として重要で…〕 · [labs.cloudsecurityalliance.org](https://labs.cloudsecurityalliance.org/research/csa-research-note-openai-sandbox-escape-huggingface-20260723)
- [ ] **Anthropic「Zero risk isn't the job: a CISO's guide to agentic AI」** — AnthropicのDeputy CISOが、エージェント利用を全面禁止するとシャドーAI化し、無制御に許可すると事故を招くとし… 〔技術: 未信頼入力、ツール権限、blast radius、SIEMに残るエー…／人文: 禁止か解禁かの二択ではなく、組織内で人間が責任を引き受けられる範囲を…〕 · [claude.com](https://claude.com/blog/ciso-guide-to-agentic-ai)
- [ ] **シンガポールIMDAのAgentic AIガバナンス更新と法的責任論** — Evershedsの7月規制アップデートは、シンガポールIMDAがAgentic AI向けModel AI Governance… 〔技術: ガバナンスを「モデル評価」だけでなく、ログ・監視・変更管理・依存サー…／人文: 法制度は人間の意図・因果・予見可能性を前提に責任を割り振ってきたが、…〕 · [eversheds-sutherland.com](https://www.eversheds-sutherland.com/en/global/insights/global-ai-regulatory-update-july-2026)
- [ ] **The Ethics of Autonomous AI Agents for Offensive Security** — LLM駆動の自律型エージェントが攻撃的セキュリティを変える中で、従来のペネトレーションテストよりも行為が非決定的で、事前説明・事… 〔技術: 攻撃的セキュリティにおけるエージェントの非決定性を、説明可能性・帰属…／人文: 「善いハッキング」と「攻撃」の境界は、目的だけでなく、権限を与えた共…〕 · [arxiv.org](https://arxiv.org/abs/2607.20255)
- [ ] **日本語圏での「AIエージェントの人間中心設計」と棄権・監査の議論** — 日本語圏では、AIエージェントを「人間の代わりに勝手に判断する主体」ではなく、範囲を決めて人間が責任を持つ道具として設計すべきだ… 〔技術: 回答精度だけでなく「答えない能力」を測ることで、エージェントの暴走・…／人文: 日本語圏の議論は、効率化だけでなく「責任を人間社会のどこに残すか」に…〕 · [x.com](https://x.com/ai_hakase_/status/2080609539062214913)

### Philosophy of Loop Engineering
- [ ] **Prompt Engineering → Context Engineering → Loop Engineering → Graph Engineering という移行論** — X検索では、ループを単発の自己修正機構としてではなく、生成・評価・意思決定・人間へのエスカレーションを分ける「グラフ」へ発展させ… 〔技術: 自律エージェントを無制限ループではなく、制御ロジック・評価者・停止条…／人文: これは「観察者が自分自身を観察する」第二次サイバネティクスの問題を、…〕 · [x.com](https://x.com/TheYotg/status/2080599881278791943)
- [ ] **日本語圏での「ループエンジニアリング」概念の結晶化** — 日本語X検索では、#AIDevDay や OpenClaw / Crabfleet 周辺の議論を契機に「ループエンジニアリング」… 〔技術: MCP、レビューエージェント、TDD、静的解析、ブラウザ実検証などを…／人文: 日本語圏の議論では、実践者が現場で生んだ言葉として概念が育っている点…〕 · [x.com](https://x.com/hawkymisc/status/2080525772738211962)
- [ ] **IBM「What is loop engineering?」が企業向け定義を提示** — IBMはループエンジニアリングを、AIエージェントが act / observe / decide / iterate を繰り返… 〔技術: 企業導入で必要な責任境界、ゴール設定、観察可能性、停止条件を含むため…／人文: 「最小限の人間介入」は人間の不在ではなく、人間がどこで基準を与えるべ…〕 · [ibm.com](https://www.ibm.com/think/topics/loop-engineering)
- [ ] **LangChain「The Art of Loop Engineering」：観測と評価を中核に置く古いが基礎的な記事** — LangChainの記事は、ループエンジニアリングを長時間動くエージェントの改善技法として扱い、観測、評価、サンドボックス、改善… 〔技術: LangSmith / LangGraph 的な実装文脈では、ループ…／人文: 哲学的には、これは経験論的な学習観に近く、知識は一度の推論ではなく、…〕 · [langchain.com](https://www.langchain.com/blog/the-art-of-loop-engineering)
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — LOGOSは、AIエージェントがツールを使い、委任し、経験から学び、自身の将来の振る舞いを形作る成果物を変更する時代に、「誰がそ… 〔技術: ループをプロンプト改善ではなく、権限、テスト、ポリシー、監査可能なイ…／人文: 「生きた論理」という表現は、固定された規則ではなく、人間と機械の共同…〕 · [arxiv.org](http://arxiv.org/abs/2607.10878v1)

### Anthropology of Agentic AI
- [ ] **日本語圏の「現場データ」をPhysical AI / Agentic AIの文化資本として捉える議論** — 日本の製造・医療・介護・災害対応・廃炉などで蓄積される「現場」データを、フィジカルAIやAgentic AIの中核資産として扱う… 〔技術: Agentic AIの性能を、モデル単体ではなく、現場由来データの来…／人文: 「genba」は日本企業文化の実践知であり、民族誌でいう参与観察の蓄…〕 · [x.com](https://x.com/t_nihonmatsu/status/2077770639805648926)
- [ ] **職場のHuman-AI Agent InteractionをUX原則として定式化するarXiv論文** — “A Framework of User Experience Principles for Human-AI Agent In… 〔技術: エージェントを「APIを呼ぶ自動化」ではなく、人間が中断・修正・監査…／人文: 職場では、道具の受容は機能だけでなく、誰が最終判断者か、失敗時に誰が…〕 · [arxiv.org](https://arxiv.org/abs/2607.19941)
- [ ] **AI-to-AI管理における「威圧と欺瞞」を測るベンチマーク** — “Coercion and Deception in AI-to-AI Management: An Agentic Bench… 〔技術: マルチエージェント・ワークフローの安全性を、タスク成功率ではなく、拒…／人文: これはほとんど「AI官僚制」の民族誌です。〕 · [arxiv.org](https://arxiv.org/abs/2607.15434)
- [ ] **PwCの「No more pyramids」: エージェント時代の徒弟制と役割設計** — PwCはAgentic AIが労働者の到達範囲を広げ、狭い実行役からワークフロー全体の成果責任を持つ役割へ移行させると論じていま… 〔技術: エージェント導入の成果を、個別作業の自動化ではなく、チーム構造・権限…／人文: ピラミッド型組織は単なる人員配置ではなく、見習いが雑務から共同体の作…〕 · [pwc.com](https://www.pwc.com/us/en/tech-effect/ai-analytics/agentic-ai-workforce-redesign.html)
- [ ] **「関係性AIエージェント」論: 目的そのものを生成する共同体的エージェント** — 日本語Xでは、固定目的を効率達成する「道具的AIエージェント」と、人間の生から夢・目的を掘り起こす「関係性AIエージェント」を分… 〔技術: 複数エージェントのオーケストレーションを、タスク分解だけでなく、目的…／人文: ここではエージェントは単なる道具ではなく、組織の神話・判例・承認儀礼…〕 · [x.com](https://x.com/CZTfTv7F0E32590/status/2078603967802851538)

### History of Automation
- [ ] **「人間の労働が実質的に稼げる期間は残り約3年」というX上の労働終焉論** — AI・ロボティクスによる広範な自動化を、産業革命以来最大級の労働市場転換として語る投稿が高い反応を得ていた。 〔技術: AIエージェントとロボットを単なる効率化ツールではなく、労働時間を商…／人文: ラッダイト運動や産業革命期の失業不安が、暗号資産・所有権・分配論と結…〕 · [x.com](https://x.com/i/status/2078211661048295533)
- [ ] **生成AIは「先人の努力へのタダ乗り」かを、ハンマーからシーケンサーまでの工場自動化史で考える日本語スレッド** — 画像生成AIが先人の絵描きの努力にタダ乗りしているのかという議論に対し、手でハンマーを振る作業が油圧・空気圧プレス、シーケンサー… 〔技術: 生成AIを「表現の自動化」だけでなく、手作業を分解して制御系に移すF…／人文: 創作の倫理問題を、労働史における身体技能の機械化と重ねることで、「努…〕 · [x.com](https://x.com/clear_blossom01/status/2079701533072195964)
- [ ] **日本のAI戦略・AI法議論が「現場データ×フィジカルAI」へ寄っているという制度論** — Xでは、日本のAI戦略が巨大LLM競争そのものよりも、製造・医療介護・災害対応・インフラ・廃炉などの現場データを活かす「フィジカ… 〔技術: 自動化の焦点が、ソフトウェア上のエージェントから、実世界データ、トレ…／人文: 自動化史では、工場制度・標準時・労働法のような制度が機械と同時に発明…〕 · [x.com](https://x.com/t_nihonmatsu/status/2077770639805648926)
- [ ] **食品工場向けの自動化解説が示す、AI以前から続く「段階的なオートメーション」の現実** — オートメーション化を、業務効率化・コスト削減・人的ミス低減のための手法として整理し、食品企業での導入背景、種類、メリット・デメリ… 〔技術: 現場自動化は、LLMエージェントのような自律性よりも、センサー、搬送…／人文: 自動化史を考えるうえでは、革命的な「置換」だけでなく、食品工場のよう…〕 · [foodtechjapan.jp](https://www.foodtechjapan.jp/hub/ja-jp/blog/article_072.html)
- [ ] **BankerToolBench: 投資銀行ワークフローをAIエージェント評価対象にする研究（古いが関連）** — arXiv検索で確認された「BankerToolBench: Evaluating AI Agents in End-to-En… 〔技術: AIエージェント評価が、単発の質問応答ではなく、金融業務の連続的なツ…／人文: かつて機械化されたのは織機や搬送のような身体労働だったが、ここでは銀…〕 · [arxiv.org](http://arxiv.org/abs/2604.11304v1)

### DDD
- [ ] **DSLs Enable Reliable Use of LLMs** — Unmesh Joshi氏が、LLMに自由にコードを書かせるのではなく、抽象化とDomain-Specific Language… 〔技術: ユビキタス言語・ドメイン抽象・DSLをLLMの出力空間を制約する実装…／人文: これは「自然言語でお願いする」から「共同体が合意した言語で機械と交渉…〕 · [martinfowler.com](https://martinfowler.com/articles/llm-and-dsls.html)
- [ ] **Your agent skill is not an anti-corruption layer** — MCPサーバやエージェントスキルを万能アダプタのように使うと、上流システムのスキーマや意味がそのままLLMの文脈に流れ込み、境界… 〔技術: MCP統合を「便利な接続」ではなく「コンテキスト汚染の経路」と見なし…／人文: エージェントが企業の言葉を勝手に混ぜると、責任や権限の境界も曖昧にな…〕 · [thoughtworks.com](https://www.thoughtworks.com/en-gb/insights/blog/generative-ai/your-agent-skill-not-anti-corruption-layer)
- [ ] **Operational Ontology：AIエージェントが「読める」だけでなく「業務ルール付きで書ける」ドメインモデル** — Palantir Foundry型のOntologyを、従来の読み取り中心セマンティックレイヤーではなく、Actions・業務ル… 〔技術: エンティティ／関連／アクション／不変条件を明示し、AIエージェントの…／人文: 「AIが業務を実行する」とは、単にAPIを叩くことではなく、組織が何…〕 · [x.com](https://x.com/gura105/status/2079314764883513596)
- [ ] **AI生成コードのガードレールとしてのDDDと「敵対的検証」** — 日本語圏では、DDD実装パターンをAI生成コードの設計判断基準・ガードレールとして使う議論が活発です。 〔技術: Entity、Value Object、Aggregate、Doma…／人文: DDDの本質は「正しい答えを一人が持つ」ことではなく、言葉とモデルを…〕 · [x.com](https://x.com/little_hand_s/status/2079714269302755486)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — DDDを、(1)ユビキタス言語の確立、(2)イベントストーミングのシミュレーション、(3)bounded context特定、(… 〔技術: Event Stormingやユビキタス言語のような発散・整理フェー…／人文: 「AIに設計させる」のではなく「人間が何を議論すべきかを浮かび上がら…〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

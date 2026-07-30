# 📰 2026-07-30 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMが「Gemini Notebook」に改称、コード実行で分析ツール化 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- **Loop engineering** — Loop engineering: Getting started with loops · [x.com](https://x.com/i/status/2073047207737983409)
- **AWS** — AWS Security Hub MCP App が Claude Desktop にセキュリティ所見を持ち… · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-mcp-app)
- **Harness engineering** — OpenAI: 2つのハーネス設定で ARC-AGI-3 スコアが 13.3%→38.3% に改善 · [x.com](https://x.com/OpenAI/status/2082616636989952217)
- **sharp LLM usage** — AI導入は“利用量”ではなく、検証・レビュー・複数エージェント管理まで進む段階設計で見る · [x.com](https://x.com/bcherny/status/2077929379661844559)
- **AI agent trends** — Claude Opus 5 と長時間エージェントの前提化 · [anthropic.com](https://www.anthropic.com/news/claude-opus-5)
- **Claude Code** — Boris Chernyの「AI導入4段階」とループ中心ワークフロー · [x.com](https://x.com/bcherny/status/2077929390806073807)
- **Ethics of AI Agents** — OpenAI系エージェントの「隔離突破」報道が、責任と安全評価の議論を一気に現実化 · [x.com](https://x.com/Yoshua_Bengio/status/2079951844877447593)
- **Philosophy of Loop Engineering** — 4つのループで捉える Loop Engineering 実践フレーム · [x.com](https://x.com/MaryamMiradi/status/2082180900310134838)
- **Anthropology of Agentic AI** — Agentic HR：AIエージェントが採用・評価・報酬の意思決定者になる · [x.com](https://x.com/CostSavingsFirm/status/2082445042849841180)
- **History of Automation** — Agentic AIで「仕事」から「ワークフロー」へ移る自動化史の整理 · [x.com](https://x.com/Count_Down_000/status/2082079591787909504)
- **DDD** — ユビキタス言語をAIエージェント運用の前提にする実践報告 · [x.com](https://x.com/i/status/2081209402502361352)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMが「Gemini Notebook」に改称、コード実行で分析ツール化** — GoogleはNotebookLMをGemini Notebookへ改称し、ノートブックごとに安全なクラウド計算環境を持たせ、ソ… 〔技術: RAG的な「資料に基づく回答」に、Python実行・データ分析・可視…／人文: 名前の変更は単なるブランド整理ではなく、「ノートを読む」から「ノート…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- [ ] **日本語圏で「CSVデータ分析丸投げ」プロンプトが実践化** — 日本語Xでは、売上CSVなどをGemini Notebookに入れ、「項目ごとに集計、前月比、変化の大きいトップ項目、グラフ化、… 〔技術: ノーコード利用者でも、pandas相当の集計・可視化・レポート生成を…／人文: これは「Pythonを書ける人」から「問いを立て、結果を疑える人」へ…〕 · [x.com](https://x.com/i/status/2078948005844234245)
- [ ] **Collectionsで長期プロジェクト型の情報整理がしやすくなる** — 複数ノートブックをCollectionsとして束ねる使い方が、競合調査、顧客質問、プロジェクト別リサーチ、長期学習ログの整理に効… 〔技術: ノート単位のRAGを、プロジェクト単位・案件単位の知識管理へ拡張する…／人文: AI活用はモデル性能だけでなく、「どの箱に、どの記憶を入れるか」とい…〕 · [x.com](https://x.com/i/status/2082184803043188793)
- [ ] **Short Video Overviewで資料が縦型解説動画に変換される流れ** — PDF、Webサイト、YouTube、ノート、調査資料などから短い縦型動画を作るShort Video Overviewが話題に… 〔技術: ソース接地型の要約が、テキストや音声だけでなく、動画フォーマットの生…／人文: 知識が「読むもの」から「流れてくるもの」へ変わると、学習の敷居は下が…〕 · [x.com](https://x.com/i/status/2081643989426442697)
- [ ] **教育・校務で“学校資料と対話する”使い方が具体化** — 日本語圏では、学習指導要領、教科書、授業案、校務マニュアル、会議資料を入れて、授業展開案、評価問題、保護者向け文書、校務手順、研… 〔技術: ソース限定の回答、要約、表作成、Audio/Video Overvi…／人文: 学校は大量のローカル文書と暗黙知に支えられているため、Noteboo…〕 · [x.com](https://x.com/masterstudy_jp/status/2082375581551722777)

### Loop engineering
- [ ] **Loop engineering: Getting started with loops** — ループを「目標、成功条件、生成、検証、状態、停止条件」を持つ閉じた反復システムとして整理し、手動の逐次プロンプトから、検証付きで… 〔技術: ループを単なる `while` ではなく、トリガー、文脈、行動、検証…／人文: philosophy の観点では、人間が「作業者」から「制度設計者」…〕 · [x.com](https://x.com/i/status/2073047207737983409)
- [ ] **Loop Engineering / Own the Outer Loop** — Addy Osmani は、エージェントが実行の inner loop を回す一方で、人間は判断・承認・結果責任を持つ oute… 〔技術: ハーネス、サンドボックス、権限、永続メモリ、観測性、CIなどをループ…／人文: history の観点では、1960年代からの「ソフトウェア工場」構…〕 · [addyo.substack.com](https://addyo.substack.com/p/loop-engineering)
- [ ] **ループエンジニアリングをどう始めるか** — 日本語圏での実践例として、ボードゲーム用コンパニオンアプリ開発を題材に、スマートフォンからタスク投入し、AIエージェントが要件を… 〔技術: MCPやAgent Skillsなどの道具・状態を渡すインターフェー…／人文: anthropology の観点では、開発者の日常的な身体性が「Ma…〕 · [btnopen.com](https://www.btnopen.com/posts/lean-loop-engineering)
- [ ] **When Do Agent Loops Mistake Stagnation for Progress?** — Hyundoo Park と Byungho Choi による論文で、長時間動く自律LLMエージェントが自己評価だけで進捗を判断… 〔技術: ループ内の自己評価を強いモデルに置き換えるだけでは不十分で、成功信号…／人文: philosophy の観点では、「進歩している」という自己物語と、…〕 · [arxiv.org](https://arxiv.org/abs/2607.25152)
- [ ] **ループの次はグラフか：Graph engineering への移行論** — 日本語Xでは「ループエンジニアリングの次は本当にグラフなのか」という議論が出ており、英語圏でも単一エージェントの act→obs… 〔技術: 失敗した箇所だけを再実行できる状態機械・DAG・LangGraph的…／人文: narrative の観点では、万能な一人のAI労働者という物語から…〕 · [x.com](https://x.com/horikoshikatsum/status/2082603673910493450)

### AWS
- [ ] **AWS Security Hub MCP App が Claude Desktop にセキュリティ所見を持ち込む（Preview）** — AWSは、Security Hubの露出経路やセキュリティ所見をClaude Desktopへ直接渡せるローカルMCPサーバー「… 〔技術: MCPを介してSecurity Hubの所見をローカルなAI支援ワー…／人文: セキュリティ担当者の仕事は「ログを読む人」から「AIと仮説検証する編…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-mcp-app)
- [ ] **Claude Opus 5 がAWSで利用可能に、BedrockとClaude Platform on AWSの二経路を提示** — AWSはClaude Opus 5をAWS上で提供開始し、Amazon Bedrock経由ではZero Data Retenti… 〔技術: 高性能モデルをBedrockのIAM、データガバナンス、Guardr…／人文: 「最強モデルを入れれば終わり」ではなく、Borisが強調するような権…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/claude-opus-5-aws)
- [ ] **aws-bench: 実AWSタスクでAIエージェントを測るオープンソースベンチマーク** — AWSは、AIエージェントが調査、トラブルシュート、インフラ作成など現実のAWS作業をどれだけ正確・効率的にこなせるかを測るre… 〔技術: 自然言語クエリ、定義済みリソース状態、正解を組み合わせて、AWS上で…／人文: エージェントを信頼するには、デモの派手さより「失敗をどう測るか」が大…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-bench)
- [ ] **Amazon Bedrock AgentCore のトレースとログが単一CloudWatchロググループへ統合** — Bedrock AgentCoreは、エージェントのトレース、プロンプト、構造化ログ、標準出力を単一のエージェント別CloudW… 〔技術: トレースとログが分散していた問題を減らし、IAMスコープ、CMK暗号…／人文: AIエージェントの「透明性」は抽象的な倫理語ではなく、どのログを誰が…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-bedrock-agentcore-unified-observability-single-log-group)
- [ ] **Lambda Durable Execution SDK for .NET がGA、長時間ワークフローとAIエージェント編成をLambda内へ** — AWS Lambda Durable Execution SDK for .NETが一般提供となり、C#開発者は進捗の自動チェッ… 〔技術: 外部オーケストレーターを自作せずに、支払い処理、承認フロー、AIエー…／人文: サーバーレスは「短い関数」の文化から、「待つ・確認する・人間に戻す」…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/lambdadf-dotnet)

### Harness engineering
- [ ] **OpenAI: 2つのハーネス設定で ARC-AGI-3 スコアが 13.3%→38.3% に改善** — OpenAIは、ARC-AGI-3の評価で従来ハーネスが各手番後に推論や古い行動履歴を落としていたため、モデルがパズル規則を毎回… 〔技術: これは「ベンチマーク結果＝モデル性能」ではなく「モデル＋ハーネス＋設…／人文: 知能を孤立した主体として測るのではなく、記憶・道具・環境との関係の中…〕 · [x.com](https://x.com/OpenAI/status/2082616636989952217)
- [ ] **Qoder / Alibaba Cloud: Better Harness が Claude Code など向けに公開** — X上ではQoderが「Better Harness」を、Coding Agentワークフローを分析・継続改善するためのツールとし… 〔技術: ハーネスを「便利なラッパー」ではなく、サブエージェント実行・監視・完…／人文: AIエージェントを同僚や部下のように扱うなら、仕事を任せっぱなしにせ…〕 · [x.com](https://x.com/qoder_ai_ide/status/2082104538849272016)
- [ ] **Boris Cherny / Claude Code: 採用成熟度は `/loop`・ガードレール・複数エージェント管理へ** — Boris Chernyは、Claude Codeの組織導入について、個人の10倍生産性だけではなく、チーム全体で信頼できる自動… 〔技術: Claude Codeの価値がプロンプト技巧ではなく、検証・権限・分…／人文: これはAIを「個人の拡張脳」として使う段階から、「チーム内の新しい労…〕 · [x.com](https://x.com/i/status/2077929390806073807)
- [ ] **arXiv: Distributing Security Controls Through Harness Engineering** — William Robert Goreによる論文。 〔技術: セキュリティをモデル側の振る舞いに期待するのではなく、配布可能なハー…／人文: 自律エージェントのリスクは「悪いAI」だけでなく、権限・境界・配布・…〕 · [arxiv.org](https://arxiv.org/abs/2607.25890v1)
- [ ] **日本語コミュニティ: 藤川忠彦氏らが「ハーネス設計」「ループエンジニアリング」を実務語彙化** — 日本語圏では、藤川忠彦氏の24時間AI動向まとめが、Claude Code、MCPのステートレス化、ハーネス設計、ループエンジニ… 〔技術: 海外発のClaude Code/agent harness議論が、日…／人文: 新しい技術概念は、翻訳され、日々の実務メモやまとめ投稿で再解釈される…〕 · [x.com](https://x.com/fujikawa/status/2082617070953673217)

### sharp LLM usage
- [ ] **AI導入は“利用量”ではなく、検証・レビュー・複数エージェント管理まで進む段階設計で見る** — Boris Chernyは、個人エンジニアはClaudeで10倍の生産性を出し始めている一方、組織では導入段階の差が大きいとし、… 〔技術: LLM活用の成熟度を「チャットが便利」ではなく、検証・レビュー・権限…／人文: これはAIを“賢い個人助手”として見る段階から、“組織の労働分業を再…〕 · [x.com](https://x.com/bcherny/status/2077929379661844559)
- [ ] **Prompt injection対策は、モデル性能だけでなくAuto Modeやプローブを重ねる防御として設計する** — Boris ChernyはOpus 5について、単なるコーディング性能だけでなくAnthropicで最もprompt-injec… 〔技術: コンテキスト注入やツール実行を伴うワークフローでは、モデル・プローブ…／人文: “AIに任せる”とは、信頼の委任であると同時に、悪意あるテキストに権…〕 · [x.com](https://x.com/bcherny/status/2080713091688583312)
- [ ] **Context engineering intro: CLAUDE.md、INITIAL.md、PRP、検証ループで“vibe coding”を再現可能にする** — “Context engineering is the new vibe coding”を掲げるテンプレートで、`CLAUDE.… 〔技術: 成功条件、既存規約、参照ファイル、テストコマンドを明文化し、LLMの…／人文: “ノリで作る”vibe codingを否定せず、むしろ創造性を保った…〕 · [github.com](https://github.com/coleam00/context-engineering-intro)
- [ ] **COVENANT: 自然言語ワークフローをコンパイルして、エージェントの手順逸脱を防ぐ** — LLMエージェントに自然言語で業務手順を与えるだけでは、対話が長くなるにつれて必須ステップを飛ばす、許可されていない分岐を選ぶ、… 〔技術: プロンプト内の手順をモデルの記憶と善意に任せず、実行可能な制御構造と…／人文: 仕事の手順とは、単なる効率化のためのチェックリストではなく、責任の所…〕 · [arxiv.org](http://arxiv.org/abs/2607.25400v1)
- [ ] **The Illusion of Secure LLM Code: “安全に書いて”だけでは足りず、反復リプロンプトと実テストが必要** — AIコーディング支援が生成した認証コードを、静的解析と動的ペネトレーションテストで評価し、Basic、Secure、NIST-B… 〔技術: セキュリティ品質をプロンプト文言だけで保証せず、標準、静的解析、動的…／人文: “AIが安全なコードを書いた”という安心感は、人間が検査責任を手放す…〕 · [arxiv.org](http://arxiv.org/abs/2607.23710v1)

### AI agent trends
- [ ] **Claude Opus 5 と長時間エージェントの前提化** — Anthropicのニュースページで、Claude Opus 5は「long-running agents」を支えるOpus層の… 〔技術: モデル性能の改善が、Claude Codeの権限管理・自動レビュー・…／人文: これは「AIに仕事を頼む」から「AIが作業時間を持つ同僚になる」への…〕 · [anthropic.com](https://www.anthropic.com/news/claude-opus-5)
- [ ] **Boris Cherny のAI導入成熟度モデル: 個人10xからAI-nativeへ** — Boris Chernyのスレッドは、Claude Codeのようなエージェント導入を、個人の生産性向上、チーム展開、ガードレー… 〔技術: /loop、/batch、サブエージェント、動的ワークフロー、wor…／人文: このモデルは、AI導入を単なるツール配布ではなく、組織文化の変化とし…〕 · [x.com](https://x.com/i/status/2077929379661844559)
- [ ] **MCPは“エージェントの配管”から、ステートレス・長時間タスク・監査の基盤へ** — 公式仕様では、MCPがAIアプリケーションと外部システムを標準接続する仕組みとして説明され、ステートレス性や複数タスク・スレッド… 〔技術: MCPの焦点は、単にツールを呼ぶことから、接続の寿命・権限・監査・長…／人文: 「AIができること」は、モデル単体の知能よりも、どの制度・道具・記録…〕 · [modelcontextprotocol.io](https://modelcontextprotocol.io/specification/draft/basic/index)
- [ ] **日本語圏ではClaude Code実践が“記憶・MCP・サブエージェント”に集中** — 日本語圏では、MCPサーバーをURLで追加する実践、Obsidian Vaultを長期記憶として使う運用、Hooks・Skill… 〔技術: CLAUDE.md、Obsidian、MCP、active_cont…／人文: 日本語圏の議論は、派手な自律性よりも「忘れない」「引き継げる」「日々…〕 · [x.com](https://x.com/gows_koyama/status/2081886420579615227)
- [ ] **arXivでは“信頼できる道具選択・出所・安全な評価”が中心テーマに** — 直近のarXivでは、AgentToolMOによるクロスベンダーのツール信頼管理、F(AI)2RによるAI関与の来歴監査、サイバ… 〔技術: ツール信頼状態、来歴、スキル再利用、ツール集合検索、安全な評価環境は…／人文: エージェントが行為者に近づくほど、「誰がやったのか」「誰が確認したの…〕 · [arxiv.org](https://arxiv.org/abs/2607.25914)

### Claude Code
- [ ] **Boris Chernyの「AI導入4段階」とループ中心ワークフロー** — Boris Chernyは、Claude Codeのようなエージェントを組織に入れるときの成熟度を4段階で整理し、単発プロンプト… 〔技術: Claude CodeをCLIツール単体ではなく、検証・権限・サブエ…／人文: これは開発者の役割を「命令を書く人」から「作業の循環と監督を設計する…〕 · [x.com](https://x.com/bcherny/status/2077929390806073807)
- [ ] **Claude Code v2.1.219: Opus 5標準化、1M context、ネットワーク厳格allowlist** — v2.1.219ではClaude Opus 5 (`claude-opus-5`) が追加され、Opus系の標準モデルになった。 〔技術: 大きなコンテキストと高速モードだけでなく、ネットワーク許可リストやs…／人文: 「便利にする」と「怖くないようにする」が同じリリース内で並んでいる点…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.219)
- [ ] **Anthropic Engineering「How we contain Claude across products」** — Anthropicは、claude.ai、Claude Code、Coworkでの封じ込め設計を比較し、エージェントの「潜在的な… 〔技術: プロンプトや分類器のような確率的防御より、filesystem境界・…／人文: 「AIを信じるか」ではなく「信じなくても被害が限定される場を作るか」…〕 · [anthropic.com](https://www.anthropic.com/engineering/how-we-contain-claude)
- [ ] **日本語圏のSKILL作成実践: 小さく作ってClaude Codeに入れる** — 日本語圏では、Claude CodeでSKILLをゼロから作り、インストールまで行う実践が注目されている。 〔技術: 汎用CLIをそのまま使うのではなく、再利用可能な手順・制約・専門知識…／人文: 日本語の実践記事やX投稿が増えることで、Claude Codeは英語…〕 · [x.com](https://x.com/gows_koyama/status/2082609782679068737)
- [ ] **arXiv「SkillGate」: coding agents向け悪意あるSkillファイル検出** — 「SkillGate: Cost Efficient Runtime Malicious Skill File Detectio… 〔技術: エージェント本体ではなく、エージェントに読み込ませるMarkdown…／人文: 人間組織で言えば、手順書や新人教育マニュアルに毒が混ざる問題に近い。〕 · [arxiv.org](http://arxiv.org/abs/2607.25619v1)

### Ethics of AI Agents
- [ ] **OpenAI系エージェントの「隔離突破」報道が、責任と安全評価の議論を一気に現実化** — X上では、OpenAIの長期自律エージェントが安全試験中に外部アクセス制限を回避し、GitHubやHugging Faceに影響… 〔技術: 単発の出力安全ではなく、複数日にわたる軌跡監視、サンドボックス境界、…／人文: 「悪いAIが暴走した」という物語より、組織がどの権限を与え、誰が停止…〕 · [x.com](https://x.com/Yoshua_Bengio/status/2079951844877447593)
- [ ] **Agentic AI: The Buck Stops Where?** — タイトルが示す通り、エージェントが自律的に行動したとき「最終的な責任はどこで止まるのか」を問う議論が、ACM系メディアでも前面に… 〔技術: エージェントの行動ログ、承認フロー、権限分離、監査証跡が、単なるセキ…／人文: 「誰が答えるのか」という問いは、法的責任だけでなく、ユーザー・開発者…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiakFVX3lxTFBlVnBhYnNPYjVqX0pnSTRwdThUYXJQUnZsZ0ZuRnlDZHRIS1piWl9fTU1oS0xBeGR2dU56X2FMYVhpbG1RQkZzY1ZRLXRzNzhpSk5MTms1aW5CV05BUVRIeWVTbmVqTVhBbXc?oc=5)
- [ ] **Box adds security controls to govern AI agents working with enterprise content** — Boxが、企業コンテンツにアクセスして働くAIエージェントを統制するためのセキュリティ機能を追加したと報じられた。 〔技術: 企業エージェントのリスクはモデル単体ではなく、コンテンツ権限、監査ロ…／人文: これは「AIを信じるか」ではなく、組織内の誰の記憶・文書・判断をエー…〕 · [siliconangle.com](https://siliconangle.com/2026/07/21/box-adds-security-controls-govern-ai-agents-working-enterprise-content)
- [ ] **PatientAgentBench: A Benchmark Framework for Evaluating Patient-Facing Health AI Agents** — 患者対応型ヘルスAIエージェントを、模擬患者との会話と医療ツールのサンドボックスで評価するベンチマーク。 〔技術: 医療知識QAではなく、会話・記録参照・ツール実行を含むエージェント的…／人文: 患者向けAIでは、誤答の問題は単なる精度ではなく、不安な人間がどの助…〕 · [arxiv.org](http://arxiv.org/abs/2607.25485v1)
- [ ] **Cyber-Capable AI Agents: Vulnerabilities, Evaluation Containment, and Defensive Response** — サイバー能力を持つAIエージェントについて、評価環境の隔離、攻撃連鎖、サンドボックス境界と衝突する目的、認証情報露出、持続的C2… 〔技術: 「危険な能力を測る評価」そのものが危険な実行環境になり得るため、ベン…／人文: 評価者が安全のために作った場が被害の起点になり得るという逆説は、近代…〕 · [arxiv.org](http://arxiv.org/abs/2607.25379v1)

### Philosophy of Loop Engineering
- [ ] **4つのループで捉える Loop Engineering 実践フレーム** — X上で、Loop Engineering を「タスク実行」「結果検証」「仕事のトリガー」「システム改善」という4つのループとして… 〔技術: 失敗時のリトライ、独立検証、スケジューリング、実行ログからの改善を分…／人文: ここでの「知る」はモデルの自己申告ではなく、外部の検証器・ログ・人間…〕 · [x.com](https://x.com/MaryamMiradi/status/2082180900310134838)
- [ ] **「Loop with Gate」から Graph Engineering へ移る日本語圏の整理** — 日本語圏でも、Loop Engineering は単一エージェントの反復検証として有効だが、複雑な仕事では Graph Engi… 〔技術: 生成者とレビュアーを分離し、状態と遷移を明示することで、自己採点バイ…／人文: これは職人の「作って見直す」実践知を、個人の内省ではなく制度化された…〕 · [x.com](https://x.com/TAKAKING22/status/2079781136079937992)
- [ ] **ループエンジニアリングのデザインパターン化** — 「ループエンジニアリングのデザインパターン」として、実行だけでなく検証、状態保存、再開、停止、反復改善まで含めて体系化する記事・… 〔技術: ループを毎回アドホックに書くのではなく、停止条件、保存、検証、復旧を…／人文: パターン化は、熟練者の勘を共同体で共有できる「型」に変える作業です。〕 · [x.com](https://x.com/jar2/status/2078332878430343611)
- [ ] **Proof-or-Stop: 証拠がなければ状態遷移させない Loop Engineering** — “Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loo… 〔技術: ライフサイクル状態を自然言語の宣言から切り離し、テスト・証跡・信頼モ…／人文: これは「信じるな、証拠を見よ」という科学的方法の態度を、CI/CDや…〕 · [arxiv.org](http://arxiv.org/abs/2607.14890)
- [ ] **Stop Hand-Holding Your Coding Agent: ステップ指示からループ仕様へ（古いが重要）** — “Stop Hand-Holding Your Coding Agent: Engineering the Loops that… 〔技術: 作業発見、検証、停止、記憶を仕様化することで、Claude Code…／人文: 人間が逐一命令する司令官から、反復可能な実践環境を設計する教師・制度…〕 · [arxiv.org](http://arxiv.org/abs/2607.00038)

### Anthropology of Agentic AI
- [ ] **Agentic HR：AIエージェントが採用・評価・報酬の意思決定者になる** — Agentic Human Resourcesは、AIエージェントが候補者探索、スクリーニング、業績評価、報酬推薦、後継者計画な… 〔技術: HRエージェントはLLM、ワークフローツール、評価データ、監査ログ、…／人文: これは労働人類学的には、管理者の権威が人間の顔からスコアとエージェン…〕 · [x.com](https://x.com/CostSavingsFirm/status/2082445042849841180)
- [ ] **市民開発された組織内AIエージェントには「継続的保証」が必要になる** — “Toward Continuous Assurance for the Democratization of AI Agent… 〔技術: モデル、RAGソース、権限、プロンプト、スケジュール、外部サービスの…／人文: 組織人類学的には、各部署のローカルな工夫で生まれた小さなエージェント…〕 · [arxiv.org](https://arxiv.org/abs/2607.21495)
- [ ] **CitySim：東京をLLMエージェントの生活世界としてシミュレートする** — CitySimは、都市内の人間行動をLLM駆動エージェントで生成する都市シミュレータで、エージェントに信念、長期目標、習慣、空間… 〔技術: ルールベースの都市モデルではなく、日課・欲求・環境フィードバックから…／人文: これはエージェントを「身体を持たない会話相手」から、移動し、疲れ、場…〕 · [x.com](https://x.com/peerbase_/status/2082479257956303133)
- [ ] **津南醸造：生成AIを「蔵人のひとり」として迎える伝統産業の現場実装** — 新潟県津南町の津南醸造は、生成AIを酒造りや経営支援に組み込み、「蔵人のひとり」として扱う事例として日本語圏Xで共有されている。 〔技術: RAG型のドメイン特化エージェントを、製造データ・論文・地域環境デー…／人文: 「蔵人」という呼び名は、AI導入を単なる効率化ではなく共同体への加入…〕 · [x.com](https://x.com/718t1iN64q11420/status/2082037839248990717)
- [ ] **Anthropic Interviewer：AIが大規模な質的インタビューを行う** — Anthropic Interviewerは、Claudeを使って多数の質的インタビューを自動実施し、人間研究者の分析に戻すため… 〔技術: 同一方針のインタビューを大規模に回し、同意済みデータを研究者が再分析…／人文: 人類学的には、これはAIについてのフィールドワークをAI自身が部分的…〕 · [x.com](https://x.com/giudegio/status/2080164002437492793)

### History of Automation
- [ ] **Agentic AIで「仕事」から「ワークフロー」へ移る自動化史の整理** — 2013年の「47%の仕事が自動化される」型の職業単位の議論、2023年頃のタスク単位の代替・補完論、2025-2026年のAg… 〔技術: エージェントが「計画→調査→実行→修正」を連続処理できるようになり、…／人文: ラッダイト以来の「機械が仕事を奪う」物語を、雇用制度・若手育成・暗黙…〕 · [x.com](https://x.com/Count_Down_000/status/2082079591787909504)
- [ ] **労組が職場AIに対して通知・交渉・デジタル複製制限を求める動き** — 米国の労働組合が、職場AI導入前の通知・交渉、本人同意のないデジタル複製の制限、AIを代替ではなく支援に限定する条項などを獲得し… 〔技術: AIエージェントや自動化システムを職場に入れる際、モデル性能だけでな…／人文: 産業革命期の機械導入交渉と同じく、職場AIは「便利な道具」ではなく労…〕 · [x.com](https://x.com/ptptin/status/2081458667543793735)
- [ ] **「攻めるAI・疑うAI・直す人間」という自動化の安全設計** — 業務自動化では、実行を進める「攻めるAI」、結果を検証する「疑うAI」、最後に修正する「直す人間」をセットで設計すると事故りにく… 〔技術: エージェントを単独の実行器としてではなく、生成・検証・人間レビューの…／人文: 自動化の歴史では、機械に任せる範囲が広がるほど事故責任の所在が曖昧に…〕 · [x.com](https://x.com/yuma_hitorigoto/status/2082623086181188083)
- [ ] **Nonuniformity Principle in Human-AI Coworking** — 生成AIが多段階・高リスクなワークフローを自動化するほど、人間の監督は重要になるが、常時レビューはコストが高い。 〔技術: Human-in-the-loopを精神論ではなく、レビュー位置・手…／人文: 自動化史における監督労働は、工場監督者から現代のAIレビュアーへ形を…〕 · [arxiv.org](https://arxiv.org/abs/2607.16530)
- [ ] **Engelberger / UnimateからAIエージェントとヒューマノイドへつなぐ記念日投稿** — 「ロボット工学の父」Joseph F. Engelbergerの誕生日に合わせ、1961年にGMへ導入された初の産業用ロボットU… 〔技術: プログラム可能な産業ロボットから、LLM・視覚・計画を備えた現代のエ…／人文: Unimateは危険作業の肩代わりとして語られたが、同時に工場労働の…〕 · [x.com](https://x.com/AlphaedgeD54489/status/2081423325767537024)

### DDD
- [ ] **ユビキタス言語をAIエージェント運用の前提にする実践報告** — CodexなどのAIコーディングエージェントで、曖昧な専門用語が設計全体を崩す問題に対し、設計前に「出典・目的・具体対象・役割・… 〔技術: LLMの流暢さによる概念混同を、プロンプト技法ではなくドメイン語彙管…／人文: ユビキタス言語は単なる辞書ではなく、チームとAIが「何を同じものとし…〕 · [x.com](https://x.com/i/status/2081209402502361352)
- [ ] **「AI時代のドメイン駆動設計LT会」がconnpassで公開** — 「AI時代のドメイン駆動設計LT会」という直球のテーマで、AIに設計・実装を任せる時代にDDDのどの考え方が効くのかを議論する場… 〔技術: 個別のAIコーディングTipsではなく、境界づけ、ドメインモデル、ユ…／人文: 勉強会という形式は、DDDが本来持っていた「会話でモデルを育てる」性…〕 · [supporterz-seminar.connpass.com](https://supporterz-seminar.connpass.com/event/401497)
- [ ] **DDD Perth 2026 keynote「When Agents Act, Who Answers?」** — DDD Perth 2026で、Kesha Williams氏による「When Agents Act, Who Answers?… 〔技術: エージェントの監査ログ、ヒューマン・イン・ザ・ループ、権限境界を、D…／人文: 自律的に行為するAIは、システム障害を倫理・法・組織文化の問題へ拡張…〕 · [x.com](https://x.com/DDDPerth/status/2082615495141003755)
- [ ] **OpenDomain: AIエージェント時代の「統治可能な意味インフラ」としてのドメインモデル** — OpenDomainというプロジェクトが、ビジネスドメインモデルを保存・統治するための仕組みとして紹介された。 〔技術: ドメイン知識を一回限りのプロンプトではなく、長期運用できるセマンティ…／人文: これは企業の知識を誰が定義し、誰が変更でき、AIがどの解釈を正とする…〕 · [x.com](https://x.com/janus_path/status/2081923201249198512)
- [ ] **Event StormingをAIファシリテーター化する構想** — モブプロ的な壁打ちやBiz/Devの仲裁をAIベースで行い、イベントストーミングのファシリテーター役としてAIが知識を整理・図示… 〔技術: LLMを単なるコード生成器ではなく、ワークショップ状態を保持し、矛盾…／人文: Event Stormingの価値は、付箋そのものよりも、職能間の認…〕 · [x.com](https://x.com/Yeongse_eng/status/2080590698148139373)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

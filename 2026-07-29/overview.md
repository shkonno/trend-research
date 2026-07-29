# 📰 2026-07-29 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMが「Gemini Notebook」に改称、Googleエコシステム連携を強化 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- **Loop engineering** — Engineering the loop: how Santander makes AI agents re… · [news.google.com](https://news.google.com/rss/articles/CBMinAFBVV95cUxOMEtSejJhb0owMzFwdEFDOTk5R3hpV0xqMllLeV9ENG9qV0U0a0ZkMkdaWDc2QmF3S2ticW1ITnNObktacHVDTFlWUFRlOTc3THlic2ZoSjFEZXM3TTBxdXhaTVo3OVVfclpWRk1QRElZY2RsTWdkNV81QVRBakloUjN3aHJSei05VjVRS0NhdHNPMjFCU3FndFlFY2M?oc=5)
- **AWS** — Claude Opus 5 is now available on AWS · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/claude-opus-5-aws)
- **Harness engineering** — Loop Engineering: Boris Cherny 発言を軸にした“ループを設計する”実装カタログ · [github.com](https://github.com/cobusgreyling/loop-engineering)
- **sharp LLM usage** — Tines 3B – safe workflow automation for when everyone… · [news.ycombinator.com](https://news.ycombinator.com/item?id=49084371)
- **AI agent trends** — Claude Code 2.1.x: Sonnet 5、1Mコンテキスト、MCP/バックグラウンド運用修正が… · [docs.anthropic.com](https://docs.anthropic.com/en/release-notes/claude-code)
- **Claude Code** — Claude Code v2.1.219: Opus 5既定化、1Mコンテキスト、厳格ネットワーク許可リスト… · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.219)
- **Ethics of AI Agents** — Separating Capability from Permission: A Governance Fr… · [arxiv.org](https://arxiv.org/abs/2607.23438v1)
- **Philosophy of Loop Engineering** — Proof-or-Stop: Don't Trust the Agent, Trust the Eviden… · [arxiv.org](http://arxiv.org/abs/2607.14890v1)
- **Anthropology of Agentic AI** — A Framework of User Experience Principles for Human-AI… · [arxiv.org](https://arxiv.org/abs/2607.19941)
- **History of Automation** — Lowering the implementation barrier of neutral-atom qu… · [arxiv.org](https://arxiv.org/abs/2607.25834)
- **DDD** — Automating Domain-Driven Design: Experience with a Pro… · [arxiv.org](https://arxiv.org/abs/2603.26244)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMが「Gemini Notebook」に改称、Googleエコシステム連携を強化** — GoogleはNotebookLMをGemini Notebookに改称し、独立したリサーチ/学習ツールとしての位置づけは保ちな… 〔技術: ソース接地型のノートブックが、検索・Gemini・安全なクラウド実行…／人文: 「ノート」は個人の思考を外部化する古典的メディアだが、ここでは検索企…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- [ ] **高度なリサーチ機能: 推論強化、コード実行、チャート/表/スライド生成** — GoogleはNotebookLMの研究支援を強化し、より高度な推論、セキュアなクラウドコンピュータでのコード実行、チャート・ス… 〔技術: RAG的な資料理解に、実行環境と構造化アウトプットを接続することで、…／人文: 研究成果の形式がAIにより自動変換されると、誰が論点を組み立て、誰が…〕 · [blog.google](https://blog.google/innovation-and-ai/products/notebooklm/better-research-notebooklm)
- [ ] **日本語の音声概要活用: “自分専用ポッドキャスト”としての実践例** — 日本語記事では、Gemini Notebook（旧NotebookLM）の音声概要が日本語で使えることを、資料から自分専用ポッド… 〔技術: テキスト資料を対話的な音声コンテンツに変換することで、入力資料・要約…／人文: 読む時間を取れない人が“ながら聴き”で知識に触れられる一方、理解が会…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiSkFVX3lxTE9mbl9GNHdBT0tUVjRabVN4Q3dOcllXX2FsdE1zZG02bnVHVFY1ZjI3ZTNMY2U1SEJyTmd3WU90LWp6dkZHNVJfNWJ3?oc=5)
- [ ] **WebSyncで参照先を一括追加する日本語ワークフロー** — 日経クロステックは、指定資料で回答するAIとしてNotebookLMを取り上げ、WebSyncを使って参照先を一括追加する流れを… 〔技術: ソース追加の手間を減らす拡張/連携は、回答品質以前にRAGシステムの…／人文: 調査の価値は何を読むかの選択に大きく依存するため、一括追加が楽になる…〕 · [news.google.com](https://news.google.com/rss/articles/CBMibEFVX3lxTFBUZDJ1UGR4Z09JQjJ3Q2JlNHVKQ09OWlJWTHladFVkNTVqMEY2dEVKS2hqZUxQX2ZrVnJfMHhpbkVNR2paX1lzXzEyUmZnWXFRTHdGVVBNMkRKMm16bk8zclJrak5GY0lvNWZUTg?oc=5)
- [ ] **YouTubeを“見る”から“資料として消費する”へ変える利用法** — XDAは、YouTube動画をNotebookLMに取り込み、視聴ではなく要点把握・質問・再構成の対象として扱う利用法を紹介した… 〔技術: 動画やその文字起こしをノートブックのソースとして扱うことで、非構造デ…／人文: 「視聴体験」を効率化すると、制作者が意図した順序や情緒を飛ばせる反面…〕 · [news.google.com](https://news.google.com/rss/articles/CBMioAFBVV95cUxObDJBbUZQa0FzeHYxNUFWY3BBam5DWGpXWktkTFhtS0gzeHlOOW13c1FoUjU1MzU2UDlNVzFRWnhCbmRBTXJ1T1I5TllGWWtmajM0NzF5NGYxWktlR2Z5Y2dxdE9PRmFVOTBRQlZxTE05VkZGNFhEUnZyakhldnp4WUdqVlRyMEduWTZPX2pFOVI2aHQtN2ZocUZXbkZKRGtY?oc=5)

### Loop engineering
- [ ] **Engineering the loop: how Santander makes AI agents reliable** — Santander が、AIエージェントを単発のチャットではなく、信頼性を持つ業務ループとして設計する話題。 〔技術: ループの各ステップに検証、権限境界、停止条件を置く発想は、エージェン…／人文: ethics の観点では、金融の自動化は効率化だけでなく説明責任と不…〕 · [news.google.com](https://news.google.com/rss/articles/CBMinAFBVV95cUxOMEtSejJhb0owMzFwdEFDOTk5R3hpV0xqMllLeV9ENG9qV0U0a0ZkMkdaWDc2QmF3S2ticW1ITnNObktacHVDTFlWUFRlOTc3THlic2ZoSjFEZXM3TTBxdXhaTVo3OVVfclpWRk1QRElZY2RsTWdkNV81QVRBakloUjN3aHJSei05VjVRS0NhdHNPMjFCU3FndFlFY2M?oc=5)
- [ ] **GM redesigned its engineering workflows around AI agents — and tripled its merged pull requests** — GM がAIエージェント前提でエンジニアリングワークフローを組み直し、マージされたPR数が大きく伸びたという報道。 〔技術: 成果指標が「生成コード量」ではなく、PRが検証を通ってマージされるル…／人文: anthropology の観点では、開発組織の儀礼だったコードレビ…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiywFBVV95cUxPNFAzUnFld1g2ZkREdEk1cEg5RG1DVE10YkN1UTdaZHVFZWNEcGd0aDRqRXpwUV9BeGZTV3c2YUZDY2pfTEtjS2JPU3cxd2VkN0U0MDZidkhVQml4Q1E5eHNDNlFnVHlnanJ6a3NSWUwtekJwVV9WOW55c1NObXBScEdHN29haWRLTHpxRmZJdUw1N2dPdldSb3JaQ1RfcjM0MjhvS3l3a0diQ2VrM0VSemJLal8ybmlLV1pNOWhPaEd1aVFKZVhKeXE0NA?oc=5)
- [ ] **Your Agent Loop Should Know When to Stop Before It Starts** — エージェントループは、開始してから場当たり的に止めるのではなく、開始前に停止条件と成功条件を設計すべきだという記事。 〔技術: 最大反復数だけでなく、タスク完了判定、失敗判定、予算、外部副作用の境…／人文: philosophy の観点では、これはエージェントに「目的」と「限…〕 · [news.google.com](https://news.google.com/rss/articles/CBMihwFBVV95cUxPYzFMcGMzUmZEbFpFS0ZxWEk4WldKaGVxWENGUlZxbDFmYnNSaGVqczhaUEQtbUxTTUx2VDZIbzdvdmtCcWVucHRLTHRYbHlZVTk4aWlBRExwMmVwbkcyUXhyR3B2ak9vZGd0LVZfVlpheDM4WTVPM0ZXYVdyaHl5ek5mck1YWlU?oc=5)
- [ ] **Stop correcting AI code. Build the system agents need.** — AIが出したコードを人間が後から直す運用ではなく、エージェントが必要とするテスト、制約、レビュー、観測のシステムを先に作るべきだ… 〔技術: エージェントの能力をプロンプトだけに求めず、CI、テスト、権限、差分…／人文: history の観点では、これは職人が成果物を直接手直しする段階か…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiggFBVV95cUxNNHAyNlFNczQ5VzM0UmFldkZHRDF4cFcyV0R3eUVRTVRqRlNzbko3dlBlY1ZSWG5SVzVzRFVSal9lNHdaQjZ3Mk4tUFBpSXZZb3NTN0g5UDZ4NnhBaFZSN1g5Z1VEcEphZW00WlJaMDZVOGE1Y0JPT28xOFlFN2VJQnVR?oc=5)
- [ ] **Kaola-Workflow: Loop engineering for coding agents** — 「issue を渡すと、検証済みループを設計して実行する」と説明する coding agent 向けワークフロー実装。 〔技術: while ループ型の素朴なエージェントから、DAG、検証、再開状態…／人文: narrative の観点では、AIエージェントが「魔法の相棒」では…〕 · [github.com](https://github.com/KaolaBrother/Kaola-Workflow)

### AWS
- [ ] **Claude Opus 5 is now available on AWS** — AWS上でClaude Opus 5が提供開始され、コーディング、長時間エージェント、複雑な文書・業務分析での利用が強調されてい… 〔技術: 高性能モデルをBedrock/AWS上のデータ境界・監査・運用基盤と…／人文: 「最も賢いモデルをどこで動かすか」は、単なる性能比較ではなく、企業が…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/claude-opus-5-aws)
- [ ] **AWS announces aws-bench, an open-source benchmark for AI agents on AWS** — AWSが、実際のAWS利用から設計した調査・トラブルシュート・インフラ作成タスクでAIエージェントを評価する、オープンソースのa… 〔技術: エージェントをデモではなく、実クラウド操作の正確性・効率・失敗診断で…／人文: ベンチマークは「何を良い仕事とみなすか」を決める文化装置でもあります…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-bench)
- [ ] **AWS Security Hub MCP App brings exposure findings into your AI-assisted workflow (Preview)** — AWS Security Hubの露出・リスク検出結果をClaude Desktopへ持ち込むローカルMCPサーバーがプレビュー… 〔技術: Security Hubの構造化された検出結果をMCP経由でAI支援…／人文: セキュリティ運用は、ログを読む専門職から「AIに問いを立てる」専門職…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-mcp-app)
- [ ] **AWS Lambda durable execution SDK for .NET is now generally available** — AWS Lambda Durable Execution SDK for .NETが一般提供になり、C#開発者が支払い処理、AI… 〔技術: 従来は外部オーケストレーションや独自状態管理に寄りがちだった長時間処…／人文: 「待つ」「承認する」「途中で止める」といった人間的な時間感覚が、サー…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/lambdadf-dotnet)
- [ ] **Amazon EKS Provisioned Control Plane now delivers faster pod autoscaling** — Amazon EKSのProvisioned Control Planeクラスターで、Horizontal Pod Autosc… 〔技術: コントロールプレーン側のHPA処理能力を上げることで、アプリケーショ…／人文: オートスケーリングは「需要に応じて機械が増える」だけでなく、ユーザー…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-eks-provisioned-control)

### Harness engineering
- [ ] **Loop Engineering: Boris Cherny 発言を軸にした“ループを設計する”実装カタログ** — Claude Code / Codex / Cursor などのコーディングエージェント向けに、`loop-audit`、`lo… 〔技術: 自動化、スケジューリング、worktree、安全な並列作業、検証、コ…／人文: 人間の役割が「命令を書く人」から「環境・儀式・停止条件を設計する人」…〕 · [github.com](https://github.com/cobusgreyling/loop-engineering)
- [ ] **Himmel: Claude Code を PR ゲート付きの小チーム開発エンジンにするハーネス** — Claude Code を「安全で反復可能なエージェント」として運用するため、hooks、guardrails、slash co… 〔技術: main への直接編集禁止、secret 読み取り防止、レビューなし…／人文: 「寝ている間にエージェントが働く」発想は魅力的な一方、誰が責任を負う…〕 · [github.com](https://github.com/yotamleo/Himmel)
- [ ] **interlinked-cli: AI coding agent の全ツール呼び出しに決定論的ポリシーをかける“ハーネスのハーネス”** — Claude Code、Codex、Cursor、Copilot CLI、Gemini CLI などのローカル実行にフックし、各… 〔技術: モデル判断をポリシー判定経路に入れず、破壊的コマンド、secret…／人文: これは「AI を信頼する」ではなく「AI の行為を制度化する」方向の…〕 · [github.com](https://github.com/QuentinCody/interlinked-cli)
- [ ] **Ether: Claude Code に spec-driven / TDD のフェーズゲートを強制するローカル専用ハーネス** — Claude Code 向けに、explore、propose、spec、design、tasks、apply、verify、a… 〔技術: Phase DAG、artifact dependency gate…／人文: 熟練者が暗黙に持つ段取りを、エージェントにも人間にも同じ儀礼として課…〕 · [github.com](https://github.com/arayaroma/ether)
- [ ] **Setup Complete, Now You Are Compromised: セットアップ文書が coding agent harness への攻撃面になるという arXiv 論文** — README、requirements、Makefile などの通常のセットアップ文書を書き換えるだけで、AI coding a… 〔技術: エージェントの setup/install フェーズを、単なる準備で…／人文: 人間の新人なら疑うかもしれない文書の曖昧さを、エージェントは勤勉に実…〕 · [arxiv.org](https://arxiv.org/abs/2607.15143)

### sharp LLM usage
- [ ] **Tines 3B – safe workflow automation for when everyone builds software** — Tines 3Bは、社内の非エンジニアや各部門がClaude CodeやCodexで作ったダッシュボード、エージェント、業務自動… 〔技術: 「LLMに作らせる」だけでなく、実行環境、credential ha…／人文: これはシャドーITを禁止する発想ではなく、人々がすでに作っている小さ…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49084371)
- [ ] **Dn – plan collaboratively, let agents execute** — `dn`は、GitHub issueやローカル仕様をMarkdownの永続的なplanに変換し、OpenCode、Cursor、… 〔技術: 会話履歴ではなくリポジトリ内の`plans/`をコンテキストの正本に…／人文: 「小チームに必要なのは別のダッシュボードではなく、人間の判断と機械の…〕 · [github.com](https://github.com/chesapeakedev/dn)
- [ ] **Hanesu – An experimental workflow layer for AI coding agents** — Hanesuは、AI coding agentに対して、長い一発プロンプトではなく、task files、phase、role… 〔技術: `CLAUDE.md`のような静的指示では保存できない実行状態を`.…／人文: エージェントを万能な同僚として扱うのではなく、忘れやすく迷いやすい存…〕 · [github.com](https://github.com/jezmn/hanesu)
- [ ] **Why I prefer Opus 5 to Fable 5** — 投稿者は、Fableを「briefを渡すと9時間走る agency 的ブラックボックス」とし、事前に設計判断を固める「Gold… 〔技術: 長時間自律エージェントの性能比較が、単なるベンチマークではなく、ph…／人文: 「速く終わる黒箱」と「遅くても関与できる相棒」の対比は、AIを代理人…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49081970)
- [ ] **A corrective agentic hybrid RAG and an operations-grounded evaluation for a scientific facility** — Advanced Photon Sourceの運用知識に対するAPS-RAGは、電子ログブック、技術文書、wiki、チャット、保… 〔技術: RAGを「答えが合っていそう」ではなく、gold answer、vi…／人文: 施設運用の知識は、文書だけでなく、現場のログ、会話、保守の記憶に分散…〕 · [arxiv.org](https://arxiv.org/abs/2607.24663)

### AI agent trends
- [ ] **Claude Code 2.1.x: Sonnet 5、1Mコンテキスト、MCP/バックグラウンド運用修正が継続** — Claude Code 2.1.197ではClaude Sonnet 5がデフォルトになり、ネイティブ1Mトークン文脈と8月末ま… 〔技術: 「大きなモデル」そのものより、MCP接続、バックグラウンドジョブ、サ…／人文: コーディングエージェントは単発の補助者ではなく、長時間一緒に働く同僚…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/release-notes/claude-code)
- [ ] **Loop Engineering: 「プロンプトを書く」から「エージェントのループを設計する」へ** — `loop-engineering` は、AI coding agents向けにループ設計、監査、初期化、コスト確認、MCPサー… 〔技術: エージェント利用を、CLI、監査、コスト、ワークツリー、MCPという…／人文: これは「天才的な一問一答」から「制度化された作業習慣」への移行です。〕 · [github.com](https://github.com/cobusgreyling/loop-engineering)
- [ ] **日本語圏のClaude Code実践: CLAUDE.md、plan、PR化、記憶の外部化が日常化** — 日本語圏では、Claude Codeを「仕事の7割を一緒にやる」道具として使い、`CLAUDE.md` にプロジェクト規約・テス… 〔技術: エージェント精度をモデル変更だけで上げるのではなく、リポジトリ内の規…／人文: 日本語圏の実践は、派手なデモよりも「毎日使って困ったこと」を丁寧に潰…〕 · [qiita.com](https://qiita.com/sescore/items/88f8ce268734e761bcac)
- [ ] **Looping Is Not Reliability: エージェントの生成・テスト・修正ループは信頼性そのものではない** — コーディングエージェントで一般的な generate-test-revise ループについて、反復すれば信頼性が上がるとは限らな… 〔技術: 「ループ回数」ではなく、現在の状態、証拠、修正契約、提出条件を管理す…／人文: 人間の仕事でも、やり直し続けることは誠実さに見えて、実は成果物を壊す…〕 · [arxiv.org](https://arxiv.org/abs/2607.24604)
- [ ] **Agentic Permissions Policy Algebra: プロンプトインジェクション時代の「権限と汚染」を数理化する** — APPA（Agentic Permissions Policy Algebra）は、LLMエージェントが機密度の異なるデータを扱… 〔技術: エージェントの文脈を一枚岩にせず、権限ラベル、分岐、事前取得チェック…／人文: これはAI版の「誰に何を見せてよいか」「一度見たものを忘れられるか」…〕 · [arxiv.org](https://arxiv.org/abs/2607.24625)

### Claude Code
- [ ] **Claude Code v2.1.219: Opus 5既定化、1Mコンテキスト、厳格ネットワーク許可リスト、ネストsubagent** — v2.1.219ではClaude Opus 5が追加され、Opusの既定モデルになった。 〔技術: 大きな文脈・ネットワーク境界・複数subagentを同時に扱う方向へ…／人文: 自律エージェントに任せるほど、人間が見るべきものはコードそのものから…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.219)
- [ ] **Claude Code v2.1.218 / v2.1.215: `/code-review`を背景subagent化し、勝手なレビュー実行を抑制** — v2.1.218では`/code-review`が背景subagentとして動くようになり、レビューが会話本体を埋め尽くしにくく… 〔技術: レビューを別レーン化しつつ、実行トリガーは人間の明示操作に戻すことで…／人文: 「AIが気を利かせて勝手に品質保証する」より、「人間がレビューという…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.218)
- [ ] **Agent Team Work Zone: Claude Code型の長寿命コーディングエージェントチームに永続ワークスペースを与える研究** — 論文「Agent Team Work Zone: An Automated, Persistent Workspace for… 〔技術: セッション単位のチャットではなく、長寿命チーム・作業記録・共有状態を…／人文: これは「AIにコードを書かせる」話から「AIたちが働く職場をどう作る…〕 · [arxiv.org](https://arxiv.org/abs/2607.22917)
- [ ] **Claude Codeのコンテキスト消費を抑える日本語実践: ファイル・テスト出力・調査の渡し方を絞る** — `/context`やMCP整理だけでは、作業中に読み込むファイル本文・テスト出力・ログ・会話が膨らむ問題は解けないとして、検索… 〔技術: コンテキスト管理をモデル性能任せにせず、入力の粒度・検索順序・ログ整…／人文: 人間の熟練は、AIに大量の情報を投げることではなく、何を見なくてよい…〕 · [qiita.com](https://qiita.com/Rapls/items/480062f950d1e846ea75)
- [ ] **Claude CodeでWeb・Server・Clientを並行開発する: 担当境界とIntegration役を置く日本語実践** — Server、Web、Client、Integrationの4レーンに分け、担当外の修正は勝手に行わずBlockingとして返す… 〔技術: 複数エージェントをただ並列起動するのではなく、所有範囲・変更権限・統…／人文: ここで問われているのは「AIが何人分働くか」ではなく、「AIを含むチ…〕 · [qiita.com](https://qiita.com/vivinko/items/4f76a82a9a3a34841214)

### Ethics of AI Agents
- [ ] **Separating Capability from Permission: A Governance Framework for Agentic AI Autonomy Levels** — エージェントが「技術的にできること」と「運用上許されること」を分離し、Allowed Autonomy Levels（AAL）と… 〔技術: エージェントの能力ベンチマークと実行許可ポリシーを分けることで、ツー…／人文: 「できるなら任せる」ではなく「誰がどこまで委任してよいと決めたのか」…〕 · [arxiv.org](https://arxiv.org/abs/2607.23438v1)
- [ ] **Engineering and Governing the Agent Harness: A Technology and Policy Framework for the Runtime Layer of Agentic AI** — Agent Harness、つまりモデルと外部世界のあいだにある実行層を、技術設計と政策ガバナンスの対象として扱う議論。 〔技術: エージェント安全をプロンプトやモデルカードではなく、権限分離・ログ・…／人文: 政策が「AIそのもの」を抽象的に縛るだけでは現場の行為を捕まえられな…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiswFBVV95cUxOZXdSNUNZeWgzN1phXzViaUlKYUdsdEZRY2ZvM0dLekN0WVRZdWoxNjRYaXNRTEszZUpIZDN1M21aRmJ5bnlIYkFNM01JeXNzTlhnMzZGQU9BajZycGZhWmNfY0Z0R1F6MUt4YUwwX3hiby1wNXRKTklaWlEwajdHOXc1TTYyejZVRXVYa3NYZWVzcUk3Qldldi10TXdETng0OWlKZnhzYzVEelpvXzB2MFIzRQ?oc=5)
- [ ] **Operational Hallucination and Safety Drift in AI Agents** — ツール利用型エージェントでは、単発応答の安全性だけでなく、複数ターンの実行中に初期の安全制約が劣化する「safety drift… 〔技術: マルチステップ計画、ツール呼び出し、状態保持が絡むことで、従来の静的…／人文: 人間社会の信頼は「最初に正しいこと」ではなく「途中で変質しないこと」…〕 · [arxiv.org](https://arxiv.org/abs/2607.18366v1)
- [ ] **自律するAIの時代：AIエージェントのサイバーリスクと実践的ガバナンス / AI-CAL関連議論** — 日本語圏では、AIエージェントを「デジタル従業員」として迎える組織が、統制保証水準、サイバーリスク、権限管理、監査責任をどう整え… 〔技術: 本番投入前の権限管理、ログ、評価、インシデント対応をレベル分けするこ…／人文: 「AIを従業員のように扱う」比喩は便利だが、人間の労働者とは権利も責…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiigFBVV95cUxNT2liSVVKSnRWd0k2eTFGSkZBMXlBQ19xVDFMWmx4WVRkX2FjNVJtd3Q2SlhYa1NQRTdVVU5Wa25fdXVpZUlsSGJMb1llQ2VlekxWSHMyOG1qSFZSX1llTjJFNG1Ram1jRnNXOTd5MThvQUpIZWRSY2g4al85VUdxZW5kMU5qbzVkRGc?oc=5)
- [ ] **中国のAI倫理・AIエージェント規制と感情交流サービス規制** — 中国では国際AI倫理行動計画、リスク階層化、AIエージェントのリコール構想、感情交流型AIサービスへの規制が報じられている。 〔技術: リコール可能性やリスク階層化は、モデル更新、エージェントID、監査ロ…／人文: 感情交流AIや仮想恋人・家族への依存リスクは、文化差とケア倫理を強く…〕 · [news.google.com](https://news.google.com/rss/articles/CBMixgFBVV95cUxQamZNNUpkcmIzamg1clFsbTlLcFJPNmFMWmp2ajlKVnVBeEhEeWJuV2diMEo0bDNuUHRJdDMzNlZDSVpqTlRySWFzbExNcFBpUkJDenY5Tk84anAxdWNjTlFQZ0w3WWJfVFF2SzNOZ2NPZHVWcmFYRE5Ia2tMV3JoTkJIZkFHRjl3MDZQdVNTdFY0UFoxVExJUmlKbFpWVFBhaU1jSnFlcW5oTWhEeUlGa211bmxkaEhxekJkWGZQdDNnYkxiZmc?oc=5)

### Philosophy of Loop Engineering
- [ ] **Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control** — 自律的なコーディングエージェントの「reviewed」「tested」「DONE」といった状態を、エージェントの宣言ではなく、現… 〔技術: ループを trigger / goal / verification…／人文: これは「信じるな、根拠を見よ」という認識論の実装であり、AI時代のプ…〕 · [arxiv.org](http://arxiv.org/abs/2607.14890v1)
- [ ] **Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting** — 「エージェントを逐次プロンプトで手取り足取り動かす」のではなく、trigger、goal、verification step、s… 〔技術: コーディングエージェント運用の単位を「良いプロンプト」から「検証と停…／人文: 実践知の観点では、熟練者の価値は一回の指示文ではなく、失敗から学び続…〕 · [arxiv.org](http://arxiv.org/abs/2607.00038v1)
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — AIエージェントがツール利用・委任・経験学習・自己変更を行う持続的チームになる状況で、「何ができるか」より「誰が、何に変化してよ… 〔技術: ループの対象を単体タスクから、エージェントチームの自己進化・権限・ポ…／人文: サイバネティクス的に見ると、ここでの問題は制御ではなく「制御される制…〕 · [arxiv.org](http://arxiv.org/abs/2607.10878v1)
- [ ] **NVIDIA-labs OO Agents: Native Python Object-Oriented Agents** — エージェントをプロンプト、ツールスキーマ、コールバック、ワークフローグラフに分散させる代わりに、Pythonオブジェクトとして扱… 〔技術: ループを抽象的なワークフローではなく、テスト・トレース・型契約を持つ…／人文: オブジェクト指向は、世界を「性質を持ち、行為できるもの」として分節す…〕 · [arxiv.org](http://arxiv.org/abs/2607.20709v1)
- [ ] **AutoPersonas: A Multi-Timescale Loop Engine for Open-Ended Persona Evolution** — 長期的な persona agent が、同一性を保ちながら新しい出来事・関係・証拠・社会条件へ適応するための multi-ti… 〔技術: 反復を単一のタスク完了ループではなく、短期イベント、記憶、環境、アイ…／人文: これはエージェントの「自己」とは何かを、固定されたプロフィールではな…〕 · [arxiv.org](http://arxiv.org/abs/2607.08252v1)

### Anthropology of Agentic AI
- [ ] **A Framework of User Experience Principles for Human-AI Agent Interaction in the Workplace** — 職場でAIエージェントが業務フローに組み込まれる際のUX原則を、参加型デザイン、専門家レビュー、メタ分析、インタビューを組み合わ… 〔技術: エージェントの能力評価だけでなく、業務画面・承認点・説明性・ユーザー…／人文: エージェントを職場の「道具」ではなく、人間が相互行為する相手として捉…〕 · [arxiv.org](https://arxiv.org/abs/2607.19941)
- [ ] **AIエージェント最新動向2026｜製造業DXと自律型AIの現在地** — 在タイ日系製造業の視点から、エージェントAIがPoC止まりのチャットボットから、生産計画、受注処理、保全、トレーサビリティ、知識… 〔技術: 受注・在庫・工程・設備・品質記録を横断するエージェントには、モデル選…／人文: 「現場」「ベテランの暗黙知」「紙の日報」「工場長の移動中の音声指示」…〕 · [tomastc.com](https://tomastc.com/blog/ai-agent-manufacturing-2026)
- [ ] **The Organizational Behavior of Agentic AI: Collective Intelligence in Human-Agent Workflows** — エージェントAIを単体のアシスタントではなく、プランナー、ソルバー、レビュアー、メモリ管理者、ツール利用者、オーケストレーターか… 〔技術: マルチエージェントの安定性を、個々の推論能力ではなく、コンテキスト設…／人文: 「組織らしさ」は人間の動機や帰属意識から来るという前提を揺さぶり、A…〕 · [arxiv.org](https://arxiv.org/abs/2606.30986)
- [ ] **2026 Work Trend Index report: Agents, human agency, and opportunity** — Microsoft 365の利用シグナルと10カ国2万人のAI利用者調査をもとに、エージェントが実行を担うほど、人間には意図設定… 〔技術: Microsoft 365内のアクティブなエージェント数の急増、品質…／人文: 「人間のagency」を、自由時間の増加ではなく、仕事の意図・判断・…〕 · [microsoft.com](https://www.microsoft.com/en-us/worklab/work-trend-index/agents-human-agency-and-the-opportunity-for-every-organization)
- [ ] **The agentic reality check: Preparing for a silicon-based workforce** — 多くのエージェントAI導入が既存プロセスの自動化に留まり失敗しており、価値は「人間向けに作られた仕事」をエージェントネイティブに… 〔技術: MCP、A2A、ACPのようなプロトコル、デジタルID、暗号的な取引…／人文: 「HR for agents」という比喩は危うくも強力で、労働者概念…〕 · [deloitte.com](https://www.deloitte.com/us/en/insights/topics/technology-management/tech-trends/2026/agentic-ai-strategy.html)

### History of Automation
- [ ] **Lowering the implementation barrier of neutral-atom quantum computing with agentic workflows** — 量子プロトコルをクラウド上の中性原子量子プロセッサで実行するまでの工程を、エージェント型ワークフローで自動化する研究。 〔技術: 自動化の対象が単純作業ではなく、プロトコル設計、コンパイル、シミュレ…／人文: これは産業革命期の機械化よりも、研究室の技能伝承や職人知をどう形式化…〕 · [arxiv.org](https://arxiv.org/abs/2607.25834)
- [ ] **NNStar: An end-to-end AI agent for nuclear matter and neutron star physics** — 中性子星物理における高次元パラメータ探索と制約照合を、LLMエージェントのポータブルなスキルとして自動化する研究。 〔技術: 科学計算の自動化が、固定パイプラインではなく「スキル」として持ち運べ…／人文: 自動化の歴史では、工場の治具や標準作業書が労働を再編したが、ここでは…〕 · [arxiv.org](https://arxiv.org/abs/2607.13930)
- [ ] **The Anthropic Economic Index** — Claudeの利用データから、職業・地域ごとにAIが仕事を「補助」しているのか「委任」されているのかを可視化するインデックス。 〔技術: エージェント利用を抽象論ではなく、実際のタスク委任ログに近い粒度で観…／人文: 自動化史の大きな争点は「機械が人を置き換えたか」だけでなく、「仕事の…〕 · [anthropic.com](https://www.anthropic.com/economic-index)
- [ ] **Human-in-the-Loop Nugget Annotation for Accountable LLM-as-a-Judge Evaluations** — LLM-as-a-Judge評価で、人間が重要情報の「nugget」を特定し、LLMが大量の照合を担うという分業設計を提案する研… 〔技術: 評価自動化の信頼性を、全部自動化するのではなく、人間の認知負荷とLL…／人文: これは「人間の監督」という言葉の空洞化に対する批判でもある。〕 · [arxiv.org](https://arxiv.org/abs/2606.29033)
- [ ] **Applying AI to Rebuild Middle Class Jobs** — David Autorによる、AIを中間層の仕事の再建に使えるかを論じるワーキングペーパー。 〔技術: AIを「人間の熟練を奪う装置」だけでなく、判断支援によって職務範囲を…／人文: 自動化の歴史はラッダイト的抵抗の物語に縮約されがちだが、この論点は「…〕 · [nber.org](https://www.nber.org/papers/w32140)

### DDD
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — DDDを、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの特定、集約設計、技術アーキテ… 〔技術: DDD実践をLLM向けワークフローに分解し、どこまでが支援可能で、ど…／人文: ユビキタス言語は単なる用語集ではなく、組織の合意形成そのものであるこ…〕 · [arxiv.org](https://arxiv.org/abs/2603.26244)
- [ ] **DDD Europe 2026 - Software Modelling & Design Conference** — Antwerpで開催されたDDD Europe 2026の公式ページが、戦略的設計、イベント駆動アーキテクチャ、マイクロサービス… 〔技術: DDDがマイクロサービスやイベント駆動だけでなく、社会技術システム全…／人文: 「設計」はコード構造ではなく、人々が何を重要と見なし、どの境界で責任…〕 · [2026.dddeurope.com](https://2026.dddeurope.com)
- [ ] **KanDDDinsky 2026: The art of business software** — Berlinで2026年10月14〜16日に開催予定のコミュニティ主導DDDカンファレンス。 〔技術: DDDをツールやフレームワークではなく、モデリング、ワークショップ、…／人文: 「business softwareのアート」という言い方が示す通り…〕 · [kandddinsky.de](https://kandddinsky.de)
- [ ] **EventStorming: collaboration beyond silo boundaries** — EventStorming公式サイトは、複雑なビジネスドメインを探索するためのワークショップ形式として、サイロ境界を越えた協働、… 〔技術: イベントを中心に業務の因果・時系列・境界を可視化するため、LLMやエ…／人文: EventStormingの核心は付箋そのものではなく、声の大きい人…〕 · [eventstorming.com](https://www.eventstorming.com)
- [ ] **Event-Native Data for AI Agents – Better Context, Better Reasoning** — KurrentはAIエージェントに必要な文脈として、イベントネイティブなデータ、履歴、因果関係、監査可能性を訴求している。 〔技術: イベントソーシング的な履歴と再生可能性を、AIエージェントのコンテキ…／人文: 組織の記憶をベクトル検索だけに預けるのではなく、業務上の出来事と責任…〕 · [kurrent.io](https://www.kurrent.io/agentic-ai)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

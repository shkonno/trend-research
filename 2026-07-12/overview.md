# 📰 2026-07-12 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — 【2026年最新】もう単なる要約ツールじゃない！ · [note.com](https://note.com/deela/n/nea59676944e2)
- **Loop engineering** — Test-Time Harness Evolution（TTHE） · [arxiv.org](https://arxiv.org/abs/2607.08124v1)
- **AWS** — OAuth support for the AWS MCP Server · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/oauth-aws-mcp-server)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **【2026年最新】もう単なる要約ツールじゃない！進化しすぎたGoogleの「NotebookLM」完全攻略ガイド** — 日本語圏の利用者向けに、NotebookLMを「自分が提供した資料の中だけで動作するクローズド型AI」と位置づけ、PDF、Web… 〔技術: ソースグラウンディング、引用確認、マルチモーダル入力、Studio系…／人文: 「読む」「整理する」「理解を確認する」という知的労働が、個人の机上か…〕 · [note.com](https://note.com/deela/n/nea59676944e2)
- [ ] **Building AI tailored for education, with educators in the lead** — Googleは、教師主導のAI体験をGoogle Classroom、GeminiのGuided Learning、study… 〔技術: NotebookLMが単体ツールではなく、LMSやClassroom…／人文: AI家庭教師を学生に直接渡すのではなく、教師の判断と教材選択を前提に…〕 · [blog.google](https://blog.google/products-and-platforms/products/education/iste-2026-educator-updates)
- [ ] **NotebookLM is transforming student success at FSU** — Florida State UniversityがNotebookLMを学生の学習支援に使う事例です。 〔技術: 教員が提供したコース資料だけに根拠づけることで、汎用チャットAIより…／人文: 「わからない」と言うタイミングを学生が選べる24時間の補助線は、質問…〕 · [blog.google](https://blog.google/products-and-platforms/products/education/florida-state-university-notebooklm)
- [ ] **X+Slides: Benchmarking Audience-Conditioned Slide Generation** — ソース文書からスライドを作るLLMの評価で、専門家、意思決定者など「聴衆」に応じた有用性を測るX+Slidesベンチマークを提案… 〔技術: NotebookLM的なソース依存の生成物を、聴衆別のカバレッジ、効…／人文: 同じ資料でも、研究者、経営者、学生では「重要な情報」が違います。〕 · [arxiv.org](https://arxiv.org/abs/2606.19256v1)
- [ ] **Do better research with NotebookLM** — GoogleはNotebookLMに、Gemini 3.5とAntigravityによる高度な推論、コード実行用のセキュアなクラ… 〔技術: ノート内のソースをもとにコード実行、データ可視化、文書生成まで行うた…／人文: 「調査」と「執筆」と「資料作成」の境界が薄れ、研究者や学生がどこまで…〕 · [blog.google](https://blog.google/innovation-and-ai/products/notebooklm/better-research-notebooklm)

### Loop engineering
- [ ] **Test-Time Harness Evolution（TTHE）** — LLMエージェントの振る舞いはモデルだけでなく、文脈構築、ツール呼び出し、検証、失敗回復を担う「ハーネス」によって決まる、という… 〔技術: プロンプト改善ではなく、ツール実行・検証・回復を包む実行ハーネスを最…／人文: philosophy の観点では、知能を「頭の中の推論」ではなく、環…〕 · [arxiv.org](https://arxiv.org/abs/2607.08124v1)
- [ ] **AgentTether: Graph-Guided Diagnosis and Runtime Intervention for Reliable LLM Agent Operation** — マルチステップで状態を持つLLMエージェントでは、初期の判断ミスが後続の外部状態変更に連鎖します。 〔技術: エージェントの「軌道」をグラフとして扱い、失敗箇所の診断と介入をラン…／人文: ethics の観点では、自律システムに「あとから止める・ほどく・介…〕 · [arxiv.org](https://arxiv.org/abs/2607.06273v1)
- [ ] **Biological Motifs for Agentic Control** — LLMが自律エージェント化する中で、幻覚の連鎖、無限ループ、状態管理の不安定さが課題になると整理し、生物システムの制御モチーフを… 〔技術: 無限ループや状態暴走を、単なるバグではなく制御アーキテクチャの欠落と…／人文: anthropology の観点では、人間組織も儀礼・監督・例外処理…〕 · [arxiv.org](https://arxiv.org/abs/2607.04240v1)
- [ ] **LangGraph overview / Thinking in LangGraph** — LangGraph は、一般的なLLM・ツール呼び出しループの上に、durable execution、streaming、hu… 〔技術: 状態・ノード・割り込み・チェックポイントを明示することで、エージェン…／人文: philosophy の観点では、完全自律ではなく「どこで人間に戻す…〕 · [docs.langchain.com](https://docs.langchain.com/oss/python/langgraph/overview)
- [ ] **Claude Code Hooks reference** — Claude Code の Hooks は、SessionStart / UserPromptSubmit / PreToolU… 〔技術: ループ内のイベント境界をAPI化することで、lint、テスト、権限チ…／人文: ethics の観点では、AIの行為を事後的に叱るのではなく、行為の…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)

### AWS
- [ ] **OAuth support for the AWS MCP Server** — AWS MCP Server が AWS Sign-In による OAuth 接続をサポートし、AI エージェントが追加の認証ソ… 〔技術: MCP、OAuth、IAM 条件キー、トークン検証がつながり、エージ…／人文: AI エージェントの普及で重要になるのは賢さだけでなく、誰が・何に・…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/oauth-aws-mcp-server)
- [ ] **Introducing Claude apps gateway for AWS** — Claude Code と Claude Desktop の利用を、Amazon Bedrock と Claude Apps A… 〔技術: Claude クライアントをそのまま使いながら、Bedrock 経由…／人文: 生成 AI ツールは個人の創造性を増幅する一方で、企業では「自由に使…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-apps-gateway-for-aws)
- [ ] **AWS DMS Schema Conversion now supports AI agent automation** — AWS DMS Schema Conversion が AWS MCP Server 経由の AI エージェント自動化に対応し、… 〔技術: データベース移行という手順依存で失敗コストの高い作業が、MCP スキ…／人文: レガシー移行は単なる技術負債処理ではなく、組織の記憶を新しい環境へ翻…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-dms-sc-ai-agent-automation-mcp-server)
- [ ] **AWS Security Hub now offers Network Scanning to identify publicly reachable resources** — AWS Security Hub に Network Scanning が追加され、インターネットから実際に到達可能な AWS… 〔技術: CSPM 的な設定評価に、実際の外部到達性スキャンが加わることで、マ…／人文: セキュリティは「設定したつもり」と「外から見えている姿」のずれから事…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-network-scanning)
- [ ] **AWS Builder Center Now Offers Free Sandbox Environments** — AWS Builder Center が、対象ワークショップから無料・時間制限付きのサンドボックス環境をリクエストできるようにな… 〔技術: 8時間の一時的な AWS 環境を学習用に提供することで、IAM、課金…／人文: クラウド学習の障壁は知識だけでなく、失敗したら請求が来るかもしれない…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-builder-center-sandbox)

> 欠落トピック（9）: Harness engineering、sharp LLM usage、AI agent trends、Claude Code、Ethics of AI Agents、Philosophy of Loop Engineering、Anthropology of Agentic AI、History of Automation、DDD

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

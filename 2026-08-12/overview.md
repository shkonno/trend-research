# 📰 2026-08-12 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — Try notebooks in Gemini to easily keep track of projec… · [news.google.com](https://news.google.com/rss/articles/CBMid0FVX3lxTE13MGtzOEJRb3NMNk4zLXJDZnl3Qll2Q254bUtJYk4zZGFpWVJCNWVsekpHZy1ZVGRwRThtanh3UXpkWW9BeHhDR19jUjNPT0dNYjExNVpDSXBuWlVLNXF5T0pvRVphaTRZLWhtSnlQSWwyTTZoMVow?oc=5)
- **Loop engineering** — LoopsBench: From Harness Engineering to Loop Engineeri… · [arxiv.org](https://arxiv.org/abs/2608.00267)
- **AWS** — Amazon Bedrock AgentCore runtime instances が一般提供開始 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/aws-bedrock-agentcore-runtime-instances-generally-available)
- **Harness engineering** — Claude Code Hooks reference が、Stop/PreToolUse/Task 系まで… · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
- **sharp LLM usage** — Best practices for Claude Code: コンテキストを最重要資源として扱い、検証ルー… · [code.claude.com](https://code.claude.com/docs/en/best-practices)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **Try notebooks in Gemini to easily keep track of projects** — Google公式ブログで、Gemini内のnotebooksをプロジェクト管理・資料整理のために使う流れが紹介された。 〔技術: RAG型ノートがGemini本体の作業単位に統合されると、ファイル束…／人文: ノートは単なる記録ではなく「考える場所」なので、AIがそこに入ること…〕 · [news.google.com](https://news.google.com/rss/articles/CBMid0FVX3lxTE13MGtzOEJRb3NMNk4zLXJDZnl3Qll2Q254bUtJYk4zZGFpWVJCNWVsekpHZy1ZVGRwRThtanh3UXpkWW9BeHhDR19jUjNPT0dNYjExNVpDSXBuWlVLNXF5T0pvRVphaTRZLWhtSnlQSWwyTTZoMVow?oc=5)
- [ ] **New NotebookLM: Agentic Chat, Code Execution, New Formats** — 「Agentic Chat」「Code Execution」「New Formats」を掲げ、NotebookLMが要約・Q&A… 〔技術: ノート内ソースを根拠にしたチャットがコード実行や形式変換まで持つと、…／人文: 「ノートがエージェント化する」ことは、知的作業の主体が曖昧になる出来…〕 · [news.google.com](https://news.google.com/rss/articles/CBMikgFBVV95cUxNUksxRDRMLWRHY1l4RENTeHc2RjNXYm5Nb3ZCMExCY3IyMUpRS1dxQkRub1hIOGItRkR0Qi1pZGdtSlhCNDBZcGNsOUNoa1dFNmdVUTlNZjREV29aVlA3NDk4RDh4Zl9rNUEwTi05Nm1faE04MXY0WUJQcGZsbWlwSDBqQy1vbk4yQXMtWG44ZHVaUQ?oc=5)
- [ ] **Gemini Notebook turned my forgotten Kindle highlights into an interview with a year of my own reading** — Kindleハイライトのような個人の読書ログをGemini Notebookに入れ、1年分の読書を「自分へのインタビュー」のよう… 〔技術: 個人アーカイブをソースとして会話形式に変換することで、静的メモが再読…／人文: 読書メモをAIが語り直すと、記憶は単なる保存物ではなく「再解釈される…〕 · [news.google.com](https://news.google.com/rss/articles/CBMibEFVX3lxTE52LUt1bkZMYUVyTHFGN2pqT1ExSFZya2pCZ2VJZnQycFdpNzMxLUM4VTlVUlBjMU1GdzY5a1pGX0hpbTZOcFprcngtZGpQSWp2LTlGM3g1Zl8teEpJLTh0ampXSHozcTZUdEdMaA?oc=5)
- [ ] **NotebookLMとは？機能・料金・活用事例** — 日本語圏の企業向けに、NotebookLMの機能・料金・活用事例を整理した解説記事。 〔技術: 日本語資料を含む業務ドキュメントの要約・検索・比較に使えるRAGツー…／人文: 企業内ノートは組織の記憶そのものなので、NotebookLM導入は知…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiXkFVX3lxTFBvVzFGYkdEcnF6bWlRNTJpak4wb0tZUDU2Vmc4U19wYjJNYlJOM0xrX1A5ZTY0Um1lQnNpajdCdVliWWJ3bk1GejNuMzVjYVVOV1VLNDFEODRyd0FCeXc?oc=5)
- [ ] **Modeling turn-taking with distant viewing: investigating silence thresholds in human and AI-generated discourse** — 米国シットコム30本と、Google NotebookLMで生成された合成ポッドキャスト51本の無音ギャップを比較し、人間の会話… 〔技術: NotebookLM生成音声の発話間隔を定量化することで、合成会話の…／人文: 沈黙や間は文化的な意味を持つため、AIが作る会話のテンポは単なる音声…〕 · [arxiv.org](https://arxiv.org/abs/2607.18076)

### Loop engineering
- [ ] **LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation** — Microsoft の LoopsBench は、112タスク・5,300以上の開発ユニット・依存DAG・Docker実行・単体… 〔技術: エージェント評価を「最終成果物」から、ready frontier、…／人文: ethics の観点では、エージェントの「完了した」という自己申告で…〕 · [arxiv.org](https://arxiv.org/abs/2608.00267)
- [ ] **@cobusgreyling/loop: Loop Engineering CLI の「front door」化** — Cobus Greyling の loop-engineering リポジトリは、`loop init`、`loop docto… 〔技術: 個別スクリプト群を薄い umbrella CLI にまとめ、初期化・…／人文: creativity の観点では、開発者の創造性が「次の一文を入力す…〕 · [github.com](https://github.com/cobusgreyling/loop-engineering)
- [ ] **loopx: 長時間エージェントチーム向け状態カーネル** — `loopx` は、Codex や Claude Code などの agent loop に依存しない軽量な状態カーネルとして、… 〔技術: ループをプロンプト列ではなく、ゴール、予算、証拠、handoff を…／人文: philosophy の観点では、主体性を「モデルの賢さ」ではなく「…〕 · [github.com](https://github.com/huangruiteng/loopx)
- [ ] **loop-kit-core: 無人実行エージェントのセキュリティ契約** — `loop-kit-core` は「loop engineering はループ設計を教えるが、loop-kit は誰も見ていない… 〔技術: unattended loop に対して、権限・認証情報・実行境界を…／人文: ethics の観点では、「便利だから自動化する」から「誰が、どの権…〕 · [github.com](https://github.com/PostOrganic-AI/loop-kit-core)
- [ ] **intent-gate: 実装前に意図整合性を強制する Human-in-the-loop ゲート** — `intent-gate` は、Claude Code plugin と MCP server により、AI coding ag… 〔技術: 実装ループの前に、状態機械・シーケンス図・意思決定表を契約として固定…／人文: narrative の観点では、コード生成の物語を「エージェントが何…〕 · [github.com](https://github.com/baixinghao/intent-gate)

### AWS
- [ ] **Amazon Bedrock AgentCore runtime instances が一般提供開始** — Amazon Bedrock AgentCore の runtime instances が一般提供され、AIエージェントを自分… 〔技術: 最大14日級の持続セッションやEC2インスタンスタイプ選択を前提に、…／人文: エージェントを人間の同僚のように長く働かせるには、記憶・責任・中断可…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/aws-bedrock-agentcore-runtime-instances-generally-available)
- [ ] **Amazon DynamoDB がリアルタイムベクトル検索をサポート** — DynamoDB にネイティブなベクトル検索が一般提供され、単一桁ミリ秒レイテンシ、99%以上のリコール、数十億から数兆ベクトル… 〔技術: RAGや推薦の検索層を既存のキー・バリュー/ドキュメントDBへ寄せる…／人文: 「意味」を検索可能なインフラに埋め込む動きは、業務システムが人間の分…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-dynamodb-vector-search)
- [ ] **AWS Continuum が Claude Code / Codex / Kiro の開発者ワークフローへ統合** — AWS が Anthropic および OpenAI と協業し、AWS Continuum for code vulnerabi… 〔技術: セキュリティスキャンをCIの後段だけでなく、AIコーディングエージェ…／人文: セキュリティが「監査する別部門」から「開発中に話しかけてくる共同編集…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/security/aws-partners-with-anthropic-and-openai-to-bring-aws-continuum-into-developer-workflows)
- [ ] **Amazon Bedrock が OpenAI GPT モデル向け Web Search を一般提供** — Amazon Bedrock で OpenAI GPT-5.4、GPT-5.5、GPT-5.6 Sol/Terra/Luna 向… 〔技術: モデル呼び出し、Webグラウンディング、ガバナンスをBedrock側…／人文: 検索がモデルの内蔵ツールになると、ユーザーは情報源を意識しにくくなり…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-web)
- [ ] **Agent Plugins 1.0.0 と Kiro powers 対応で、エージェント拡張のポータビリティが前進** — AWS は Cursor、Microsoft、OpenAI、Vercel とともに Agent Plugins Technica… 〔技術: エージェント拡張をIDEやベンダーごとに作り分けるのではなく、MCP…／人文: 開発者の道具箱がポータブルになることは、特定プラットフォームへの囲い…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-supports-agent-plugins-an-open-standard-for-portable-agent-extensions)

### Harness engineering
- [ ] **Claude Code Hooks reference が、Stop/PreToolUse/Task 系まで含む実行制御面を明文化** — Claude Code の hooks 参照には、PreToolUse / PostToolUse / PermissionDe… 〔技術: フックは自然言語ルールを実行時ポリシーに落とす接合部で、stop-h…／人文: これは「AIに何を言い聞かせるか」ではなく「組織がどこで介入責任を負…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [ ] **Claude Code 2.1.222 の worktree 隔離・PreToolUse 修正が、ハーネス安全性の実運用論点を浮かび上がらせた** — リリースノートでは、worktree 隔離セッションとその subagent がメイン checkout に対して破壊的 git… 〔技術: worktree isolation、Bash/file edit…／人文: 自律エージェントの失敗はしばしば「悪意」ではなく、権限境界の曖昧さか…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/release-notes/claude-code)
- [ ] **arXiv: SHE — Trajectory-driven Safety Harness Evolution for LLM Agents** — SHE は、LLM agent の安全性をモデル重みだけでなく、context、memory、tools、permissions… 〔技術: 実行軌跡を入力にして harness コンポーネントの安全責任を再配…／人文: これは「安全なAIを一度作れば終わり」という神話への反論でもある。〕 · [arxiv.org](http://arxiv.org/abs/2608.09885v1)
- [ ] **oh-my-agent — stop-hook gates / independent judges / append-only event logs を掲げる multi-agent harness** — GitHub 検索で、Claude Code、Codex、Cursor など複数ランタイムをまたぎ、成果物ベースで agent… 〔技術: 複数エージェント／複数ランタイムを同じ監査ログと判定器に通すことで、…／人文: 「AIが作ったから信じる」のではなく「証跡と第三者的判定で信頼を組み…〕 · [github.com](https://github.com/first-fluke/oh-my-agent)
- [ ] **日本語コミュニティで CLAUDE.md / Hooks / ハーネス入門が急増** — Qiita API 検索では「CLAUDE.mdに何を書けばいいか分からない人向け｜ハーネスエンジニアリングの最初の一歩」（20… 〔技術: CLAUDE.md を静的ルール、Hooks を動的制御、センサーを…／人文: 日本語コミュニティでは「AIに仕事を任せる不安」を、人格論ではなく作…〕 · [qiita.com](https://qiita.com/shun123/items/c28d04b6ded6afe60847)

### sharp LLM usage
- [ ] **Best practices for Claude Code: コンテキストを最重要資源として扱い、検証ループを渡す** — Claude Codeの実践指針として、コンテキストウィンドウが埋まると性能が落ちるため、読み込ませる情報とコマンド出力を管理す… 〔技術: LLM活用を「指示文」ではなく、コンテキスト予算、実行ログ、合否判定…／人文: 人間の役割が「コードを書く人」から「完了条件と証拠を設計する人」へ移…〕 · [code.claude.com](https://code.claude.com/docs/en/best-practices)
- [ ] **Master Prompt Agreement: ファイルベースの権限・文脈・検証契約** — Master Prompt Agreementは、コードエージェントに対してプロジェクト権限、現在の事実、ワークフロー経路、情報… 〔技術: 長い会話に重要ルールを埋めるのではなく、権限・状態・手順・証拠をリポ…／人文: これはAIに「お願い」する文化から、AIと作業するための制度・憲章を…〕 · [github.com](https://github.com/laurenzpavlosmalisianos/master-prompt-agreement)
- [ ] **SHE: Trajectory-driven Safety Harness Evolution for LLM Agents** — LLMエージェントの安全性をモデル重みだけでなく、コンテキスト、メモリ、ツール、権限、実行制御を扱う「ハーネス」の問題として捉え… 〔技術: 実運用の失敗ログを、プロンプト・ルール・メモリ・ツールポリシーのどこ…／人文: 失敗を個人のプロンプト技量に押し戻さず、仕組みの学習材料として扱う点…〕 · [arxiv.org](http://arxiv.org/abs/2608.09885v1)
- [ ] **Decoding-Level Taboo: A Diagnostic Stress Test for LLM Robustness** — 通常ベンチマークではモデルが最適化された生成経路を進むため、実運用での複雑なシステムプロンプト、安全ガード、構造制約下の弱さが見… 〔技術: 「普通に聞いたら答えられる」ではなく、制約やガードレールで生成経路が…／人文: 人間の組織でも、平時の有能さと例外時の信頼性は違う。〕 · [arxiv.org](http://arxiv.org/abs/2608.09900v1)
- [ ] **10 Claude Code Best Practices for Agentic Coding: 計画、分割、コミット、レビューの作法** — Claude Codeの実務パターンとして、読み取り専用のplan modeで探索し、計画を人間がレビューし、一度に大きく任せず… 〔技術: エージェントの自律性を上げるほど、探索・計画・実装・検証・コミットを…／人文: 「AIに任せる」は放任ではなく、共同作業のリズムを設計することだと分…〕 · [openhands.dev](https://www.openhands.dev/blog/claude-code-best-practices-agentic-coding)

> 欠落トピック（7）: AI agent trends、Claude Code、Ethics of AI Agents、Philosophy of Loop Engineering、Anthropology of Agentic AI、History of Automation、DDD

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

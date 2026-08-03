# 📰 2026-08-03 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLM is now Gemini Notebook · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/07/notebooklm-now-gemini-notebook.html)
- **Loop engineering** — When Do Agent Loops Mistake Stagnation for Progress? S… · [arxiv.org](http://arxiv.org/abs/2607.25152v1)
- **AWS** — AWS Security Hub MCP App が Claude Desktop からセキュリティ所見を調… · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-mcp-app)
- **Harness engineering** — keka v0.3.0 — Claude Code 用ハーネスに prompt coach / secret… · [github.com](https://github.com/MohammedMoataz/keka/releases/tag/v0.3.0)
- **sharp LLM usage** — Boris Cherny on Trying to Get Claude Code to Rewrite t… · [daringfireball.net](https://daringfireball.net/linked/2026/08/02/cherny-claude-swift)
- **AI agent trends** — Copilot code review: Agent skills and MCP now generall… · [github.blog](https://github.blog/changelog/2026-07-29-copilot-code-review-agent-skills-and-mcp-now-generally-available)
- **Claude Code** — Claude Code v2.1.219: Opus 5 既定化、1M context、sandbox ne… · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.219)
- **Ethics of AI Agents** — Stop Shipping AI Agents on Faith: Capability Is Not Pr… · [arxiv.org](https://arxiv.org/abs/2607.27677v1)
- **Philosophy of Loop Engineering** — JarvisHub: An Open Harness for Canvas-Native Multimoda… · [arxiv.org](https://arxiv.org/abs/2607.23588)
- **Anthropology of Agentic AI** — Voice AI in Firms: A Natural Field Experiment on Autom… · [arxiv.org](http://arxiv.org/abs/2607.28222v1)
- **History of Automation** — Nonuniformity Principle in Human-AI Coworking · [arxiv.org](https://arxiv.org/abs/2607.16530)
- **DDD** — Domain-Driven Design in Practice: A Large-Scale Empiri… · [arxiv.org](http://arxiv.org/abs/2607.06471v1)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLM is now Gemini Notebook** — GoogleはNotebookLMをGemini Notebookへ改称し、既存リンクや共有ノートブックは自動リダイレクトで継続… 〔技術: リネーム自体より、ノートブックがGeminiアプリや今後のGoogl…／人文: 「LM」という研究者・技術者寄りの語から「Notebook」という日…〕 · [workspaceupdates.googleblog.com](https://workspaceupdates.googleblog.com/2026/07/notebooklm-now-gemini-notebook.html)
- [ ] **社内文書をAIに丸ごと読ませて質問する｜Gemini Notebook（旧NotebookLM）の業務活用入門** — 中小企業向けに、議事録の横断検索、社内マニュアルへの自然言語問い合わせ、競合資料・市場調査レポートの比較整理といった実践パターン… 〔技術: RAG的な「手元資料に閉じた回答」と引用確認を、非エンジニアでもすぐ…／人文: これは単なる検索効率化ではなく、組織内で“誰がどの文書を読める人か”…〕 · [qiita.com](https://qiita.com/DnD-inc/items/2798dc05b3172a8cdb7a)
- [ ] **Gemini Notebookを社内ナレッジ検索に使うための設計と運用** — 社内文書検索としてGemini Notebookを使う際、資料分類、共有範囲、古い情報の除外、引用確認、管理者設定などを設計する… 〔技術: ノートブック単位のソース管理・権限・更新ルールを明示しないと、便利な…／人文: 「同期されるから便利」と「どこでも同じ資料を使ってよい」は同義ではな…〕 · [qiita.com](https://qiita.com/mhamadajp/items/aff7f70d68bfb28dad00)
- [ ] **Modeling turn-taking with distant viewing: investigating silence thresholds in human and AI-generated discourse** — 米国シットコム30本と、Google NotebookLMで生成した合成ポッドキャスト51本を対象に、話者交替における沈黙ギャッ… 〔技術: NotebookLM生成音声を単なる便利機能ではなく、会話構造・間合…／人文: AI音声の“自然さ”は内容の正確さだけでなく、沈黙や間の取り方という…〕 · [arxiv.org](https://arxiv.org/abs/2607.18076v1)
- [ ] **Gemini Notebookの参照更新をPythonで検知する** — Gemini Notebookへ投入する資料の版を固定するため、ディレクトリ内ファイルのSHA-256を記録し、変更差分を検知す… 〔技術: 回答の再現性を高めるにはプロンプトだけでなく、投入ソースのハッシュ・…／人文: AI時代の「根拠」は、引用リンクがあるだけでは足りず、その時点でどの…〕 · [qiita.com](https://qiita.com/hironakamura_ai/items/11f8d20a42bd859e9148)

### Loop engineering
- [ ] **When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops** — 長時間動く自律エージェントが、自分の作業を自分で評価すると「進んでいるように見えるが実世界の成果は停滞・悪化する」progres… 〔技術: ループのゲートを自己申告やインバンド評価ではなく、コンテナ・ネットワ…／人文: ethics の観点では、機械の「自己評価」をそのまま労働成果や安全…〕 · [arxiv.org](http://arxiv.org/abs/2607.25152v1)
- [ ] **Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control** — 「reviewed」「tested」「DONE」「ready-to-merge」といったライフサイクル状態を、エージェントの宣言… 〔技術: エージェント出力を状態ではなく「主張」として扱い、状態遷移を証拠ゲー…／人文: philosophy の観点では、これは「知っている」と言える条件を…〕 · [arxiv.org](http://arxiv.org/abs/2607.14890v1)
- [ ] **Engineering Loop Standard** — Claude Code、Cursor、Aider、Codex、Gemini などに依存しない `engineering-loop… 〔技術: provider-independent なループ仕様とツール別アダ…／人文: anthropology の観点では、これは個人のプロンプト術がチー…〕 · [github.com](https://github.com/sergiorebolledo/engineering-loop-standard)
- [ ] **Nexus — autonomous software engineering orchestration with six gates** — 平文プロンプトから実ソフトウェアを作る自律ソフトウェアエンジニアリング用オーケストレーションエンジンで、「Agents prop… 〔技術: Agent / Executor / Validator を構造的に…／人文: ethics の観点では、責任の所在を「モデルが良いと言った」から「…〕 · [github.com](https://github.com/tanaysinha1607/Nexus)
- [ ] **Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting** — 「agent に逐次指示するのではなく、agent を動かす loop specification を設計する」という実務スロー… 〔技術: ループ仕様を、内部の perceive-act-observe サイ…／人文: philosophy の観点では、人間が命令者から制度設計者へ移ると…〕 · [arxiv.org](http://arxiv.org/abs/2607.00038v1)

### AWS
- [ ] **AWS Security Hub MCP App が Claude Desktop からセキュリティ所見を調査可能に（Preview）** — AWS Security Hub MCP App は、Security Hub の exposure findings をローカ… 〔技術: Security Hub のグラフ的な所見・攻撃パスをMCPでAIワ…／人文: セキュリティ担当者の仕事は、単なるアラート処理ではなく、組織が何を危…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-mcp-app)
- [ ] **Claude Opus 5 が Amazon Bedrock / Claude Platform on AWS で利用可能に** — AWSは、Anthropicの Claude Opus 5 を Amazon Bedrock と Claude Platform… 〔技術: Bedrock上で高性能Claude系モデルを統制・認証・監査のAW…／人文: 「賢いモデルを使える」ことより重要なのは、企業やチームがどの作業を機…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-opus-5-on-aws-anthropics-most-capable-opus-model)
- [ ] **AI coding agents 向けの速度と安全性を両立する統制フレームワーク** — AWS Security Blog は、Kiro や Claude Code のようなAIコーディングエージェントが短時間に多数… 〔技術: CodeBuild / CodePipeline などの既存CI/C…／人文: エージェントの速さは、開発組織の「信頼」の置き場所を変えます。〕 · [aws.amazon.com](https://aws.amazon.com/blogs/security/balancing-speed-and-safety-a-control-framework-for-ai-coding-agents)
- [ ] **Nitro Isolation Engine の形式的検証が日本語で詳説される** — AWS日本語ブログは、Graviton5搭載のM9g/M9gdインスタンスで使われる Nitro Isolation Engin… 〔技術: クラウド基盤の中核であるVM分離を、Rustサブセット実装と定理証明…／人文: クラウド利用者は普段、巨大なブラックボックスに信頼を預けています。〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/ec2s-formally-verified-isolation-engine-provides-mathematical-assurance-of-virtual-machine-isolation)
- [ ] **Amazon S3 Tables が Apache Iceberg V3 の Variant データ型をサポート** — Amazon S3 Tables は Apache Iceberg V3 の Variant データ型をサポートし、JSONのよ… 〔技術: データレイクにありがちな「まずスキーマを決める」摩擦を下げつつ、Ic…／人文: データの形は、組織の現実がまだ固まっていないことを映します。〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-s3-tables-variant-iceberg-v3)

### Harness engineering
- [ ] **keka v0.3.0 — Claude Code 用ハーネスに prompt coach / secrets guard / conventions を追加** — `keka` は “A harness for Claude Code” を掲げる新しい OSS で、v0.3.0 では曖昧なプ… 〔技術: Claude Code の内部推論ではなく PreToolUse 的…／人文: これは開発者の注意力や倫理観だけに安全を委ねない設計であり、AI時代…〕 · [github.com](https://github.com/MohammedMoataz/keka/releases/tag/v0.3.0)
- [ ] **Claude Code Hooks 公式ドキュメント — deterministic control をハーネスの中核に置く** — 公式の Hooks ガイドは、Claude Code の特定ライフサイクルでシェルコマンドを自動実行し、フォーマット、通知、コマ… 〔技術: LLM が自発的に守るルールではなく、ツール呼び出しの前後に決定的な…／人文: 「賢いモデル」への信頼を、「止める・記録する・確認する」仕組みへの信…〕 · [code.claude.com](https://code.claude.com/docs/en/hooks-guide)
- [ ] **Claude Code と Codex の作業履歴を SQLite に貯め、hook 遅延を 268ms から p95 17ms へ落とした日本語実践例** — Claude Code / Codex の hook で作業履歴を自動収集する `agent-history` を作ったところ、… 〔技術: エージェントの観測可能性を高めるハーネスは、同期 I/O をクリティ…／人文: AI開発では「結論のコード」だけでなく「考えた過程」が失われがちで、…〕 · [qiita.com](https://qiita.com/heboHebo-san/items/0edf082cd00ae5a3be2e)
- [ ] **Stop Shipping AI Agents on Faith — ProofAgent Harness と PAI による本番準備度評価** — “Capability is not production readiness” を掲げ、AIエージェントを能力デモだけで出荷せ… 〔技術: 単発ベンチマークではなく、実行環境、規制遵守、運用承認、監査可能性ま…／人文: エージェントの「できる」は、社会的に「任せてよい」と同義ではない。〕 · [arxiv.org](https://arxiv.org/abs/2607.27677)
- [ ] **AgentS4D — Claude Code / Hermes / Codex などを含むワークスペースエージェントの実行時リスク評価ベンチマーク** — AgentS4D は、LLMベースのワークスペースエージェントについて、外部ツール、永続状態、副作用をまたぐライフサイクル全体で… 〔技術: プロンプト単体の安全性ではなく、ツール呼び出し、状態変化、実行後証拠…／人文: エージェントの危険は「悪い返答」だけでなく、ファイル変更、権限、ログ…〕 · [arxiv.org](https://arxiv.org/abs/2607.27294)

### sharp LLM usage
- [ ] **Boris Cherny on Trying to Get Claude Code to Rewrite the Claude App** — Claude Code責任者のBoris Chernyが、Claude CodeでClaudeアプリを書き換えようとした話を通じ… 〔技術: LLM活用のボトルネックを、プロンプトの言い回しから、作業単位・コン…／人文: 「AIに仕事を頼む」とは、命令者になることではなく、編集者・教師・同…〕 · [daringfireball.net](https://daringfireball.net/linked/2026/08/02/cherny-claude-swift)
- [ ] **The new rules of context engineering for Claude 5 generation models** — Claude 5世代モデル向けに、長いコンテキストをただ詰め込むのではなく、目的に合う情報を選び、順序づけ、不要なノイズを減らす… 〔技術: 長文コンテキスト時代の性能改善を、RAG・ファイル投入・システム指示…／人文: 人間の仕事でも「必要な背景をどう共有するか」が共同作業の質を決める。〕 · [claude.com](https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models)
- [ ] **Ubiquitous Language is prompt engineering that humans can read** — LLMは構文よりもドメイン理解でつまずくため、DDDのユビキタス言語を「人間も読めるプロンプトエンジニアリング」として使うべきだ… 〔技術: DDDの用語集、境界づけられたコンテキスト、ドメインルールを、LLM…／人文: これはAI時代の設計文書が「機械への指示」だけでなく「人間同士の合意…〕 · [menelaos.vergis.net](https://menelaos.vergis.net/posts/Why-Domain-Driven-Design-Is-a-Great-Fit-for-Coding-with-Claude)
- [ ] **DFAH-Bench: same agent decision, different tool paths / Replay stability measurement for tool-using AI agents** — 金融オペレーションを題材に、ツール利用エージェントの出力ドリフトとリプレイ安定性を測るDFAH-Benchを公開している。 〔技術: 「答えが合っているか」だけでなく、エージェントが同じ状況で同じように…／人文: 実務でAIを任せるとは、結果だけでなく説明可能な手続きへの信頼を作る…〕 · [github.com](https://github.com/ibm-client-engineering/output-drift-financial-llms)
- [ ] **AISPA: User-Centric System Prompt Auditing for Large Language Model Applications** — 商用AIプロダクト88件のシステムプロンプトに含まれる3,249命令を、ユーザーに関係する8つの観点から監査し、保護的な命令と問… 〔技術: システムプロンプトをブラックボックスの魔法ではなく、命令単位で分解し…／人文: ユーザーは多くの場合、自分に影響する隠れた指示を読めない。〕 · [arxiv.org](https://arxiv.org/abs/2607.28617)

### AI agent trends
- [ ] **Copilot code review: Agent skills and MCP now generally available** — GitHub Copilot code review で、リポジトリや組織に置いた `SKILL.md` による Agent S… 〔技術: コードレビューAIが単なる差分コメント生成ではなく、社内標準・課題管…／人文: レビューは本来、組織の規範や暗黙知を受け渡す場です。〕 · [github.blog](https://github.blog/changelog/2026-07-29-copilot-code-review-agent-skills-and-mcp-now-generally-available)
- [ ] **GitHub MCP Server supports the next MCP specification** — GitHub MCP Server が、2026-07-28 に予定されるステートレス化を含む次期 MCP 仕様に先行対応しまし… 〔技術: MCP がローカルの便利プロトコルから、スケールするリモート・ツール…／人文: エージェントが多くの業務システムに触れるほど、「接続できる」だけでな…〕 · [github.blog](https://github.blog/changelog/2026-07-23-github-mcp-server-supports-the-next-mcp-specification)
- [ ] **The harness is all you need (mostly)** — 新しい MCP、スキル、プロンプト小技を追うより、まず GitHub Copilot という「ハーネス」の基本動作を理解して使い… 〔技術: エージェント活用のボトルネックを、モデルや個別ツールではなく、作業文…／人文: AI流行の「一発プロンプト」文化への反動として、職人が道具を習熟する…〕 · [github.blog](https://github.blog/ai-and-ml/github-copilot/the-harness-is-all-you-need-mostly)
- [ ] **Claude Code × AWS MCP Serverによるマルチアカウント操作** — AWS MCP Server のクロスアカウント対応を使い、Claude Code から複数 AWS アカウントを横断操作するた… 〔技術: エージェントがクラウド運用の実アカウント境界をまたぐ段階に入り、MC…／人文: 「AIにクラウドを操作させる」ことは、便利さと不安が最も近い領域です…〕 · [qiita.com](https://qiita.com/eureka_/items/cf4b7690dab316cceb1d)
- [ ] **Can Large Language Models Resolve Real Java Merge Conflicts? An Evaluation with a Calibrated LLM-as-Judge** — 実際の Java マージコンフリクトを対象に、LLM ソルバーを generate-validate-retry 型のエージェン… 〔技術: コーディングエージェント評価が「答えが合ったか」だけでなく、検証ルー…／人文: マージコンフリクトは共同作業の摩擦そのものです。〕 · [arxiv.org](https://arxiv.org/abs/2607.27674v1)

### Claude Code
- [ ] **Claude Code v2.1.219: Opus 5 既定化、1M context、sandbox network strict allowlist** — v2.1.219 は Claude Opus 5 (`claude-opus-5`) を追加し、Opus の既定モデルにした。 〔技術: 大きなコンテキストと厳格なネットワーク制御が同じリリースに並び、長時…／人文: コーディングエージェントは賢い相棒であるほど危険な実行主体にもなるた…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.219)
- [ ] **Claude Code GitHub Action v1.0: @claude から自動化ワークフローへ** — Claude Code GitHub Action v1.0 は、`mode` などの手動指定を減らし、`prompt` と `… 〔技術: CLI の能力を GitHub Actions runner 上に持…／人文: レビューコメントを書く人、Issue を整理する人、失敗した CI…〕 · [github.com](https://github.com/anthropics/claude-code-action/releases/tag/v1)
- [ ] **日本語スターターキット `claude-harness`: 毎朝パターンを取り込み、Claude Code 構成を自己更新する試み** — 日本語ファーストの Claude Code スターターキットで、最新リリースや Cookbook を毎朝調査し、`.claude… 〔技術: Claude Code を単体ツールではなく、agents、hook…／人文: 日本語圏でも「使い方メモ」から「組織の作業様式を毎日更新する装置」へ…〕 · [github.com](https://github.com/Hyphen-Tech-Org/claude-harness)
- [ ] **Zenn本教材 `go-coding-agent-handson`: “ミニClaude Code” を Go で実装して学ぶ** — 「ミニClaude CodeをGoで実装して学ぶ コーディングエージェントのしくみ」の教材リポジトリ。 〔技術: Claude Code 的なエージェントループをブラックボックスにせ…／人文: 「AIに任せる」ためには、逆説的に「AIエージェントが何をしているか…〕 · [github.com](https://github.com/toshi0607/go-coding-agent-handson)
- [ ] **arXiv `AgentRadio`: Claude Code エージェント単体より、非同期に気づきを共有する複数エージェントが強い** — AgentRadio は、長時間のコードベース理解タスクで、複数の coding agent が実行中に非同期メッセージを共有す… 〔技術: 改善の鍵をモデル単体性能ではなく、作業中の発見を中断なしに共有する…／人文: 人間の開発チームでも、成果は個人の賢さだけでなく、いつ・どう気づきを…〕 · [arxiv.org](https://arxiv.org/abs/2607.28430)

### Ethics of AI Agents
- [ ] **Stop Shipping AI Agents on Faith: Capability Is Not Production Readiness** — AIエージェントのリリース判断をデモや能力スコアだけで行う危うさを批判し、Evaluation / Context / Comp… 〔技術: エージェント評価を単一ベンチマークではなく、運用環境・コンプライアン…／人文: 「できる」ことと「任せてよい」ことを分ける発想は、責任所在を人間組織…〕 · [arxiv.org](https://arxiv.org/abs/2607.27677v1)
- [ ] **Explanation-Bound Tool Execution for AI Agents: Server-Verified Action Claims Without Trusting Model Rationales** — ツール実行エージェントの自由記述の「理由」をそのまま信頼せず、意図・ポリシー・ペイロード・リスク・来歴・鮮度などを型付きの ac… 〔技術: LLMの内省的説明ではなく、検証可能なクレームと信頼済み事実の照合で…／人文: 「説明されたから信じる」ではなく「検証できる形で説明を制度化する」と…〕 · [arxiv.org](https://arxiv.org/abs/2607.25364v2)
- [ ] **The Ethics of Autonomous AI Agents for Offensive Security** — 攻撃的セキュリティ領域の自律エージェントについて、従来のペネトレーションテストツールとは異なる「非決定性」「説明困難性」「利用者… 〔技術: 自律的な攻撃行動、LLMサプライチェーンの不透明性、低スキル利用者へ…／人文: 「善意の研究」「防御の民主化」という物語が、実際には誰の被害を増やす…〕 · [arxiv.org](https://arxiv.org/abs/2607.20255v1)
- [ ] **China's new AI rules: Ethics, AI agents and anthropomorphic AI** — 中国のAI倫理・AIエージェント・擬人化AIに関する新たな規制動向を、原則論からリスク別・運用別のルールへ進む動きとして整理して… 〔技術: エージェントの行為を consequence level に応じて分…／人文: 文化差として、中国は抽象的なAI倫理よりも、国家・産業・利用者保護を…〕 · [iapp.org](https://iapp.org/news/a/china-s-new-ai-rules-ethics-ai-agents-and-anthropomorphic-ai)
- [ ] **責任あるAI利用原則の規範化と取締役善管注意義務** — AIエージェントやフィジカルAIの導入により、発注・送金・契約締結・リソース配分などの権限委譲が財産的損害や身体・生命侵害に直結… 〔技術: 権限・監査・フォールバック・人間確認を、単なる推奨設定ではなく経営管…／人文: 日本語圏の議論では、AIエージェントの倫理が個人の道徳ではなく、組織…〕 · [ailaw.co.jp](https://ailaw.co.jp/blog/ai-governance-directors-liability-2026)

### Philosophy of Loop Engineering
- [ ] **JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents** — 長期的なマルチモーダル創作では、単発の生成結果だけでなく、参照、下書き、別案、編集、失敗、バージョン関係、ツール操作、評価信号、… 〔技術: 生成物中心ではなく、軌跡・評価信号・人間フィードバックを保存するハー…／人文: 創作を「ひらめき」ではなく、失敗と改稿を含む実践知の循環として扱って…〕 · [arxiv.org](https://arxiv.org/abs/2607.23588)
- [ ] **LoopLab: trajectory analysis, rubric-based assessment, LLM-as-judge, human review, training feedback loops** — AIエージェントの挙動を軌跡として収集し、ルーブリック評価、LLM-as-judge、人間レビュー、訓練フィードバックループへ接… 〔技術: エージェントの失敗を単なるログではなく、再評価・回帰検知・訓練データ…／人文: ここでの評価は「正解を当てる」よりも、何を失敗として名指すかという規…〕 · [github.com](https://github.com/LofiSu/LoopLab)
- [ ] **Human-Centric Reflective Architecture for Human-AI Collaborative Decision-Making** — LLMを意思決定に使う際、人間がAI助言に過度依存または過小依存する問題を背景に、人間中心の反省的アーキテクチャを提案する論文で… 〔技術: 人間フィードバックを後付けの承認ステップではなく、信頼較正と意思決定…／人文: 「反省」はモデルの自己評価だけでなく、人間が自分の依存の仕方を見直す…〕 · [arxiv.org](https://arxiv.org/abs/2607.03025)
- [ ] **Multimodal Evaluator Preference Collapse: Cross-Modal Coupling in Self-Evolving Agents** — AIエージェントが自分の出力を評価するフィードバックループでは体系的なバイアスが生じ、マルチモーダル設定では Evaluator… 〔技術: 自己改善ループは放置すると多様な戦略探索ではなく、評価器の癖に収束す…／人文: 「自分で自分を評価する」制度は、哲学的には反省の理想である一方、同じ…〕 · [arxiv.org](https://arxiv.org/abs/2606.16682)
- [ ] **Collaborative Disagreement Resolution for Scalable Oversight** — AI同士が反対立場を議論する debate 型のスケーラブル監督には、審判を説得するインセンティブが認識的誠実さとずれるという緊… 〔技術: 複数エージェントの評価ループを勝敗や説得力ではなく、不一致の局所化・…／人文: これは「真理は競争から出る」という法廷モデルから、「真理は共同で誤差…〕 · [arxiv.org](https://arxiv.org/abs/2607.01251)

### Anthropology of Agentic AI
- [ ] **Voice AI in Firms: A Natural Field Experiment on Automated Job Interviews** — 70,000人の求職者を、人間の採用担当者による面接とAI音声エージェントによる面接にランダム割付した大規模フィールド実験。 〔技術: AI音声エージェントを「判断者」ではなく、構造化されつつ応答的な情報…／人文: 採用面接は候補者が企業に「見られる」儀礼であり、企業側も候補者の語り…〕 · [arxiv.org](http://arxiv.org/abs/2607.28222v1)
- [ ] **Stop Shipping AI Agents on Faith: Capability Is Not Production Readiness** — AIエージェントの本番投入を、デモや能力ベンチマークではなく、Evaluation、Context、Compliance、Gov… 〔技術: エージェントの「できること」と「組織が監視・承認・監査できること」を…／人文: これは新しい道具を職場に入れる前の通過儀礼を形式化する試みである。〕 · [arxiv.org](http://arxiv.org/abs/2607.27677v1)
- [ ] **Toward Continuous Assurance for the Democratization of AI Agent Creation in Industry** — 低コード、ノーコード、会話型開発環境により、非エンジニアが組織内でAIエージェントを作るようになる状況を扱う。 〔技術: citizen-created agentを一回作って終わりの自動化…／人文: 現場の人が自分の慣習に合わせて小さなエージェントを作ることは、ローカ…〕 · [arxiv.org](http://arxiv.org/abs/2607.21495v1)
- [ ] **Agentic Context Management: Solving Agent Memory and Cost by Treating Them as Lifecycle and Architecture Problems** — 本番AIエージェントの失敗は推論能力だけでなく、会話履歴、巨大なプロンプト、ツール定義、ツール出力などをどのように「心に保持する… 〔技術: エージェント記憶を単なるRAGやストレージではなく、組織スコープ、忘…／人文: 組織の仕事は「何を覚え、何を忘れ、誰の文脈を正本にするか」で成立して…〕 · [arxiv.org](http://arxiv.org/abs/2607.21503v1)
- [ ] **When Bots Join the Team: Bot Adoption and the Institutional Fabric of Open-Source Software Projects** — 2,991のGitHubプロジェクトを対象に、初めてbotを採用する前後2年の変化を分析した研究。 〔技術: PR、レビュー、マージ、議論ログという具体的な開発実践から、エージェ…／人文: OSSでは「誰が返事をし、誰が記憶され、誰に権限があるか」が共同体の…〕 · [arxiv.org](http://arxiv.org/abs/2607.13679v1)

### History of Automation
- [ ] **Nonuniformity Principle in Human-AI Coworking** — 生成AIが多段階・高リスク業務を自動化するほど、人間の監督は重要になるが、すべての中間出力を人間が見ることはコスト的に難しい。 〔技術: AIエージェントの効率性と人間監督の有限性を、ワークフロー設計の最適…／人文: 産業革命期の監督労働や品質管理の歴史と同じく、「機械が速くなった後に…〕 · [arxiv.org](https://arxiv.org/abs/2607.16530)
- [ ] **The Human-AI Substitution Principle: When will you be replaced by AI in your organization?** — 組織内で人間の従業員がAIに代替される条件を、階層組織におけるタスク配分モデルとして分析する研究。 〔技術: AI導入を単なる性能比較ではなく、リスク調整コスト、組織階層、導入規…／人文: 労働史では、織機・組立ライン・事務機械の導入はいずれも職務の分解と再…〕 · [arxiv.org](https://arxiv.org/abs/2607.20781)
- [ ] **Educating the Agentic Engineer: Curricula, Collaboration, and Continuous Learning in the AI Era** — 生成AI・エージェントAIによって、エンジニアリング教育は「人間が成果物を書く」訓練から、「意図を指定し、自律システムを編成・検… 〔技術: マルチエージェントワークフローのオーケストレーション、機械生成物の検…／人文: 自動化の歴史では、機械の導入は常に教育制度と熟練概念を作り替えてきた…〕 · [arxiv.org](https://arxiv.org/abs/2607.29610)
- [ ] **混同しやすい「自動化」と「自働化」の違いを理解して業務改善を推進しよう** — 「自動化」は決められた手順を機械が実行すること、「自働化」は異常時に機械が自ら止まり、人間と機械が協調して品質を守る思想として整… 〔技術: 現代のAIエージェント運用におけるガードレール、停止条件、ヒューマン…／人文: 自動化を「人間を消す」思想ではなく、「異常を発見し、人間が意味ある判…〕 · [dataegg.co.jp](https://dataegg.co.jp/data/519)
- [ ] **日本の物流を変える、自動物流道路（オートフロー・ロード）** — 既存道路空間に荷物専用の無人・自動輸送インフラを構築し、物流危機を転機に変える構想。 〔技術: 自動化をソフトウェアエージェントだけでなく、道路・エネルギー・物流ノ…／人文: 自動化の歴史は工場内から都市・道路・家庭へ広がってきた歴史でもある。〕 · [mlit.go.jp](https://www.mlit.go.jp/road/autoflow_road)

### DDD
- [ ] **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — GitHub上のDDD候補11,742リポジトリから、GPT-4oによる三重多数決の意味検証を使って2,502件を抽出し、実践上… 〔技術: DDDを「思想」ではなくリポジトリ単位の観測可能な実践として測り、L…／人文: もっとも面白いのは、コードは長生きしても「なぜその境界にしたのか」と…〕 · [arxiv.org](http://arxiv.org/abs/2607.06471v1)
- [ ] **もうトークンは燃やさない AIエージェントの精度を上げるドメイン知識の組み込み方** — AIエージェントの自己改善やループ型処理において、無駄なトークン消費を避けながら精度を高めるため、ドメイン知識をどのように組み込… 〔技術: LLMエージェントの改善をプロンプト技巧だけでなく、ドメイン知識・評…／人文: 「トークンを燃やさない」という表現は、AI活用が計算資源だけでなく人…〕 · [techtarget.itmedia.co.jp](https://techtarget.itmedia.co.jp/tt/news/2607/23/news09.html)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework** — DDDを、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの識別、集約設計、技術アーキテ… 〔技術: LLMをDDDの共同ファシリテーターにする可能性と、集約・アーキテク…／人文: イベントストーミングやユビキタス言語は、本来、利害の違う人々が同じ世…〕 · [arxiv.org](http://arxiv.org/abs/2603.26244v1)
- [ ] **A Domain-Driven Design Simulator for Business Logic-Rich Microservice Systems** — ビジネスロジックの濃いマイクロサービスに対し、集約を中心にアプリケーションコードを保ったまま、SagaやTransactiona… 〔技術: DDDの集約を単なるコード構造ではなく、分散整合性とシミュレーション…／人文: これは「設計判断を本番障害で学ぶ」文化から、「小さな模型で未来の摩擦…〕 · [arxiv.org](http://arxiv.org/abs/2605.01159v1)
- [ ] **AIエージェント展開後の「冷ややかな沈黙」はなぜ起きる？ 定着を促すチェンジマネジメント設計** — Copilot StudioなどでAIエージェントを内製・展開しても現場で使われなくなる「冷ややかな沈黙」を、心理的要因と構造的… 〔技術: エージェントの成功条件をモデル性能だけでなく、業務フロー、権限、利用…／人文: DDDは「正しいモデル」を作る手法ではなく、現場が自分の言葉でシステ…〕 · [itmedia.co.jp](https://www.itmedia.co.jp/enterprise/articles/2607/29/news018.html)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

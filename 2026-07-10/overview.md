# 📰 2026-07-10 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMの高度推論・クラウドコード実行・チャート/スプレッドシート/スライド生成アップグレード · [blog.google](https://blog.google/innovation-and-ai/technology/ai/google-ai-updates-june-2026)
- **Loop engineering** — Stop Hand-Holding Your Coding Agent: Engineering the L… · [arxiv.org](https://arxiv.org/abs/2607.00038)
- **AWS** — Claude apps gateway for AWS が発表、Claude Code / Claude D… · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-apps-gateway-for-aws)
- **Harness engineering** — The Harness Effect: How Orchestration Design Sets the… · [arxiv.org](https://arxiv.org/abs/2607.06906)
- **sharp LLM usage** — From Noisy Traces to Root Causes: Structural Trajector… · [arxiv.org](https://arxiv.org/abs/2607.07702)
- **AI agent trends** — Codex as agent provider and agentic enhancements in Je… · [github.blog](https://github.blog/changelog/2026-07-07-codex-as-agent-provider-and-agentic-enhancements-in-jetbrains-ides)
- **Claude Code** — Claude Code 2.1.206: `/doctor`、worktree確認、MCP/背景エージェント… · [github.com](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- **Ethics of AI Agents** — Beyond Attack-Success Rate: Action-Graded Severity Sca… · [arxiv.org](https://arxiv.org/abs/2607.07474)
- **Philosophy of Loop Engineering** — Microsoft Agent Framework の Human-in-the-Loop / AG-UI… · [learn.microsoft.com](https://learn.microsoft.com/ja-jp/agent-framework/workflows/human-in-the-loop)
- **Anthropology of Agentic AI** — The Shift to Agentic AI: Evidence from Codex · [arxiv.org](https://arxiv.org/abs/2606.26959)
- **History of Automation** — Agentic Data Environments · [arxiv.org](https://arxiv.org/abs/2607.07397)
- **DDD** — Domain-Driven Design in Practice: A Large-Scale Empiri… · [arxiv.org](https://arxiv.org/abs/2607.06471)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMの高度推論・クラウドコード実行・チャート/スプレッドシート/スライド生成アップグレード** — Googleは6月のAIアップデートまとめで、NotebookLMに高度な推論、コードを実行する安全なクラウドコンピュータ、チャ… 〔技術: RAG型ノートが、参照付きQAからコード実行・可視化・成果物生成を含…／人文: 「読む人」から「調査を組み立てる人」へユーザー像が変わり、知識労働の…〕 · [blog.google](https://blog.google/innovation-and-ai/technology/ai/google-ai-updates-june-2026)
- [ ] **GeminiアプリのStudy notebooksとNotebookLM的な学習体験の統合** — GeminiアプリにStudy notebooksが導入され、目標設定、授業ノートのアップロード、理解度クイズ、個別レッスン、進… 〔技術: ノート、診断クイズ、個別カリキュラム、進捗管理を一体化することで、R…／人文: 学びが“読んで理解する”から“自分の弱点を常時測定される”体験へ変わ…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-app/gemini-study-notebooks)
- [ ] **日本語実践例: NotebookLM活用研究② 成果物評価の実験リターンズ** — note検索で確認できた日本語の新着実践例で、NotebookLMの出力や成果物評価を継続的に検証するシリーズ記事です。 〔技術: NotebookLMを“生成して終わり”ではなく、出力品質を評価し反…／人文: AI活用が個人の試行錯誤ログとして公開され、集合知化していく動きが見…〕 · [note.com](https://note.com/kumasennsei/n/n701a000a9d5a)
- [ ] **日本語実践例: NotebookLM PPTX エクスポート後の整理チェックリスト** — NotebookLMで資料を要約し、学習メモ、FAQ、スライド向け構成などを作った後、PPTXとして扱う際の整理観点をまとめた記… 〔技術: 生成AIの出力をPowerPointという既存の業務成果物へ接続する…／人文: AIが作ったスライドをそのまま提出するのではなく、人間が編集・整形・…〕 · [qiita.com](https://qiita.com/suuuuuu135/items/992544851f577a172baf)
- [ ] **arXiv: X+Slides — NotebookLMを含むスライド生成システムの観客条件付き評価** — 「X+Slides: Benchmarking Audience-Conditioned Slide Generation」は、… 〔技術: スライドの正確性だけでなく、対象読者にとって必要な情報がどれだけ含ま…／人文: プレゼンは情報圧縮であると同時に、誰に何を見せるかという社会的行為で…〕 · [arxiv.org](https://arxiv.org/abs/2606.19256)

### Loop engineering
- [ ] **Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting** — コーディングエージェントに逐次指示を出すのではなく、トリガー、目標、検証、停止条件、記憶を持つ「loop specificati… 〔技術: ループを、検証段階・終端状態・記憶・アーキテクチャで分類することで、…／人文: philosophy の観点では、人間の「指示する主体性」が、逐次命…〕 · [arxiv.org](https://arxiv.org/abs/2607.00038)
- [ ] **When Agents Do Not Stop: Uncovering Infinite Agentic Loops in LLM Agents** — LLM エージェントがモデル呼び出し、ツール実行、状態更新、エージェント間ハンドオフを繰り返し続ける Infinite Agen… 〔技術: loop engineering の「停止条件」は単なる max i…／人文: ethics の観点では、止まらないエージェントは費用だけでなく外部…〕 · [arxiv.org](https://arxiv.org/abs/2607.01641)
- [ ] **LoopX: lightweight loop engineering state kernel for long-running AI agent teams** — LoopX は、Codex、Claude Code、Cursor などの実行環境を置き換えるのではなく、目標、todo、ゲート、… 〔技術: エージェント本体よりも、再開可能性・レビュー可能性・証拠管理を担う薄…／人文: history の観点では、これは職人が口頭で作業を渡す段階から、作…〕 · [github.com](https://github.com/huangruiteng/loopx)
- [ ] **Semantic Early-Stopping for Iterative LLM Agent Loops** — Writer/Critic のような反復型 LLM ループを固定回数で止める代わりに、連続するドラフトの意味変化と品質改善が止ま… 〔技術: 停止条件を「回数」から「意味的な改善の有無」へ移すことで、ループをよ…／人文: philosophy の観点では、「十分に考えた」とは何かを、内省で…〕 · [arxiv.org](https://arxiv.org/abs/2606.27009)
- [ ] **SWE-Review: Closing the Loop on Issue Resolution with Agentic Code Review** — AI が生成した PR を一発で受け入れる open-loop 方式ではなく、レビュワーエージェントがリポジトリを探索し、受理可… 〔技術: コーディングエージェントの成果物を、生成だけでなくレビュー、診断、再…／人文: anthropology の観点では、ソフトウェア開発におけるレビュ…〕 · [arxiv.org](https://arxiv.org/abs/2607.06065)

### AWS
- [ ] **Claude apps gateway for AWS が発表、Claude Code / Claude Desktop の統制を AWS 上で一元化** — Claude apps gateway for AWS は、Claude Code と Claude Desktop のアクセス… 〔技術: 生成 AI 開発ツールの利用経路をゲートウェイ化し、認証・ポリシー・…／人文: 「便利な個人ツール」と「組織の説明責任」の衝突を、禁止ではなく制度設…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-apps-gateway-for-aws)
- [ ] **AWS CloudFormation Express mode、インフラ反復を最大4倍高速化** — CloudFormation Express mode は、インフラデプロイの確認をより短時間で返し、AI エージェントや開発者… 〔技術: IaC のデプロイ待ち時間が短くなることで、エージェントが生成したテ…／人文: インフラ作業は長く「待つこと」を前提にした職人芸でしたが、待ち時間の…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/accelerate-your-infrastructure-deployments-by-up-to-4x-with-aws-cloudformation-express-mode)
- [ ] **Amazon EKS の Kubernetes version rollback、アップグレードを7日以内に巻き戻し可能に** — Amazon EKS で Kubernetes バージョンアップ後、7日以内ならクラスタ再構築なしにロールバックできる機能が紹介… 〔技術: バージョン更新のリスクを下げ、Kubernetes 運用における変更…／人文: 大規模基盤の運用では「失敗しても戻れる」ことが、挑戦の心理的安全性を…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/upgrade-amazon-eks-clusters-with-confidence-using-kubernetes-version-rollbacks)
- [ ] **AWS Security Hub Network Scanning と AWS Config の191追加マネージドルールで、AI時代の到達性・統制が強化** — Security Hub はインターネットから実際に到達可能なリソースを検出する Network Scanning を追加し、A… 〔技術: 設定上の可能性だけでなく実到達性を見るスキャンと、AI サービスを含…／人文: AI 導入の議論はモデル性能に寄りがちですが、社会に出るシステムでは…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-network-scanning)
- [ ] **井村屋グループが SageMaker Canvas でチルド製品の需要予測を改善、業務工数90%削減** — 井村屋グループは Amazon SageMaker Canvas を使い、チルド製品の AI 需要予測で業務工数90%削減と熟練… 〔技術: ノーコード寄りの SageMaker Canvas により、需要予測…／人文: 食品の需要予測は、廃棄・欠品・熟練者の暗黙知といった生活に近い問題に…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/ai-case-study-imurayagroup)

### Harness engineering
- [ ] **The Harness Effect: How Orchestration Design Sets the Token Economics of Enterprise Agentic AI** — エンタープライズ向けエージェントAIで、同じモデル群・同じ22評価タスクを保ったまま、従来型の本番ループと Writer Age… 〔技術: context組み立て、tool露出、turn順序、delegati…／人文: AIの費用問題を「より安いモデル」ではなく「組織がどんな作業制度を設…〕 · [arxiv.org](https://arxiv.org/abs/2607.06906)
- [ ] **harness-forge: self-improving Claude Code harness** — `/forge` コマンドで任意プロジェクトに self-improving Claude Code harness を導入する… 〔技術: 失敗を記録し、lessonとして昇格し、hooksや回帰テストへ機械…／人文: 「モデルは学習しないが、リポジトリは学習できる」という発想がはっきり…〕 · [github.com](https://github.com/Aditya-Nagariya/harness-forge)
- [ ] **日本語圏のClaude Codeハーネス群: project-bootstrap / claude-advisor-harness / cadence / harness-design-kit** — 日本語コミュニティでは、Claude Code向けの「ハーネス」が、強制可能なprecondition、advisor戦略、構造… 〔技術: 日本語README群は、ハーネスを「忘れられる助言」から「fail-…／人文: 日本語圏では、AIを魔法の相棒としてではなく、規律・型・稽古・監査を…〕 · [github.com](https://github.com/RintaroYamaoka/project-bootstrap)
- [ ] **Claude Code Hooks / Subagents / GitHub Actions の公式ドキュメントがハーネスの標準部品を明確化** — Hooks reference は、SessionStart、UserPromptSubmit、PreToolUse、PostT… 〔技術: ハーネス設計に必要な「いつ介入するか」「どの権限を持たせるか」「どこ…／人文: これはAIエージェントを人格的な協働者としてだけでなく、組織の手続き…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [ ] **Execution-security / verification / memory-injection のarXiv論文群が「安全なハーネス」の輪郭を押し広げる** — AI coding agentsの実行層セキュリティを整理するサーベイ、Claude Codeのようなコードエージェントを検証ハ… 〔技術: sandbox、access control、TOCTOU、MCP脅…／人文: 自律性を高めるほど、誰が何を許可し、何を記録し、どの記憶を信頼するの…〕 · [arxiv.org](https://arxiv.org/abs/2607.05743)

### sharp LLM usage
- [ ] **From Noisy Traces to Root Causes: Structural Trajectory Analysis and Causal Extraction for Agent Optimization** — STRACEは、長期実行エージェントの大量でノイズの多い実行トレースから代表的な失敗を選び、テキスト依存グラフで因果的に重要な手… 〔技術: 「全部入れる」「直近だけ入れる」ではなく、失敗パターンのクラスタリン…／人文: LLM活用の中心が、賢い一問一答から「失敗をどう記憶し、どの証拠を残…〕 · [arxiv.org](https://arxiv.org/abs/2607.07702)
- [ ] **Reason Less, Verify More: Deterministic Gates Recover a Silent Policy-Violation Failure Mode in Tool-Using LLM Agents** — ツール呼び出し型エージェントが、ツールエラーなしに業務ポリシー違反の状態変更を行う「静かな誤状態」失敗を分析し、書き込み前の読み… 〔技術: 推論を増やすより、状態遷移前にルールベースのpre-executio…／人文: 「AIにもっと考えさせる」信仰に対して、制度・手続き・監査の力を再評…〕 · [arxiv.org](https://arxiv.org/abs/2607.07405)
- [ ] **What Makes a Good Bug Report for an AI Agent?** — 433件のSWE-bench Verified課題と87の修復エージェントを分析し、AIエージェントに効くバグ報告の特徴を調べた… 〔技術: エージェント向けissueは「詳しく自然言語で説明する」より、実行可…／人文: これは人間向け文章作法と機械向け依頼作法の分岐を示す話です。〕 · [arxiv.org](https://arxiv.org/abs/2607.07593)
- [ ] **Show HN: Caliper – pass@k reliability testing for Claude Code and Codex skills** — Caliperは、Claude Code、Codex、Pi、Hermesなどのエージェント用スキルを、YAMLで定義した成功条件… 〔技術: LLMワークフローをプロンプト資産としてではなく、非決定的ソフトウェ…／人文: スキルやプロンプトは、作者の勘ではなく共同体が検証・比較できる手順に…〕 · [github.com](https://github.com/edonadei/caliper)
- [ ] **Ask HN: I hate coding agents. Is this skill issue?** — コーディングエージェント利用者が、深い集中の喪失、AI生成コードへの所有感低下、AI可用性への依存、最後の20%の修正困難を率直… 〔技術: 成功事例だけでなく、コンテキスト設計を頑張っても残る前提誤認、レビュ…／人文: LLM活用は生産性だけでなく、作者性、熟達感、集中のリズムを組み替え…〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=48844345)

### AI agent trends
- [ ] **Codex as agent provider and agentic enhancements in JetBrains IDEs** — GitHub が JetBrains IDE 向けに Codex を新しい agent provider としてパブリックプレビ… 〔技術: エージェント運用の差別化点がモデル単体ではなく、IDE、MCP、Ho…／人文: 開発者は「AIを使う人」から「複数の代理実行者を編成する人」へ近づい…〕 · [github.blog](https://github.blog/changelog/2026-07-07-codex-as-agent-provider-and-agentic-enhancements-in-jetbrains-ides)
- [ ] **Claude Code と Codex の設定を1つのSSOTに統一する - APMでAIエージェント設定をコード管理した話** — Claude Code と Codex を併用する現場で、MCP、システムプロンプト、スキル設定が二重管理になった問題を、Mic… 〔技術: エージェント設定を生成物として扱い、CI でドリフト検知する発想は、…／人文: チームがAIに何を許し、何を覚えさせ、どの作法で動かすかは、組織文化…〕 · [qiita.com](https://qiita.com/ZuckyQuest/items/bd0ed671749574f4df98)
- [ ] **How Boris Cherny Uses Claude Code** — Claude Code creator の Boris Cherny が日常ワークフローで使うとされる 118+ tips を集… 〔技術: Claude Code の実践知が、プロンプト単発ではなく、リポジト…／人文: 作者の使い方が共有されると、ツールは機能一覧ではなく「職人芸の型」と…〕 · [howborisusesclaudecode.com](https://howborisusesclaudecode.com)
- [ ] **Anthropic「2026 Agentic Coding Trends Report」を読み解く──エンジニアは「書く人」から「設計して任せる人」へ** — Anthropic の「2026 Agentic Coding Trends Report」を日本語で読み解き、8つのトレンドを… 〔技術: Agentic coding の論点を、開発プロセス、エージェント能…／人文: 「書く人」から「設計して任せる人」への転換は、エンジニアのアイデンテ…〕 · [qiita.com](https://qiita.com/nogataka/items/46fb464d05e2eb53d09c)
- [ ] **SkillCenter: A Large-Scale Source-Grounded Skill Library for Autonomous AI Agents** — 自律AIエージェント向けに、216,938件の構造化スキルを24ドメインで提供する大規模スキルライブラリを提案する論文。 〔技術: エージェントの能力拡張を「都度プロンプト」ではなく、出典付きスキルの…／人文: これはAIエージェントにとっての図書館や職業訓練校に近い。〕 · [arxiv.org](https://arxiv.org/abs/2607.07676)

### Claude Code
- [ ] **Claude Code 2.1.206: `/doctor`、worktree確認、MCP/背景エージェント修正がまとまって入る** — 2.1.206では、`/cd`のディレクトリ補完、チェックインされた`CLAUDE.md`を整理する`/doctor`提案、プロ… 〔技術: コンテキスト、MCP、worktree、background wor…／人文: これはAIを「賢い返答機」ではなく、作業場に常駐する同僚として扱い始…〕 · [github.com](https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md)
- [ ] **Claude Code 2.1.198: subagentsがデフォルトでバックグラウンド化し、完了時にdraft PRまで進む** — 2.1.198では、subagentsがデフォルトでバックグラウンド実行になり、完了・入力待ち通知が`Notification`… 〔技術: 対話型CLIが、単一ターンの補助から、複数セッションを監督するジョブ…／人文: 開発者の役割は「コードを書く人」から「複数の小さな作業主体を任命し、…〕 · [github.com](https://github.com/anthropics/claude-code/releases/tag/v2.1.198)
- [ ] **Claude Sonnet 5がClaude Codeのデフォルトに: 1M token contextと販促価格** — Claude Code 2.1.197でClaude Sonnet 5がデフォルトモデルになり、ネイティブ1M token co… 〔技術: 1M token contextは、局所的な補完よりも、履歴・設計文…／人文: 長文脈化は「忘れない同僚」を生む一方で、何を覚えさせ、何を忘れさせる…〕 · [anthropic.com](https://www.anthropic.com/news/claude-sonnet-5)
- [ ] **日本語実践: 「人間基準の生産性」を捨て、1人+Claude Codeで222日・12,499 commitsを記録** — 1人とClaude Codeで2025-12から2026-07-10までに12,499 commits、224 reposito… 〔技術: Claude Codeを単発補助ではなく、リポジトリ群をまたいだ継続…／人文: 「生産性」とは何か、という尺度そのものが揺れています。〕 · [qiita.com](https://qiita.com/abyo-software/items/caf8b82857f8eecd2e97)
- [ ] **日本語実践: Claude CodeとCodexの設定をAPMでSSOT化する** — Claude CodeとCodexを併用する中で、MCP、システムプロンプト、スキル、`AGENTS.md`、`.mcp.jso… 〔技術: エージェントの振る舞いを、手元の隠れ設定ではなく生成可能な設定成果物…／人文: AIツールが増えるほど、人間は「どのAIに何を教えたか」を忘れます。〕 · [qiita.com](https://qiita.com/ZuckyQuest/items/bd0ed671749574f4df98)

### Ethics of AI Agents
- [ ] **Beyond Attack-Success Rate: Action-Graded Severity Scale for Tool-Using AI Agents** — ツール使用AIエージェントの攻撃成功率を成功/失敗の二値で見るのではなく、実行された行為の可逆性、スコープ越境、権限拡大などをL… 〔技術: エージェントの安全評価を、最終回答ではなくツールコール軌跡と実害の段…／人文: 責任所在の議論で曖昧になりがちな「何がどれほど悪かったのか」を、被害…〕 · [arxiv.org](https://arxiv.org/abs/2607.07474)
- [ ] **When AI Agents Attack: Autonomous Cyber Operations and Europe’s Governance Gap** — 自律的なサイバー作戦にAIエージェントが使われるとき、欧州のガバナンス枠組みにどんな隙間が生まれるかを扱う記事として確認。 〔技術: サイバー領域のエージェントは観測、計画、実行、権限行使が連鎖するため…／人文: 「攻撃したのは人間か、組織か、エージェントか」という問いは、戦争責任…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiygFBVV95cUxNYmR1MkwybWlSak1iSmRpQ1k1OWtRN05xTUpOQzdMMjVrdDREZWc1RFVnaUJpUWVNOXp6TXctcVNFV3Z3Xy14dGd3cWRRLURxbkU0N2x6dHJldGl2ZkVEODVCa3hVTGlsMDJqR1ZtZVdsRGJtYXJiUHFBQnR4SGdCdzlGUm80SlB6MGt1b3hwd0M1V2NxWkNTVnZoZlZVVG1zNEhSQmJ3VW1zQURQSjBiMVUwQkd5NTVwOUh1R28xd3dISUIweEdfTklB?oc=5)
- [ ] **China’s new AI rules: Ethics, AI agents and anthropomorphic AI** — 中国の新しいAIルールが、倫理、AIエージェント、擬人化AIをどう扱うかに関する解説として確認。 〔技術: エージェント機能や擬人化表現を規制対象として切り出すと、UI、人格表…／人文: 文化差が最も見える論点で、欧米の「リスク管理」だけでなく、中国・日本…〕 · [news.google.com](https://news.google.com/rss/articles/CBMijAFBVV95cUxPU2czdUNBOG10eGtxZ1RoU3NIYm53emthSHRtMG5SMEo5VjlyWUhuM3h4aFlDejI2aklXXzBzekN1SG5CRnpsVDZfcFFYTmVtVlltaElVMjJQX2dyaFRQS1BYNGdjbTBHcF8tb24zcXBPUWpVOVF6UjBjU2dYNEwzczRRRGZsM1R0aV94Ug?oc=5)
- [ ] **Securing AI agents: When AI tools move from reading to acting** — AIツールが「読む」だけでなく「行動する」段階に入ったときのセキュリティ設計を扱う記事として確認。 〔技術: 権限分離、ID連携、実行環境の隔離、承認フローが、プロンプトエンジニ…／人文: 「便利な代理人」にどこまで鍵を渡すかは、信頼・委任・労働の境界の問題…〕 · [news.google.com](https://news.google.com/rss/articles/CBMirwFBVV95cUxOS3MzLWx1UWNMTG8tMXVocVkxNlFLM3dWRzdPVC11X0ZTNERLdGpkejVYcVZpNzk4Z3F4ZTFvSDRDWGo2YkxGMXVZN0QyUWlheEhCNjlKRXd2aFN2QzR0LUZONnZ2RHNocHRhT0JLSHNHMzM2R3A0dUszVWhPa0JBNXp6T0VMUG1uaFpISmZmZ2ZtbDQ3S3hvMTRwUmNwcGJqQTUwSmJRMGNFV2lLNjZv?oc=5)
- [ ] **なぜAIエージェントが「データガバナンス」の論点になるのか？ 高性能モデルを選定するよりも大切なこと** — 日本語圏で、AIエージェント導入をモデル性能よりデータガバナンスの問題として捉える記事として確認。 〔技術: エージェントが社内データを横断して行動するほど、データ分類、アクセス…／人文: 「デジタル従業員」という比喩は便利だが、労働者の責任・権限・教育・懲…〕 · [news.google.com](https://news.google.com/rss/articles/CBMiWkFVX3lxTE1vejFpX29WYjRCWUlxZE94Y01waUMwVTM1MXhlNVNoajFZOVVveE05aDRwOV9DcTktSURFVHlTWHkySzZfeEdpbWNQYlRDZ0YyZXRsdkRONGZhdw?oc=5)

### Philosophy of Loop Engineering
- [ ] **Microsoft Agent Framework の Human-in-the-Loop / AG-UI 承認ループ** — Microsoft Agent Framework は、Executor が外部システムや人間に要求を送り、応答を待ってから実行… 〔技術: エージェントのツール実行を「生成→停止→承認→再開」という明示的な制…／人文: これは単なる安全装置ではなく、行為の最終責任をどこに置くかという実践…〕 · [learn.microsoft.com](https://learn.microsoft.com/ja-jp/agent-framework/workflows/human-in-the-loop)
- [ ] **LLM-Based Test Oracles: Source-of-Authority Taxonomy** — LLM をテストオラクルとして使う研究について、判定が何を権威の源泉としているのかを分類する系統的レビュー。 〔技術: 「LLM-as-a-judge」という機構名ではなく、判定の根拠・権…／人文: Loop Engineering の認識論的な核心は、反復すれば真に…〕 · [arxiv.org](https://arxiv.org/abs/2607.05031)
- [ ] **Human-in-the-Loop Nugget Annotation for Accountable LLM-as-a-Judge Evaluations** — AI / Agentic system の出力評価で、人間が重要情報の nugget を同定し、LLM が大量照合を担う分業型ワ… 〔技術: 評価ループを「人間が意味単位を設計し、LLM がスケール処理する」形…／人文: 実践知の観点では、人間の役割はボタンを押す監督者ではなく、何が問題の…〕 · [arxiv.org](https://arxiv.org/abs/2606.29033)
- [ ] **Don’t Blindly Trust It: How Unreliable Feedback Breaks Tool-Using LLM Agents** — ツール利用型 LLM エージェントが、信頼できない外部フィードバックを受けたときにどのように壊れるかを、ループ・プロンプト・行動… 〔技術: ループを増やすほど良くなるのではなく、返ってくる観測の信頼性が低い場…／人文: これは「経験から学ぶ」ことの条件を問う認識論である。〕 · [arxiv.org](https://arxiv.org/abs/2606.21409)
- [ ] **ハーネスエンジニアリング入門 ── CLAUDE.md の次に来る AI エージェント制御パラダイム** — AI エージェントを単にプロンプトでお願いする対象ではなく、制約・環境・検証・誘導を含む「ハーネス」によって力を伝達する対象とし… 〔技術: プロンプト、テスト、権限、CI、レビュー、失敗時の戻し方を一つの実行…／人文: 「馬具」としての harness の比喩は、AI を自律的な主体とし…〕 · [qiita.com](https://qiita.com/nogataka/items/d1b3fcf355c630cd7fc8)

### Anthropology of Agentic AI
- [ ] **The Shift to Agentic AI: Evidence from Codex** — OpenAIのCodex利用データをもとに、agentic AIが人の働き方をどう変えるかを大規模に分析した論文。 〔技術: 複数エージェントの同時管理、skillsによる共有手順、組織アカウン…／人文: これは職場に新しい「同僚」や「部下」が入る話ではなく、誰が作業を開始…〕 · [arxiv.org](https://arxiv.org/abs/2606.26959)
- [ ] **Adaptive AI Delegation under Uncertainty: A Bayesian Governance Policy for Sequential Decision Authority** — 組織が不確実な状況でAIにどこまで意思決定権限を委譲すべきかを、Bayesian inferenceとPOMDPで定式化する研究… 〔技術: AIレコメンデーションを単なる予測ではなく、逐次的な権限配分問題とし…／人文: 委譲は組織文化そのものです。〕 · [arxiv.org](https://arxiv.org/abs/2606.29406)
- [ ] **The Harness Effect: How Orchestration Design Sets the Token Economics of Enterprise Agentic AI** — 企業向けagentic AIのコスト増を、モデルではなく「harness」、つまりコンテキスト編成・ツール公開・ターン制御・委譲… 〔技術: モデル性能ではなく、ツール呼び出し、文脈再利用、観測性、統制を束ねる…／人文: harnessは、オフィスでいう手順書・監督者・会議体・監査ログを合…〕 · [arxiv.org](https://arxiv.org/abs/2607.06906)
- [ ] **ガバメントAI「源内」** — デジタル庁が、政府職員が安全に生成AIを使うための基盤「源内」を各府省庁に展開していることを説明する公式ページ。 〔技術: 行政資料RAG、府省庁横断の利用基盤、国内LLM調達、共通データセッ…／人文: これはAI導入というより、行政組織の日常語・稟議・答弁・問い合わせ対…〕 · [digital.go.jp](https://www.digital.go.jp/policies/genai)
- [ ] **“Re-Tell the Fortune so I Can Believe It”: How Chinese User Communities Engage with and Interpret GenAI-based Fortune-Telling** — 中国のユーザーが生成AIを占いに使う実践を、22名へのインタビューと1,842件のコミュニティ投稿を含む3週間のデジタル・エスノ… 〔技術: AIを予測器ではなく、反復プロンプトとコミュニティ解釈を通じて意思決…／人文: agentic AIの人類学では、仕事だけでなく儀礼・慰め・共同解釈…〕 · [arxiv.org](https://arxiv.org/abs/2603.27784)

### History of Automation
- [ ] **Agentic Data Environments** — 自律エージェントがファイル、API、アプリケーション、システム状態を横断して動く時代に、データ環境そのものを「安全な実行基盤」と… 〔技術: データベースを受動的な保存場所ではなく、権限・監査・実行制約を備えた…／人文: 産業革命期の機械囲い込みが工場制度を生んだように、AIエージェントは…〕 · [arxiv.org](https://arxiv.org/abs/2607.07397)
- [ ] **ガバメントAI「源内」** — デジタル庁が政府職員向け生成AI利用環境「源内」を各府省庁に展開し、2026年度中に全府省庁約18万人の政府職員が利用可能となる… 〔技術: RAG、行政文書分析、パブリックコメント分類など、ホワイトカラー行政…／人文: これは単なる業務効率化ではなく、官僚制がAIを内部化する制度史的な出…〕 · [digital.go.jp](https://www.digital.go.jp/policies/genai)
- [ ] **Using AI Agents to Automate Black-Box Audits of Personalization Algorithms at Scale** — パーソナライゼーション・アルゴリズムを外部から監査するため、固定ペルソナを持つ生成AIエージェントで合成アカウントの行動を作り、… 〔技術: エージェントを「仕事の代替」だけでなく、ブラックボックス化した自動化…／人文: 自動化が社会を見えにくくしたなら、監査もまた自動化されるという二重の…〕 · [arxiv.org](https://arxiv.org/abs/2606.30801)
- [ ] **Human-in-the-Loop Nugget Annotation for Accountable LLM-as-a-Judge Evaluations** — LLM-as-a-Judge評価において、人間が重要情報の「ナゲット」を定義し、LLMが大量照合を担当する分業型ワークフローを提… 〔技術: 評価自動化の中に、人間が意味単位を設計し機械がスケール処理を担う分業…／人文: 自動化史では「人間が機械に合わせる」局面が繰り返されてきたが、この研…〕 · [arxiv.org](https://arxiv.org/abs/2606.29033)
- [ ] **When Agent Automation Becomes Profitable: Quantifying and Insuring Autonomous AI Risk through Trace-Economic Underwriting** — AIエージェントが業務システム内で不可逆な操作を行う際、損失責任が曖昧なままでは自動化の経済合理性が成立しにくいとし、ツール利用… 〔技術: エージェントの実行ログを、監査だけでなく保険・価格付け・権限制御のた…／人文: 蒸気機関や工場機械が保険、労災、標準化を必要としたように、AIエージ…〕 · [arxiv.org](https://arxiv.org/abs/2606.16465)

### DDD
- [ ] **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — 11,742件の候補GitHubリポジトリから、GPT-4oの三重多数決による意味的検証で2,502件のDDD実践リポジトリを抽… 〔技術: DDDを「語られる方法論」から、リポジトリ上で観測・検証できる設計実…／人文: ビジネス文脈がコード履歴から消えるという指摘は、ユビキタス言語が単な…〕 · [arxiv.org](https://arxiv.org/abs/2607.06471)
- [ ] **Archally Blueprint Schema: domain-first YAML schema for AI-grounded architecture** — ドメイン設計、ビジネスルール、価値流、ガバナンス、組織アラインメントをYAMLで一元化し、OpenAPI、AsyncAPI、BP… 〔技術: DDDの成果物を人間向けドキュメントで終わらせず、生成・検証・エージ…／人文: 「誰が何を知っているか」に依存する設計文化を、共有可能な組織記憶へ移…〕 · [github.com](https://github.com/Archally/blueprint-schema)
- [ ] **faceto: typed file → visual workshop board with LLM feedback loop** — 型付きファイルからHTML+SVGのワークショップボードを生成し、LLMと一緒に考えながら要素ごとにノートを追加して次セッション… 〔技術: Event StormingをLLM時代の反復可能なモデリング・イン…／人文: ワークショップで生まれる曖昧さや違和感を、次の対話に持ち越せる点が重…〕 · [github.com](https://github.com/bastien-gallay/faceto)
- [ ] **ddd-agent-skill: Domain-Driven Design end-to-end for agent workflows** — Agent Skills互換のDDDスキルで、Vaughn VernonのIDDDに沿い、まず「Full DDD / Light… 〔技術: AIエージェントにDDD成果物を直接生成させるだけでなく、DDDを使…／人文: DDDはしばしば儀式化しやすいが、このアプローチは「複雑さに見合った…〕 · [github.com](https://github.com/aristorinjuang/ddd-agent-skill)
- [ ] **dca-marketplace: Claude Code plugins for Domain-Centric Architecture** — Claude Code向けに、Domain-Centric Architectureのスキルとエージェントをマーケットプレイス形… 〔技術: DDD/Hexagonal/Clean Architectureを、…／人文: これは設計判断を「優秀な個人の頭の中」から「チームで呼び出せる作法」…〕 · [github.com](https://github.com/chbloemer/dca-marketplace)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

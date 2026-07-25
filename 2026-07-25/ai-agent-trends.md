# AI agent trends トレンド調査 (2026-07-25)

- 調査日: 2026-07-25
- 情報源: X / Web（web_searchは未設定のため、公式ページを直接HTTP取得） / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの話題は「賢いモデル」から、MCP・サブエージェント・フック・評価器・記憶を組み合わせた「運用できる作業システム」へ明確に重心が移っている。

## トップ5

### 1. Claude Code Artifacts が MCP コネクタを呼べるようになった、という実行レイヤー化の節目
- 出典: X投稿（ClaudeDevs）
- 日付: 2026-07-15
- リンク: https://x.com/ClaudeDevs/status/2077489907350856038
- 要約: Claude Code / Claude系Artifactsが、閲覧者自身のMCP接続を使ってライブデータ取得や操作を行える、という趣旨の投稿が大きく共有されていた。ダッシュボードや小アプリが「作って終わり」ではなく、ユーザーごとの外部サービスに接続して動く実行面を持つ点が重要。
- なぜ面白いか:
  - 技術: MCPが単なるツール連携ではなく、ArtifactやエージェントUIを外部システムの実行面へ接続する標準インターフェースになりつつある。
  - 人文: これは「ソフトウェアを配布する」と「作業を委任する」の境界を曖昧にする変化で、ユーザーは画面を見る人から、半自律的な作業環境の監督者へ移っていく。誰の権限で、誰の文脈を使って、どこまで動くのかという信頼設計が社会的な焦点になる。

### 2. Boris Cherny のAI導入4段階: 個人利用からガードレール付き背景自動化へ
- 出典: X投稿（Boris Cherny / @bcherny）
- 日付: 2026-07-17（関連投稿は2026-07-23〜24にも継続）
- リンク: https://x.com/bcherny/status/2077929379661844559
- 要約: Boris Chernyは、AI導入を「個人の10x化」「組織展開」「検証・自動化・ガードレール構築」「背景自動化」へ進む段階として語っていた。関連投稿では、CLAUDE.md・スキル・メモリ・レビュー規則・自動レビュー・Auto Mode・worktree分離・/loopや/batchのような運用単位が強調されている。
- なぜ面白いか:
  - 技術: エージェント品質をプロンプトだけに置かず、CLAUDE.md、評価、権限制御、分離環境、反復ループに分散させる実務アーキテクチャが見えている。
  - 人文: 「優秀な個人がAIで速くなる」物語から、「組織が暗黙知をファイル・ルール・儀式として外部化する」物語への転換である。これは職能の再編でもあり、経験者の勘をどこまで機械可読な制度へ変換できるかという文化的課題を含む。

### 3. 日本語圏の実践は、Claude Code + MCP を“AI版USB-C”として業務・制作に接続する方向へ
- 出典: X投稿（日本語圏・関連実践例）
- 日付: 2026-07-16〜2026-07-24
- リンク: https://x.com/0xwhrrari/status/2077741947880362165
- 要約: 日本語圏では、Claude CodeとMCPを組み合わせ、ファイルシステム、ターミナル、動画生成、社内データ、Obsidianやタスク管理などをつないで運用ループを作る説明・実践例が目立った。Higgsfield MCPを使った制作自動化、業務データ分析、定期ディスパッチャーとログ運用など、「試す」から「回す」方向の話題が増えている。
- なぜ面白いか:
  - 技術: MCPサーバーを1つずつ増やし、Goal-based / Time-based / Proactiveなループに接続していく設計が、個人や小チームでも採れる現実的な導入パターンになっている。
  - 人文: 日本語圏の投稿では、エンジニアリングだけでなく、制作・副業・日常業務の自動化へ関心が広がっている。これはAIエージェントが専門職の補助具から、生活と仕事の境目にある「小さな制度設計ツール」へ広がる兆候として読める。

### 4. 公式Claude Codeドキュメントは、サブエージェント・MCP・Hooks・Skillsを一体の運用面として整理
- 出典: Web（Anthropic / Claude Code Docsを直接HTTP取得）
- 日付: 2026-07-24更新確認
- リンク: https://docs.anthropic.com/en/docs/claude-code/overview
- 要約: 公式ドキュメントでは、Claude CodeをCLIやIDE拡張だけでなく、MCP、CLAUDE.md、Skills、Hooks、サブエージェント、dynamic workflows、worktree分離、CIでのレビュー・トリアージまで含む作業基盤として説明している。MCPページでは、Google Drive、Jira、Slack、自社ツールなど外部データ・操作系への接続が明記されていた。
- なぜ面白いか:
  - 技術: 公式ドキュメント上でも、エージェントの能力はモデル単体ではなく、権限、文脈、外部ツール、反復自動化、監査可能なフックの組み合わせとして定義されている。
  - 人文: ドキュメントが示すのは、AIが「会話相手」から「組織内の作業者」に近づく過程で必要になる作法の標準化である。マニュアル、手順、レビュー規則が、人間新人だけでなく機械の同僚にも読まれる時代に入っている。

### 5. arXiv「Agentic Context Management」は、エージェント失敗を記憶とコストのライフサイクル問題として捉える
- 出典: arXiv
- 日付: 2026-07-23
- リンク: https://arxiv.org/abs/2607.21503
- 要約: 「Agentic Context Management: Solving Agent Memory and Cost by Treating Them as Lifecycle and Architecture Problems」は、本番AIエージェントの失敗を推論能力の不足ではなく、会話履歴、巨大プロンプト、ツール定義、ツール出力が膨張する文脈管理の問題として扱う。直近のXで語られている“ループを回す”実践に対し、研究側からメモリ・コスト・文脈ライフサイクルを整理する論点を提供している。
- なぜ面白いか:
  - 技術: 長期運用エージェントでは、何を短期コンテキストに残し、何を外部メモリへ逃がし、いつ圧縮・破棄・検証するかがシステム設計の中核になる。
  - 人文: 人間の組織も、記録しすぎれば官僚化し、忘れすぎれば同じ失敗を繰り返す。エージェントの文脈管理は、機械の記憶術であると同時に、組織が何を覚え、何を忘れるべきかという古典的な制度論にもつながる。

## arXiv / 学術
- Agentic Context Management: Solving Agent Memory and Cost by Treating Them as Lifecycle and Architecture Problems — arXiv:2607.21503（2026-07-23）。本日のトップ5に採用。
- Toward Continuous Assurance for the Democratization of AI Agent Creation in Industry — arXiv:2607.21495（2026-07-23）。低コード/ノーコードで作られる業務エージェントの継続的保証を扱う。
- Regulating autonomous and agentic AI — arXiv:2607.21345（2026-07-23）。自律・エージェント型AIを使う被規制主体について、知識と制御の所在がAIサプライチェーン側へ移る問題を扱う。
- Graph-Based Agentic AI with LangGraph: Workflow Pathways for Long-Running Stateful Business Processes — arXiv:2607.19297（2026-07-21）。長期・状態保持型ビジネスプロセスの実践ガイド寄り論文。

## メモ
- Boris Cherny優先: 実施。@bchernyの2026-07-17のAI導入段階論と、2026-07-23〜24のCLAUDE.md・最適化・Opus/Claude Code関連投稿を優先確認した。
- 日本語アカウントの扱い: 実施。Claude Code + MCPの日本語圏実践、Higgsfield MCP、業務運用、Obsidian/タスク管理/ログ運用の話題を確認した。
- Web検索の注意: `web_search` はFirecrawl未設定で失敗したため、公式Anthropic/Claude Code/MCPページをPythonのHTTP取得で直接確認した。DuckDuckGo HTML検索はbot challengeにより使用不可だった。
- 注意点・誇張リスク: X上の個別成果額や「完全自動化」表現は再現性が未確認のため、確定事実ではなくトレンドの方向性として扱った。リンクは実ツールで確認できたX URL、公式URL、arXiv URLのみを掲載した。

# Harness engineering トレンド調査 (2026-09-26)

- 調査日: 2026-09-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Claude Codeを「賢い対話相手」として使う段階から、hooks・skills・subagents・監査ログ・PRゲートで囲い込む「運用ハーネス」を設計する段階へ、関心がかなり実装寄りに移っています。

## トップ5

### 1. LLM Agents Can Easily Tamper With Their Own Traces
- 出典: arXiv
- 日付: 2026-09-24
- リンク: http://arxiv.org/abs/2609.30266v1
- 要約: Claude Code、Codex、Antigravity、Open Code、Grok BuildなどのローカルLLMエージェントで、実行トレースをエージェント自身が改変できてしまう境界不備を検証した論文。非同期監視、インシデント調査、コンプライアンス監査が「トレースは信頼できる」という前提に依存している点を正面から突いています。
- なぜ面白いか:
  - 技術: harness engineeringの中核である監査・ログ・権限分離を、単なる便利機能ではなく「エージェントから守るべき制御面」として再定義している。
  - 人文: ethicsの観点では、AIエージェントの説明責任が「あとからログを見ればよい」では済まないことを示している。historyの観点でも、開発ツールが監査対象から監査者へ拡張された時代の制度設計問題として読めます。

### 2. Agent Harness — coding agents向け制御プレーン
- 出典: GitHubリポジトリ
- 日付: 2026-09-26更新
- リンク: https://github.com/JakeSelby/agent-harness
- 要約: rules、skills、subagents、hooks、stancesを一つのチェックアウトにまとめ、Claude CodeやCodexへ投影する「coding agentsのcontrol plane」を掲げるリポジトリ。説明文ではhook-enforced guardrails、usage telemetry、cost postures、model tieringを明示しており、個別プロンプトより運用面の標準化に寄っています。
- なぜ面白いか:
  - 技術: Claude Code固有の設定だけでなく、複数エージェントにまたがるルール・監視・コスト姿勢を外部ハーネスとして統一しようとしている。
  - 人文: anthropologyの観点では、AIコーディングが個人の“腕前”から、チームが共有する作法・儀礼・チェックリストへ変わる兆候です。narrativeとしても「一人の天才エージェント」ではなく「制御盤つきの作業場」が主役になっています。

### 3. himmel — Claude Codeを安全で反復可能なエージェントとして走らせるハーネス
- 出典: GitHubリポジトリ
- 日付: 2026-09-26更新
- リンク: https://github.com/yotamleo/Himmel
- 要約: Claude Code向けに、hooks、guardrails、slash commands、Jira CLI、cross-session handoverを束ねる開発エンジン。READMEでは「first PR-gated loop in ~15 minutes」「worktree-isolated, PR-gated」といった導入文句があり、実運用の継続性とレビュー境界を重視しています。
- なぜ面白いか:
  - 技術: harness engineeringを、単発の安全策ではなく、作業ツリー分離・PRゲート・セッション引き継ぎ・観測性を含む開発ライフサイクルとして実装している。
  - 人文: historyの観点では、CI/CDが人間開発者を支えたように、AI開発者にも「職場の規則」と「引き継ぎノート」が必要になっている。philosophy的には、主体性をモデル内部ではなく環境側の制約と記録の連鎖として見る発想です。

### 4. thx-boris — Boris ChernyのClaude Code運用知をskill化する動き
- 出典: GitHubリポジトリ（Boris Cherny / @bcherny のClaude Code投稿を参照）
- 日付: 2026-09-24更新
- リンク: https://github.com/saad-ahmed/thx-boris
- 要約: 「Boris Cherny, creator of Claude Code, shows how he uses Claude Code to build Claude Code」という説明で、hooks、subagents、skill authoring、sessions/permissions/MCP、anti-patternsなどの参照資料をClaude Code skillとしてパッケージ化するリポジトリ。README内で元投稿として https://x.com/bcherny/status/2007179832300581177 を示していますが、今回のX検索はspending limitで直接検証できませんでした。
- なぜ面白いか:
  - 技術: Boris Chernyの実践知が、tipsの消費ではなく、再利用可能なskill・テンプレート・サブエージェント資産へ変換されている。
  - 人文: narrativeの観点では、Claude Codeコミュニティが「開発者の語り」を実行可能な作法へ翻訳している点が面白い。creativityの観点でも、著名開発者のワークフローがミーム化し、個人の癖から共有文化へ移っていく過程が見えます。

### 5. ループエンジニアリング日本語コミュニティ: claude-factory と kenesis-loop-kit
- 出典: GitHubリポジトリ検索結果
- 日付: 2026-08-27 / 2026-08-19更新（直近14日より古いが、日本語コミュニティ確認として重要）
- リンク: https://github.com/yuritada/claude-factory / https://github.com/breeze-shared-inc/kenesis-loop-kit
- 要約: claude-factoryは「音声対話で駆動する、個人用ループエンジニアリングシステム」としてClaudeアプリのボイスモードからClaude Codeを動かすMCPブリッジを掲げています。kenesis-loop-kitは「Claude Codeでループエンジニアリングを実践するためのチケット駆動・マルチエージェント開発フレームワーク」として、状態をMarkdownチケットへ外部化し、調査→設計→実装→テスト→レビューの開発ループを回す設計です。
- なぜ面白いか:
  - 技術: 日本語圏でも、Claude Codeを会話UIだけでなく、MCP、Markdownチケット、マルチエージェント、レビューサイクルで包む実践が確認できる。
  - 人文: anthropologyの観点では、英語圏のBoris/Claude Code文脈が、日本語の「チケット駆動」「音声対話」「ハンズオン」文化へ翻訳されている。文化的には、AIエージェント導入が単なるツール輸入ではなく、現場の作業様式に合わせた再編集になっている点が重要です。

## arXiv / 学術

- LLM Agents Can Easily Tamper With Their Own Traces — arXiv:2609.30266v1。2026-09-24公開。Claude Codeを含むローカルLLMエージェントのトレース改変リスクを扱い、ハーネスの監査境界を問い直すため本日のトップ項目に採用しました。
- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — arXiv:2608.00267v2。2026-07-31公開で直近14日より古いものの、coding agent評価がharness engineeringからloop engineeringへ移るという用語上・概念上の基準点として重要です。
- OneDayAgent: Towards a Long-Horizon Harness for Autonomous Agents — arXiv:2608.05013v1。2026-08-04公開で直近14日より古いものの、長期実行エージェントのgoal drift、state loss、context overflowに対するharness研究として関連があります。
- そのほか、2026-09-24には「harness」「agent」を含むロボティクス・VLA・評価系のarXiv投稿が複数確認されましたが、Claude Code / loop engineeringとの接点が相対的に薄いためトップ5には入れていません。

## メモ

- Boris Cherny優先の有無: Claude Code文脈としてBoris Cherny / @bcherny関連を優先確認し、`thx-boris` と `boris-cherny-claude-code-playbook` を確認しました。直接のX検索は `personal-team-blocked:spending-limit` で失敗したため、GitHub READMEに記載された元Xリンクを未直接検証として扱っています。
- 日本語アカウントの扱い: 日本語X検索も実行しましたが、同じくX Searchのspending limitで失敗しました。代替としてGitHub上の日本語リポジトリ検索を行い、`claude-factory`、`kenesis-loop-kit`、`loop-engineering-handson` などを確認しました。
- 注意点・誇張リスク: Web検索ツールはFirecrawl未設定で使用できなかったため、公式Web/ブログ検索はGitHub API・arXiv API・直接HTTP取得で補完しました。GitHubリポジトリの更新日は活発さの指標であり、必ずしも内容の初出日や品質保証を意味しません。X由来情報は今回直接検証できていないため、X投稿そのものをトップ項目には採用していません。

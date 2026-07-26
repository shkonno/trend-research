# Harness engineering トレンド調査 (2026-07-26)

- 調査日: 2026-07-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIコーディングの焦点は「賢いモデル」単体から、モデルを安全に回し、記憶・権限・評価・分業を外側から支えるハーネス設計へ移っている。

## トップ5

### 1. A harness for every task: dynamic workflows in Claude Code
- 出典: Anthropic / Claude Blog
- 日付: 2026-06-02公開、2026-07-23更新（古いが直近更新あり）
- リンク: https://claude.com/blog/a-harness-for-every-task-dynamic-workflows-in-claude-code
- 要約: Claude Codeがタスクごとに独自のマルチエージェント・ハーネスをその場で書き、調査、セキュリティ分析、Code Review、agent teamsなどのワークフローを構成できるという記事。デフォルトのコーディング用ハーネスを超えて、複数の視点・検証・再利用可能なワークフローを組み立てる方向性が示されている。
- なぜ面白いか:
  - 技術: 「エージェントを使う」から「エージェントが自分の実行環境・分業・検証ループを生成する」へ一段抽象度が上がっている。
  - 人文: これは職人が工具箱を選ぶ段階から、仕事ごとに工房そのものを組み替える段階への移行に近い。人間側には、どの仕事を自動化するかだけでなく、どんな検証文化や責任分担をハーネスに埋め込むかが問われる。

### 2. Delivery, Not Storage: Cue-Anchored Working Memory as a Harness Property for Coding Agents
- 出典: arXiv
- 日付: 2026-07-23
- リンク: https://arxiv.org/abs/2607.20972v1
- 要約: コーディングエージェントの長期運用では、メモリを「文書として保存して自発的に読む」だけでは不十分で、状況の手がかりに応じてハーネスが決定論的に記憶を注入するべきだと主張する論文。実験では、任意のメモリ利用がほぼ発生しない一方、ハーネス所有の cue-anchored memory は compaction をまたいでも情報を届けられると報告している。
- なぜ面白いか:
  - 技術: メモリをモデル能力ではなくハーネスの配送責務として扱うため、長時間・反復タスクでの失念や再読コストを構造的に減らせる。
  - 人文: 人間の熟練も、手順書だけでなく「この場面ではこれを思い出す」という身体化された手がかりに支えられている。AIエージェント設計が、記憶をデータベースではなく作業環境との関係として捉え始めた点が興味深い。

### 3. Tencent WorkBuddy Bench: A Multi-Domain Coding-Agent Benchmark with Contamination-Resistant Task Construction
- 出典: arXiv
- 日付: 2026-07-23
- リンク: https://arxiv.org/abs/2607.20911v1
- 要約: Code、Web、Office、Securityの4領域にまたがるコーディングエージェント評価スイートで、実コミットや業務シナリオからタスクを再構成し、検索で答えが拾われにくい contamination-resistant な作りにしている。評価ハーネス、テスト、参照解、データセットを公開し、CodeBuddy CodeとClaude Codeの2つの agent harness で実行したと説明している。
- なぜ面白いか:
  - 技術: ベンチマークを単なる問題集ではなく、環境・採点・ハーネス・監査可能性を含む再現可能な実行系として設計している。
  - 人文: 「AIが仕事をできるか」を測るには、現場の曖昧な依頼やセキュリティ文脈をどう再現するかが重要になる。評価設計そのものが、仕事という文化的実践をどうモデル化するかという問いになっている。

### 4. Orca: local harness for Claude Code / Codex subagents
- 出典: GitHub repository
- 日付: 2026-05-29作成、2026-07-26更新（古いが直近更新あり）
- リンク: https://github.com/alex2481kobe/orca
- 要約: Claude CodeやCodexなど既存のCLIエージェントを変えずに、MCP経由でサブエージェントを spawn し、待機し、結果を判定するローカルデーモン型ハーネス。READMEでは「新しいチャットUIやモデルではなく、既に使っているCLIエージェントの周囲に置くハーネス」と位置づけ、git worktree分離、監査ゲート、スマホ用ダッシュボードなどを掲げている。
- なぜ面白いか:
  - 技術: モデル非依存・CLI非依存の外部ハーネスとして、複数エージェントの依存関係、実行隔離、判定をローカルに寄せている。
  - 人文: これは「万能AIアプリ」ではなく、既存の作業習慣を尊重しながら周辺の足場を強くする発想である。人間の監督者が複数の職人を束ねるように、ハーネスが作業者間の約束事を保持する。

### 5. Skill Harness: reusable AI agent skills の評価ハーネス
- 出典: GitHub repository
- 日付: 2026-06-04作成、2026-07-26更新（古いが直近更新あり）
- リンク: https://github.com/MrBinnacle/skill-harness
- 要約: Claude Codeを含むエージェント向けスキルが本当に役立つかを、同じタスクを「スキルあり/なし」で走らせて KEEP / CUT / UNMEASURED と判定する評価ハーネス。READMEでは、測れないものにもっともらしい点数を付けず、UNMEASURED と明示する姿勢を前面に出している。
- なぜ面白いか:
  - 技術: スキルをコンテキストに常駐させるコストを、実行比較と保守判断の問題として扱い、エージェント拡張の棚卸しを可能にする。
  - 人文: 「役に立っている気がする」を数値のふりで正当化せず、測定不能を測定不能として扱う倫理がある。AI時代の道具選びでは、追加する能力だけでなく、捨てる勇気と説明責任も重要になる。

## arXiv / 学術
- Delivery, Not Storage: Cue-Anchored Working Memory as a Harness Property for Coding Agents — arXiv:2607.20972v1。ハーネス所有の手がかり付きメモリ配送を、コーディングエージェントの信頼性要件として扱う。
- Tencent WorkBuddy Bench: A Multi-Domain Coding-Agent Benchmark with Contamination-Resistant Task Construction — arXiv:2607.20911v1。評価ハーネスとデータセットを公開し、Claude Codeを含む agent harness 上でマルチドメイン実務タスクを検証する。

## メモ
- Boris Cherny優先の有無: X検索で `from:bcherny` を含むクエリを実行したが、x_search は credits / subscription 制限で失敗した。Bing RSSによる `site:x.com` 代替検索でも Boris Cherny / @bcherny と Harness engineering の有効な接点は確認できなかったため、本ファイルでは未確認として扱う。
- 日本語アカウントの扱い: 日本語クエリ（Claude Code、ハーネス、評価ハーネス、ループエンジニアリング等）を試したが、X検索は同上の制限、Bing RSSは汎用Claude解説や辞書系ページが中心で、採用できる日本語コミュニティ発信は確認できなかった。
- 注意点・誇張リスク: GitHub項目はスター数が少なく、エコシステムの確立というより「兆し」として扱うべき。Web検索ツールは未設定、X検索は外部課金制限により直接結果が得られなかったため、公式ページ、GitHub API、arXiv API、Bing RSS、直接HTTP取得で補完した。

# Claude Code トレンド調査 (2026-10-02)

- 調査日: 2026-10-02
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Claude Code は「よく動くCLI」から、mod・AGENTS.md・MCP・監視・安全研究を巻き込んだ拡張可能な作業環境へ一段進んでいる。

## トップ5

### 1. Claude Code Mods: TypeScriptでClaude Codeの挙動そのものを拡張
- 出典: Anthropic公式ブログ / Claude Code公式ドキュメント / Hacker News
- 日付: 2026-10-01
- リンク: https://claude.com/blog/claude-code-mods
- 要約: Anthropicは、Claude Codeのプロンプト、ツール呼び出し、UI、コマンドなどをTypeScript関数で変更できる「Mods」を公開した。公式ドキュメントでは、modはClaude Code内部で動くプラグインとして、ペイン追加、ツール呼び出しの保留・変更、独自コマンド実行、状態共有などを可能にすると説明されている。
- なぜ面白いか:
  - 技術: Claude Codeが単なるLLM付き端末ではなく、イベントフックとUI拡張を持つエージェント実行基盤へ近づいた点が大きい。
  - 人文: 開発者は「AIに何を頼むか」だけでなく「AI作業環境をどのような制度・儀礼・監督構造にするか」を設計する立場になる。便利さと同時に、modがユーザー権限でファイル・秘密情報・セッションを見られるという信頼の問題も前面化した。

### 2. Claude Code v2.1.287: “You should know” サイドエージェントと運用系修正
- 出典: Claude Code CHANGELOG / GitHub Releases相当の公式変更履歴
- 日付: 2026-10-01
- リンク: https://code.claude.com/docs/en/changelog.md
- 要約: v2.1.287では、深い挙動変更を許すClaude Modsに加え、見落としを横から指摘する組み込みmod “You should know” が追加された。MCPサーバーのURL prompt、OpenTelemetryの`prompt_text`、Remote Control、tool heartbeat、危険な`rm`に関する安全確認、screen reader周りなど、多数の実運用修正も入っている。
- なぜ面白いか:
  - 技術: 本体エージェントとは別の監視的サイドエージェントを入れることで、単一モデルの推論品質だけでなく、作業中の注意配分や見落とし検出をシステム側で補強している。
  - 人文: 「優秀な個人アシスタント」像から、「同僚・レビュアー・見張り役が同じ作業場にいる」像へ移っている。これは開発現場の責任分担や、誰が最後に気づくべきだったのかという倫理的問いを変える。

### 3. AGENTS.md対応: CLAUDE.md以外のエージェント指示ファイルを読む組み込みmod
- 出典: GitHub commit / built-in `agents-md` README / Hacker News
- 日付: 2026-09-18（HNでは2026-09-20にも再共有）
- リンク: https://github.com/anthropics/claude-code/commit/a92ea1cdb11ad21f9d583fad2db181dfdac918a6
- 要約: Claude Codeに、`AGENTS.md`を`CLAUDE.md`と同様のプロジェクト指示として扱うbuilt-in modが追加された。`claude-md-or-agents-md`、`claude-md-and-agents-md`、`managed-only`などのモードで、既存のCLAUDE.md文化とAGENTS.md文化の併存を調整できる。
- なぜ面白いか:
  - 技術: リポジトリ内のエージェント向け指示を特定ベンダー名に閉じず、複数ツールが共有しやすい形式へ寄せる実装で、プロジェクトコンテキスト管理の相互運用性が上がる。
  - 人文: これはAI開発環境における「作法の標準化」に近い。人間のオンボーディング文書と同じように、エージェントにも共同体のルールや禁忌を読ませる文化が制度化されつつある。

### 4. 日本語実践: `.mcp.json`でMCPサーバー設定をチーム配布する手順
- 出典: Qiita（日本語実践記事）
- 日付: 2026-10-02
- リンク: https://qiita.com/yureki_lab/items/fd65228d931a9c33cbde
- 要約: 日本語圏では、Claude CodeのMCPサーバー設定を`.mcp.json`でチームに配る実装手順や、local/project/userスコープの優先順位、`${VAR}`展開、承認待ちでプロジェクトサーバーが出てこない問題など、導入時の具体的な詰まりどころを扱う記事が出ている。単なる新機能紹介ではなく、チーム運用で「なぜ動かないのか」を潰すタイプの実践共有になっている。
- なぜ面白いか:
  - 技術: MCP連携を個人のローカル設定から、リポジトリ・チーム単位で再現可能な設定配布へ移すことで、Claude Codeの利用を属人的な環境構築から運用設計へ押し上げている。
  - 人文: 日本語圏の実践記事は、華やかなデモよりも「権限、スコープ、承認、環境変数で詰まる」という現場の摩擦を丁寧に言語化している。AI導入の文化は、成功談よりもこうした失敗の共有によって成熟する。

### 5. Skill-Based AI Agents for Power-System Studies: Claude Code CLIを工学研究ワークフローに組み込む
- 出典: arXiv
- 日付: 2026-09-30
- リンク: http://arxiv.org/abs/2609.40272v1
- 要約: 電力系統解析向けに、MCP接続された工学ツール、再利用可能なskills、subagents、ローカルshell/Python実行を組み合わせたskill-based agentic frameworkを提案し、OpenAI Agents SDK経路とClaude Code CLI経路を評価している。Claude Codeが一般的なソフトウェア開発だけでなく、専門領域のシミュレーション・検証作業に持ち込まれている点が重要である。
- なぜ面白いか:
  - 技術: Claude Codeのread/write/bash/MCP/subagent的なプリミティブが、専門家の解析ツールをつなぐ実験基盤として使われ、LLMエージェントがドメイン固有ツールチェーンに接続されている。
  - 人文: 電力系統のような公共性の高い領域では、AIによる効率化は単なる生産性問題ではなく、専門家の判断、説明責任、安全余裕と結びつく。人間専門家がどこで介入するかを明示する研究は、AIを社会インフラに入れる際の重要な語彙になる。

## arXiv / 学術
- Skill-Based AI Agents for Power-System Studies / arXiv:2609.40272v1 / 2026-09-30。Claude Code CLIをMCP・skills・subagentsと組み合わせ、電力系統解析の専門ワークフローで評価。
- Pretext: Defeating Malicious Skill Detection Frameworks for AI Agents / arXiv:2609.39607v1 / 2026-09-30。Claude Code周辺のskills/mods的拡張が広がるほど、悪性スキル検出・回避の問題が重要になる。
- Approval Laundering: Systematizing Approval--Execution Binding Failures in AI Coding-Agent Harnesses / arXiv:2609.38983v1 / 2026-09-30。承認した操作と実際に実行される操作の結びつきが崩れる問題を扱い、Claude Codeのような承認型コーディングエージェント運用に近い。

## メモ
- Boris Cherny優先の有無: @bcherny / Boris Chernyを含むX検索を最優先で試行したが、x_searchは`personal-team-blocked:spending-limit`で失敗した。Hacker News APIやローカル過去レポート検索でも、直近14日のClaude Codeに直接紐づくBoris Cherny本人発言は確認できなかったため、未確認の投稿は採用していない。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で失敗した。代替としてQiita APIで直近の日本語Claude Code実践記事を確認し、MCP設定配布の記事をトップ5に含めた。
- 注意点・誇張リスク: Hermesの標準`web_search`/`web_extract`はFirecrawl未設定で失敗したため、公式ドキュメント・公式ブログ・GitHub raw/patch・Hacker News Algolia API・Qiita API・arXiv APIを直接HTTP取得して確認した。X上の反応量は確認できていないため、ランキングは「実URLで確認できた一次情報・実践性・研究的含意」を基準にした。

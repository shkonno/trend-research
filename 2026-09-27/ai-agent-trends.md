# AI agent trends トレンド調査 (2026-09-27)

- 調査日: 2026-09-27
- 情報源: X / Web / arXiv（X検索は xAI クレジット上限、Web検索は Firecrawl 未設定で失敗。代替として GitHub API、公式ドキュメント直取得、arXiv API、X公開ページへの直接HTTP確認を使用）
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの焦点は「賢いデモ」から、モデル制御・監査ログ・MCP接続・本番デプロイを含む運用可能性へ移っている。

## トップ5

### 1. Claude Code v2.1.283: 管理設定・MCP進捗・OpenTelemetryが運用寄りに強化
- 出典: GitHub Releases（anthropics/claude-code）
- 日付: 2026-09-25
- リンク: https://github.com/anthropics/claude-code/releases/tag/v2.1.283
- 要約: Claude Code v2.1.283 では、`availableModelsMatch` と `deniedModels` によるモデル利用制御、MCP/WebFetch/WebSearch出力の OpenTelemetry 記録、`/doctor prompt-audit`、MCP進捗通知や stdio MCP サーバ終了処理の修正が追加された。GitHub API上では Claude Code リポジトリ自体も 2026-09-27 時点で更新が続いており、エージェントCLIが組織運用の対象になっていることが分かる。
- なぜ面白いか:
  - 技術: エージェントの失敗を「モデルが悪い」で済ませず、モデル許可リスト、トレース、MCPライフサイクル、プロンプト監査まで管理面を細かく制御し始めている。
  - 人文: これは開発者個人の相棒から、組織の統制対象としてのAIへの移行を示す。便利さとガバナンスの緊張が、日々の開発文化そのものに入り込んできた。

### 2. arXiv: “LLM Agents Can Easily Tamper With Their Own Traces” が監査ログの前提を揺さぶる
- 出典: arXiv API
- 日付: 2026-09-24
- リンク: http://arxiv.org/abs/2609.30266v1
- 要約: 論文は、Claude Code、Codex、Antigravity、Open Code、Grok Build などのローカルLLMエージェントが、自身の実行トレースを削除できる境界不備を示した。著者らは、監査・インシデント調査・コンプライアンス用ログをエージェントの制御外に置く独立した傍受メカニズムで保存すべきだと提案している。
- なぜ面白いか:
  - 技術: エージェント監視の根拠であるトレースが改ざん可能なら、評価・監査・安全性検証の基盤をホスト外または権限分離された層に置き直す必要がある。
  - 人文: 「行為者が自分の記録を編集できる」という問題は、会計・歴史記述・権力監視と同じ古典的テーマである。AIエージェントにも、記憶と証言を誰が管理するかという制度設計が必要になった。

### 3. GitHub MCP Server v1.12.2: Issue/PR コメント操作が細かく拡張
- 出典: GitHub Releases（github/github-mcp-server）
- 日付: 2026-09-16
- リンク: https://github.com/github/github-mcp-server/releases/tag/v1.12.2
- 要約: GitHub公式MCP Server v1.12.2 は `update_issue_comment`、Issue/PRコメントリアクション削除系ツールを追加した。大きな新機能ではないが、エージェントがGitHub上の共同作業に参加する際の「編集」「取り消し」「反応管理」が粒度高くなっている。
- なぜ面白いか:
  - 技術: MCPが読み取り・検索だけでなく、GitHub上の協働オブジェクトを細かく変更する操作面へ進んでいる。
  - 人文: エージェントがコメントやリアクションを扱えるようになると、開発チームの会話空間そのものに機械が参加する。誰が発言を編集し、誰が合意を示したのかという社会的意味を、ツール設計が背負うことになる。

### 4. GoLive Skill v0.1.0-alpha.4: エージェントに本番デプロイを任せるための信頼文書と確認手順
- 出典: GitHub Releases（mikehasa/golive-skill）
- 日付: 2026-09-26
- リンク: https://github.com/mikehasa/golive-skill/releases/tag/v0.1.0-alpha.4
- 要約: GoLive Skill は、エージェントがホスティング、DB、ドメイン、メール、決済などを検出・計画・承認・適用・検証するためのオープンソースAgent Skill。alpha.4では日本語を含む複数言語README、初回本番デプロイ時の `--confirm-live`、信頼・復旧文書、認証情報削除、レポートの秘匿化などが追加された。
- なぜ面白いか:
  - 技術: エージェントの自動化対象がコード生成から、本番環境の構成・リカバリ・資格情報管理まで広がっている。
  - 人文: 「AIに本番権限を渡せるか」という問いに、機能だけでなく信頼文書、確認儀式、翻訳、復旧手順で答えようとしている点が重要である。自動化は技術より先に、安心して委任できる物語を必要とする。

### 5. ZCode v3.14.3: 長時間ワークフローの並行度・再利用・状態表示を改善
- 出典: GitHub Releases（zai-org/ZCode）
- 日付: 2026-09-24
- リンク: https://github.com/zai-org/ZCode/releases/tag/v3.14.3
- 要約: Z.ai の coding agent harness である ZCode は、実行中ワークフローの並行度を停止せず調整できる機能、ワークフロー修正・再起動時の再利用ロジック、大規模ワークフローのリアルタイム状態表示、スクリプト送信・修正効率の改善を加えた。GitHub APIでは 2026-09-20 作成、2026-09-27 時点で 6,800 star 超の新興プロジェクトとして確認された。
- なぜ面白いか:
  - 技術: エージェント実行を単発のチャットではなく、並行度・状態表示・再実行コストを持つワークフロー実行基盤として扱っている。
  - 人文: 人間の仕事は常に「途中で状況が変わる」ため、停止せず調整できるエージェント基盤は人間の現場感覚に近い。AIを命令機械ではなく、変化する作業場の参加者として設計する方向性が見える。

## arXiv / 学術
- LLM Agents Can Easily Tamper With Their Own Traces — arXiv:2609.30266v1。ローカルLLMエージェントが自分のトレースを削除できる問題を報告し、独立したログ取得機構を提案。
- Coding Agents for Generalized Task and Motion Planning Problems — arXiv:2609.30233v1。Claude Code と Codex 系エージェントを、一般化TAMP問題のプログラム合成に使う研究。100件近い環境評価で、手作りプランナや一発生成より高い成功率を示したと報告。
- RAPID: Robot Agentic Programming from Demonstrations — arXiv:2609.30249v1。1つの視覚デモからロボットプログラムを生成・検証・改良するエージェントループを提案。

## メモ
- Boris Cherny優先の有無: @bcherny を対象に X検索ツールを実行したが、xAI側の `personal-team-blocked:spending-limit` により取得できなかった。X公開ページ `https://x.com/bcherny` も直接HTTPではプロフィールHTMLのみ確認でき、直近投稿本文は取得できなかったため、Boris発の項目は本日トップ5に入れていない。
- 日本語アカウントの扱い: 日本語クエリでX検索を実行したが同じクレジット上限で失敗。代替として GoLive Skill の日本語README追加を日本語圏読者に関係する実践例として扱った。日本語圏X実践例は本調査時点では実ツールで確認できなかった。
- 注意点・誇張リスク: Web検索ツールは Firecrawl 未設定で失敗したため、一般Web記事の横断検索は限定的。GitHub API、公式リリース、公式ドキュメント、arXiv APIで検証できるリンクだけを採用し、X由来の未確認情報は採用していない。

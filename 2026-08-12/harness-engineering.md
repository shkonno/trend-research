# Harness engineering トレンド調査 (2026-08-12)

- 調査日: 2026-08-12
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「プロンプトを書く技術」から、フック・権限・作業木隔離・評価・監査ログでエージェントを運用可能にする実装規律へ移っている。

## トップ5

### 1. Claude Code Hooks reference が、Stop/PreToolUse/Task 系まで含む実行制御面を明文化

- 出典: Anthropic 公式ドキュメント
- 日付: 2026-08-12 時点でページ更新確認
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks
- 要約: Claude Code の hooks 参照には、PreToolUse / PostToolUse / PermissionDenied / Stop / SubagentStart / TaskCreated / TaskCompleted など、エージェント実行の前後や失敗点に差し込む制御点が整理されている。ハーネスエンジニアリングの中核である「モデルの外側で止める・記録する・許可する」ための公式インターフェースが見える。
- なぜ面白いか:
  - 技術: フックは自然言語ルールを実行時ポリシーに落とす接合部で、stop-hook gates、権限チェック、監査ログ、MCP ツール制御を同じ設計面で扱える。
  - 人文: これは「AIに何を言い聞かせるか」ではなく「組織がどこで介入責任を負うか」という制度設計の問題である。人間の職場でいう承認印・監査証跡・作業分掌が、エージェントの身体にあたる harness に移植されている。

### 2. Claude Code 2.1.222 の worktree 隔離・PreToolUse 修正が、ハーネス安全性の実運用論点を浮かび上がらせた

- 出典: Anthropic 公式リリースノート
- 日付: 2026-08-12 調査時点のリリースノート掲載内容
- リンク: https://docs.anthropic.com/en/release-notes/claude-code
- 要約: リリースノートでは、worktree 隔離セッションとその subagent がメイン checkout に対して破壊的 git コマンドを実行できていた問題の修正、また background agent tasks で PreToolUse auto-allow hooks が tool restrictions を迂回していた問題の修正が確認できた。これは harness の安全性が「機能追加」ではなく、境界条件のバグ修正として日々鍛えられていることを示す。
- なぜ面白いか:
  - 技術: worktree isolation、Bash/file edit の適用範囲、PreToolUse の許可判定は、Claude Code / loop engineering の安全な自動化に直結する低レイヤの制御点である。
  - 人文: 自律エージェントの失敗はしばしば「悪意」ではなく、権限境界の曖昧さから生まれる。ここでは責任の所在をモデルから環境設計へ移し、事故後に規則をどう修正するかという歴史的な安全工学に近い動きが見える。

### 3. arXiv: SHE — Trajectory-driven Safety Harness Evolution for LLM Agents

- 出典: arXiv
- 日付: 2026-08-10
- リンク: http://arxiv.org/abs/2608.09885v1
- 要約: SHE は、LLM agent の安全性をモデル重みだけでなく、context、memory、tools、permissions、runtime control を管理する agent harness の問題として扱う論文。固定的なデプロイ成果物としての harness ではなく、軌跡からリスクを読み取り進化させる対象として捉える点が、直近の harness engineering そのものに近い。
- なぜ面白いか:
  - 技術: 実行軌跡を入力にして harness コンポーネントの安全責任を再配分する発想は、評価・監査・自動修復をつなぐ研究方向である。
  - 人文: これは「安全なAIを一度作れば終わり」という神話への反論でもある。社会制度が事故事例を通じて改訂されるように、エージェントの制度＝harness も運用史を持つものとして描かれている。

### 4. oh-my-agent — stop-hook gates / independent judges / append-only event logs を掲げる multi-agent harness

- 出典: GitHub リポジトリ
- 日付: 2026-08-12 更新確認
- リンク: https://github.com/first-fluke/oh-my-agent
- 要約: GitHub 検索で、Claude Code、Codex、Cursor など複数ランタイムをまたぎ、成果物ベースで agent run を検証する multi-agent harness として oh-my-agent が上位に出た。説明文では stop-hook gates、independent judges、append-only event logs が明示され、単一モデルではなく「検査する仕組み」を中心に置いている。
- なぜ面白いか:
  - 技術: 複数エージェント／複数ランタイムを同じ監査ログと判定器に通すことで、Claude Code 固有のワークフローからポータブルな harness へ抽象化している。
  - 人文: 「AIが作ったから信じる」のではなく「証跡と第三者的判定で信頼を組み立てる」方向で、ソフトウェア開発における信頼の根拠が会話から記録へ移っている。これは職人芸を制度化する動きでもある。

### 5. 日本語コミュニティで CLAUDE.md / Hooks / ハーネス入門が急増

- 出典: Qiita 記事群
- 日付: 2026-08-10〜2026-08-12
- リンク: https://qiita.com/shun123/items/c28d04b6ded6afe60847
- 要約: Qiita API 検索では「CLAUDE.mdに何を書けばいいか分からない人向け｜ハーネスエンジニアリングの最初の一歩」（2026-08-11）、「Claude Codeに『違反できないコード』を書かせる：ガイドとセンサーの設計」（2026-08-11）、「CLAUDE.mdは書いても守られない——ルールが効かなくなる3つの理由と、22件の事故から学んだハーネスエンジニアリング」（2026-08-10）などが確認できた。日本語圏でも、単なるプロンプト共有から、CLAUDE.md、hooks、sensor、事故学を含む運用設計へ関心が移っている。
- なぜ面白いか:
  - 技術: CLAUDE.md を静的ルール、Hooks を動的制御、センサーを観測面として分ける発想は、Claude Code を現場導入する際の最小 harness 設計になる。
  - 人文: 日本語コミュニティでは「AIに仕事を任せる不安」を、人格論ではなく作業手順・事故例・ガードレールで語り直している。これは自動化への恐れを、共同作業の作法へ翻訳する文化的プロセスとして面白い。

## arXiv / 学術

- SHE: Trajectory-driven Safety Harness Evolution for LLM Agents — arXiv:2608.09885v1 — agent harness を context / memory / tools / permissions / runtime control の安全進化問題として扱う。
- Evo-Bench: Can Language Models Improve Agent Harness? — arXiv:2608.09096v1 — harness evolution を、通常のタスク解決能力から切り分けて測るベンチマークとして確認。
- A^2E: An End-to-End Agent Auditing Engine — arXiv:2608.07346v2 — agent harness ecosystem に対する包括的な評価・監査パイプラインとして関連。
- Skill-Use: Can LLMs Actually Use Skills in Agentic Harnesses? — arXiv:2608.04828v1 — skills を agentic harness 内で実際に認識・適用できるかを評価する研究として関連。

## メモ

- Boris Cherny優先の有無: X 検索で @bcherny / Claude Code / harness / loop engineering を確認しようとしたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、Boris Cherny の直近投稿は本調査では確認できなかった。
- 日本語アカウントの扱い: X 日本語検索も同じ理由で失敗したため、代替として Qiita API で日本語コミュニティ記事を確認し、トップ5の第5項目に反映した。
- Web検索の注意: Hermes の web_search / web_extract は Firecrawl 未設定で失敗したため、公式ドキュメント、GitHub API、Qiita API、HN Algolia API、arXiv API への直接 HTTP 取得で補完した。
- 注意点・誇張リスク: GitHub リポジトリのスター数や説明文は検索 API 取得時点のメタデータであり、実装品質を保証しない。Qiita 記事群もコミュニティの関心を示す材料として扱い、個別主張の真偽は未検証。

# Loop engineering トレンド調査 (2026-08-18)

- 調査日: 2026-08-18
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Loop engineering は「モデルを一度呼ぶ」から、計画・実行・観測・レビュー・再試行をどう閉じるかへ焦点が移り、エージェント運用の設計論として急速に具体化しています。

## トップ5

### 1. neal: planner / coder / reviewer を分けるローカル multi-agent coding loop
- 出典: HN / GitHub README
- 日付: 2026-08-13（Show HN）、2026-08-17（GitHub updated / pushed）
- リンク: https://github.com/navels/neal
- 要約: neal は、planner、coder、reviewer を別ロールとして動かし、計画をスコープに分割して実装・レビュー・最終レビューまで回すローカルな coding loop です。README では、coder と reviewer を別ベンダーにして「同じモデルが自分を採点する」問題を避け、各スコープを新しいコンテキストで始めることで長期タスクのドリフトを抑える設計が強調されています。
- なぜ面白いか:
  - 技術: ループの単位を「1プロンプト」ではなく、plan → scoped execution → read-only review → final review → resumable artifacts に分解しており、実務の変更管理に近い制御面を持っています。
  - 人文: philosophy の観点では、これは「判断主体」を単一の知能ではなく役割分担された制度として設計する試みです。history 的にも、ペアプログラミングやコードレビューの社会的慣行を、LLM 時代の機械的なチェック・アンド・バランスへ翻訳している点が興味深いです。

### 2. Substructure: TOML と webhook で agent loop を外部システムから制御するエンジン
- 出典: HN / 公式サイト / 公式ドキュメント
- 日付: 2026-08-13（Show HN、docs updated）
- リンク: https://substructure.ai/
- 要約: Substructure は、クラウドまたはセルフホストで動くエージェント実行エンジンで、`substructure.toml` に LLM、MCP、Slack、agent を記述して運用できます。`llms.txt` と docs では、engine が各ステップを提案し、webhook 側が承認・変更・一時停止・独自ツール実行を返すことで、SDK なしに loop を制御できると説明されています。
- なぜ面白いか:
  - 技術: loop の中身を black box にせず、decision proposal を HTTP 境界で差し替え可能にしているため、人間承認、既存業務システム、MCP 認可、Slack セッションを同じ制御面に乗せられます。
  - 人文: anthropology の観点では、エージェントが「個人のラップトップ上の相棒」から「チーム共有の業務参加者」へ移る瞬間を示しています。ethics 的には、鍵や承認や人間の割り込みを loop の設計要素に入れることが、責任所在を曖昧にしないための重要な前進です。

### 3. HyperProbe: 本番障害を read-only probe で閉じる AI on-call loop
- 出典: HN / 公式サイト
- 日付: 2026-08-05（Launch HN）
- リンク: https://www.hyperprobe.co
- 要約: HyperProbe は、PagerDuty、Datadog、Slack などのアラートを起点に、ログ・トレースを読み、疑わしい行に read-only の仮想 breakpoint / probe を置き、本番トラフィックから変数状態を捕捉して RCA を確認する AI on-call agent です。公式サイトでは、probe は非停止・読み取り専用・監査ログ付き・承認ゲート可能で、PII redaction や private VPC / self-hosting も掲げています。
- なぜ面白いか:
  - 技術: 観測不足のまま推論を続けるのではなく、loop の途中で「本番から追加証拠を安全に取る」アクションを入れて diagnosis を閉じる設計になっています。
  - 人文: ethics の観点では、本番環境に入る AI の権限を read-only と監査可能性に限定する点が重要です。narrative 的には、深夜の war room というエンジニア文化の苦痛を、推測ではなく証拠収集の物語へ変えようとしている点が刺さります。

### 4. Armature: MCP / Claude Connector / ChatGPT App の利用セッションを eval に変換する loop
- 出典: HN / 公式サイト
- 日付: 2026-08-03（Show HN、直近約14日よりやや古いが関連性が高いため採用）
- リンク: https://armature.tech/
- 要約: Armature は、ユーザーが Claude、ChatGPT、MCP 経由でプロダクトをどう使ったかをセッションとして捕捉し、上位ワークフローを eval に変換するとうたうツールです。公式メタデータでは、regression を検知し、改善を出荷前に証明するための analytics and evals for your MCP と説明されています。
- なぜ面白いか:
  - 技術: 実ユーザーの agent session を評価データに戻すことで、observability → workflow mining → eval → regression prevention というプロダクト改善 loop を作っています。
  - 人文: anthropology の観点では、人間がエージェント越しに製品を使う行動そのものが、新しい「利用民族誌」のデータになります。creativity の観点では、トップワークフローを eval 化する発想は、ユーザーの予期せぬ使い方を開発ロードマップへ戻す編集プロセスでもあります。

### 5. Second Thought: ReAct の待ち時間に並列推論を走らせる agent loop 研究
- 出典: arXiv
- 日付: 2026-08-13
- リンク: http://arxiv.org/abs/2608.13667v1
- 要約: 論文 “Second Thought: Reasoning in Parallel as LLM Agents Act and Observe” は、ReAct 型エージェントが action / observation を待つ間に reasoning が凍結される問題を「reasoning idle window」と呼び、Thought 後に複数の補助ブランチを並列生成して観測到着時に統合する training-free framework を提案しています。著者らは、複数ベンチマークで turn count を下げ、main-thread decoding を削減できると報告しています。
- なぜ面白いか:
  - 技術: loop の逐次性を前提にせず、環境待ちの空白を speculative / parallel reasoning に使うことで、agent loop の時間構造そのものを最適化しています。
  - 人文: philosophy の観点では、「行為しながら考える」だけでなく「観察を待ちながら別の可能世界を考える」主体像を示しています。history 的には、OS の非同期処理やパイプライン化の発想が、推論するエージェントの認知モデルへ流れ込んでいるように見えます。

## arXiv / 学術

- 見つかった論文:
  - “Second Thought: Reasoning in Parallel as LLM Agents Act and Observe” — arXiv:2608.13667v1（2026-08-13）。ReAct loop の action / observation 待ち時間を parallel reasoning に使う研究。
  - “ATLAS: Discovering Agent Strategies through LLM-Guided Abstraction and Automata Learning” — arXiv:2608.14352v1（2026-08-14）。agent trajectory から有限状態モデルを復元し、成功経路や failure loop を分析する研究。
  - “When Personal Memory Has No Single Answer: Evaluating LLM Agents under Irreducible Conflict” — arXiv:2608.13921v1（2026-08-14）。長期 memory loop における矛盾・未決定性・過信を評価する研究。

## メモ

- Boris Cherny優先の有無: Loop engineering は Claude 固有トピックではないため Boris Cherny 優先は適用せず、一般の agent loop / observability / eval / orchestration を優先しました。
- 日本語アカウントの扱い: X検索は英語・日本語の両方で実行しましたが、x_search は本調査時点で `personal-team-blocked:spending-limit` により失敗しました。そのため、日本語 X 投稿は確認できず、HN、公式サイト、GitHub、arXiv、直接 HTTP 取得で補完しました。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で失敗したため、検索面は HN Algolia、GitHub API、公式ページの直接取得、arXiv API に依存しています。各項目は実在リンクで確認しましたが、スタートアップの性能主張（例: 時間短縮、低 overhead）は第三者検証ではなく公式記述として扱うべきです。

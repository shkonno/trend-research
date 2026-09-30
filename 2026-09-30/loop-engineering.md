# Loop engineering トレンド調査 (2026-09-30)

- 調査日: 2026-09-30
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「1回の良いプロンプト」から、「観測・判断・実行・検証・回復をどのように循環させるか」という運用設計へ焦点が移っている。

## トップ5

### 1. agentd-dev/source-code: MCP-native な最小エージェント実行ループ
- 出典: GitHub リポジトリ（Web検索代替として GitHub API で確認）
- 日付: 2026-09-30 更新
- リンク: https://github.com/agentd-dev/source-code
- 要約: Rust 製の小さな静的バイナリで、1つの指示と1つの LLM エンドポイントを受け取り、「think → tool call → observe → repeat」を終端状態または新イベントまで回すエージェントランタイム。MCP-native / cloud-native を掲げ、ループをフレームワークではなく運用単位として切り出している点が目立つ。
- なぜ面白いか:
  - 技術: ループの最小構成を「状態遷移・ツール呼び出し・観測・終端条件」に分解しており、agent loop をサービス部品として監視・再起動・再利用しやすい。
  - 人文: anthropology の観点では、AI エージェントが「作業者」ではなく、待機・応答・再開を行う半自律的な制度参加者として扱われ始めている。ethics の観点では、終端条件や再起動条件を誰が決めるのかが、責任境界の設計問題になる。

### 2. mixpeek/amux: 複数コーディングエージェントの制御プレーン
- 出典: GitHub リポジトリ（Web検索代替として GitHub API で確認）
- 日付: 2026-09-29 更新
- リンク: https://github.com/mixpeek/amux
- 要約: Claude Code、Codex、Gemini ワーカーを共有ボード、atomic task、schedule、loop、origin-stamped messaging、model switching、self-healing recovery で束ねる Rust 製の制御プレーン。単一エージェントのループではなく、チームとしてのループを操作対象にしている。
- なぜ面白いか:
  - 技術: 並列ワーカー、タスク粒度、メッセージの出自、モデル切替、自己回復を同じ制御面に置くことで、ループをスケールさせるときの観測可能性と介入点を増やしている。
  - 人文: history の観点では、工場の作業分担やチケット駆動開発の歴史が、AI ワーカーの編成原理として再演されている。narrative の観点では、「AI チームを走らせる」という物語が、個人の相棒 AI から組織的な労働編成へ移っている。

### 3. krishankant/harnessy: agent loop を教材化する Harness engineering コース
- 出典: GitHub リポジトリ（Web検索代替として GitHub API で確認）
- 日付: 2026-09-29 更新（2026-09-28 作成）
- リンク: https://github.com/krishankant/harnessy
- 要約: Python で AI agent harness を週ごとに作る教材で、model adapters、agent loop、tools、context/memory、traces/evals、hooks/approvals、subagents、retries、streaming、cost limits、sandboxing、prompt-injection defense まで扱う。Loop engineering を実務カリキュラムへ落とし込む動きとして興味深い。
- なぜ面白いか:
  - 技術: ループそのものだけでなく、承認、評価、リトライ、コスト制限、サンドボックスを同時に教えることで、loop を安全な実行環境込みで設計する発想になっている。
  - 人文: ethics の観点では、承認フックやコスト上限は「AI に何を任せ、どこで人間が止めるか」という統治設計である。creativity の観点では、教材化によって暗黙知だった agent loop 設計が共有可能なクラフトへ変わっていく。

### 4. TacoTakumi/specflo: Markdown artifacts 上の brainstorm → spec → plan → execute ループ
- 出典: GitHub リポジトリ（Web検索代替として GitHub API で確認）
- 日付: 2026-09-29 更新
- リンク: https://github.com/TacoTakumi/specflo
- 要約: AI coding agents 向けの spec-driven software engineering CLI で、brainstorm、spec、plan、execute の循環を Markdown artifacts としてディスク上に残す。ループの「各反復で何が決まったか」をファイルとして固定する点が、実務上の監査性につながる。
- なぜ面白いか:
  - 技術: 中間成果物を Markdown に固定することで、LLM の一過性のコンテキストを外部化し、再実行・レビュー・差分管理しやすい agent loop にしている。
  - 人文: philosophy の観点では、思考を外部記号に預ける「拡張された心」の実装例として読める。narrative の観点では、コード生成の過程を後から読める物語に変換し、人間が納得や異議申し立てをしやすくする。

### 5. Anthropic「Building effective agents」: evaluator-optimizer などの基礎パターン整理
- 出典: Anthropic Engineering Blog
- 日付: 2024-12-19 公開、2026-08-10 更新（古いが基礎として関連）
- リンク: https://www.anthropic.com/engineering/building-effective-agents
- 要約: 信頼できる AI agents を作るための実践知として、単純な workflow と自律的 agent を分け、prompt chaining、routing、parallelization、orchestrator-workers、evaluator-optimizer などの構成を整理している。Loop engineering の言語を考えるうえで、特に「評価者が出力を検査し、改善者が修正する」循環の基礎資料になる。
- なぜ面白いか:
  - 技術: evaluator-optimizer 型のループは、生成と評価を分離し、品質改善を単発推論ではなく反復制御として扱うため、実装と運用の両方で再利用しやすい。
  - 人文: philosophy の観点では、自己反省を「内面」ではなく、評価器・最適化器・ログという外部構造に分散させている。ethics の観点では、信頼性をモデルの賢さだけに帰さず、検査可能な手続きとして設計する姿勢が重要である。

## arXiv / 学術
- 直近約14日で Loop engineering / agent loop に強く対応する新規 arXiv は、本調査時点で確認されませんでした（arXiv API は 429/timeout が発生したため、直接ページで基礎論文を確認）。
- 古いが関連する基礎文献: 「Reflexion: Language Agents with Verbal Reinforcement Learning」arXiv:2303.11366、2023-03-20 投稿、2023-10-10 最終改訂。リンク: https://arxiv.org/abs/2303.11366
- 古いが関連する基礎文献: 「Self-Refine: Iterative Refinement with Self-Feedback」arXiv:2303.17651、2023-03-30 投稿、2023-05-25 最終改訂。リンク: https://arxiv.org/abs/2303.17651

## メモ
- Boris Cherny 優先の有無: 本トピックは Claude 固有ではないため優先対象外。
- 日本語アカウントの扱い: 日本語 X 検索を実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、X 由来の個別投稿は採用していない。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で失敗したため、GitHub API、公式ページ直接取得、arXiv 直接ページ確認で補完した。上記 GitHub 項目は更新日時ベースでは直近だが、スター数が小さい新興リポジトリも含むため、普及度ではなく「loop engineering 的に面白い設計要素」を基準に選定した。

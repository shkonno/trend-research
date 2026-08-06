# AI agent trends トレンド調査 (2026-08-06)

- 調査日: 2026-08-06
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの話題は「賢いモデル」から、複数エージェントの運用、コスト可視化、MCP経由の実世界操作、長時間タスクの検証可能な継続へ移っている。

## トップ5

### 1. agentacct: コーディングエージェントの作業・費用・トークンをローカルで可視化
- 出典: GitHub リポジトリ（GitHub検索およびREADMEを直接確認）
- 日付: 2026-07-24 作成（GitHub検索結果で確認）
- リンク: https://github.com/mikehasa/agentacct
- 要約: Claude Code、Codex、OpenCodeなどがローカルに残すセッションログを読み、ツール利用、変更ファイル、テスト実行、時間、トークン、推定コストをTUIで表示するローカルファーストの「Agent Work Intelligence」。ログイン、サーバー、テレメトリなしでエージェント作業を監査できる点が強い。
- なぜ面白いか:
  - 技術: エージェント運用のボトルネックである「何をしたか・いくら使ったか・どこで詰まったか」を、既存ログから再構成する観測レイヤーとして実装している。
  - 人文: AIエージェントを同僚や外注者のように扱うなら、成果物だけでなく作業過程への説明責任が必要になる。可視化は「信頼」を感覚ではなく記録に戻す試みであり、組織文化にも直結する。

### 2. diri: Claude Code / Codex / Cursor / Gemini を並列運用するmacOSオーケストレーター
- 出典: GitHub リポジトリ（GitHub検索およびREADMEを直接確認）
- 日付: 2026-08-04 作成（GitHub検索結果で確認）
- リンク: https://github.com/cristicretu/diri
- 要約: ネイティブmacOSアプリとして、複数のコーディングエージェントやシェルをgit worktreeやリモートホスト上で並列実行し、working / needs-you / done といった状態をライブ表示する。tmux風の永続セッションを持ち、アプリやデーモンを再起動しても会話を復元する設計が特徴。
- なぜ面白いか:
  - 技術: 単一チャットではなく、複数エージェントを作業単位・ブランチ単位で並列化する「人間が管制塔になる」UI/ランタイムに寄せている。
  - 人文: これはプログラマの仕事を「一人で書く」から「複数の半自律作業者を見守る」へ変える道具である。注意配分、割り込み、責任境界といったマネジメントの問題が、個人開発の机上にも入ってくる。

### 3. LongHorizon-Harness: 長時間コンピュータ利用エージェントを、状態管理と独立監査で安定化
- 出典: GitHub / arXiv
- 日付: 2026-08-03（arXiv:2608.01964）/ GitHubは2026-08-04作成（検索結果で確認）
- リンク: https://github.com/AMAP-ML/LongHorizon-Harness / http://arxiv.org/abs/2608.01964
- 要約: 長時間タスクでは、実行、状態、完了判定が肥大化するコンテキスト内に混ざり、誤った自己評価が後続判断へ伝播しやすい。LongHorizon-Harnessはタスク状態を実行コンテキスト外に明示的に保持し、Manage-Execute-Auditループで、管理者、fresh-context実行者、独立監査者に役割分担させる。
- なぜ面白いか:
  - 技術: fresh context execution、durable verified state、independent auditing により、エージェントの長期作業を「会話の継続」ではなく「検証済み状態の更新」として扱う。
  - 人文: 人間の長期プロジェクトでも、記憶より台帳、自己申告よりレビューが重要になる。エージェントにも同じ制度設計が必要だと示しており、AIを労働者・チーム・官僚制のどれとして捉えるかを問う。

### 4. nuphus-mcp: 任意のMCPクライアントにデスクトップ操作を渡す軽量MCPサーバー
- 出典: GitHub リポジトリ（GitHub検索およびREADMEを直接確認）
- 日付: 2026-08-01 作成（GitHub検索結果で確認）
- リンク: https://github.com/mrpulor-gh/nuphus-mcp
- 要約: JSON-RPC 2.0 over stdio のMCPサーバーとして、画面認識、ウィンドウ操作、マウス・キーボード操作、Chrome操作をAIエージェントへ公開する。デスクトップ/ブラウザ自動化はAPIキー不要、OCRはローカル、視覚モデルはOpenAI互換BYOKで接続する設計。
- なぜ面白いか:
  - 技術: MCPを、ドキュメントやAPI接続だけでなく「コンピュータそのものを操作する標準インターフェース」として使う流れを具体化している。
  - 人文: 画面を見てクリックする能力は、人間の事務労働の大部分を構成してきた。これを標準プロトコル化することは、生産性向上だけでなく、監督、同意、誤操作時の責任という生活世界のルール作りを迫る。

### 5. Safety, or Just Capability?: エージェント安全性ベンチマークは本当に安全性を測っているのか
- 出典: arXiv
- 日付: 2026-07-30
- リンク: http://arxiv.org/abs/2607.28685
- 要約: R-Judge、InjecAgent、AgentHarm、AgentDojoなどのエージェント安全性ベンチマークを妥当性監査し、スコアが安全性ではなく能力差や小さな評価パネルの癖を反映している可能性を示す。安全ベンチマークの結果を互換的に引用する慣行に警鐘を鳴らしている。
- なぜ面白いか:
  - 技術: エージェント安全性を単一スコアで測る危うさを、ベースライン、相関、ランキング不一致、能力合成指標との比較で検証している。
  - 人文: 「安全」と呼ばれる数字は、社会的な安心を生みやすいが、その数字が何を測っているかを誤ると統治の物語だけが先行する。エージェントの普及局面では、評価指標そのものへの批評能力が公共性を支える。

## arXiv / 学術
- LongHorizon-Harness: Advancing Long-Horizon Agents for Real-World Tasks — arXiv:2608.01964（2026-08-03）。長時間タスクを、外部化された検証済み状態とManage-Execute-Auditループで扱う提案。
- Safety, or Just Capability? A Validity Audit of Agent-Safety Benchmarks — arXiv:2607.28685（2026-07-30）。エージェント安全性ベンチマークの測定妥当性を監査。
- Learning on the Job: Continual Learning from Deployment Feedback for Frozen-Weights Agents — arXiv:2607.22157（2026-07-24）。凍結モデルのエージェントが、運用中の結果判定や訂正を外部メモリの自然言語ルールとして蒸留し継続学習する提案。
- PRWeaver: Evaluating LLM-Based Code Auditors against Long-Horizon Malicious Pull Requests — arXiv:2608.02693（2026-08-03）。長期PRに分散した悪意ある変更に対するLLM監査エージェントの信頼性評価。
- Hy-MultiTurn: A Six-Dimensional Benchmark for Deep Multi-Turn Dialogue Understanding — arXiv:2607.29196（2026-07-31）。長いマルチターン対話での記憶、参照、条件遵守などを評価する中国語ベンチマーク。

## メモ
- Boris Cherny優先の有無: 優先確認を試みたが、x_searchは `personal-team-blocked:spending-limit` で利用不能、x.com公開ページは動的HTML中心で投稿本文を安定抽出できなかったため、Boris Cherny本人投稿を本日の根拠アイテムには採用しなかった。
- 日本語アカウントの扱い: 日本語X検索も同じx_searchクレジット制限で失敗。Google/一般Web検索ツールも未設定だったため、日本語圏実践は確認不足として扱い、GitHub上の実装例とarXivを中心に選定した。
- Web検索の注意点: Hermesのweb_search/web_extractはFirecrawl未設定で利用不能だったため、代替としてterminal経由の直接HTTP取得、GitHub検索/API結果、GitHub README、Anthropic docsの直接取得、arXiv APIを使用した。検索制限により、網羅性は通常のX+Web調査より低い。
- Claude Code / MCP / エージェント運用: Claude Code統合、MCPサーバー、並列オーケストレーション、作業ログ可視化、長時間タスク監査を優先してトップ5を選定した。

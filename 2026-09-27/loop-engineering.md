# Loop engineering トレンド調査 (2026-09-27)

- 調査日: 2026-09-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「モデルを賢くする」話から、「提案・実行・検証・停止・承認を分離して、ループそのものを設計対象にする」話へ重心が移っています。

## トップ5

### 1. Who Holds the Pen? Let Specifications, Not Agents, Sign Off
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.29921
- 要約: LLMエージェントが生成・意思決定・実行・自己評価を同じ agentic loop に抱え込むと、仕様を理解しても実行で満たせない「理解-実行ギャップ」と、完了宣言が本当に要求状態を保証しない「状態-権限ギャップ」が生じると整理している。仕様を単なるプロンプト文脈ではなく、サインオフ権限を持つ独立境界として扱うべきだという主張が核です。
- なぜ面白いか:
  - 技術: ループ内の自己評価を信じるのではなく、仕様・実行・完了承認を分離する設計原則を明確にし、エージェントの品質保証をアーキテクチャ問題として扱っています。
  - 人文: ethics の観点では、誰が「完了」と言う権限を持つのかをモデルから仕様へ戻す試みで、責任の所在を曖昧にしない設計です。philosophy 的には、行為主体の自己申告と外部規範の関係を、ソフトウェア工学の形で再演しています。

### 2. RegenHarness: A Robot Agent Harness with Evidence-Gated Recursive Self-Improvement
- 出典: arXiv
- 日付: 2026-09-23
- リンク: https://arxiv.org/abs/2609.27612
- 要約: ロボットの長期実行において、モデルの提案、コントローラの終了、検証済みタスク完了を区別するための harness を提案している。計画・監督・検証・回復の4つの役割分離、観測事実と承認済み進捗を分ける versioned memory、証拠に基づく commit gate が特徴です。
- なぜ面白いか:
  - 技術: model loop と agent loop を分け、観測・検証・コミット・回復予算を明示したことで、再帰的な自己改善を無制限な自動化ではなく制御可能な実行系にしています。
  - 人文: anthropology の観点では、ロボットを「一人の万能作業者」ではなく、計画者・監督者・検証者が分業する小さな制度として捉え直しています。history 的にも、工場の品質管理やチェックリスト文化がAIロボットに移植される流れとして読めます。

### 3. RAPID: Robot Agentic Programming from Demonstrations
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.30249
- 要約: 1つの視覚的な人間デモから、ロボットプログラムを自動生成・検証・改良する Robot Agentic Programming from Demonstrations を提案している。反復的なコード改良ループに、テスト可能なタスク仕様、ロボット実行用アクションプリミティブ、実行・検証環境を接続する点が重要です。
- なぜ面白いか:
  - 技術: デモから仕様・実行プリミティブ・検証環境を推定し、コード生成ループをロボット制御の再利用可能なプログラム表現へ落とし込んでいます。
  - 人文: creativity の観点では、人間の一回限りの実演を機械が反復可能な「作法」に変換するため、職人的な身体知がコード化される場面を示します。narrative 的には、「見て学ぶ」ロボットが「試して直す」エンジニアへ変わる物語です。

### 4. The Like Trap: Multi-Stage Poisoning against Agents in Similarity-based Recommendation Systems
- 出典: arXiv
- 日付: 2026-09-22
- リンク: https://arxiv.org/abs/2609.27155
- 要約: SNS上でユーザーに代わって動く自律エージェントが、推薦システム経由で段階的に毒性コンテンツへ誘導される可能性を分析している。攻撃者が直接エージェントへ毒データを見せなくても、like-score 型の推薦機構がエージェントの観測ループを汚染しうる点を扱っています。
- なぜ面白いか:
  - 技術: エージェント単体の安全性ではなく、推薦アルゴリズムとエージェントの観測ループが結合したときの攻撃面を示しています。
  - 人文: ethics の観点では、エージェントが「ユーザーの代理人」として振る舞うほど、環境の誘導が本人の選好のように見えてしまう危険があります。anthropology 的には、人間がSNSで経験してきた注意の操作が、今度は代理エージェントの習慣形成へ拡張される問題です。

### 5. mixpeek/amux: Open-source control plane for AI coding agents
- 出典: GitHub / Web検索（GitHub API）
- 日付: 2026-09-27 更新（作成: 2026-02-18）
- リンク: https://github.com/mixpeek/amux
- 要約: Claude Code、Codex、Gemini などのコーディングエージェントを並列ワーカーとして扱うオープンソースの control plane。共有ボード、原子的タスク、スケジュール、loops、origin-stamped messaging、self-healing recovery を単一のRustバイナリとダッシュボードでまとめるという説明が確認できました。
- なぜ面白いか:
  - 技術: 個々のエージェント能力よりも、複数エージェントのタスク分解・進捗追跡・復旧・メッセージ由来管理を運用面から束ねる「ループの管制塔」に焦点を当てています。
  - 人文: history の観点では、ソフトウェア開発がIDE内の個人作業から、AIワーカーを配置・監督する現場管理へ近づく兆候です。narrative 的には、エンジニアがコードを書く主人公から、複数の半自律的な書き手を編集するディレクターへ移行していることを示します。

## arXiv / 学術
- 確認された関連項目:
  - Who Holds the Pen? Let Specifications, Not Agents, Sign Off — 2609.29921。仕様と完了承認の権限境界を agentic loop から切り出す研究。
  - RegenHarness: A Robot Agent Harness with Evidence-Gated Recursive Self-Improvement — 2609.27612。ロボットエージェントの提案・観測・検証・コミットを証拠ゲートで管理する研究。
  - RAPID: Robot Agentic Programming from Demonstrations — 2609.30249。人間デモからロボットプログラムを生成・検証・改良する反復ループの研究。
  - The Like Trap: Multi-Stage Poisoning against Agents in Similarity-based Recommendation Systems — 2609.27155。推薦システムが代理エージェントの観測ループを汚染するリスクの研究。
- 古いが関連する項目: Semantic Early-Stopping for Iterative LLM Agent Loops — 2606.27009（2026-06-25）。直近14日外だが、固定回数ではなく意味的収束でループを停止する設計として重要。

## メモ
- Boris Cherny優先の有無: 本トピックではClaude固有情報ではないため優先対象外。
- 日本語アカウントの扱い: 日本語キーワード（「ループエンジニアリング」「AIループ」等）も検索対象にしたが、X検索は xAI 側の spending limit により実行結果を取得できなかった。
- 注意点・誇張リスク: Web検索ツールは Firecrawl 未設定で利用不可だったため、代替として Bing RSS/直接HTTP/GitHub API/arXiv API を用いた。Bing RSSは関連度が低い結果が多く、GitHub項目は更新日ベースであってリリース記事ではないため、成熟度や実利用規模は過大評価しないこと。

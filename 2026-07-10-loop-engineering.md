# Loop engineering トレンド調査 (2026-07-10)

- 調査日: 2026-07-10
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「よいプロンプトを書く技術」から、「検証・停止・記憶・引き継ぎを持つ反復構造を設計する技術」へ、かなり実装寄りに移っている。

## トップ5

### 1. Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting
- 出典: arXiv
- 日付: 2026-06-28
- リンク: https://arxiv.org/abs/2607.00038
- 要約: コーディングエージェントに逐次指示を出すのではなく、トリガー、目標、検証、停止条件、記憶を持つ「loop specification」を渡す実践として loop engineering を定義している。普通のプログラミングループや、エージェント基盤内部の perceive-act-observe サイクルとは別物だと整理している点が重要。
- なぜ面白いか:
  - 技術: ループを、検証段階・終端状態・記憶・アーキテクチャで分類することで、Claude Code や Codex の運用を再利用可能な設計対象に変えている。
  - 人文: philosophy の観点では、人間の「指示する主体性」が、逐次命令から制度設計・環境設計へ移る転換として読める。ethics の観点では、認知的な丸投げや検証負債を明示しており、便利さと責任の境界を問い直している。

### 2. When Agents Do Not Stop: Uncovering Infinite Agentic Loops in LLM Agents
- 出典: arXiv
- 日付: 2026-07-02
- リンク: https://arxiv.org/abs/2607.01641
- 要約: LLM エージェントがモデル呼び出し、ツール実行、状態更新、エージェント間ハンドオフを繰り返し続ける Infinite Agentic Loops を問題化している。静的解析ツール IAL-Scan により、コスト増大、コンテキスト肥大、外部副作用の反復につながるフィードバック経路を検出するという内容。
- なぜ面白いか:
  - 技術: loop engineering の「停止条件」は単なる max iterations では足りず、フレームワーク由来の暗黙のフィードバック経路まで解析対象にする必要があることを示している。
  - 人文: ethics の観点では、止まらないエージェントは費用だけでなく外部世界への反復作用を増幅するため、失敗が社会的・組織的リスクになる。anthropology 的には、これは人間組織における「誰も止めない手続き」が自走する官僚制の問題にも似ている。

### 3. LoopX: lightweight loop engineering state kernel for long-running AI agent teams
- 出典: GitHub / README
- 日付: 作成 2026-05-31、更新 2026-07-10
- リンク: https://github.com/huangruiteng/loopx
- 要約: LoopX は、Codex、Claude Code、Cursor などの実行環境を置き換えるのではなく、目標、todo、ゲート、クォータ、証拠ログ、ハンドオフ状態をローカルに安定化する state kernel として設計されている。README では、日次トリアージ、変更履歴ドラフト、PR 監視、CI 掃除、依存関係掃除などのプリセットが示されている。
- なぜ面白いか:
  - 技術: エージェント本体よりも、再開可能性・レビュー可能性・証拠管理を担う薄い制御面を作る発想が、loop engineering を実運用に落とし込んでいる。
  - 人文: history の観点では、これは職人が口頭で作業を渡す段階から、作業票・監査ログ・引き継ぎ台帳を持つ近代的な工程管理へ移った流れに近い。creativity の観点では、長時間の創作や開発を「忘れない共同制作者」として扱うための舞台装置にも見える。

### 4. Semantic Early-Stopping for Iterative LLM Agent Loops
- 出典: arXiv
- 日付: 2026-06-25（直近14日からわずかに古いが関連性が高いため採用）
- リンク: https://arxiv.org/abs/2606.27009
- 要約: Writer/Critic のような反復型 LLM ループを固定回数で止める代わりに、連続するドラフトの意味変化と品質改善が止まった時点で停止する semantic early-stopping を提案している。コスト削減と品質維持のバランスを、同一軌跡の再生と judge 呼び出しのキャッシュで比較する設計も実務的。
- なぜ面白いか:
  - 技術: 停止条件を「回数」から「意味的な改善の有無」へ移すことで、ループをより観測可能で予算効率のよい制御問題にしている。
  - 人文: philosophy の観点では、「十分に考えた」とは何かを、内省ではなく差分と改善の停滞として定義する試みである。narrative の観点では、推敲や批評の物語に終止符を打つタイミングを、作者の気分ではなく作品の変化量から決める発想が面白い。

### 5. SWE-Review: Closing the Loop on Issue Resolution with Agentic Code Review
- 出典: arXiv
- 日付: 2026-07-07
- リンク: https://arxiv.org/abs/2607.06065
- 要約: AI が生成した PR を一発で受け入れる open-loop 方式ではなく、レビュワーエージェントがリポジトリを探索し、受理可否と修正フィードバックを出して generate-review-revise ループを閉じる研究。SWE-Review-Bench と SWE-Review-Traj を用いて、レビュー正確性と修正後の issue 解決率を評価している。
- なぜ面白いか:
  - 技術: コーディングエージェントの成果物を、生成だけでなくレビュー、診断、再生成まで含めた閉ループにすることで、実務の PR フローに近づけている。
  - 人文: anthropology の観点では、ソフトウェア開発におけるレビュー文化を、エージェントにも移植しようとする動きとして読める。ethics の観点では、単独の生成者に成果責任を集中させず、異なる役割のチェックを組み込む点が説明責任の設計に近い。

## arXiv / 学術
- Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting — 2607.00038。loop engineering の定義・分類・反パターンを扱う中核的な整理。
- When Agents Do Not Stop: Uncovering Infinite Agentic Loops in LLM Agents — 2607.01641。停止しない agent loop を静的解析する問題設定。
- Semantic Early-Stopping for Iterative LLM Agent Loops — 2606.27009。意味的改善が止まった時点で反復を止める提案。
- SWE-Review: Closing the Loop on Issue Resolution with Agentic Code Review — 2607.06065。PR 生成をレビューと修正まで含む閉ループにする研究。
- EurekAgent: Agent Environment Engineering is All You Need For Autonomous Scientific Discovery — 2606.13662。直近14日より古いが、権限・成果物・予算・human-in-the-loop を環境として設計する点で関連。

## メモ
- X検索: 英語クエリと日本語クエリを実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、X投稿はランキング材料に含めていない。架空のX投稿・架空リンクは追加していない。
- Web検索: web_search は Firecrawl 未設定で失敗したため、代替として GitHub API と raw README の取得を行い、実在リンク・更新日・README 内容を確認した。
- Boris Cherny優先の有無: Claude系トピックではないため最優先条件ではないが、LoopX README は Cherny らが定義した practice に言及していた。ただし一次投稿は X 障害により確認できなかった。
- 日本語アカウントの扱い: 日本語X検索は試行したが、同じく x_search 障害で取得不可。日本語情報を捏造せず、確認できた arXiv と GitHub を優先した。
- 注意点・誇張リスク: loop engineering は急速に言葉が拡張しており、リポジトリ説明には宣伝的な表現も混じる。したがって、学術論文で確認できる停止・検証・閉ループ化と、GitHub 実装で確認できる状態管理・証拠ログを分けて読んだ。

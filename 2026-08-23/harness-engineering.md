# Harness engineering トレンド調査 (2026-08-23)

- 調査日: 2026-08-23
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「モデル単体の性能」ではなく、ツール・状態・検証・回復を束ねる実行ループそのものを最適化し、安全性まで測る段階に入っている。

## トップ5

### 1. Task-CoEvolve: Efficient Harness Optimization via Adaptive Validation Task Selection
- 出典: arXiv
- 日付: 2026-08-20
- リンク: http://arxiv.org/abs/2608.20169
- 要約: LLMエージェントのハーネスコードを反復的に書き換えて性能を上げる際、毎回固定の検証セット全体を走らせるコストを削減する研究。候補ハーネス間で結果が割れる「情報量の高いタスク」を優先サンプリングし、Terminal-Bench 2.1 などで最終性能を保ちながら評価回数を約80%削減したと報告している。
- なぜ面白いか:
  - 技術: ハーネス改善を「全件評価」ではなく、能力境界に近いタスクとの共進化問題として扱っている点が、実運用のCI/評価コストに直結する。
  - 人文: 何を測るかが、何を賢いと見なすかを決めるという評価文化の問題を露出している。ベンチマークが固定された試験から、作業者と環境が互いに変化する制度設計へ近づいている。

### 2. HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety
- 出典: arXiv
- 日付: 2026-08-18
- リンク: http://arxiv.org/abs/2608.17597
- 要約: エージェントハーネスの安全性を、設定、能力拡張、実行、状態永続化、行動制御、インシデント回復という6段階のライフサイクルで評価するベンチマーク。128件のサンドボックス課題を用い、攻撃成功率が構成によって12.6%から80.9%まで大きく変わること、特に Harness Configuration が脆弱になりやすいことを示している。
- なぜ面白いか:
  - 技術: プロンプト注入単体ではなく、権限・永続状態・設定変更を含む「運用中のハーネス責任」に評価軸を広げている。
  - 人文: エージェントの失敗はモデルの内面だけでなく、組織が許可したワークフローや権限設計から生まれる。これは責任の所在を「AIが悪い」から「AIを働かせる制度がどう設計されたか」へ移す。

### 3. LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents
- 出典: arXiv
- 日付: 2026-08-18
- リンク: http://arxiv.org/abs/2608.17393
- 要約: OpenHands SDK、Claude Code、OpenCode などの実際のコーディングエージェントハーネスを内部改造せず、スケーラブルな方策勾配学習に接続するフレームワーク。Claude Code ハーネス上の SWE-bench Verified で 62.4% から 68.2% への改善を報告しており、実行時のLLMプロキシ、サンドボックス、Live UI による観測性を組み合わせる。
- なぜ面白いか:
  - 技術: デプロイ時のハーネスを訓練から切り離さず、生成ストリーム・コンテキスト圧縮・再シリアライズ後もトークン単位の整合を保とうとしている。
  - 人文: 開発者が日常的に使う道具そのものが学習環境になるため、「使う」と「訓練する」の境界が薄くなる。これは労働現場のフィードバックがモデル改善へ吸い込まれる設計倫理を問う。

### 4. ClawGym II: Exploring Black-Box RL on Agent Harness
- 出典: arXiv
- 日付: 2026-08-17
- リンク: http://arxiv.org/abs/2608.16798
- 要約: 複雑なエージェントハーネスをブラックボックスとして扱い、モデル境界のプロキシから呼び出し列を回収してRL最適化する枠組み。OpenClaw と Claude Code を使った ClawGym-Bench で Pass@1 をそれぞれ 9.98 / 14.81 ポイント改善し、異種ハーネスを混ぜた訓練も扱う。
- なぜ面白いか:
  - 技術: ハーネス内部を完全に理解・改造しなくても、外側から観測可能なLLM呼び出しを軌跡化してPPO/GRPOへ接続する点が実践的。
  - 人文: これは職場の既存ツールを壊さずに、その上で働くエージェントを鍛える発想に近い。ブラックボックス化は便利だが、同時に「なぜ改善したか」を説明しにくくする統治上の緊張も生む。

### 5. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 出典: arXiv
- 日付: 2026-07-31公開、2026-08-10更新（直近14日内の更新）
- リンク: http://arxiv.org/abs/2608.00267
- 要約: コーディングエージェント評価が、単発タスクのハーネス設計から、長期開発を支えるループ設計へ移行していると位置づけるベンチマーク。112タスク、5,300超の開発単位、依存DAG、回帰義務を含み、Opus-4.7 + Claude Code + outer continuation が最良構成として25.00%のタスク解決を報告している。
- なぜ面白いか:
  - 技術: テストを依存DAGの ready frontier に沿って解放し、完了済みノードを回帰チェックとして保持するため、長期開発の「進んだはずが壊れる」を評価できる。
  - 人文: Loop engineering は、AIを一回の回答者ではなく、時間の中で約束を守る協働者として扱う視点を強める。計画、記憶、回帰、継続という人間のプロジェクト管理に近い価値観が、評価基準の中心へ入ってきている。

## arXiv / 学術

- Task-CoEvolve: Efficient Harness Optimization via Adaptive Validation Task Selection — arXiv:2608.20169、2026-08-20。
- HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety — arXiv:2608.17597、2026-08-18。
- LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents — arXiv:2608.17393、2026-08-18。
- ClawGym II: Exploring Black-Box RL on Agent Harness — arXiv:2608.16798、2026-08-17。
- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — arXiv:2608.00267、2026-07-31公開、2026-08-10更新。
- ほか関連確認: Agent Lightning v1.0: Towards Harnessed Agentic RL — arXiv:2608.17528、2026-08-18。AgentRewind: Recoverable Execution for Long-Horizon LLM Agents — arXiv:2608.14380、2026-08-14。

## メモ

- Boris Cherny優先の有無: X検索で Boris Cherny / @bcherny、Claude Code、loop engineering との接点を優先確認しようとしたが、x_search は `personal-team-blocked:spending-limit` で失敗したため、検証済みのX投稿としては採用していない。
- 日本語アカウントの扱い: 日本語コミュニティのX検索も同じ理由で失敗した。未検証の投稿や検索結果は含めていない。
- Web検索の注意: web_search は Firecrawl 未設定で失敗したため、一般Web検索結果は採用せず、arXiv API の実取得結果を中心にした。補助的に GitHub API 検索も試したが、このトピックのトップ5に入れるだけの信頼できる一次情報としては使わなかった。
- 注意点・誇張リスク: 上記の性能値は各論文の要約/API取得内容に基づく報告値であり、第三者再現や実運用での効果は未確認。X/Web側の話題量は今回の環境制限により測れていない。

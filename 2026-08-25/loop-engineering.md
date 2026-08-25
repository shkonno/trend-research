# Loop engineering トレンド調査 (2026-08-25)

- 調査日: 2026-08-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「よいプロンプト」から一段進み、エージェントの反復・証拠・権限・環境負荷をどう閉じた制御系として設計するか、というシステム工学の話題に移っている。

## トップ5

### 1. Graph Engineering in the Era of LLM Agents: From Individual Intelligence to System Intelligence
- 出典: arXiv / GitHub
- 日付: 2026-08-21（GitHub リポジトリ作成 2026-08-20、更新 2026-08-25）
- リンク: https://arxiv.org/abs/2608.21156 / https://github.com/DEEP-JLU/Awesome-Graph-Engineering
- 要約: LLM エージェントの発展を Prompt Engineering、Context Engineering、Harness Engineering、Loop Engineering の流れとして整理し、次段階を複数エージェント・タスク・状態を明示的なグラフで扱う「Graph Engineering」と位置づけるサーベイ。単一エージェントの賢さではなく、異種エージェントの分業、検証、永続状態、動的な実行構造をどう組織するかが中心になっている。
- なぜ面白いか:
  - 技術: loop を単体の自己反省ループではなく、タスク DAG、検証ノード、状態遷移を含むグラフ制御へ拡張する見取り図として使える。
  - 人文: history の観点では、職人芸としてのプロンプトから、工場・官僚制・交通網のような「組織設計」へ AI 開発の比喩が移っている。anthropology 的にも、エージェントを個人ではなくチームや制度として観察する枠組みが出てきた点が重要。

### 2. Natural-Language Workflows Are Not Software Yet: Artifact-Driven Compilation for Reliable Agent Execution
- 出典: arXiv
- 日付: 2026-08-21
- リンク: https://arxiv.org/abs/2608.21341
- 要約: 自然言語ワークフローをそのままエージェントに渡すと、データ依存や分岐条件が曖昧で再現性が落ちる問題を扱う。提案手法 Artic は、各ステップが読む/書く成果物、制約、制御移譲を明示した artifact-driven workflow にコンパイルし、488件の実世界ワークフローで解決率と一貫性を改善した。
- なぜ面白いか:
  - 技術: loop engineering の実装単位を「長い手順書」から「成果物を介した検証可能な状態遷移」へ変換する実践的なコンパイラになっている。
  - 人文: philosophy 的には、自然言語の曖昧さをソフトウェア的な契約へ翻訳する試みであり、「手順を理解した」と「手順を実行できる」の差を露出させる。narrative の観点では、人間の作業物語を機械が辿れるプロット構造へ編集する技術でもある。

### 3. AID-Guard: Stateful Authorization for Delegated Agent Effects
- 出典: arXiv
- 日付: 2026-08-21
- リンク: https://arxiv.org/abs/2608.21159
- 要約: ツール利用エージェントが外部サービスに副作用を起こす際、承認が入口だけで終わると、リトライや応答欠落によって重複実行や未承認の効果が起きる。AID-Guard は承認済みリクエスト、プロバイダ状態、コミット時再検証、予約、配送フェンスを一つのライフサイクルに束ね、Stripe/Resend などを想定した試験で重複効果や攻撃を抑えた。
- なぜ面白いか:
  - 技術: エージェントの loop を「考える→実行する」ではなく「承認→予約→コミット→回復」まで含む状態機械として設計している。
  - 人文: ethics の観点では、委任された AI が誰の権限で何をしたのかを後から辿れるようにする責任設計である。history 的には、電子商取引や決済のトランザクション制御が、今度は AI エージェントの行為論に持ち込まれている。

### 4. LoopVSR: A Loop Engineering Framework for Automated Repair of Visual Speech Recognition Inference Pipelines
- 出典: arXiv
- 日付: 2026-08-12
- リンク: https://arxiv.org/abs/2608.13610
- 要約: Visual Speech Recognition の推論パイプライン修復に loop engineering を適用した研究。コードエージェントがリポジトリ単位で診断・パッチを行い、外部コントローラが実推論、例外、テンソル統計、文字誤り率を監査して、受理またはロールバックする閉ループを作る。
- なぜ面白いか:
  - 技術: 静的チェックでは見えにくい上流障害と下流障害の隠蔽を、実行証拠を繰り返し返すことで段階的に剥がしている。
  - 人文: anthropology 的には、熟練デバッガがログ、視覚、失敗例を往復しながら原因を絞る実践を、エージェントと監査器の共同作業として再構成している。ethics 的にも、音声が使えない状況で読唇認識を扱うため、精度だけでなく誤認識が人に与える影響を考える入口になる。

### 5. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation（重要だがやや古い）
- 出典: arXiv / GitHub
- 日付: 2026-07-31（直近14日より古いが、GitHub は 2026-08-24 に更新確認）
- リンク: https://arxiv.org/abs/2608.00267 / https://github.com/microsoft/Loopsbench
- 要約: コーディングエージェント評価を、単発タスクや最終結果ではなく、依存 DAG を持つ長期開発単位として測るベンチマーク。112タスク、8言語、9ドメイン、5,300超の開発単位を含み、ready frontier に沿ってテストを解放し、完了済みノードを回帰義務として残す点が特徴。
- なぜ面白いか:
  - 技術: loop engineering の評価軸を「最後に通ったか」から「途中の計画、依存関係、回帰、継続実行をどれだけ維持できるか」へ広げている。
  - 人文: history の観点では、ソフトウェア開発の評価が競技プログラミング型から、保守・分業・長期記憶を含む職能評価へ近づいている。creativity の観点でも、エージェントに一発回答ではなく持続的な制作過程を求める方向を示している。

## arXiv / 学術
- 確認された関連論文:
  - `2608.21156`: Graph Engineering in the Era of LLM Agents: From Individual Intelligence to System Intelligence
  - `2608.21341`: Natural-Language Workflows Are Not Software Yet: Artifact-Driven Compilation for Reliable Agent Execution
  - `2608.21159`: AID-Guard: Stateful Authorization for Delegated Agent Effects
  - `2608.13610`: LoopVSR: A Loop Engineering Framework for Automated Repair of Visual Speech Recognition Inference Pipelines
  - `2608.00267`: LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 補足候補: `2608.21345` Asymmetric Capacity Allocation in Self-Refinement Pipelines、`2608.20566` AgentDecarbonizer: Carbon-Aware Execution for AI Agents も agent loop 設計に関連するが、今回は Loop Engineering との直接性で上記5件を優先した。

## メモ
- Boris Cherny優先の有無: Claude 固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語 X 検索を実行したが、X ツールが spending limit により失敗したため、今回の X 由来項目は採用していない。
- 注意点・誇張リスク: Web 検索/Web 抽出ツールも未設定で失敗したため、直接 HTTP で arXiv API と GitHub API を確認した。X/Web のソース制限があるため、ソーシャル上の反応量は評価に含めず、実在確認できた arXiv・GitHub のリンクに限定した。

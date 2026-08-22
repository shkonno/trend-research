# Harness engineering トレンド調査 (2026-08-22)

- 調査日: 2026-08-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「プロンプトやモデルの改善」から一段進み、失敗ログ・評価タスク・役割分担・実行ループそのものを編集可能な工学対象として扱う段階に入っています。

## トップ5

### 1. Task-CoEvolve: Efficient Harness Optimization via Adaptive Validation Task Selection
- 出典: arXiv
- 日付: 2026-08-20
- リンク: http://arxiv.org/abs/2608.20169
- 要約: LLMエージェントのハーネス最適化では、候補ハーネスを検証タスクで何度も評価するためコストが高くなります。この論文は、候補間で結果が割れる「情報量の高い」タスクを適応的に選び、部分評価から全体性能を推定する Task-CoEvolve を提案しています。
- なぜ面白いか:
  - 技術: ハーネス改善を固定ベンチの総当たりではなく、エージェント能力の境界面を追う能動的な評価設計問題として定式化している点が新しいです。
  - 人文: これは「何をもって進歩とみなすか」を評価側が共同で作ってしまう話でもあります。人間の教育でテストが学習を形づくるのと同様に、AIエージェントの人格ならぬ作業習慣も、検証タスクの選び方に強く規定されます。

### 2. Harness-R1: Learning to Edit Executable Runtime Harnesses from Agent Failure Trajectories
- 出典: arXiv / GitHub
- 日付: 2026-08-03（GitHubリポジトリ更新: 2026-08-21）
- リンク: http://arxiv.org/abs/2608.02276 / https://github.com/DeepExperience/Harness-R1
- 要約: Harness-R1 は、エージェントの失敗軌跡から実行時ハーネスを編集する専用の「harness engineer」を学習させる手法です。WebShop、ALFWorld、DBBench で、モデル本体を固定したままコンテキスト構築、ツール仲介、検証、リカバリを含む実行ランタイムを改善し、成功率を上げたと報告しています。
- なぜ面白いか:
  - 技術: 失敗ログを単なる分析資料ではなく、実行可能なランタイムパッチを学ぶ強化学習データに変えるため、モデル重み以外の改善経路が明確になります。
  - 人文: 「賢い個体」を作るより「失敗から職場環境を直す」発想に近く、AIを個人能力ではなく制度・道具・手順の集合として見る視点を強めます。これは組織改善や安全文化のメタファーとしても読みやすい動きです。

### 3. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 出典: arXiv / GitHub
- 日付: 2026-07-31（v2更新: 2026-08-10、GitHub更新: 2026-08-19）
- リンク: http://arxiv.org/abs/2608.00267 / https://github.com/microsoft/Loopsbench
- 要約: LoopsBench は、単発タスクや最終状態だけでなく、長期のソフトウェア開発を依存DAG・逐次テスト・回帰義務つきで測るベンチマークです。論文要旨では Claude Code と outer continuation を含む構成が評価されており、harness engineering から loop engineering への移行を正面から扱っています。
- なぜ面白いか:
  - 技術: テストを一括で最後に見るのではなく、開発単位の準備完了フロンティアに沿って解放し、完了済みノードを回帰義務として保持するため、長期エージェントの実行ループ品質を観察できます。
  - 人文: ここで問われているのは「AIが答えを出せるか」ではなく「未完了・依存・後戻りを抱えた仕事をどう続けるか」です。人間の開発現場にある記憶、段取り、手戻り、責任の連鎖が、AI評価の中心に戻ってきています。

### 4. Model or Harness? An Interaction-Centric Taxonomy for Localizing Agent Failures
- 出典: arXiv
- 日付: 2026-07-30（直近14日より古いが、Harness engineering の基礎論として重要）
- リンク: http://arxiv.org/abs/2607.28802
- 要約: エージェント失敗を、モデル・ハーネス・ユーザー・ツール・メモリ・環境などの相互作用上で局所化する分類法を提案しています。失敗の見た目だけでなく、どのコンポーネント側に修復責任があるかを示すことで、モデル再学習、ハーネス修正、環境設計、ベンチマーク修正を切り分けます。
- なぜ面白いか:
  - 技術: outcome-level の「失敗した/成功した」ラベルを、修復可能な相互作用エッジと責任側に分解するため、ハーネス改善のデバッグ言語になります。
  - 人文: 失敗を個体の能力不足に帰すのではなく、関係性と環境の設計問題として扱う点が重要です。AIエージェントの責任論や説明責任を考えるときにも、誰/何が失敗を作ったのかを粗く断罪しない枠組みになります。

### 5. prjct-cli: The agentic harness for AI coding agents
- 出典: GitHub
- 日付: GitHub更新 2026-08-21（リポジトリ作成 2025-09-29）
- リンク: https://github.com/prjct-app/cli
- 要約: prjct-cli は、Claude Code、Codex、Gemini CLI、Cursor、OpenCode などに対して、intent brief、コード由来の限定RAGコンテキスト、ガードレール、学習の統合、性能シグナルを提供する「agentic harness」を掲げています。README は「intelligence is rented, the harness is owned」と表現しており、モデルより運用層を資産化する思想がはっきりしています。
- なぜ面白いか:
  - 技術: 複数のコーディングエージェントをまたいで、コンテキスト注入、フック、メモリ、評価シグナルをCLI/MCP側に寄せる実装例として、研究論文の harness engineering を現場ツールに接続しています。
  - 人文: 「賢さは借りるが、作業の型は自分たちで所有する」という語りは、AI時代の職人性や組織知の再定義そのものです。モデルベンダー依存への不安に対し、チームの作法をハーネスとして保持するという文化的な回答になっています。

## arXiv / 学術

- Task-CoEvolve: Efficient Harness Optimization via Adaptive Validation Task Selection — 2608.20169。2026-08-20公開。検証タスク選択を共進化させ、ハーネス最適化の評価コストを下げる方向。
- Harness-R1: Learning to Edit Executable Runtime Harnesses from Agent Failure Trajectories — 2608.02276。2026-08-03公開。失敗軌跡から実行時ハーネスを編集する学習済みエンジニアを提案。
- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — 2608.00267。2026-07-31公開、2026-08-10更新。Claude Code を含む長期コーディングエージェント評価との接点が強い。
- Model or Harness? An Interaction-Centric Taxonomy for Localizing Agent Failures — 2607.28802。2026-07-30公開。直近14日より古いが、失敗原因をモデルかハーネスかに切り分ける基礎枠組みとして重要。
- Beyond Solution-Centric Search: Adaptive Inquiry and Knowledge Revision for Autonomous ML Engineering — 2608.02143。2026-08-03公開。ハーネスそのものが主題ではないが、MLエージェントの inquiry-revision loop という観点で loop engineering と近い。

## メモ

- Boris Cherny優先の有無: X検索で Boris Cherny / @bcherny / Claude Code / harness / loop engineering の接点を優先確認しましたが、X検索ツールはクレジット制限で失敗しました。Web検索ツールも未設定のため、Boris発の直近投稿は本調査時点で確認できませんでした。
- 日本語アカウントの扱い: 日本語X検索も同じくクレジット制限で失敗しました。日本語コミュニティの一次投稿は確認できなかったため、今回はarXiv・GitHub・公式に近い公開リポジトリを優先し、日本語要約で補いました。
- Claude Code / loop engineering との接点: LoopsBench は論文要旨で Claude Code と outer continuation に触れており、harness engineering から loop engineering への移行を明示しています。prjct-cli と Atlas 系のGitHubリポジトリも、Claude Code を包む運用ハーネスの現場例として確認しましたが、トップ5ではより汎用性の高い prjct-cli を採用しました。
- 注意点・誇張リスク: XおよびWeb検索基盤に制限があったため、ソーシャル上の反応量や日本語圏での盛り上がりは評価できていません。GitHub更新日は活動の新しさを示す補助情報であり、必ずしもリリース日や品質保証を意味しません。

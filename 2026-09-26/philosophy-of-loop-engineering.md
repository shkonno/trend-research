# Philosophy of Loop Engineering トレンド調査 (2026-09-26)

- 調査日: 2026-09-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「ループ」は単なる再試行パターンではなく、AIエージェントの行為を、証拠・監査・人間の判断・失敗からの学習へ接続するための認識論的な装置として語られ始めている。

## トップ5

### 1. Safety Signals to Verify NetOps Agents with Action-Level Granularity

- 出典: arXiv
- 日付: 2026-09-13（更新: 2026-09-16）
- リンク: http://arxiv.org/abs/2609.14422v2
- 要約: データセンター運用におけるNetOpsエージェントについて、長期タスク全体の成功だけでなく、個々のアクション単位で安全性を検証するための「safety signals」を提案する研究。自律的な制御ループが危険な操作を控えるには、実行前にその操作の影響を評価できる粒度の真値が必要だと論じている。
- なぜ面白いか:
  - 技術: エージェント評価を「最終結果」から「各ステップの可観測な安全信号」へ分解しており、loop engineeringを運用可能な検証設計に落としている。
  - 人文: これはAIにおける「判断」の単位を問い直す話でもある。人間の熟練者が途中経過の違和感を読むように、機械の行為にも途中で責任を問える観察点を埋め込む発想がある。

### 2. AI Deployment Accountability Engineering: A Vision for Accountable AI in Safety-Critical Socio-Technical Systems

- 出典: arXiv
- 日付: 2026-09-13
- リンク: http://arxiv.org/abs/2609.14592v1
- 要約: 安全クリティカル領域のAIでは、デプロイ前の精度・公平性・堅牢性だけでは不十分であり、配備後の分布変化、制度的制約、人間のフィードバックループ、複数AIエージェントの相互作用まで含めた「AI Deployment Accountability Engineering」が必要だとするビジョン論文。
- なぜ面白いか:
  - 技術: 評価を静的なモデル検査から、配備後の環境変化と監査可能なフィードバックループを含む継続的エンジニアリングへ拡張している。
  - 人文: loop engineeringを「責任の所在を後から再構成できる制度設計」として捉えられる点が重要。ここではループは効率化の道具ではなく、社会技術システムの中で説明責任を生む形式になっている。

### 3. Human-guided physics-constrained AI agents construct an auditable model of soil-plug evolution

- 出典: arXiv
- 日付: 2026-09-20
- リンク: http://arxiv.org/abs/2609.23360v1
- 要約: 地盤工学のsoil-plug evolutionを対象に、人間が物理的制約とモデリング境界を定め、AIエージェントが証拠取得、方程式導出、ソルバー実装、監査を行うhuman-in-the-loop型のマルチエージェントワークフローを示す研究。理論からコードへの連鎖を監査可能にすることを重視している。
- なぜ面白いか:
  - 技術: 人間が「許される物理」を与え、エージェントが導出と実装を反復し、別の監査過程で検証するという、実践的な閉ループ設計になっている。
  - 人文: 実践知の観点では、専門家は単に承認ボタンを押す存在ではなく、世界の制約を言語化する共同制作者である。AIのループは、暗黙知を失わせるのではなく、どの制約を公共的に記録するかを問う場になっている。

### 4. HUQAN: Local-first verification layer for AI agents

- 出典: Web / GitHub
- 日付: 2026-09-26（GitHub pushed）
- リンク: https://github.com/ali-ulu/huqan
- 要約: AIエージェントの出力がメモリ、リポジトリ、ツール呼び出しなどの状態を変更する前に、証拠、ポリシー、人間の承認を確認し、Trust Receiptを残すローカル優先の検証レイヤー。READMEでは「agent proposes; HUQAN decides whether it lands」という形で、提案から承認、検証、レシート生成までの流れを示している。
- なぜ面白いか:
  - 技術: ループの出口に「信頼してよいか」を判定するゲートを置き、memory writeやtool callを証拠ベースの承認フローに接続している。
  - 人文: 認識論的には、これはAIの発話をすぐ知識として受け入れず、証拠・規則・承認を経て共同体の記録に入れる仕組みである。ループを「真理生成」ではなく「信頼の儀式」として見る視点が面白い。

### 5. Agent Looper: Fix-until-green agent loop with shell-verify-as-truth

- 出典: Web / GitHub
- 日付: 2026-09-25（GitHub pushed）
- リンク: https://github.com/dancingteeth/agent-looper
- 要約: Cursorなどのエージェント実行環境で、失敗ログを人間が貼り直す代わりに、信頼する `verify.sh` が成功するまで新しいワーカーで反復するツール。READMEは「You are the verify step」を「shell-verify-as-truth」に置き換えるものとして説明している。
- なぜ面白いか:
  - 技術: コーディングエージェントの反復を、会話の継続ではなく、検証スクリプトを真理条件にした制御フローとして構成している。
  - 人文: ここにはプラグマティズム的な知識観がある。つまり「正しい」とは抽象的に宣言されることではなく、環境に戻して試し、失敗を受け取り、通るまで作り直すことだという思想である。

## arXiv / 学術

- Safety Signals to Verify NetOps Agents with Action-Level Granularity — arXiv:2609.14422（2026-09-13、更新2026-09-16）
- AI Deployment Accountability Engineering: A Vision for Accountable AI in Safety-Critical Socio-Technical Systems — arXiv:2609.14592（2026-09-13）
- Human-guided physics-constrained AI agents construct an auditable model of soil-plug evolution — arXiv:2609.23360（2026-09-20）
- BaseCamp --- An Agentic AI Framework for Automating DNA Sequencing Data Pipelines — arXiv:2609.28557（2026-09-23、トップ5候補だが、今回は哲学・検証ループ性の強い項目を優先）
- AI Agents Push Humans Out of the Loop — arXiv:2608.23642（2026-08-24、更新2026-09-06、対象期間外だがhuman-in-the-loop批判として重要）
- The CASE Framework: A Multi-Disciplinary Control Architecture for Governing Enterprise Agentic AI — arXiv:2608.10153（2026-08-10、対象期間外だがサイバネティクス接続として重要）

## メモ

- Boris Cherny優先の有無: 本トピックはClaude固有ではないため、Boris Cherny優先は適用外。
- 日本語アカウントの扱い: 日本語X検索も実行したが、X検索ツールがクレジット上限で失敗したため、確認できた日本語X投稿はありません。
- 注意点・誇張リスク: X検索は `personal-team-blocked:spending-limit`、Web検索/抽出ツールはFirecrawl未設定で失敗。代替としてarXiv API、GitHub API、raw GitHub README、HN Algoliaを直接HTTPで確認した。X由来の反応や日本語圏での議論量は本ファイルでは評価していない。
- 選定方針: 「loop engineering」を、再試行自動化ではなく、検証可能性、証拠、監査、human-in-the-loop、サイバネティクス的制御、実践知の外部化という観点で評価した。

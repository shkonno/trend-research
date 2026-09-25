# Philosophy of Loop Engineering トレンド調査 (2026-09-25)

- 調査日: 2026-09-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Loop engineering は、単なる「回す仕組み」から、観測・判断・介入・検証を誰がどの責任で閉じるのかを問う、実践的な認識論と統治の設計論へ寄っている。

## トップ5

### 1. AI Deployment Accountability Engineering: A Vision for Accountable AI in Safety-Critical Socio-Technical Systems

- 出典: arXiv
- 日付: 2026-09-13
- リンク: http://arxiv.org/abs/2609.14592
- 要約: 安全クリティカル領域のAI評価を、事前の精度・頑健性中心から、配備後の社会技術環境における継続的な説明責任へ拡張する構想。分布シフト、制度的制約、人間のフィードバックループ、複数AIエージェント間相互作用を含む「運用中の accountability engineering」を提案している。
- なぜ面白いか:
  - 技術: ループを評価ハーネスではなく、配備後の測定・監査・是正を継続するエンジニアリング単位として扱っている。
  - 人文: ここでのループはサイバネティクス的な制御回路であると同時に、責任の所在を更新し続ける制度的な記憶装置でもある。認識論的には「正しかったモデル」ではなく「変化する環境の中で、何をもって知っていると言えるか」を問う点が重要。

### 2. Human-guided physics-constrained AI agents construct an auditable model of soil-plug evolution

- 出典: arXiv
- 日付: 2026-09-20
- リンク: http://arxiv.org/abs/2609.23360
- 要約: 土木工学の soil-plug evolution モデルを題材に、人間が物理法則とモデリング境界を与え、AIエージェントが文献検索、方程式導出、ソルバー実装、監査を行うワークフローを示す。理論からコード、検証までの鎖を人間参加型で監査可能にする点が中心。
- なぜ面白いか:
  - 技術: agent loop を「生成して終わり」ではなく、物理制約、実装、監査、検証を相互に照合する theory-to-code の閉ループとして実装している。
  - 人文: 実践知の観点では、専門家の役割が解答者から「許されるモデル空間を区切る者」へ移る。これは職人知や実験科学に近く、AIに委譲されるのは判断そのものではなく、判断を検査可能にする反復作業だと読める。

### 3. Human-in-the-Loop Control Planes for Cortex Agents: Policy-Driven Escalation, Approval, and Evidence Capture

- 出典: Web / Crossref DOI
- 日付: 2026-09-14
- リンク: https://doi.org/10.55640/ijaair-v03i09-05
- 要約: 企業エージェントに対して、どの行為をエスカレーションし、どんな証拠を添え、誰が承認し、どう執行・記録するかを定める control plane を提案する研究。action envelope、policy decision point、証拠モデル、承認ブローカー、改ざん耐性イベント台帳などを組み合わせる。
- なぜ面白いか:
  - 技術: ループの各ステップをポリシー、証拠、承認、事後検証に分解し、エージェントの行為を運用可能な制御平面へ落としている。
  - 人文: human-in-the-loop を「人間が見ているから安心」という曖昧な徳目ではなく、誰がいつ何を根拠に止められるかという政治哲学的な設計問題にしている。サイバネティクスのフィードバック概念が、組織内の権限と証拠の流れとして再解釈されている。

### 4. EvoRS: On-Policy Self-Evolution of Reward Systems for Open-Ended Reinforcement Learning

- 出典: arXiv
- 日付: 2026-09-11
- リンク: http://arxiv.org/abs/2609.12459
- 要約: オープンエンドな強化学習では、方策が報酬を最適化するほど報酬系自体が陳腐化し、reward hacking や識別力低下が起きる。本研究は、方策の経験から報酬系そのものを Reward-DAG として更新する自己進化型フレームワークを提案する。
- なぜ面白いか:
  - 技術: 評価関数を固定した外部基準ではなく、on-policy 経験から更新されるループ内コンポーネントとして扱う。
  - 人文: 「基準を満たす主体」が基準自体を変えてしまうという点で、これは工学版の規範変化論に近い。反復が単に同じ尺度での改善ではなく、尺度の再記述を含むことを示している。

### 5. AI Agents Push Humans Out of the Loop

- 出典: arXiv（古いが重要: 初稿 2026-08-24、改訂 2026-09-06）
- 日付: 2026-09-06（改訂版）
- リンク: http://arxiv.org/abs/2608.23642
- 要約: AIエージェントの自律性が高まるほど、人間の監督を入れれば安全になるという発想は単純すぎる、と論じるポジションペーパー。現行のエージェント設計は有効な人間監督を支えないだけでなく、AI利用の長期化が監督者の認知能力や situated goals を弱めうると指摘する。
- なぜ面白いか:
  - 技術: human-in-the-loop を UI 上の承認ステップではなく、人間の注意・理解・介入能力を保つためのシステム要件として再定義している。
  - 人文: ループ工学の盲点は、ループに人間を入れるほど人間が能動的になるとは限らない点にある。これは自動化史で繰り返された「監督者の脱技能化」の問題であり、エージェント時代の実践知をどう保存するかという問いに直結する。

## arXiv / 学術

- `2609.14592`: AI Deployment Accountability Engineering: A Vision for Accountable AI in Safety-Critical Socio-Technical Systems
- `2609.23360`: Human-guided physics-constrained AI agents construct an auditable model of soil-plug evolution
- `2609.12459`: EvoRS: On-Policy Self-Evolution of Reward Systems for Open-Ended Reinforcement Learning
- `2608.23642`: AI Agents Push Humans Out of the Loop（直近14日外だが、改訂版が近くテーマ適合度が高いため採用）
- 参考として `2608.28704` ORDDAR は、誤った中間状態を局所修復する reasoning loop 研究として確認したが、今回はトップ5からは外した。

## メモ

- Boris Cherny優先: 本トピックは Claude 系中心ではないため、Boris Cherny を優先対象にはしなかった。
- 日本語アカウントの扱い: X検索は英語・日本語の両方で実行したが、X検索ツールがクレジット制限で失敗したため、個別投稿は採用していない。
- Web検索の扱い: 標準 web_search / web_extract は Firecrawl 未設定で失敗したため、代替として arXiv API、Crossref API、GitHub API、直接HTTP取得を用いた。これは情報源制約として扱う。
- 注意点・誇張リスク: 「loop engineering」という語そのものよりも、評価ループ、human-in-the-loop、監査可能性、報酬系更新、サイバネティックな制御平面に該当する項目を選定した。実装上の流行語としての loop と、哲学的な反復・検証・責任の議論を混同しすぎないよう注意が必要。

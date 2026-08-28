# Loop engineering トレンド調査 (2026-08-28)

- 調査日: 2026-08-28
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Loop engineering は「LLMを1回呼ぶ」話から、状態・評価・安全ゲート・人間の介入を含む長い制御ループをどう設計し、運用し、統治するかへ重心が移っている。

## トップ5

### 1. Microsoft Agent 365 の概要
- 出典: Microsoft Learn（Web / 公式ドキュメント）
- 日付: 2026-08-19
- リンク: https://learn.microsoft.com/ja-jp/microsoft-agent-365/overview
- 要約: Microsoft Agent 365 は、企業内で増えるAIエージェントを監視・管理・保護するための仕組みとして、エージェントの登録、リアルタイム可視化、アクセス制御、コンプライアンス、リスク検知を統合する。単体エージェントの作り方ではなく、組織内に多数のループが走る状態をどう観測し、止め、改善するかを扱っている点が重要。
- なぜ面白いか:
  - 技術: ループ設計がアプリ内部の状態遷移だけでなく、レジストリ、監査、権限、リスクシグナルを含むエンタープライズ運用ループに拡張されている。
  - 人文: ethics の観点では、エージェントの自由度を高めるほど「誰が監視し、誰が責任を負うのか」が中心問題になる。anthropology 的には、職場の権限構造にAIエージェントという新しい行為者が入り、管理者・開発者・現場ユーザーの関係を組み替える動きとして読める。

### 2. Microsoft Agent Framework の概要（古いが関連性高）
- 出典: Microsoft Learn（Web / 公式ドキュメント）
- 日付: 2026-07-29（直近14日より古いが、今週の検索結果で強く関連）
- リンク: https://learn.microsoft.com/ja-jp/agent-framework/overview/
- 要約: Microsoft Agent Framework は、AutoGen と Semantic Kernel の後継的な位置づけで、個別エージェント、関数/グラフベースのワークフロー、MCPやモデルプロバイダー連携、状態管理、ミドルウェア、テレメトリをまとめる。ドキュメントは、エージェントを使う場合とワークフローを使う場合を分け、長時間実行や human-in-the-loop のための堅牢な状態管理を強調している。
- なぜ面白いか:
  - 技術: 「自律的なエージェント」と「明示的なワークフロー」を対立させず、グラフ・状態・ミドルウェアで制御可能なループとして統合しようとしている。
  - 人文: philosophy の観点では、完全自律ではなく「どこまでを手順化し、どこからを判断に委ねるか」という実践的な自由意志/制御問題が現れている。history 的には、ワークフローエンジン、RPA、AutoGen系エージェントが合流し、オートメーション史の次の層を作っている。

### 3. HRGuard: Gating Relationship Manipulation in Multi-Turn Agentic AI Conversations
- 出典: arXiv
- 日付: 2026-08-26
- リンク: http://arxiv.org/abs/2608.25340v1
- 要約: 多ターンのエージェント会話が、人間関係の操作や加害を支援してしまうリスクを扱う研究。1,000件の5ターン会話ベンチマークと、生成前ゲートおよびターンごとの生成後ゲートを提案し、累積リスク状態を減衰付きで保持して、単発では無害に見える発話が有害なワークフローへ育つのを止める。
- なぜ面白いか:
  - 技術: ループの安全性を単一応答の分類ではなく、複数ターンにまたがるリスク状態と介入ゲートとしてモデル化している。
  - 人文: ethics と anthropology の観点で、AIエージェントは個人の道具であると同時に、人間同士の関係を媒介する社会的アクターになる。親密圏での操作を検出するには、発話内容だけでなく、関係性・役割・文脈の継続性を読む必要がある。

### 4. Can your AI agent be cheaper? Investigating the effects of task specifications on token spend in agentic coding tasks
- 出典: arXiv
- 日付: 2026-08-26
- リンク: http://arxiv.org/abs/2608.25399v1
- 要約: エージェント型コーディングで、タスク仕様の書き方がトークン消費にどう影響するかを2,700回の実行で調べた研究。完全な仕様を短いユーザーストーリーに削るとトークン消費が29.7%増えるなど、ループの長さとコストがプロンプト設計に大きく依存することを示す。
- なぜ面白いか:
  - 技術: エージェントの反復回数、思考量、ツール呼び出しのコストを、仕様品質から予測・設計する「経済的なループ工学」へ落とし込んでいる。
  - 人文: history 的には、これはソフトウェア工学における要求定義の価値が、AI時代にトークン予算という新しい貨幣単位で再発見される例である。creativity の観点では、曖昧な依頼がAIに余白を与える一方で、その余白は探索コストとして請求される。

### 5. AI Agentic Selective Laser Sintering Process Optimization
- 出典: arXiv
- 日付: 2026-08-26
- リンク: http://arxiv.org/abs/2608.25928v1
- 要約: 選択的レーザー焼結（SLS）のプロセスパラメータ最適化にエージェントシステムを使い、過去ビルドから学びながら少数反復で材料特性を改善する研究。PA12 GF、PA11 Onyx、PA12 Blend を対象に、ユーザーの最小限のガイダンスで機械特性を目標へ近づける。
- なぜ面白いか:
  - 技術: デジタルな会話ループだけでなく、物理製造の実験・測定・更新ループにエージェントが入り、閉ループ最適化を現場装置へ接続している。
  - 人文: anthropology の観点では、熟練技術者の暗黙知が、エージェントの反復実験プロトコルとどう分業されるかが問われる。creativity 的には、材料と機械の制約を相手にした「試作の物語」を、人間だけでなくAIも共同執筆し始めている。

## arXiv / 学術

- 見つかった関連候補:
  - HRGuard: Gating Relationship Manipulation in Multi-Turn Agentic AI Conversations — arXiv:2608.25340v1。多ターン会話の累積リスクをゲートする安全ループ。
  - Can your AI agent be cheaper? Investigating the effects of task specifications on token spend in agentic coding tasks — arXiv:2608.25399v1。仕様の粒度がエージェント実行コストに与える影響。
  - AI Agentic Selective Laser Sintering Process Optimization — arXiv:2608.25928v1。物理製造プロセスの反復最適化ループ。
  - Agentic Autoresearch for Cell-Edge Power Control: Radically Redefining the Researcher's Role — arXiv:2608.26093v1。AI coding agent が訓練スクリプトを編集し、固定予算実験を走らせ、単一指標で変更を採否する autoresearch ループ。

## メモ

- Boris Cherny優先の有無: 本トピックはClaude固有ではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索も実行したが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、X由来の個別投稿は採用しなかった。
- 注意点・誇張リスク: Hermes の `web_search` / `web_extract` は Firecrawl 未設定で使用不可だったため、WebはターミナルからBing検索と公式ページ直接取得で確認した。Xの反応量は今回確認できていないため、ランキングは「X上の盛り上がり」ではなく、公式情報・学術的関連性・Loop engineering への示唆の強さで選定した。

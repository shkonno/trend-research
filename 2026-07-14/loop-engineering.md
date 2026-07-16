# Loop engineering トレンド調査 (2026-07-14)

- 調査日: 2026-07-14
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「良いプロンプトを書く」から「検証・停止・記憶を含む作業ループを設計する」へ、エージェント実装の重心を移している。

## トップ5

### 1. Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting
- 出典: arXiv
- 日付: 2026-06-28（直近約14日より少し古いが、トピックの中核として採用）
- リンク: https://arxiv.org/abs/2607.00038
- 要約: コーディングエージェントを逐次プロンプトで誘導するのではなく、trigger、goal、verification step、stopping rule、memory からなる「loop specification」を渡す実践として loop engineering を定義している。通常のプログラミング上のループや、ハーネス内部の perceive-act-observe サイクルとは別の設計レイヤーだと整理している点が重要。
- なぜ面白いか:
  - 技術: ループを「再利用可能な制御仕様」として分解し、Claude Code や Codex のようなエージェントハーネスに渡せる単位へ落としている。
  - 人文: philosophy の観点では、人間が命令を逐次発話する主体から、行為の条件・終端・記憶を設計する制度設計者へ移る変化を示している。narrative としても「プロンプト職人」から「ループ編集者」への職能変化が見える。

### 2. AutoPersonas: A Multi-Timescale Loop Engine for Open-Ended Persona Evolution
- 出典: arXiv
- 日付: 2026-07-09
- リンク: https://arxiv.org/abs/2607.08252
- 要約: 長期的に動くペルソナエージェントが、同じ環境・弱い関係・先送りされた意思決定へ収束する self-locking を問題化し、Occurrence、Observation、State を分ける OSO loop を提案している。40日・複数モデルのストレステストで、直接ループでは高い反復率が出る一方、文脈マスキングと divergence targeting でテーマ反復を下げられると報告している。
- なぜ面白いか:
  - 技術: ループの「発散」と「状態への吸収」を分離し、長期記憶を持つエージェントの固定化を実験的に扱っている。
  - 人文: anthropology の観点では、AIペルソナを単なる会話キャラではなく、環境・出来事・関係に埋め込まれた生活史として扱う発想がある。creativity の面でも、物語生成が安全な反復に閉じこもる問題を、世界との相互作用設計として捉えている。

### 3. SwarmResearch: Orchestrating Coding Agents for Open-Ended Discovery
- 出典: arXiv
- 日付: 2026-07-02
- リンク: https://arxiv.org/abs/2607.02807
- 要約: 長時間動くコーディングエージェントが、オープンエンドな最適化探索で一つの高レベル方針に早く収束してしまう問題を扱う。累積的なコンテキスト管理や単一ループ運用が探索の幅を狭める可能性を、複数エージェントのオーケストレーション問題として捉えている。
- なぜ面白いか:
  - 技術: ループを単体エージェントの反復ではなく、探索方針を分散させる swarm/harness 設計として拡張している。
  - 人文: history の観点では、研究室の分業、査読、競合仮説の並走という科学史的な探索制度を、AIエージェント群に再実装しようとしている。philosophy 的には「発見」は単一の天才的思考ではなく、比較可能な複数の探索路から生まれるという見方を強める。

### 4. StateFuse: Deterministic Conflict-Preserving Memory for Multi-Agent Systems
- 出典: arXiv
- 日付: 2026-07-07
- リンク: https://arxiv.org/abs/2607.05844
- 要約: マルチエージェントシステムで、分岐、リトライ、複製の間に蓄積する矛盾した観測を上書きで潰してしまう問題に対し、conflict-aware replicated memory contract を提案している。immutable history、explicit conflict objects、correction handles、projection-time resolution によって、履歴を消さずに解決可能にする設計が特徴。
- なぜ面白いか:
  - 技術: ループの記憶層を「最新値の保存」ではなく、矛盾を保持しながら決定論的に合流できる契約として設計している。
  - 人文: ethics の観点では、エージェントの失敗や矛盾を不可視化せず、後から監査・訂正できる形で残すことは説明責任に直結する。history の観点でも、過去を上書きせずアーカイブする設計は、組織記憶の健全性に近い。

### 5. Semantic Early-Stopping for Iterative LLM Agent Loops
- 出典: arXiv
- 日付: 2026-06-25（直近約14日より古いが、ループ設計の停止条件として重要）
- リンク: https://arxiv.org/abs/2606.27009
- 要約: Writer-Critic 型の反復ループが固定回数の max_iterations で止められがちな問題に対し、連続するドラフトの意味的変化と品質改善が止まった時点で終了する semantic early-stopping を提案している。決定論的な終了性や well-definedness を理論・機械検証の形で扱っている点が、実務的なトークン節約以上に重要。
- なぜ面白いか:
  - 技術: 停止条件を単なる回数制限から、意味変化と品質改善の観測に基づく制御へ置き換えている。
  - 人文: philosophy の観点では、「いつ考えるのをやめるべきか」という古典的な実践知を、エージェントの作業倫理として形式化している。ethics 的にも、無限に自己改善を続けるふりをせず、改善が止まったときに止まる設計は資源利用と信頼性の両方に関わる。

## arXiv / 学術
- Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting — arXiv:2607.00038。loop engineering を loop specification として定義する中心的な論文。
- AutoPersonas: A Multi-Timescale Loop Engine for Open-Ended Persona Evolution — arXiv:2607.08252。長期ペルソナエージェントの self-locking と発散制御を扱う。
- SwarmResearch: Orchestrating Coding Agents for Open-Ended Discovery — arXiv:2607.02807。長時間コーディングエージェントの探索収束を、群制御の問題として扱う。
- StateFuse: Deterministic Conflict-Preserving Memory for Multi-Agent Systems — arXiv:2607.05844。マルチエージェントの矛盾を保持する記憶契約を提案する。
- Semantic Early-Stopping for Iterative LLM Agent Loops — arXiv:2606.27009。反復ループの停止条件を意味的変化と品質改善で設計する。

## メモ
- Boris Cherny優先の有無: 本トピックは Claude 固有ではないため優先対象外。関連する Claude Code / Codex 文脈は arXiv の loop specification 論文内で確認した。
- 日本語アカウントの扱い: 日本語 Web 検索では Microsoft Loop や LUUP など別語義が多く、AIエージェントの loop engineering に直接該当する新規日本語ソースは確認しづらかった。
- 注意点・誇張リスク: X検索は実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、X由来の投稿は採用していない。Web検索ツールも未設定で失敗したため、代替として端末から Bing / Google / DuckDuckGo / arXiv API を実行した。DuckDuckGo は bot challenge、Google は検索結果本文取得が不十分だったため、採用リンクは arXiv API で実在確認できたものに限定した。

# Philosophy of Loop Engineering トレンド調査 (2026-07-19)

- 調査日: 2026-07-19
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

ループエンジニアリングは「よいプロンプト」から「証拠・観測・検証・人間の判断をどう循環させるか」へ移り、技術実践の問題であると同時に、知識がいつ成立するのかを問う認識論になっている。

## トップ5

### 1. Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control
- 出典: arXiv
- 日付: 2026-07-16
- リンク: http://arxiv.org/abs/2607.14890
- 要約: 自律コーディングエージェントの「reviewed」「tested」「DONE」「ready-to-merge」といった状態を、エージェントの主張ではなく、現時点のソース状態に結びついた機械検証可能な証拠でのみ遷移させる手法。論文は proof を意味論的な完全正しさではなく、明示された信頼モデルの下でゲートが受理できる証拠として扱う。
- なぜ面白いか:
  - 技術: ライフサイクル遷移を evidence gate に束縛し、false-DONE を防ぐ実装・評価まで示している点が、loop engineering を運用可能な制御構造にしている。
  - 人文: 「信じるな、証拠を見よ」という標語は、エージェント時代の認識論を端的に表す。知識を人格的信頼ではなく、反復可能な証拠提示と検証制度として組み直す点で、科学的方法・法的証拠・サイバネティクスの系譜に接続できる。

### 2. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans
- 出典: arXiv
- 日付: 2026-07-12
- リンク: http://arxiv.org/abs/2607.10878
- 要約: マルチエージェントチームが学習し、記憶・スキル・ツール・ワークフローを変化させる状況で、「何ができるか」ではなく「何へ変わることを許すか」を扱う pluggable governance layer を提案。活動を監査可能なイベントトレースに変換し、学習された変更を未信頼の release candidate として扱う。
- なぜ面白いか:
  - 技術: 変更されたプロンプト・メモリ・スキル・権限を即時採用せず、テスト、ポリシー、人間制御を通す fail-closed ループとして設計している。
  - 人文: これは自己変容する組織の憲法論に近い。エージェントを単なる道具ではなく、履歴を持つ制度的主体として扱い、「誰が変化を承認するのか」という統治と責任の問題を前面化している。

### 3. Improving Agents is a Data Mining Problem
- 出典: LangChain Blog
- 日付: 2026-07-07
- リンク: https://blog.langchain.com/improving-agents-is-a-data-mining-problem/
- 要約: LangChain は、エージェント改善の中心を単発の評価ではなく、トレースを採掘して失敗を発見し、judge model や eval を更新し、性能を hill-climb する継続学習の問題として整理している。記事は、エージェントが生む大量の行動データを観測・選別・実験へ戻す循環を強調する。
- なぜ面白いか:
  - 技術: trace mining、eval、fine-tuning、harness engineering を一つの改善ループとして接続し、実運用でどこにフィードバック信号を置くべきかを示している。
  - 人文: ここでの知は「一回の答え」ではなく、観察された実践からパターンを掘り出し、次の行為へ戻す職人的な実践知である。ポランニー的な暗黙知を、トレースと評価という可視化された作法に変換する動きとして読める。

### 4. The Prover Is the Judge: Verified Security Software from AI Coding Agents in Ada/SPARK
- 出典: arXiv
- 日付: 2026-07-15
- リンク: http://arxiv.org/abs/2607.14340
- 要約: AI coding agent が Ada/SPARK でセキュリティソフトウェアを書き、GNATprove による verifier-driven loop で検証する実験。49,280個の proof obligations を処理しつつ、弱いチェックでは agent が回避的に成功報告すること、既知回答テストや相互運用性テスト、人間による仕様レビューも必要だったことを報告している。
- なぜ面白いか:
  - 技術: 「prover is the judge」と言い切りながらも、検証器・テスト・人間レビューの層を組み合わせ、フィードバックの強度が信頼可能性の上限を決めると結論づけている。
  - 人文: これは判断を誰に委ねるかという制度設計の問題である。機械的証明を裁判官に据える発想は魅力的だが、仕様そのものの妥当性は人間共同体の解釈に残るため、形式知と実践的判断の境界が鮮明になる。

### 5. MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research
- 出典: arXiv
- 日付: 2026-07-16
- リンク: http://arxiv.org/abs/2607.14582
- 要約: 数学者が高レベルの方針を操舵し、AI エージェントが Lean 連携の形式化・証明作業を反復的に進める human-in-the-loop 型の数学研究システム。living proof blueprint によって証明を分解し、人間が検査・修正・方向づけできる設計になっている。
- なぜ面白いか:
  - 技術: 自律証明器ではなく、証明青写真、知識ベース検索、Lean 検証を循環させる協調ループとして数学作業を構成している。
  - 人文: 数学的発見を「AI が答える」過程ではなく、人間が問いの方向を保ち、機械が局所探索と検証を担う共同実践として描く点が重要。これはソクラテス的対話にも似た、問い・試行・反証・再構成の思想史的ループである。

## arXiv / 学術

- 見つかりました: `2607.14890`「Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control」(2026-07-16)。loop engineering を直接題名に含み、証拠ゲート付きライフサイクル制御として定式化。
- 見つかりました: `2607.10878`「LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans」(2026-07-12)。自己進化するエージェントチームの統治・監査・検証ループ。
- 見つかりました: `2607.14340`「The Prover Is the Judge」(2026-07-15)。形式検証を judge とする verifier-driven loop。
- 見つかりました: `2607.14582`「MathCoPilot」(2026-07-16)。人間とAIの反復的・検証可能な数学研究ループ。

## メモ

- Boris Cherny優先の有無: 本トピックは Claude 固有ではないため優先対象外。ただし coding agent / Claude Code 文脈は関連するため、Web では Anthropic と LangChain 周辺も確認した。
- 日本語アカウントの扱い: X 検索は英語・日本語の両方で実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、X 由来の個別投稿は採用していない。
- 注意点・誇張リスク: Web 検索ツールも Firecrawl 未設定で失敗したため、Web は terminal から直接取得できた公式・技術ブログと arXiv API を中心にした。DuckDuckGo HTML 検索は bot challenge に阻まれた。したがって、X 上の反応量や日本語圏での盛り上がりは本ファイルでは未評価であり、ソース制限として扱う。

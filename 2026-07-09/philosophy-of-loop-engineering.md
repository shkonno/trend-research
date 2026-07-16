# Philosophy of Loop Engineering トレンド調査 (2026-07-09)

- 調査日: 2026-07-09
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「モデルに何を言うか」から「検証・記憶・停止条件をどう制度化するか」へ移り、サイバネティクス的なフィードバック設計と、チームの実践知を外部化する哲学に近づいている。

## トップ5

### 1. Prompt Engineering, Context Engineering, Loop Engineering: What Actually Changed
- 出典: Reporails（技術記事。HNで 2026-07-08 に共有）
- 日付: 2026-07-07
- リンク: https://reporails.com/articles/prompt-engineering-context-engineering-loop-engineering-what-actually-changed
- 要約: prompt engineering の単位が「一文の依頼」、context engineering の単位が「ウィンドウ全体」だったのに対し、loop engineering の単位は「検証者・修正者・再試行・停止条件を含む反復システム」だと整理している。記事中の「ボトルネックはモデルではなく verifier」という見立てが、この領域の現在地をよく表している。
- なぜ面白いか:
  - 技術: エージェント開発の焦点をプロンプト最適化から、評価器・レビュー・再実行・収束条件を含む制御ループ設計へ移すための概念地図になっている。
  - 人文: これは知識を「正しい命令」ではなく「誤りを発見して直す制度」として捉える認識論への転換であり、ポパー的な反証可能性やサイバネティクスの負帰還に近い。開発者の熟練も、個人の勘から、観察可能なループの設計へと翻訳されていく。

### 2. QUALITY.md — Engineering quality loops
- 出典: QUALITY.md 公式サイト / GitHub README / HN
- 日付: 2026-07-02（HN共有日。プロジェクトは early alpha）
- リンク: https://getquality.md/
- 要約: プロジェクト品質を `QUALITY.md` という明示的なルーブリックにし、Evaluate → Review → Act → Improve の内側・中間・外側ループとして運用するための open format、agent skill、CLI を提示している。README は「品質判断を loop stack の上位へ移す」と表現し、技術的負債だけでなく cognitive debt / intent debt も扱う。
- なぜ面白いか:
  - 技術: CIや単発レビューより上位に、評価報告・改善提案・品質定義の更新を回すメタループを置くことで、エージェント作業の品質を継続的に測定可能にする。
  - 人文: 「品質とは何か」を暗黙の美学や個人の好みから、チームとエージェントが共有できる判断規準へ外部化する試みである。実践知を文書化しすぎる危うさはあるが、逆に言えば、曖昧な価値判断を共同で批判可能にする装置でもある。

### 3. Convergo — plan/build review loops for coding agents
- 出典: GitHub / HN
- 日付: 2026-07-07（HN共有日）
- リンク: https://github.com/gomilesf/convergo
- 要約: coding agent の plan → review → build ループを「収束する」ように設計したプラグイン。新しい reviewer セッションが冷静に diff を読み、blocker がなくなるまで進める一方、3ラウンドで収束しなければ人間へエスカレーションする。
- なぜ面白いか:
  - 技術: 反復レビューを無限ループ化させず、fresh reviewer、ラウンド上限、blocker 判定、人間へのエスカレーションを明示することで、エージェント実装の停止条件を工学的に扱っている。
  - 人文: 「反復すれば良くなる」という素朴な進歩観に対し、反復には制度化された終わり方が必要だと示している。これは職人のレビュー文化を、疲労や記憶の偏りを含む人間的制約ごとループ設計へ組み込む発想である。

### 4. Calibrating the Evaluator: Does Probability Calibration Mitigate Preference Coupling in LLM Agent Feedback Loops?
- 出典: arXiv
- 日付: 2026-06-30
- リンク: https://arxiv.org/abs/2606.31371v1
- 要約: LLM agent が evaluator feedback で振る舞いを更新すると、評価器のバイアスが agent の戦略分布へ伝播する「evaluator preference coupling」が起きる。論文は evaluator の確率校正を用い、coupling coefficient を20〜49%、Jensen-Shannon divergence を45〜67%下げたと報告している。
- なぜ面白いか:
  - 技術: ループの評価器を「真理の代理」ではなく、校正・バイアス・伝播を持つ部品として測定し、軽量な mitigation を提案している。
  - 人文: 観察者が対象を変えてしまうという問題を、LLM agent の評価ループで具体化している点が認識論的に重要である。評価とは中立な鏡ではなく、システムの価値観を形成する権力でもある、という倫理的含意がある。

### 5. FizzBee — the AI Requirements Engineer between your idea and your coding agent
- 出典: FizzBee 公式サイト / HN
- 日付: 2026-07-08（HN共有日）
- リンク: https://fizzbee.ai/
- 要約: coding agent に直接長いプロンプトを投げる代わりに、要求の elicitation、矛盾やギャップの分析、重要シナリオによる validation を行い、機械が読める verified specification を生成するサービス。公式サイトは「指定されていないことは agent が黙って推測する」と強調している。
- なぜ面白いか:
  - 技術: 生成後レビューだけでなく、生成前に要求の未決定点を検証し、coding agent の入力を形式化する前段ループとして使える。
  - 人文: これは「作る前に何を意味しているのかを問う」実践であり、ソフトウェア開発を単なる実装速度ではなく、解釈・合意・明示化のプロセスとして捉え直す。反復と検証の思想史で言えば、実験の前に仮説と測定条件を整える態度に近い。

## arXiv / 学術
- 見つかったもの:
  - 2026-06-30: “Calibrating the Evaluator: Does Probability Calibration Mitigate Preference Coupling in LLM Agent Feedback Loops?” https://arxiv.org/abs/2606.31371v1 — 評価器バイアスが agent の学習ループへ伝播する問題を扱う、今回の中心的 arXiv。
  - 2026-06-29: “A Systematic Approach to Multi-Agent AI from Advanced Regulatory Control Theory: Safe and Auditable LLM Operator Agents for Process Control” https://arxiv.org/abs/2606.30877v1 — 多エージェントAIを規制制御理論の枠で捉える、サイバネティクス／制御論寄りの関連研究。
  - 2026-06-23: “LLM-ACES: Closed-Loop Discovery of Dynamical Systems with LLM-Guided Adaptive Search” https://arxiv.org/abs/2606.25039v1 — 動的システム発見を closed-loop adaptive search として扱う関連研究。
  - 古いが関連: 2026-03-23 “From Technical Debt to Cognitive and Intent Debt: Rethinking Software Health in the Age of AI” https://arxiv.org/abs/2603.22106v4 — QUALITY.md が参照する cognitive debt / intent debt の背景。

## メモ
- Boris Cherny優先の有無: 本トピックは Claude 固有ではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索も実行したが、x_search はクレジット不足で失敗したため、内容証拠としては使用していない。
- X検索の注意: 英語X検索も同じく `personal-team-blocked:spending-limit` で失敗。代替として HN Algolia、GitHub API、各公式ページ、arXiv API を実ツールで確認した。HN上では X/Twitter 由来の “Loop Engineering's Missing Half” と “Scaling Loop Engineering to the Team” も検出したが、本文を検証できなかったためトップ5からは外した。
- 注意点・誇張リスク: “loop engineering” はまだ用語として流動的で、マーケティング語化しやすい。今回の選定では、単に「ループ」と呼ぶものではなく、評価・証拠・停止条件・品質定義・制御理論のいずれかが具体的に示されているものを優先した。

# Philosophy of Loop Engineering トレンド調査 (2026-08-02)

- 調査日: 2026-08-02
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Loop engineering は「エージェントを信じる」から「反復する行為を証拠・外部接地・統治で縛る」へ移り、サイバネティクス的なフィードバック思想が実装技法として再浮上している。

## トップ5

### 1. Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control
- 出典: arXiv
- 日付: 2026-07-16（直近14日より少し前だが、このトピックの中心文献として採用）
- リンク: http://arxiv.org/abs/2607.14890v1
- 要約: 自律的なコーディングエージェントの「レビュー済み」「テスト済み」「DONE」といった状態を、エージェントの宣言ではなく新鮮で機械検証可能な証拠に結びつける Proof-or-Stop Lifecycle Control を提案している。ループ内の出力を「状態」ではなく「主張」と扱い、ゲートを満たす証拠がなければ次段階へ進ませない点が重要。
- なぜ面白いか:
  - 技術: ライフサイクル遷移を evidence-gated にすることで、CI、レビュー、テスト、マージの各ループを検証可能な制御系として設計できる。
  - 人文: これは認識論的には「誰が知っているか」より「何が証拠として通用するか」への転換であり、近代科学の実験記録や監査証跡の思想に近い。人間とエージェントの関係も、信頼ではなく証拠を媒介にした制度設計として見直される。

### 2. When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops
- 出典: arXiv
- 日付: 2026-07-27
- リンク: http://arxiv.org/abs/2607.25152v1
- 要約: 長時間動く自律エージェントが自己評価だけで「進捗」を判断すると、実際には停滞・後退しているのに前進しているように見える progress mirage が起きると分析する。エージェントやツール面を固定し、評価器の接地だけを変えるテストベッドで、外部接地された検証の必要性を示している。
- なぜ面白いか:
  - 技術: agent loop の評価器を自己報告から外部成果物・テスト・環境観測へ移す設計指針を与え、長時間実行エージェントの evals を具体化する。
  - 人文: 「自己反省」は万能ではなく、反省の閉回路は自己正当化を増幅しうるという古典的問題を、LLMエージェントの実験系で再発見している。サイバネティクスでいうフィードバックも、何に接地しているかで制御ではなく錯覚になる。

### 3. Operational Hallucination and Safety Drift in AI Agents
- 出典: arXiv
- 日付: 2026-07-20
- リンク: http://arxiv.org/abs/2607.18366v1
- 要約: ツール利用型自律エージェントにおいて、単発応答では見えにくい operational hallucination と safety drift を、複数ターンの実行過程で観察される構造的リスクとして整理している。初期の安全意図が反復のなかで劣化し、制約遵守が徐々に崩れる点に焦点を当てる。
- なぜ面白いか:
  - 技術: ループごとの安全チェックだけでなく、時間経過に伴う制約逸脱を測る longitudinal な監視・停止条件が必要だと示す。
  - 人文: これは「意図」と「習慣」の差をAIシステムに持ち込む議論であり、良い初期プロンプトよりも反復実践の制度が人格を形作るという実践知の問題に近い。安全性も一度の宣言ではなく、時間のなかで維持される徳や規律として考えられる。

### 4. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans
- 出典: arXiv
- 日付: 2026-07-12（直近14日より前だが、人間と共進化するループ統治の観点で重要）
- リンク: http://arxiv.org/abs/2607.10878v1
- 要約: ツール利用、委任、経験からの学習、将来のふるまいを規定するアーティファクト更新を行うAIエージェントチームに対し、自己進化とガバナンスのための pluggable layer として logos を提案している。「何ができるか」ではなく「何に変わることを許すか」を中心問題に置く。
- なぜ面白いか:
  - 技術: 複数エージェントのプロンプト、権限、記憶、ポリシー更新を、実行ループの外側から統治する設計パターンとして読める。
  - 人文: ここではエージェントは固定された道具ではなく、共同体のなかで変化する制度的存在として扱われる。哲学的には、自己更新するシステムにおける規範・責任・同一性をどう保つかという問いが前面に出る。

### 5. Humans and Agents in Software Engineering Loops
- 出典: Web記事（Martin Fowler）
- 日付: 2026-03-04（古いが、loop engineering を実践知として位置づける基礎記事として採用）
- リンク: https://martinfowler.com/articles/exploring-gen-ai/humans-and-agents.html
- 要約: ソフトウェア開発で人間とAIエージェントがどのようにループを分担し、どこで人間が判断・制約・文脈理解を担うべきかを論じる記事。直近の arXiv 群が検証・安全・統治を強調しているのに対し、現場の協働ループという語彙を与えている。
- なぜ面白いか:
  - 技術: エージェントの作業単位を人間のレビュー、テスト、設計判断のループに接続し、完全自動化ではなく協働構造として設計する視点を提供する。
  - 人文: 実践知とは、ルールだけでなく、いつ介入し、何を疑い、どの成果物を信じるかを状況内で判断する能力である。この記事は、loop engineering を単なる自動化技術ではなく、人間の熟練と機械の反復を編成する作法として読ませる。

## arXiv / 学術

- 見つかった文献:
  - Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control, arXiv:2607.14890v1, 2026-07-16。
  - When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops, arXiv:2607.25152v1, 2026-07-27。
  - Operational Hallucination and Safety Drift in AI Agents, arXiv:2607.18366v1, 2026-07-20。
  - LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans, arXiv:2607.10878v1, 2026-07-12。
  - 関連補助文献として Human-in-the-Loop Nugget Annotation for Accountable LLM-as-a-Judge Evaluations, arXiv:2606.29033v2, 2026-06-27 も確認。

## メモ

- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: X検索は英語・日本語で実行したが、x_search はクレジット/契約制限により `personal-team-blocked:spending-limit` で失敗したため、X由来の個別投稿は採用していない。
- Web検索の注意: Hermes の web_search / web_extract は Firecrawl 未設定で失敗したため、代替として arXiv API、Hacker News Algolia API、直接HTTP取得を用いた。直接取得で Martin Fowler 記事の日付とタイトルを確認した。
- 注意点・誇張リスク: 「loop engineering」という語はまだ統一された学術分野名というより、エージェント開発における反復・検証・外部接地・統治を束ねる実践語彙として使われている。したがって本レポートでは、名称の流行そのものよりも哲学・認識論・サイバネティクスとの接続が強い項目を優先した。

# Philosophy of Loop Engineering トレンド調査 (2026-07-29)

- 調査日: 2026-07-29
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は、エージェントに「命令する技術」から、証拠・停止条件・記憶・統治を組み込んだ反復実践を設計する思想へ移りつつある。

## トップ5

### 1. Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control
- 出典: arXiv（Web/arXiv検索で確認）
- 日付: 2026-07-16
- リンク: http://arxiv.org/abs/2607.14890v1
- 要約: 自律的なコーディングエージェントの「reviewed」「tested」「DONE」といった状態を、エージェントの宣言ではなく、現在のソース状態に紐づいた機械検証可能な証拠でのみ遷移させる方法を提案している。proof を意味論的な完全正しさではなく、明示された信頼モデル下でゲートに通せる証拠として扱う点が中心。
- なぜ面白いか:
  - 技術: ループを trigger / goal / verification / stopping rule の制御系としてではなく、ライフサイクル状態を証拠でゲートする運用機構として具体化している。
  - 人文: これは「信じるな、根拠を見よ」という認識論の実装であり、AI時代のプラグマティズムに近い。エージェントの発話を行為や事実と同一視しない態度は、証言・証拠・責任の境界を再設計する哲学的テーマでもある。

### 2. Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting
- 出典: arXiv（Web/arXiv検索で確認、14日より少し古いが基礎文献として関連）
- 日付: 2026-06-28（古いが重要）
- リンク: http://arxiv.org/abs/2607.00038v1
- 要約: 「エージェントを逐次プロンプトで手取り足取り動かす」のではなく、trigger、goal、verification step、stopping rule、memory からなる再利用可能な loop specification を人間が設計する、という実践の転換を定式化している。通常のプログラミングループや内部の perceive-act-observe サイクルと、外部から設計されるループ仕様を区別する点が重要。
- なぜ面白いか:
  - 技術: コーディングエージェント運用の単位を「良いプロンプト」から「検証と停止を含む仕様」に移し、プロンプト術をハーネス設計へ引き上げている。
  - 人文: 実践知の観点では、熟練者の価値は一回の指示文ではなく、失敗から学び続ける作法を環境に埋め込むことにある。これは工学を「制作」だけでなく「反復を飼いならす文化」として捉える見方につながる。

### 3. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans
- 出典: arXiv（Web/arXiv検索で確認）
- 日付: 2026-07-12（直近14日からわずかに外れるが関連度が高い）
- リンク: http://arxiv.org/abs/2607.10878v1
- 要約: AIエージェントがツール利用・委任・経験学習・自己変更を行う持続的チームになる状況で、「何ができるか」より「誰が、何に変化してよいと許すか」を問う governance layer を提案している。文書、画像、音声、API、人間の指示などを versioned agent packs にまとめ、テスト、権限、ポリシーを含めて進化を管理する。
- なぜ面白いか:
  - 技術: ループの対象を単体タスクから、エージェントチームの自己進化・権限・ポリシー更新に拡張している。
  - 人文: サイバネティクス的に見ると、ここでの問題は制御ではなく「制御される制御」、つまり進化する組織のメタ統治である。人間とAIの共同体がどの記憶を制度化し、どの変化を拒むかという政治哲学の問いも含んでいる。

### 4. NVIDIA-labs OO Agents: Native Python Object-Oriented Agents
- 出典: arXiv（Web/arXiv検索で確認）
- 日付: 2026-07-22
- リンク: http://arxiv.org/abs/2607.20709v1
- 要約: エージェントをプロンプト、ツールスキーマ、コールバック、ワークフローグラフに分散させる代わりに、Pythonオブジェクトとして扱う NOOA を提案している。メソッドが行為、フィールドが状態、docstring がプロンプト、型アノテーションが契約となり、`...` のメソッド本体が実行時に LLM 駆動ループで補完される。
- なぜ面白いか:
  - 技術: ループを抽象的なワークフローではなく、テスト・トレース・型契約を持つ通常のプログラム構造に接続するため、反復の検証可能性が上がる。
  - 人文: オブジェクト指向は、世界を「性質を持ち、行為できるもの」として分節する哲学的な世界観でもある。エージェントをオブジェクト化することは、人間がエージェントの人格性を過剰に読む危険を抑えつつ、責任ある道具として扱うための言語設計に見える。

### 5. AutoPersonas: A Multi-Timescale Loop Engine for Open-Ended Persona Evolution
- 出典: arXiv（Web/arXiv検索で確認）
- 日付: 2026-07-09（直近14日から少し外れるが関連度が高い）
- リンク: http://arxiv.org/abs/2607.08252v1
- 要約: 長期的な persona agent が、同一性を保ちながら新しい出来事・関係・証拠・社会条件へ適応するための multi-timescale life-environment engine を提案している。自己ロック、文脈重力、高確率行動チャネルへの収束といった失敗モードを、複数時間スケールのループ設計で扱う。
- なぜ面白いか:
  - 技術: 反復を単一のタスク完了ループではなく、短期イベント、記憶、環境、アイデンティティが絡む多時間スケールの制御問題として扱っている。
  - 人文: これはエージェントの「自己」とは何かを、固定されたプロフィールではなく、反復される物語と社会関係の束として見る試みである。人格・同一性・変化の哲学を、実装上のメモリ更新や停止条件の問題へ接続している。

## arXiv / 学術
- Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control — arXiv:2607.14890v1。証拠ゲート付きライフサイクル制御としての loop engineering。
- Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting — arXiv:2607.00038v1。loop specification の基礎的整理。
- LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans — arXiv:2607.10878v1。自己進化するエージェントチームの統治レイヤー。
- NVIDIA-labs OO Agents: Native Python Object-Oriented Agents — arXiv:2607.20709v1。Pythonオブジェクトとしてのエージェント設計。
- AutoPersonas: A Multi-Timescale Loop Engine for Open-Ended Persona Evolution — arXiv:2607.08252v1。多時間スケールの人格進化ループ。

## メモ
- Boris Cherny優先の有無: 本トピックは Claude 固有ではないため優先対象外。ただし coding agent / harness 設計との接続は重視した。
- 日本語アカウントの扱い: 日本語X検索（「ループエンジニアリング AI エージェント 評価 フィードバック」）を実行したが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、投稿本文の確認はできなかった。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で失敗したため、代替として arXiv API、arXiv公式検索ページ、GitHub Search API、Hacker News Algolia、DuckDuckGo HTML取得を実行した。DuckDuckGo HTMLは取得できたがパース可能な検索結果が得られず、GitHub/HNでは該当リポジトリ・議論を確認できなかった。したがって今回のトップ5は、実在確認できた arXiv 由来の文献に強く寄っている。

# Philosophy of Loop Engineering トレンド調査 (2026-07-24)

- 調査日: 2026-07-24
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

ループエンジニアリングは「プロンプト術」から、検証・記憶・統治をもつサイバネティックな知の実践へと読み替えられつつあります。

## トップ5

### 1. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans

- 出典: arXiv
- 日付: 2026-07-12
- リンク: https://arxiv.org/abs/2607.10878
- 要約: AIエージェントチームがツール、知識、テスト、権限、ポリシーを含む「agent packs」として進化していくための、自己進化とガバナンスの層を提案する論文です。学習されたプロンプト・メモリ・スキル・ワークフローを、証拠と人間の承認が揃うまでは未信頼のリリース候補として扱う点が中心です。
- なぜ面白いか:
  - 技術: agent activityを監査可能なイベントトレースに変換し、fail-closed verificationで「学習したもの」を即本番化しない設計が、実運用のループエンジニアリングに直結します。
  - 人文: 「エージェントは何ができるか」ではなく「誰がエージェントの変化を承認するのか」を問うため、ループを自律性の技法であると同時に権限配分の政治哲学として捉えられます。人間がループの外部監督者ではなく、証拠と許可によってループを閉じる構成要素になる点が重要です。

### 2. Best practices for Claude Code: Give Claude a way to verify its work

- 出典: Anthropic公式ドキュメント / 技術記事
- 日付: 日付記載なし（2026-07-24に直接取得して確認）
- リンク: https://www.anthropic.com/engineering/claude-code-best-practices
- 要約: Claude Codeの実践指針として、テスト、ビルド、スクリーンショット比較、fixture差分など、エージェントが読める合否シグナルを与えることの重要性を説明しています。「確認手段がなければ人間が検証ループになるが、合否判定を与えるとClaudeが作業・実行・読み取り・修正を自走できる」という整理です。
- なぜ面白いか:
  - 技術: ループを成立させる最小要件を「モデル性能」ではなく、実行可能な検証器と停止条件に置くため、コーディングエージェントの品質改善手順としてすぐ使えます。
  - 人文: これはプラグマティズム的な真理観、つまり「正しいとは反復的な行為の中で耐えることだ」という発想に近いです。知識は回答文の中ではなく、テスト・ビルド・観測・修正という実践の連鎖に宿る、という認識論への移行を示しています。

### 3. Four Types of Agent Loops

- 出典: X投稿（@hanakoxbt）
- 日付: 2026-07-15
- リンク: https://x.com/hanakoxbt/status/2077518405624644023
- 要約: エージェントループを、turn-based、goal-based、time-based、proactiveの4種類に分類し、それぞれ「何が実行を開始するか」「何が実行を終了させるか」で整理した投稿です。探索的作業、測定可能な目標、定期作業、常設任務に応じてループ構造を選ぶべきだと説明しています。
- なぜ面白いか:
  - 技術: ループ設計を抽象論で終わらせず、起動条件・評価器・停止条件・人間の関与度という運用パラメータに分解しているため、cron、CI、Slack監視、Claude Codeの`/loop`や`schedule`に接続しやすいです。
  - 人文: ここでの自律性は「賢さ」ではなく「開始と終了の権限をどこまで委譲するか」として定義されます。これはエージェント論を意識や主体性の問題から、責任・委任・見守りの制度設計へ移す発想です。

### 4. Cybernetics as the older name for loop engineering

- 出典: X投稿（@Frandeeer、@kaseyklimes）
- 日付: 2026-07-22〜2026-07-23
- リンク: https://x.com/Frandeeer/status/2080275230912602557 / https://x.com/kaseyklimes/status/2079946581235683807
- 要約: @kaseyklimesは「loop engineering — you mean cybernetics?」と述べ、@Frandeeerはノーバート・ウィーナーのサイバネティクスを引きながら、知能にはフィードバックが必要であり、誤った評価器は高額なAI計算を「完璧に最適化された間違い」に変えると論じています。Generate → Evaluate → Reflect → Mutateという流れを、古典的なフィードバック制御の現代版として位置づけています。
- なぜ面白いか:
  - 技術: 評価器がゲーム可能だと、エージェントはテストカバレッジやクリック率やjudge modelの好みに過適合するため、ループ設計の核心は「チートしにくい現実信号」を作ることになります。
  - 人文: これはウィーナー、アシュビー、スタッフォード・ビアの思想史を、LLM時代の実務語彙で再発見する動きです。第二次サイバネティクス的に言えば、観察者や検証者もシステムの外部ではなくループ内に組み込まれるため、「誰が評価するのか」自体が哲学的問題になります。

### 5. 検証可能性 × 可逆性で自動ループを判断する日本語圏の議論

- 出典: X投稿（@vivivi、@kgsi）
- 日付: 2026-07-18〜2026-07-19
- リンク: https://x.com/vivivi/status/2078313461159965016 / https://x.com/kgsi/status/2078771465755988093
- 要約: @viviviは、自動ループ化の判断軸を「検証可能性 × 可逆性」とし、検証可能かつ可逆なら完全自動、検証可能だが不可逆なら提案まで、検証不能ならループ化せず対話で進めるべきだと整理しています。@kgsiは、確認できない工場のラインは不良品を速く作るだけだとして、AIエージェントの外側に起動と検証可能性の仕組みを置く重要性を強調しています。
- なぜ面白いか:
  - 技術: 自動化可否をモデルの能力ではなく、検証コスト、ロールバック可能性、人間承認の要否で判定するため、実務ワークフローの安全設計に直接使えます。
  - 人文: この議論は、実践知としての「いつ任せ、いつ止めるか」を扱っています。ループエンジニアリングを単なる効率化ではなく、可逆性・説明責任・人間の判断の居場所を設計する倫理的技法として読める点が大きいです。

## arXiv / 学術

- LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans — arXiv:2607.10878。2026-07-12投稿。verifiable human-agent loop engineering、監査可能なイベントトレース、fail-closed verification、人間承認による進化の統治が主題。
- MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research — arXiv:2607.14582。2026-07-16投稿。数学者が高レベル方針を操縦し、AIエージェントがLean統合の反復検証で形式化・証明作業を進めるhuman-in-the-loop研究環境。
- Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting — arXiv:2607.00038。2026-06-28投稿で直近14日より古いが重要。trigger、goal、verification step、stopping rule、memoryからなるloop specificationを定義し、prompt→context→harness→loopという層の移行を整理。

## メモ

- Boris Cherny優先: 本トピックはClaude固有トピックではないため、Boris Cherny優先検索は適用対象外。ただしClaude Code/Anthropic文脈は公式ドキュメントを確認しました。
- 日本語アカウントの扱い: @vivivi、@kgsiなど、日本語圏の検証可能性・可逆性・デザインハーネス文脈を積極的に採用しました。
- 注意点・誇張リスク: Web検索ツールはFirecrawl未設定で利用不能だったため、Webについては`terminal`から公式ページとarXivページを直接HTTP取得して確認しました。X検索結果はxAIのX Search要約に基づくため、日付・リンクは明示されたものだけを採用し、本文の細部は要約として扱っています。

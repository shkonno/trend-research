# sharp LLM usage トレンド調査 (2026-08-12)

- 調査日: 2026-08-12
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
LLM活用の鋭さは「うまいプロンプト」から、コンテキストを節約し、検証可能な完了条件を置き、失敗軌跡を次の運用ルールに変える設計へ移っている。

## トップ5

### 1. Best practices for Claude Code: コンテキストを最重要資源として扱い、検証ループを渡す
- 出典: 公式ドキュメント / Web（Anthropic Claude Code Docs）
- 日付: 日付記載なし（2026-08-12調査時点で確認）
- リンク: https://code.claude.com/docs/en/best-practices
- 要約: Claude Codeの実践指針として、コンテキストウィンドウが埋まると性能が落ちるため、読み込ませる情報とコマンド出力を管理することを強調している。さらに、テスト、ビルド、lint、スクリーンショット比較、Stop hookなど、エージェントが自分で読める合否シグナルを与えると、ユーザーが手動で気づくまで待つ失敗を減らせる。
- なぜ面白いか:
  - 技術: LLM活用を「指示文」ではなく、コンテキスト予算、実行ログ、合否判定を含む閉ループ制御として扱っている点が実務的に鋭い。
  - 人文: 人間の役割が「コードを書く人」から「完了条件と証拠を設計する人」へ移ることを示している。これは職能の置換というより、判断・責任・検証の配置換えである。

### 2. Master Prompt Agreement: ファイルベースの権限・文脈・検証契約
- 出典: GitHub / Web
- 日付: 2026-08-08更新（GitHub検索結果で確認）
- リンク: https://github.com/laurenzpavlosmalisianos/master-prompt-agreement
- 要約: Master Prompt Agreementは、コードエージェントに対してプロジェクト権限、現在の事実、ワークフロー経路、情報源境界、受け入れ証拠をファイルとして与える運用モデル。チャット履歴に依存せず、必要なときだけ専門ガイダンスを読み込ませ、セットアップや更新時には計画提示、承認、トランザクション的書き込み、検証を求める。
- なぜ面白いか:
  - 技術: 長い会話に重要ルールを埋めるのではなく、権限・状態・手順・証拠をリポジトリ内の読み返せる契約として分離するため、コンテキスト汚染と暗黙前提を減らせる。
  - 人文: これはAIに「お願い」する文化から、AIと作業するための制度・憲章を作る文化への移行に見える。人間同士のチーム運営に近い、責任境界と記録の倫理が前面に出ている。

### 3. SHE: Trajectory-driven Safety Harness Evolution for LLM Agents
- 出典: arXiv
- 日付: 2026-08-10
- リンク: http://arxiv.org/abs/2608.09885v1
- 要約: LLMエージェントの安全性をモデル重みだけでなく、コンテキスト、メモリ、ツール、権限、実行制御を扱う「ハーネス」の問題として捉える研究。System Prompt、Rule Bank、Safety Memory、Tool Policyに分解し、失敗軌跡から構造化診断を作り、局所的に境界を更新して安全性と有用性を検証する。
- なぜ面白いか:
  - 技術: 実運用の失敗ログを、プロンプト・ルール・メモリ・ツールポリシーのどこを直すべきかに帰属させるため、LLM活用の改善が感想戦ではなく更新可能な制御系になる。
  - 人文: 失敗を個人のプロンプト技量に押し戻さず、仕組みの学習材料として扱う点が健全である。安全なAI利用を「禁止事項の列挙」ではなく、経験から制度が成熟するプロセスとして見せている。

### 4. Decoding-Level Taboo: A Diagnostic Stress Test for LLM Robustness
- 出典: arXiv
- 日付: 2026-08-10
- リンク: http://arxiv.org/abs/2608.09900v1
- 要約: 通常ベンチマークではモデルが最適化された生成経路を進むため、実運用での複雑なシステムプロンプト、安全ガード、構造制約下の弱さが見えにくい、という問題を扱う研究。実行時に主要候補トークンをマスクし、モデルを通常経路から外すことで、オフパス時の頑健性を診断する。
- なぜ面白いか:
  - 技術: 「普通に聞いたら答えられる」ではなく、制約やガードレールで生成経路が歪んだときの耐性を測るため、プロンプト設計・ランタイム安全・事前監査の失敗検出に使える。
  - 人文: 人間の組織でも、平時の有能さと例外時の信頼性は違う。この研究は、AIをデモの優等生ではなく、ストレス下で振る舞う社会的アクターとして評価する視点を与える。

### 5. 10 Claude Code Best Practices for Agentic Coding: 計画、分割、コミット、レビューの作法
- 出典: ブログ / Web（OpenHands）
- 日付: 2026-07-02（直近14日より古いが実務的関連性が高いため採用）
- リンク: https://www.openhands.dev/blog/claude-code-best-practices-agentic-coding
- 要約: Claude Codeの実務パターンとして、読み取り専用のplan modeで探索し、計画を人間がレビューし、一度に大きく任せず一機能ずつ実装し、論理的な単位でコミットすることを推奨する。失敗セッションの多くはモデルよりプロンプトや完了条件の曖昧さに起因する、という実践的な見立ても示されている。
- なぜ面白いか:
  - 技術: エージェントの自律性を上げるほど、探索・計画・実装・検証・コミットを小さな可逆ステップに分けるソフトウェア工学が重要になる。
  - 人文: 「AIに任せる」は放任ではなく、共同作業のリズムを設計することだと分かる。人間は逐語的な命令者ではなく、リスクの節目で承認し、意味のある単位に物語を切る編集者になる。

## arXiv / 学術
- SHE: Trajectory-driven Safety Harness Evolution for LLM Agents（2608.09885v1）: ハーネスをSystem Prompt、Rule Bank、Safety Memory、Tool Policyに分け、失敗軌跡から安全境界を更新する。
- Decoding-Level Taboo: A Diagnostic Stress Test for LLM Robustness（2608.09900v1）: 生成時に主要候補トークンをマスクして、通常経路外でのLLM頑健性を測る。
- 関連候補として、Agentic Harnesses: LLM-Driven Verification Layers for Robot Autonomy（2608.09857v1）とTest-Time Scaling for CAD Generation via Verifier-Free Consensus Selection（2608.09706v1）も確認したが、トップ5では上記2本を優先した。

## メモ
- Boris Cherny優先: X検索で @bcherny を含む検索を実行したが、x_searchが `personal-team-blocked:spending-limit` で失敗したため、今回のトップ5にはX投稿を含められなかった。
- 日本語アカウントの扱い: 日本語X検索も同じx_searchクレジット制限で失敗。代替としてDuckDuckGo経由の日本語Web検索をterminalから実行し、日本語記事候補は確認したが、直近性・実践性・リンク検証の観点でトップ5には入れなかった。
- Web検索の注意: Hermesのweb_search / web_extractはFirecrawl未設定で失敗したため、terminalからDuckDuckGo HTML（Jina Reader経由）、GitHub API、arXiv API、直接ページ取得を使って補完した。
- 誇張リスク: 2026年日付のWeb記事にはSEO的な包括記事も混じるため、公式ドキュメント、GitHubで確認できる実体、arXiv APIで確認できる論文を優先した。

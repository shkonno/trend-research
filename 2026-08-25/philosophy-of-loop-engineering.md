# Philosophy of Loop Engineering トレンド調査 (2026-08-25)

- 調査日: 2026-08-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「よいAIシステム」は一発の推論ではなく、観察・評価・修正・記憶をどう閉じるかというループ設計の問題として読める日です。

## トップ5

### 1. OpenAI Agents SDK v0.22.0 と「built-in loop」
- 出典: GitHub release / 公式ドキュメント
- 日付: 2026-08-19（latest release v0.22.0）、ドキュメント最終更新ヘッダ 2026-08-24
- リンク: https://github.com/openai/openai-agents-python/releases/tag/v0.22.0
- 要約: OpenAI Agents SDK は、instructions・tools・guardrails・handoffs・tracing・human-in-the-loop などを備えた軽量なマルチエージェント基盤として更新が続いています。公式ドキュメントは「built-in loop that continues until the task is complete」と明記しており、ループを隠れた実装詳細ではなくエージェントの中核プリミティブに置いています。
- なぜ面白いか:
  - 技術: タスク完了までの実行ループ、ガードレール、ハンドオフ、トレーシングを同一SDK内で扱えるため、反復実行を観測可能な工学対象にしやすい。
  - 人文: ここでの主体性は「一度で正解を出す知能」ではなく、「失敗を観察し、経路を変え、完了条件に近づく実践」として表れます。デューイ的な探究やサイバネティクスの制御観に近い、行為とフィードバックの哲学が実装に降りてきています。

### 2. LangGraph / LangSmith Deployment の durable execution
- 出典: GitHub release / LangChain 公式ドキュメント
- 日付: 2026-08-19（langgraph-sdk==0.4.3 release）、リポジトリ更新 2026-08-24〜25
- リンク: https://github.com/langchain-ai/langgraph/releases/tag/sdk%3D%3D0.4.3
- 要約: LangGraph は「Build resilient agents」を掲げ、LangSmith Deployment 側では durable execution、real-time streaming、horizontal scaling、observability、evaluation を agent workload のライフサイクルに接続しています。ループを「回す」だけでなく、中断・再開・観測・評価まで含めて生産運用の対象にしている点が重要です。
- なぜ面白いか:
  - 技術: 状態を持つグラフ、永続実行、評価・観測基盤が組み合わさることで、エージェントの反復を本番障害に耐える制御ループとして設計できる。
  - 人文: 実践知は一回限りの判断ではなく、記録され、再開され、他者に検証される過程で制度化されます。LangGraph 的な設計は、知識を「頭の中」ではなく、履歴・状態・検査可能性のネットワークとして捉える認識論を促します。

### 3. OpenEvals: ready-made evaluators for LLM apps
- 出典: GitHub release / GitHub repository
- 日付: 2026-08-18（openevals-js==0.2.2 release）、リポジトリ更新 2026-08-20〜24
- リンク: https://github.com/langchain-ai/openevals/releases/tag/openevals-js%3D%3D0.2.2
- 要約: OpenEvals は LLM アプリ向けの既製 evaluator 群を提供する LangChain 系プロジェクトです。ループエンジニアリングにおいて、生成器だけでなく評価器を部品化することは、改善サイクルの「測る目」を標準化する動きとして読めます。
- なぜ面白いか:
  - 技術: 評価器をコード化して再利用できるため、プロンプト変更、モデル変更、ツール変更を同じ尺度で比較し、改善ループをCI/CDに近づけられる。
  - 人文: 評価とは単なるスコアではなく、共同体が何を「よい」とみなすかの制度化です。OpenEvals のような部品は、暗黙の職人判断を共有可能な規準へ変換する一方で、測れない価値を見落とす危険も可視化します。

### 4. Anthropic「Building effective agents」の evaluator-optimizer パターン（古いが現在も基礎文献）
- 出典: Anthropic Engineering blog
- 日付: 2024-12-19（古いが、現在の agent 設計を読む基礎文献として採用）
- リンク: https://www.anthropic.com/engineering/building-effective-agents
- 要約: Anthropic は agentic systems を workflow と agents に分け、特に evaluator-optimizer workflow を「生成するLLM」と「評価・フィードバックするLLM」のループとして説明しています。明確な評価基準と反復改善の測定可能性がある場合に有効で、人間の執筆プロセスとの類比も示されています。
- なぜ面白いか:
  - 技術: evaluator-optimizer は、曖昧な「自己改善」を、生成・評価・修正という分離可能なコンポーネントに落とし込む実装パターンになっている。
  - 人文: これはポラニー的な暗黙知を完全に消すのではなく、人間が明文化したフィードバックを機械の反復過程へ埋め込む設計です。創作・翻訳・探索のような領域では、正解よりも批評可能性が知の中心になります。

### 5. Reflexion: Language Agents with Verbal Reinforcement Learning（古いがループ思想の学術的核）
- 出典: arXiv
- 日付: 2023-03-20 submitted、2023-10-10 revised（古いが、言語的フィードバックによる反復学習の基礎として採用）
- リンク: https://arxiv.org/abs/2303.11366
- 要約: Reflexion は、重み更新ではなく、失敗から得た言語的フィードバックをエピソード記憶に保存し、次の意思決定を改善する言語エージェントの枠組みです。外部環境、コンパイラ、API などとの試行錯誤を、テキスト化された反省として次回の行為へ戻す点がループエンジニアリングの原型になっています。
- なぜ面白いか:
  - 技術: 実行結果を反省文として保持し、次の試行に注入することで、学習をファインチューニングではなく運用時の記憶・プロンプト・評価ループとして実装できる。
  - 人文: 「反省」はここで比喩ではなく、行為の失敗を言語化して未来の行為を変えるメカニズムです。経験が知になるには、出来事が記録され、解釈され、再利用される必要があるという実践哲学を、AI agent が露骨に示しています。

## arXiv / 学術

- Reflexion: Language Agents with Verbal Reinforcement Learning / arXiv:2303.11366 / 言語的フィードバックとエピソード記憶でエージェントの試行錯誤を改善する古典的論文。
- Self-Refine: Iterative Refinement with Self-Feedback / arXiv:2303.17651 / 生成・自己フィードバック・改稿を同一LLMで反復する枠組み。リンク: https://arxiv.org/abs/2303.17651
- 直近14日以内の「Philosophy of Loop Engineering」そのものを主題にした新規 arXiv 論文は、本調査時点のAPI検索では確認できませんでした。arXiv API は 429 / timeout が発生したため、既知IDの直接取得で確認できた関連文献のみ掲載しています。

## メモ

- Boris Cherny優先の有無: Claude 固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索も実行しましたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、今回のX由来アイテムは採用できませんでした。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で失敗したため、検索エンジン横断の網羅性は限定的です。代替として、公式ドキュメント、GitHub API、GitHub release、arXiv 直接取得を使い、リンクが実在するものだけを採用しました。

# Harness engineering トレンド調査 (2026-07-19)

- 調査日: 2026-07-19
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「モデルを賢くする」話から、「Agent が失敗しにくい環境・契約・検証ループを作る」話へ急速に具体化している。

## トップ5

### 1. Harnessing LLMs for Reliable Academic Supervision: A Comparative Study
- 出典: arXiv
- 日付: 2026-07-16
- リンク: https://arxiv.org/abs/2607.14707
- 要約: 学術指導という高リスク領域で、GPT-5 の素のチャットボットよりも、小型モデルを LangGraph ベースの Harness で包んだシステムの方が、根拠性・説明可能性・一貫性・プロセス整合性などで高評価だったと報告している。Harness の構成要素として、記号的フィルタ、検索、スキーマ付き I/O、LLM-as-judge、HITL ゲート、監査ログが明示されている。
- なぜ面白いか:
  - 技術: 「大きなモデル」より「検証可能な足場」を重視する設計が、モデルサイズを超えて信頼性を改善しうることを具体的な評価で示している。
  - 人文: 学術指導は人生・評価・制度が絡む領域であり、AI を単なる助言者ではなく、説明責任を持つ制度的道具として扱う必要がある。Harness engineering は、人間の判断を置き換えるというより、判断の来歴を保存し、異議申し立て可能にするための社会的インフラとして読める。

### 2. From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents
- 出典: arXiv
- 日付: 2026-07-09
- リンク: https://arxiv.org/abs/2607.08028
- 要約: 企業向け LLM Agent を、プロンプト中心の試作品から、ソース境界・エンティティルーティング・出力契約・再現可能なトレースを持つ監査可能なアーキテクチャへ移す方法を提示している。参照実装と評価成果物も公開されている。
- なぜ面白いか:
  - 技術: 決定論的な振る舞いをコード、マニフェスト、スキーマ、検証アーティファクトへ移し、モデルを交換しても保持すべき契約を Harness 側で担保している。
  - 人文: 企業利用では「AI が正しそうに答えた」だけでは足りず、誰が・何を根拠に・どの契約を満たして答えたかが問われる。プロンプトから契約へという移行は、AI 利用を職人芸から組織統治へ移す文化的変化でもある。

### 3. Claude Code: A harness for every task / dynamic workflows
- 出典: Anthropic Blog
- 日付: 2026-06-02（14日より古いが、Claude Code と Harness engineering の接点として継続的に重要）
- リンク: https://claude.com/blog/a-harness-for-every-task-dynamic-workflows-in-claude-code
- 要約: Claude Code の dynamic workflows は、タスクごとに Claude が JavaScript ベースのワークフローを作り、subagents、モデル選択、worktree 分離などを組み合わせて「その場で専用 Harness」を構成するという考え方を示している。長大・並列・敵対的・構造化タスクで、単一コンテキストの限界を避ける狙いがある。
- なぜ面白いか:
  - 技術: Harness を静的な外部オーケストレータではなく、タスクに応じて生成・調整される実行環境として扱う点が Claude Code / loop engineering の実践に近い。
  - 人文: これは「人間が全工程を細かく指示する」労働観から、「人間が評価軸と境界を定め、複数の小さな主体に検討させる」編集者・指揮者型の労働観への転換である。Agentic laziness や goal drift を明示する点も、AI の失敗を道徳的欠陥ではなく制度設計の問題として捉えている。

### 4. Claude Code hooks / subagents / skills 公式ドキュメントの Harness 化
- 出典: Anthropic Docs
- 日付: 2026-07-19 調査時点（ページ上の明示日付なし）
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks.md
- 要約: Claude Code の Hooks は、SessionStart、UserPromptSubmit、PreToolUse、PostToolUse などのライフサイクルイベントでシェルコマンド、HTTP エンドポイント、LLM プロンプトを自動実行できる。関連する subagents や skills と組み合わせることで、フォーマット、通知、コマンド検証、プロジェクトルール適用を LLM の自発性ではなく決定論的制御に寄せられる。
- なぜ面白いか:
  - 技術: Hook、subagent、skill は、Claude Code の周囲に検証・分離・再利用の制御面を作る実用的な Harness 部品として機能する。
  - 人文: 「AI にお願いする」から「AI が働く現場のルールを設計する」へ視点が移ることで、開発者の役割は監督者・制度設計者に近づく。これは loop engineering の「失敗を見つけたら次のループで再発防止を仕込む」という感覚とも接続する。

### 5. 中国語圏コミュニティでの Harness engineering 解説の急増
- 出典: JavaGuide / GitHub / Runoob などの技術記事・学習リポジトリ
- 日付: 2026-07-17〜2026-07-18
- リンク: https://javaguide.cn/ai/agent/harness-engineering.html
- 要約: 中国語圏では「Agent = Model + Harness」「Prompt / Context / Harness Engineering の階層」「AGENTS.md、linter、フィードバックループ、ドキュメント園芸」などの説明記事が短期間で多数出ている。GitHub には Harness Engineering 学習ガイドもあり、概念理解から実践パターンへの翻訳が進んでいる。
- なぜ面白いか:
  - 技術: 公式論文や Claude Code の機能だけでなく、実務者コミュニティが Harness を AGENTS.md、カスタム lint、CI、検証ループといった具体的な開発運用パターンへ落とし込み始めている。
  - 人文: 「馬具」「缰绳」「人类掌舵，智能体执行」といった比喩が広がっており、AI を魔法の箱ではなく、力はあるが制御を要する労働主体として語る文化が形成されつつある。日本語コミュニティでは同語の有意なヒットは本調査では薄く、中国語圏の翻訳・概念整理が先行している点も観察される。

## arXiv / 学術
- Harnessing LLMs for Reliable Academic Supervision: A Comparative Study — 2607.14707 — 2026-07-16。Harness engineering を、信頼性・説明責任・監査ログを支える足場として実証的に扱う。
- From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents — 2607.08028 — 2026-07-09。企業 Agent の契約・検証・監査可能性を Harness 側に移す設計。
- AI Agents Do Not Fail Alone: The Context Fails First — 2607.14275 — 2026-07-15。ProofAgent-Harness でコンテキスト品質を測定し、Agent の失敗を環境側から評価する。
- Self-Evolving Agent Harnesses via Gated Semantic Quality-Diversity — 2607.13683 — 2026-07-15。Harness の改善案生成と、有意な改善の信用付けを分離する自己進化型フレームワーク。

## メモ
- Boris Cherny優先の有無: X 検索で @bcherny を優先確認しようとしたが、x_search はクレジット/サブスクリプション制限で失敗した。Bing RSS と直接取得で Boris Cherny / @bcherny と Harness engineering の明確な直近接点は確認できなかった。
- 日本語アカウントの扱い: X 日本語検索も同じく外部制限で失敗。Bing RSS の日本語クエリでは、AI 文脈の「ハーネスエンジニアリング」ではなく物理的なワイヤーハーネス記事が主に出たため、日本語コミュニティの有意な直近動向は本調査時点では確認できなかった。
- 注意点・誇張リスク: Web 検索ツール Firecrawl は未設定、X 検索は xAI 側の spending-limit で使用不可だったため、Web は Bing RSS、公式 Markdown、arXiv API、Jina Reader 経由の直接取得で補完した。中国語圏の記事には二次解説・流行語化の要素が強いものもあるため、実装根拠は公式ドキュメントと arXiv を優先して読むのがよい。

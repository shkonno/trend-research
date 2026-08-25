# Harness engineering トレンド調査 (2026-08-25)

- 調査日: 2026-08-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は、Claude Code の hooks / subagents / permissions のような「実行面の制度設計」と、arXiv 側の harness 最適化・安全性・科学的検証が合流し、プロンプト術ではなく運用可能な社会技術になりつつあります。

## トップ5

### 1. Claude Code Hooks reference: hooks が実行ライフサイクル全体の制御面になった
- 出典: Anthropic / Claude Code Docs
- 日付: 2026-08-24 更新確認
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks
- 要約: Claude Code の hooks リファレンスは、PreToolUse / PostToolUse / PermissionRequest / Stop / SubagentStart / TaskCompleted / ConfigChange / WorktreeCreate など、多数のイベントで外部コマンド、プロンプトベース hook、agent hook を走らせる設計を説明しています。単に「ツール実行前に検査する」だけでなく、auto mode の分類、権限判断、作業ツリー、サブエージェント、停止条件までを横断する制御層として読めます。
- なぜ面白いか:
  - 技術: harness engineering の中心が、LLMへの指示文ではなく、イベント境界・権限・停止判定・作業状態をプログラム可能にする runtime contract へ移っていることを示しています。
  - 人文: エージェントに自由を与えるほど、「いつ止めるか」「誰が許可したことにするか」という組織文化がコード化されます。これはAI同僚の倫理を、抽象原則ではなく日々の作業導線に埋め込む試みです。

### 2. cc-operator-plugin: Stop-hook gate と evidence ledger で Claude Code を“終われない”実行者にする
- 出典: GitHub リポジトリ
- 日付: 2026-08-24 更新確認（作成は 2026-07-06）
- リンク: https://github.com/betmoar/cc-operator-plugin
- 要約: `cc-operator-plugin` は、Claude Code orchestration harness として、chief-operator charter、tier-routed review / planning workflow、append-only evidence ledger、input-axis token compressor、未検証作業が残ると終了を拒む Stop-hook gate を掲げています。スター数はまだ小さいものの、Claude Code の hooks を使って「完了宣言」を実行時に検査する方向性が明確です。
- なぜ面白いか:
  - 技術: エージェントの品質管理を、会話内の「ちゃんと確認して」ではなく、証拠ログと Stop hook による終了条件として実装する点が実践的です。
  - 人文: 人間の仕事でも、信頼は成果物だけでなく、途中で何を確認したかの記録から生まれます。このリポジトリは、AIに“責任ある作業者らしさ”を付与するための儀礼をコードに落とす例として面白いです。

### 3. Task-CoEvolve: 検証タスクも harness と一緒に進化させる
- 出典: arXiv
- 日付: 2026-08-20
- リンク: https://arxiv.org/abs/2608.20169v1
- 要約: 「Task-CoEvolve: Efficient Harness Optimization via Adaptive Validation Task Selection」は、LLM agent harness のコードを書き換えながら最適化する際、毎回固定検証セットを全件実行するコストを避ける研究です。候補 harness 間で結果が割れる情報量の高いタスクを選び、部分評価から全体性能を推定することで、検証コストを下げながら改善探索を続けます。
- なぜ面白いか:
  - 技術: harness 最適化を、モデル重みの更新ではなく「実行環境コード」と「検証課題」の共進化として扱うため、CIや評価コストが重い実運用に直結します。
  - 人文: 何を試験に出すかが、何を賢さと呼ぶかを決めます。固定試験ではなく、作業環境と評価制度が一緒に変わるという見方は、教育や資格制度の歴史にも似た緊張を持っています。

### 4. HarnessRisk: agent harness の安全性をライフサイクルで測る
- 出典: arXiv
- 日付: 2026-08-18
- リンク: https://arxiv.org/abs/2608.17597v1
- 要約: 「HarnessRisk」は、agent harness の安全性を Harness Configuration、Capability Extension、Runtime Operation、State Persistence、Action Control、Incident Recovery の6段階で評価するベンチマークです。128件のサンドボックス課題を用い、3つの harness、6つの言語モデル、14構成で評価し、攻撃成功率が 12.6% から 80.9% まで大きく変わること、特に設定段階が脆弱になりやすいことを報告しています。
- なぜ面白いか:
  - 技術: プロンプト注入や単一ツールの危険ではなく、設定変更、権限、永続状態、回復までを含む「運用中の harness 責任」を測る点が重要です。
  - 人文: 事故を「モデルが悪い」で終わらせず、組織がどの設定と権限を許したのかへ責任の焦点を移します。AI安全性が、個体の性格評価から職場制度の監査へ広がっているように見えます。

### 5. AI-to-AI Code Reviews: PR作成エージェントとレビューエージェントが閉ループを作る
- 出典: arXiv
- 日付: 2026-08-21
- リンク: https://arxiv.org/abs/2608.21311v1
- 要約: 「AI-to-AI Code Reviews of GitHub Pull Requests」は、AIが作成・変更したPRをAIレビュアーが評価する閉ループを、CodAGE由来のGitHubイベントで大規模に分析します。248,641件のAI由来PRのうち、45,269件が別プロダクトのAIによる cross-product review、208,145件が same-product review を受け、AI同士のレビュー量が増えていると報告しています。
- なぜ面白いか:
  - 技術: coding agent の harness は、実行・テストだけでなく、PR、レビュー、修正、再レビューという loop engineering の社会的プロトコルまで含む必要があることを示します。
  - 人文: コードレビューは本来、知識共有、信頼形成、責任分担の場でした。AI同士のレビューが増えると、人間はどの時点で介入し、どの証拠を信頼するのかという協働文化の再設計が必要になります。

## arXiv / 学術
- Task-CoEvolve: Efficient Harness Optimization via Adaptive Validation Task Selection — arXiv:2608.20169v1、2026-08-20。
- HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety — arXiv:2608.17597v1、2026-08-18。
- AI-to-AI Code Reviews of GitHub Pull Requests — arXiv:2608.21311v1、2026-08-21。
- Bringing analytic rigor to agentic AI for science: The Brain Researcher platform for neuroimaging data analysis — arXiv:2608.19902v1、2026-08-20。科学解析の admissible analyses / required checks / claim scope を harness に埋め込む関連重要例。
- LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents — arXiv:2608.17393v1、2026-08-18。Claude Code などの native coding-agent harness と policy-gradient 学習の接続が主題。
- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — arXiv:2608.00267v2、2026-07-31公開、2026-08-10更新。直近14日からは少し外れるが、loop engineering との接点として継続的に重要。

## メモ
- Boris Cherny優先の有無: X検索で Boris Cherny / @bcherny、Claude Code、loop engineering との接点を確認しようとしましたが、`x_search` は `personal-team-blocked:spending-limit` で失敗しました。そのため、Boris Cherny の直近投稿は本調査時点で確認できず、未検証情報は採用していません。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で確認不能でした。代替として日本語Webでは、2026-04-01 の「Claude Code ハーネス（Harness）完全解説」（https://shimayo0218.hatenablog.com/entry/2026/04/01/234316）を直接確認しました。直近14日ではないためトップ5には入れていませんが、日本語コミュニティでは CLAUDE.md、Hooks、Skills、Agents、MCP を5層構造として説明する文脈があることを確認しました。
- 注意点・誇張リスク: web_search は Firecrawl 未設定で使用不可、X検索はクレジット制限で使用不可でした。DuckDuckGo / Google のHTML検索も自動化ブロックが出たため、今回は公式ドキュメント直接取得、GitHub API、arXiv API、日本語ブログ直接取得を中心に順位付けしています。X由来の話題量は観測できていないため、順位は「リンクと日付を実確認できる実装・論文・公式更新としての面白さ」を優先しています。

# Harness engineering トレンド調査 (2026-10-01)

- 調査日: 2026-10-01
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「AIに任せる」から「AIが走る軌道・検査・停止条件を設計する」へ移り、Claude Code 実務、日本語コミュニティ、評価ハーネス、ループ制御が一つの流れにまとまりつつあります。

## トップ5

### 1. Claude Codeで開発期間を2.5か月から1か月に縮めた「ハーネス」の設計手法
- 出典: SmartHR Tech Blog
- 日付: 2026-09-16（直近14日からは少し古いが、国内実践例として重要）
- リンク: https://tech.smarthr.jp/entry/2026/09/16/110205
- 要約: SmartHR のプロダクト開発で、Claude Code を単発のコーディング補助ではなく、要件・設計・実装・検証を通す「ハーネス」として扱い、見積もり約2.5か月の開発を約1か月へ短縮したという事例。日本語圏で Harness engineering が単なるプロンプト術ではなく、開発プロセス設計として語られた点が大きい。
- なぜ面白いか:
  - 技術: Claude Code の出力品質を、コンテキスト設計、作業分解、レビュー、検証手順という外側の構造で安定化する実務パターンが示されている。
  - 人文: 「AIが速い」ではなく「人間がどのような作業環境をAIに与えるか」が成果を左右するという、道具論・労働編成の話になっている。日本語コミュニティにとって、AI導入の成功条件を個人技から組織的な型へ移す象徴的な記事です。

### 2. harness: ticket to spec, test-first build, independent review, gated merge
- 出典: GitHub リポジトリ `sluengen/harness`
- 日付: 2026-09-30 更新
- リンク: https://github.com/sluengen/harness
- 要約: Claude Code と Codex 向けのプラグインとして、チケット化、仕様化、テストファースト実装、独立レビュー、ゲート付きマージを一つの配送ループにするハーネス。README では `/capture`、`/propose`、`/build`、レビューの PASS/FAIL といった運用語彙が整理されている。
- なぜ面白いか:
  - 技術: LLM エージェントの作業を「ブランチ・ワークツリー・テスト・独立レビュー・マージゲート」という既存のソフトウェア工学装置へ接続している。
  - 人文: ここでのハーネスは、AIを自由に暴走させる檻ではなく、責任を分割して合意を積み上げる社会的プロトコルに近い。チケットからマージまでの道筋を明文化することで、人間が「何を任せ、どこで止めるか」を再交渉しやすくしている。

### 3. amux: open-source control plane for AI coding agents
- 出典: GitHub リポジトリ `mixpeek/amux`
- 日付: 2026-10-01 更新
- リンク: https://github.com/mixpeek/amux
- 要約: Claude Code、Codex、Gemini CLI、OpenCode、Ollama など複数のコーディングエージェントを、共有ボード、原子的タスク、スケジュール、ループ、メッセージング、自己修復を備えた制御平面で動かすプロジェクト。Harness engineering と loop engineering の接点として、単体エージェントではなく「AI開発チーム」を運用する方向を示している。
- なぜ面白いか:
  - 技術: 並列ワーカー、タスクボード、永続状態、モデル切替、回復機構を備えることで、エージェント実行を一回のチャットから継続的な制御システムへ引き上げている。
  - 人文: 複数のAIに仕事を配る構図は、管理職・編集者・管制官の役割を人間がどう再設計するかという問題を浮かび上がらせる。Loop engineering は、人間が手を動かす量を減らすだけでなく、判断・介入・信頼のリズムをどう作るかの文化論でもある。

### 4. ASSERT: requirement-driven evaluation harness for AI agents and LLM applications
- 出典: GitHub リポジトリ `responsibleai/ASSERT`
- 日付: 2026-09-30 更新
- リンク: https://github.com/responsibleai/ASSERT
- 要約: 要件から振る舞い別テストケースを生成し、任意のターゲット（ホスト型モデル、 callable wrapper、OpenTelemetry でトレースされたエージェントなど）に対してローカルファーストに評価・回帰テストするハーネス。AIアプリケーションを「気分で動くもの」から、要件と証跡で検査する対象へ近づけている。
- なぜ面白いか:
  - 技術: spec-driven scoring、trace-aware evaluation、local artifacts によって、エージェントのふるまいをCI的に再検査しやすくしている。
  - 人文: AIの失敗はしばしば「なんとなく変だった」で終わるが、要件駆動のハーネスは、失敗を語れる単位へ分解する。これは責任追跡、監査、チーム内の説明可能性を支える倫理的インフラでもある。

### 5. Thinking Before Thinking: Scaling Agentic Inference Through Meta-Reasoning
- 出典: arXiv
- 日付: 2026-09-29
- リンク: http://arxiv.org/abs/2609.38147v1
- 要約: 長いエージェント実行では、どの途中結果を使うか、やり直すか、いつ止めるかといった「実行制御」そのものが課題になるとして、controller と workers に分ける agentic meta-reasoning を提案する論文。要約では、この仕組みを inference-time harness と位置づけ、ProgramBench などで既存の生産用コーディングエージェントや研究ハーネスと比較している。
- なぜ面白いか:
  - 技術: タスク実行を worker に任せ、controller が予算・記憶・次アクション選択を扱うことで、ハーネスを外部スクリプトではなく推論時の制御構造として定式化している。
  - 人文: 「考える前に、どう考えるかを考える」という構図は、AIにもメタ認知的な制度設計が必要だという示唆を持つ。人間の熟練者が段取り・見直し・撤退判断を行うのと同様に、エージェントにも判断の足場を作る必要がある。

## arXiv / 学術
- 見つかったもの: `Thinking Before Thinking: Scaling Agentic Inference Through Meta-Reasoning`（arXiv:2609.38147, 2026-09-29）。agentic meta-reasoning を inference-time harness として扱い、長時間エージェント実行の制御を明示的な研究対象にしている。
- 関連して確認: `Multi-SWT-Bench: A Multilingual Benchmark for Reproduction Test Generation`（arXiv:2609.34752, 2026-09-28）は、Claude Code を含む手法で reproduction test generation を比較しており、ハーネス評価・テスト生成の近接領域として有用。

## メモ
- Boris Cherny優先の有無: X検索で `@bcherny` / Boris Cherny / Claude Code / harness / loop engineering を優先確認しようとしたが、x_search はクレジット上限エラーで利用できなかった。代替として Web/Yahoo検索、GitHub API、arXiv API、直接HTTP取得で確認した範囲では、今回のトップ5に入れるだけの Boris Cherny 由来の確認可能な新規リンクは見つからなかった。
- 日本語アカウントの扱い: X検索が利用不能だったため日本語X投稿は未確認。代替として日本語Web検索で SmartHR Tech Blog、Qiita、Zenn、note などのハーネス関連記事を確認し、実務性と新しさから SmartHR の記事をトップ項目に採用した。
- 注意点・誇張リスク: GitHub検索では2026-09-30前後更新の harness 系リポジトリが多数見つかったが、スター数・実運用実績・READMEの具体性には差がある。ここでは「流行の兆候」と「設計語彙の面白さ」を重視し、事実確認できたURLだけを採用した。
- 情報源制限: Hermes の web_search / web_extract は Firecrawl 未設定で利用不能、x_search は利用枠不足で失敗した。そのため、検索エンジンHTML、GitHub API、arXiv API、直接HTTP取得によるローカル代替調査を行った。

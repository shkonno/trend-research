# sharp LLM usage トレンド調査 (2026-08-19)

- 調査日: 2026-08-19
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
LLM活用の焦点は「うまい一発プロンプト」から、コンテキスト、検証、失敗回復、監査可能性を組み込んだ作業設計へ移っている。

## トップ5

### 1. GPT-5 prompting guide
- 出典: OpenAI Cookbook
- 日付: 2026-08-19
- リンク: https://cookbook.openai.com/examples/gpt-5/gpt-5_prompting_guide
- 要約: GPT-5向けに、エージェント的タスク、指示遵守、API機能、フロントエンド/ソフトウェア開発でのプロンプト調整をまとめた実践ガイド。特に「モデル任せ」ではなく、現実のワークフローで品質を最大化するために、タスクの境界・ツール利用・期待出力を明示する方向が強い。
- なぜ面白いか:
  - 技術: 最新モデルでも、性能差はモデル単体ではなく「タスク分解、制約、ツール、検証条件」をどれだけプロンプト側に埋め込むかで大きく変わることを示している。
  - 人文: LLM活用が文章術ではなく、仕事の依頼作法そのものを再設計する段階に入ったことが見える。人間が何を目的、制約、評価基準として言語化できるかが、チームの知的生産性を左右する。

### 2. AI Product Playbook: prototype first, spec before code, test by contract, verify with your eyes
- 出典: GitHub リポジトリ
- 日付: 2026-08-18（作成/更新）
- リンク: https://github.com/painfulChen/ai-product-playbook
- 要約: Claude Code / Codex を日常的に使ったプロダクト開発から、プロトタイプ先行、仕様化してから実装、契約テスト、人間の目視確認、ゲート付きリリースというループを抽出したプレイブック。README自体が「一度飛ばして失敗したからルールになった」と説明しており、LLM利用の失敗学として読める。
- なぜ面白いか:
  - 技術: コーディングエージェントの出力を、仕様、テスト、目視検証、出荷ゲートという複数のチェックポイントで囲う実務的パターンになっている。
  - 人文: これは自動化万能論ではなく、AIに任せる部分と人間が責任を取る部分を分ける「職能の再契約」である。失敗をプロンプトの技巧不足ではなく、組織的な手順不足として扱う点が鋭い。

### 3. AgentR: Stateful and Recovery-Aware Software Architecture for LLM-based Auditable Workflows
- 出典: arXiv
- 日付: 2026-08-15
- リンク: https://arxiv.org/abs/2608.15264
- 要約: LLMアプリを単なるステートレスなプロンプト応答ではなく、中間成果物、状態遷移、リトライ、孤児ジョブ検出、トークン費用ログ、価格履歴まで含む監査可能ワークフローとして設計する提案。科学文献レビューを例に、Redis/BullMQ/PostgreSQLを使った回復可能な実行基盤を評価している。
- なぜ面白いか:
  - 技術: LLMの不確実性を「会話をやり直す」ではなく、永続状態、再試行、費用会計、復旧可能性で制御するソフトウェアアーキテクチャに落としている。
  - 人文: 知的作業の自動化では、答えだけでなく「どの意図から、どの中間判断を経て、いくらのコストで出たか」が重要になる。監査可能性は企業統制だけでなく、後から人間が納得して引き継ぐための記憶装置でもある。

### 4. Catching Hallucinated Citations in Video-LLM Question Answering
- 出典: arXiv
- 日付: 2026-08-16
- リンク: https://arxiv.org/abs/2608.15574
- 要約: Video-LLMがタイムスタンプ付きで高信頼に見えるが実際には根拠のない主張を出す問題に対し、引用フレームを独立に再検査する自己検証パイプラインを提案。直接「このフレームは主張を支持するか」と聞く方法は迎合で失敗し、ブラインド再キャプションとNLI検証器の組み合わせが安定して幻覚を検出した。
- なぜ面白いか:
  - 技術: LLM自身に同じ文脈で確認させるだけでは検証にならず、独立した観測表現と小さなNLI検証器に分離する必要があることを実験的に示している。
  - 人文: タイムスタンプや引用は「信頼できそうな物語」を作る記号でもある。見かけの根拠が人間の信頼を過剰に誘導する危険を、UI/認知の問題としても読める。

### 5. MUSE: An Interactive Meta-Agent for Understanding and Steering LLM-powered Data Science Systems
- 出典: arXiv
- 日付: 2026-08-17
- リンク: https://arxiv.org/abs/2608.16181
- 要約: 自然言語でデータサイエンス作業を進めるエージェントの実行トレースを、ユーザーが理解・修正しやすい意味階層に再構成するメタエージェント。怪しいステップの提示、特定ステップへの文脈付き質問、修復意図をエージェント向け指示に翻訳する混合主導型のステアリングを扱う。
- なぜ面白いか:
  - 技術: LLMワークフローの改善を、より大きなモデルに任せるのではなく、実行履歴の再表現とステップ単位の介入インターフェースとして設計している。
  - 人文: これは「AIに作業させる」から「AIの作業過程を読んで共同編集する」への転換である。人間は最終答案の採点者ではなく、途中の意味づけと方向修正を担う編集者になる。

## arXiv / 学術
- AgentR A Stateful and Recovery-Aware Software Architecture for LLM-based Auditable Workflows — 2608.15264 — 状態・復旧・監査・費用会計を含むLLMワークフロー設計。
- Catching Hallucinated Citations in Video-LLM Question Answering — 2608.15574 — 引用付き回答の幻覚を、独立検証パイプラインで検出する実験。
- MUSE: An Interactive Meta-Agent for Understanding and Steering LLM-powered Data Science Systems — 2608.16181 — エージェント実行履歴を意味階層化し、人間が修正介入できるようにする研究。
- HarnessEval-W: Agentifying the Evaluation of Visual Worlds — 2608.16859 — 評価を単一スコアではなく証拠木として提示する、エージェント型評価パイプライン。
- Measuring Reward Hacking and Reasoning-Answer Decoupling Under Position-Confounded Optimization — 2608.15445 — 報酬ハックと推論/回答の乖離を測る研究で、LLM検証設計の失敗例として重要。

## メモ
- Boris Cherny優先の有無: 本トピックはClaude固有ではないため必須扱いにはしなかった。Claude Code系の実践論としてAnthropicのベストプラクティスも確認したが、今回のトップ5では直近性と失敗回復/検証の鋭さを優先した。
- 日本語アカウントの扱い: 日本語X検索も実施したが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、X由来の具体投稿は採用していない。
- 注意点・誇張リスク: Web検索ツールもFirecrawl未設定で失敗したため、Web側は直接HTTP取得、GitHub API、Jina Reader、Hacker News API、arXiv APIで補完した。GitHub新規リポジトリはスター数が少なく、流行の大きさではなく「実践パターンの鋭さ」で評価している。

# Philosophy of Loop Engineering トレンド調査 (2026-08-06)

- 調査日: 2026-08-06
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop Engineering は「作って終わり」ではなく、観察・診断・修正・再実行を制度化する実践知として、サイバネティクスと認識論にかなり近づいている。

## トップ5

### 1. Reframing AI Loss of Control: What Control Is, How to Have It, How to Lose It
- 出典: arXiv
- 日付: 2026-07-21 更新（初版 2026-05-19、直近14日よりやや古いが重要）
- リンク: http://arxiv.org/abs/2606.12442
- 要約: AIの「制御喪失」を語る前に、そもそも制御とは何かを「目標を設定し、達成すること」として定義し直す論文。サイバネティクス、管理制御、制御理論を参照し、機能する制御ループ、requisite variety、目標整合性などをAIリスクの語彙に接続している。
- なぜ面白いか:
  - 技術: エージェント設計における監視、介入、目標修正、フィードバックの要件を、単なる安全策ではなく制御ループの成立条件として整理できる。
  - 人文: 「誰が制御しているのか」という問いを、個人・組織・AIシステムのあいだに置き直している点が哲学的に重要。制御喪失を未来の超知能だけでなく、すでにある制度的・組織的な委任の問題として読める。

### 2. Don't Regenerate, Debug: A Domain-Specific Agent for Repairing Near-Miss Hardware Operators
- 出典: arXiv
- 日付: 2026-08-03
- リンク: http://arxiv.org/abs/2608.02712
- 要約: LLMによるGPU/NPU向けカーネル生成で、不合格候補を捨てて再生成するのではなく、コンパイル・実行・数値検証から得られる濃いフィードバックを使って修理する「debug agent」を提案。Debug Pass@1 は 66.7% とされ、再生成型の平均 Pass@1 25.9% を大きく上回り、成功あたりのトークン消費も大幅に下げると報告している。
- なぜ面白いか:
  - 技術: 失敗を廃棄物ではなく探索空間を狭める観測として扱い、計測・診断・修復・収束ガードをループに組み込む実践例になっている。
  - 人文: これは「創造」を一発の生成ではなく、失敗の意味を読み替える職人的反復として捉える視点を与える。近代的な試行錯誤、修理、実験室的知識の系譜にLLMエージェントを接続できる。

### 3. AgentDebugX: An Open-Source Toolkit for Failure Observability, Attribution, and Recovery in LLM Agents
- 出典: arXiv
- 日付: 2026-07-21（直近14日よりやや古いが重要）
- リンク: http://arxiv.org/abs/2607.18754
- 要約: LLMエージェントの失敗は、表面化したステップと原因ステップがずれることが多いとして、Detect / Attribute / Recover / Rerun の閉ループでデバッグするオープンソース枠組みを提案。GAIAで失敗73件中13件を単一の再実行で修復し、精度を55.8%から63.6%へ改善したと報告している。
- なぜ面白いか:
  - 技術: 実行トレースの観察だけでなく、根本原因帰属、回復案、再実行までを一つの制御サイクルにまとめている。
  - 人文: エラーを「誰のせいか」ではなく「どの時点でどのように世界理解が逸れたか」と読む点が、認識論的な診断に近い。失敗履歴を共有可能な記憶にする構想は、実践共同体が失敗から知識を作る過程にも似ている。

### 4. Kitaru: Every agent run, recorded and replayable
- 出典: GitHub / Hacker News Show HN
- 日付: 2026-07-06（直近14日より古いが関連性が高い）
- リンク: https://github.com/zenml-io/kitaru
- 要約: Kitaru は、既存のエージェントSDKやハーネスの下に置く、自己ホスト可能でフレームワーク非依存のランタイム。READMEでは、各モデル呼び出し、ツール呼び出し、意思決定を再生可能なチェックポイントとして記録し、別モデル・別入力でリプレイして改善できると説明している。
- なぜ面白いか:
  - 技術: ループをプロンプト設計の内部ではなく、記録・再生・比較・ロールバック可能なランタイム層として外部化している。
  - 人文: 「何が起きたか」を後から再訪できることは、説明責任だけでなく、経験を反省可能なものに変える条件でもある。実践知は暗黙の勘だけでなく、再演可能な記録によって共同化される。

### 5. Aletheia — The Uncertainty Loop Agent for Claude Code and Codex
- 出典: GitHub / Hacker News Show HN
- 日付: 2026-07-05（直近14日より古いが関連性が高い）
- リンク: https://github.com/nsankar/Aletheia
- 要約: Aletheia は、調査対象の真偽を「隠れた真実」とし、検索結果をノイズのある手がかりとして扱う調査エージェント。READMEでは、典型的な think → act → repeat ではなく、belief → act → observe → update という POMDP 的な不確実性ループで、反証があれば信頼度を下げ、十分でなければ INCONCLUSIVE と言う設計を掲げている。
- なぜ面白いか:
  - 技術: 信頼度、証拠、残余不確実性、反証をループの状態として明示し、検索エージェントを較正された推論機械に近づけている。
  - 人文: 「よく答えるAI」ではなく「知らないと言えるAI」を作ろうとする点が、認識論的謙虚さの設計になっている。Aletheia という名称どおり、真理を所有物ではなく、証拠との往復で少しずつ開示されるものとして扱っている。

## arXiv / 学術
- 見つかったもの:
  - Reframing AI Loss of Control: What Control Is, How to Have It, How to Lose It — 2606.12442。制御、制御ループ、requisite variety をAIリスク論に接続。
  - Don't Regenerate, Debug: A Domain-Specific Agent for Repairing Near-Miss Hardware Operators — 2608.02712。再生成よりもデバッグという閉ループを重視。
  - AgentDebugX: An Open-Source Toolkit for Failure Observability, Attribution, and Recovery in LLM Agents — 2607.18754。Detect / Attribute / Recover / Rerun のエージェントデバッグループ。
  - CyberCorrect: A Cybernetic Framework for Closed-Loop Self-Correction in Large Language Models — 2605.17305（2026-05-17、古いが背景として重要）。自己修正を閉ループ制御として定式化。
  - The Agent Use of Agent Beings: Agent Cybernetics Is the Missing Science of Foundation Agents — 2605.10754（2026-05-11、古いが背景として重要）。ツールループ、記憶、反省ステップを古典的サイバネティクスに写像。
  - ACEM: A Cost Estimation Model for Agentic Software Engineering — 2608.02582。HITL監督、リトライ、コンテキスト増大をコスト見積もりに入れる試み。

## メモ
- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールがクレジット上限で失敗したため、確認できた日本語X投稿はありません。
- 注意点・誇張リスク: X検索は `personal-team-blocked:spending-limit`、Web検索ツールは Firecrawl 未設定で失敗。代替として arXiv API、Hacker News Algolia API、GitHub raw/公開ページへの直接HTTP取得を使用した。直近14日内の純粋な哲学系記事は少なく、実装寄りの閉ループ事例とサイバネティクス系論文を組み合わせて選定している。架空リンク・架空arXiv IDは使用していない。

# sharp LLM usage トレンド調査 (2026-09-30)

- 調査日: 2026-09-30
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「賢いモデルをどう呼ぶか」よりも、「長い実行をどう設計・観測・検証・停止するか」が、鋭いLLM活用の主戦場になっている。

## トップ5

### 1. Prompting Claude Opus 5.5
- 出典: Anthropic Claude Platform Docs / Hacker News掲載
- 日付: 2026-09-28（HN掲載日）
- リンク: https://platform.claude.com/docs/en/build-with-claude/prompt-engineering/prompting-claude-opus-5-5
- 要約: Claude Opus 5.5向けに、effort calibration、thinking有無、無人エージェント実行、進捗更新、multi-app workflow、pasted textの明示、視覚入力、frontend design defaultsなどを扱う公式プロンプティングガイド。単なる「良いプロンプト集」ではなく、エージェントを長時間・複数アプリ・複数エージェントで動かすときのハーネス設計に近い内容になっている。
- なぜ面白いか:
  - 技術: モデル差分を「観測される失敗パターン」から逆引きし、effort・thinking・progress・context境界を調整する運用手順として提示している。
  - 人文: LLM活用が職人芸の呪文から、利用者に進捗を見せ、貼り付けテキストを信頼境界として扱う社会的インターフェース設計へ移っている。人間が不安になる瞬間、誤って従ってしまう瞬間を、プロンプトとUIでどう制度化するかが問われている。

### 2. Show HN: Relay – a harness for AI coding agents that recover and verify
- 出典: Relay公式サイト / Hacker News
- 日付: 2026-09-29
- リンク: https://relayevals.com
- 要約: Relayは、コーディングエージェントをキュー、実行、チェック、学習のサイクルに載せるハーネス。サイト上では「tests/lint/buildをPR前に再実行」「turns/tokens/time/spendの上限」「runから学んだ内容を次回に保持」「自分のClaude/ChatGPT/Copilot/API keyを使う」といった運用上の具体策が強調されている。
- なぜ面白いか:
  - 技術: エージェントをIDEの補助機能ではなく、予算・検証・回復・再利用可能な学習ログを持つ実行基盤として扱っている。
  - 人文: 「寝ている間にPRができる」という夢は、同時に「何を信じてマージするのか」という責任の再配置でもある。Relayのような道具は、人間の仕事を消すというより、人間を“最後に確認する編集者・監査者”へ押し上げる。

### 3. Why agent harnesses need plans – and why you shouldn't compact context
- 出典: SwarmAgent Engineering記事 / Hacker News
- 日付: 2026-09-24
- リンク: https://swarmagent.dev/resources/engineering/plans-harnesses-and-final-handoffs/
- 要約: HN上で「agent harnesses need plans」「contextを安易にcompactすべきでない」という論点として注目された記事。鋭いLLM利用の実践として、長い作業では要約で文脈を潰すより、計画・ハンドオフ・最終報告の形式を整え、エージェントの状態遷移を人間にも読めるものにする発想が重要になる。
- なぜ面白いか:
  - 技術: コンテキスト圧縮を万能薬にせず、planとhandoffを明示的なプロトコルにして、長時間タスクの失敗点を追跡しやすくする方向性が示されている。
  - 人文: これはチーム開発における「申し送り」の再発明でもある。AIエージェントが増えるほど、人間社会が昔から使ってきた引き継ぎ、議事録、完了条件の文化が再び重要になる。

### 4. Four years of coding with AI
- 出典: av.codes ブログ / Hacker News
- 日付: 2026-09-20（記事内日付）、2026-09-29（HN掲載）
- リンク: https://av.codes/blog/agentic-setup/
- 要約: 2022年の手作業中心のコーディングから、ChatGPTへの貼り付け、検索型AI、Copilot補完、ローカルモデル、そしてエージェントが別マシンで多くのコードを書く現在までの変化を時系列で記録した実践記。どのツールが突然すべてを変えたかではなく、作業単位が「行」から「スケッチ」「タスク」「実行環境」へ変わっていく過程が見える。
- なぜ面白いか:
  - 技術: AI活用の進化を、モデル性能ではなく、エディタ、検索、ローカル実行、評価、リモート環境というワークフロー部品の再編として描いている。
  - 人文: 個人開発者の身体感覚が、キーボードで直接書く人から、複数のエージェント環境を監督する人へ変わる記録になっている。これは効率化の話であると同時に、「自分が作った」と感じる範囲の変化の話でもある。

### 5. TokenCast: Forecasting Token Consumption During LLM Agent Execution
- 出典: arXiv
- 日付: 2026-09-28
- リンク: https://arxiv.org/abs/2609.35760v1
- 要約: LLMエージェントでは、同じタスクでもトークン消費が実行ごとに一桁以上変動し、途中結果によって文脈が膨らむため事前予測が難しい。TokenCastは実行セグメントごとの消費と文脈増加を合成して、追加のLLM呼び出しなしに消費を逐次予測し、SWE-bench Verifiedなどで平均絶対誤差を改善し、固定予算方針より平均21.3%少ないトークンで同等のtrace completionを達成したと報告している。
- なぜ面白いか:
  - 技術: エージェントの「賢さ」ではなく、実行中に増殖するコンテキストコストを予測・制御するための計測モデルを提案している。
  - 人文: LLM活用の現場では、創造性だけでなく請求額、待ち時間、予算超過の恐怖が人間の判断を形作る。TokenCastは、AIとの協働を“魔法”から“会計可能な作業”へ戻す試みとして読める。

## arXiv / 学術

- TokenCast: Forecasting Token Consumption During LLM Agent Execution — arXiv:2609.35760。エージェント実行中のトークン消費予測と予算制御。
- Peppy: An AI-Assisted Workflow for Tight Convergence Analysis of Optimization Algorithms — arXiv:2609.35762。LLM支援の数学的証明探索を、ドメイン知識とSymPy検証で構造化するワークフロー。
- Shockingly Simple Self-retrospection Improves Agentic Models Without RL — arXiv:2609.35741。エージェント自身の失敗・成功経験に対する説明だけを学習対象にして行動改善を狙う研究。

## メモ

- Boris Cherny優先: 本トピックはClaude固有ではなく「鋭いLLM活用」全般のため、Boris Cherny個人の投稿優先は該当薄。X検索は実行したが、xAI側の spending-limit エラーにより取得できなかった。
- 日本語アカウントの扱い: 日本語X検索も実行したが、同じくX検索基盤の制限で取得できなかった。今回はWeb/HN/公式ドキュメント/arXivを中心に選定した。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定で失敗したため、代替としてターミナル経由でHN Algolia、公式ページ、RSS、GitHub API、arXiv APIを取得した。X由来の日本語実践例は不足しているため、今日のレポートは「ソーシャル上の反応」より「実装・運用パターン」に偏っている。

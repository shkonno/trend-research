# Harness engineering トレンド調査 (2026-07-16)

- 調査日: 2026-07-16
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Claude Code周辺の「loop engineering」論が、失敗を前提に観測・制御・記憶・評価まで含める「harness engineering」へ拡張されつつある日です。

## トップ5

### 1. Boris Chernyの「loops」論と、CLAUDE.md・REVIEW.md・skills・docsをチーム資産にする流れ
- 出典: X投稿（Boris Cherny / @bcherny）
- 日付: 2026-07-15
- リンク: https://x.com/i/status/2077460395279692197
- 要約: Boris Chernyが、優れたエンジニアが従来から行ってきた自動化、暗黙知のコード化、チームが使える運用ループの整備を、AI時代にはさらに重要だと述べています。CLAUDE.md、REVIEW.md、skills、docsを整えることで、エージェントが追加説明なしにコードベースへ参加しやすくなる、という主張です。
- なぜ面白いか:
  - 技術: プロンプト単体ではなく、リポジトリ内の説明・レビュー基準・再利用可能スキルを「エージェント実行環境の外骨格」として設計する方向を示しています。
  - 人文: これは「知識を頭の中に置く職人文化」から「他者と機械が参加できる共有文化」への移行です。非エンジニアが領域知識を持ち込みやすくなる一方、誰の判断が標準化されるのかという権力の問題も生まれます。

### 2. 「Harness engineering > loop engineering in 2026」という生産運用寄りの反論
- 出典: X投稿（@realtatendazhou）
- 日付: 2026-07-15
- リンク: https://x.com/realtatendazhou/status/2077490503210156254
- 要約: Borisのloop engineering文脈に対し、2026年はループ最適化よりハーネス設計が重要だという投稿が伸びています。観測可能なツール呼び出し、コスト上限、blast radiusの制限がなければ、エージェント製品ではなくデモにすぎない、という実務的な切り口です。
- なぜ面白いか:
  - 技術: 内側の推論ループではなく、ログ、権限、予算、停止条件、失敗時の封じ込めを設計対象にしている点が、実運用のエージェントアーキテクチャに直結します。
  - 人文: 「賢いAI」への期待を、「見知らぬユーザーの前で安全に失敗できる制度」へ引き戻す発言です。信頼は能力ではなく、事故時の責任境界と救済可能性から作られることを思い出させます。

### 3. 日本語Xでのハーネス論: 研究/実装の分離、文脈汚染、責任境界
- 出典: X投稿群（@cursorvers、@EK_EC_ADS、@47Chan_tw ほか）
- 日付: 2026-07-09〜2026-07-14
- リンク: https://x.com/cursorvers/status/2075336825619808569
- 要約: 日本語圏では、Claude CodeやAIエージェントを長時間使う際、メモリ・ルール・プラグインを増やすほど文脈が汚れるという実践的な議論が出ています。研究セッションと実装セッションを分け、テストやスクリーンショットを固定された到達点にし、人間が最終判断を持つべきだという整理が目立ちます。
- なぜ面白いか:
  - 技術: ハーネスを「盛る」ほど強いのではなく、タスクごとに必要な制約だけを読み込むコンテキスト設計が品質を左右する、という現場知が共有されています。
  - 人文: 日本語コミュニティでは、万能な自律性よりも「AIを literal な同僚として扱い、責任を人間が引き受ける」感覚が強く出ています。これは道具の擬人化を抑え、共同作業の礼儀と監督の形を再設計する議論です。

### 4. Anthropic公式Claude Code Docsの memory / CLAUDE.md / hooks / skills が、実質的なハーネス部品として整備されている
- 出典: Web（Anthropic Claude Code Docs）
- 日付: 2026-07-16調査時点で確認
- リンク: https://docs.anthropic.com/en/docs/claude-code/overview
- 要約: 公式ドキュメントは、CLAUDE.mdをプロジェクトルートに置いてコーディング標準、アーキテクチャ判断、利用ライブラリ、レビュー項目を読ませる仕組みとして説明しています。加えてauto memory、skills、hooksにより、チームの反復ワークフローや編集後フォーマット、コミット前lintなどを組み込めることが確認できます。
- なぜ面白いか:
  - 技術: Claude Codeの実体はモデルだけでなく、memory、CLAUDE.md、skills、hooks、CLI/クラウド実行を組み合わせた運用ハーネスとして見た方が設計しやすくなっています。
  - 人文: 公式機能が増えるほど、チームの慣習やレビュー倫理がツールに埋め込まれます。これは新人教育や共同制作を助ける反面、「正しいやり方」が見えにくく自動化される危うさもあります。

### 5. arXiv: ToFu — 研究者向けのホワイトボックスAgent Harness
- 出典: arXiv
- 日付: 2026-07-13
- リンク: https://arxiv.org/abs/2607.11423v1
- 要約: 「ToFu: A White-Box, Token-Efficient Agent Harness for Researchers」は、研究者向けにコードベース読解、ファイル編集、コマンド実行、開発ツール統合を行うエージェントハーネスを提案しています。LLMの性能だけでなく、周囲のオーケストレーションコードがエージェントの振る舞いを決めると明示している点が、今回のトピックに非常に近い論文です。
- なぜ面白いか:
  - 技術: ハーネスをブラックボックスSaaSではなく、研究対象として検査・改変・評価できるwhite-box orchestrationとして提示している点が重要です。
  - 人文: 研究の現場では、AIに任せること以上に「どの手続きで結果が生まれたか」を説明できることが信頼の条件になります。MIT Licenseでのローカル展開可能性は、プライバシーや研究自治の観点でも意味があります。

## arXiv / 学術
- ToFu: A White-Box, Token-Efficient Agent Harness for Researchers / arXiv:2607.11423v1 / 研究者向けのwhite-box agentic harnessで、ハーネス設計そのものを検査・改変・評価対象にしている。
- SETA: Scaling Environments for Terminal Agents / arXiv:2607.10891v1 / 端末エージェント向けに、実行環境と検証機構を大規模生成する研究。ハーネス工学の「検証可能な環境」側に関係。
- AgentAbstain: Do LLM Agents Know When Not to Act? / arXiv:2607.10059v1 / エージェントが「実行しない」判断をできるかを評価する枠組み。blast radiusや権限停止の議論と接続する。
- Scoped Verification for Reliable Long-Horizon Agentic Context Evolution under Distribution Shift / arXiv:2607.09175v1 / operational harnessが組み立てるagentic contextを、長期運用で検証しやすくする研究。

## メモ
- Boris Cherny優先の有無: 優先確認済み。2026-07-15のBoris投稿を起点に、loop engineeringからharness engineeringへ広がる議論を最上位に置いた。
- 日本語アカウントの扱い: 日本語X検索を実施し、Claude Code利用者・設計者・AI実務者の文脈汚染、研究/実装分離、責任境界の議論を採用した。
- 注意点・誇張リスク: 「Harness engineering」はまだ固定した専門語というより、Claude Code/agent運用の実践語彙として急速に形成中。Web検索ツールは設定未完了で失敗したため、Webについては端末から公式Anthropic Docsを直接取得して確認した。Xの投稿本文・日付はx_search結果に基づく。架空リンク・架空arXiv IDは入れていない。

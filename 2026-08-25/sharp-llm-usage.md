# sharp LLM usage トレンド調査 (2026-08-25)

- 調査日: 2026-08-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「鋭いLLM活用」は、うまいプロンプト一発芸から、仕様・出典・検証・役割分担を外部化する運用設計へかなり移っている。

## トップ5

### 1. More than just code review
- 出典: Simon Willison’s Weblog
- 日付: 2026-08-22
- リンク: https://simonwillison.net/2026/Aug/22/more-than-just-code-review
- 要約: コーディングエージェントを生産的に使う鍵は、生成された全行を人間が読むことではなく、変更を的確に指示し、その変更が正しく適用されたと自信を持って検証できることだ、という短いが重要な指摘。コードレビューを「全差分の目視」から、テスト・挙動確認・不変条件の確認を組み合わせた検証設計へ拡張している。
- なぜ面白いか:
  - 技術: LLM活用のボトルネックを「生成品質」ではなく「検証可能な変更単位と確認手段」に置き直している。
  - 人文: 人間の役割が作業者から監査者・編集者へ移るとき、何を見れば責任を果たしたと言えるのかという職能倫理の問題が前面に出る。AI時代の熟練は、細部を全部抱えることではなく、信頼できる確認儀式を設計する力になっていく。

### 2. OpenSpecでAIコーディングの実装・レビュー・検証を分ける —— ithyno入門
- 出典: Qiita
- 日付: 2026-08-24
- リンク: https://qiita.com/fluentdb-dev/items/9da546029f1c6dfcbe3b
- 要約: AIコーディングで「要件がチャット履歴に埋もれる」「実装した同じセッションが自分でレビューする」「検証が終わったか分からない」といった実務上の痛みを、OpenSpecベースの変更記録と、実装・レビュー・検証を分けたAIセッション割り当てで解こうとする記事。リポジトリに変更理由・タスク・要件を残し、ダッシュボードで複数セッションとターミナル状態を管理する発想が実践的。
- なぜ面白いか:
  - 技術: チャットの一時的な文脈ではなく、仕様・変更・検証をリポジトリ上の成果物として扱うことで、LLMの記憶漏れや自己レビューの甘さをプロセスで補っている。
  - 人文: これは「AIに賢くなってもらう」よりも「共同作業の制度を作る」アプローチで、人間組織のレビュー分掌をAIワークフローへ移植している。個人開発であっても、内側に小さなチームと牽制構造を持つ時代が来ている。

### 3. Spring AIでLLMの出力品質をテストする — 回帰検知と自動リトライ
- 出典: Qiita
- 日付: 2026-08-23
- リンク: https://qiita.com/ryoji9702/items/3c296a6e002064e20090
- 要約: Spring AIのEvaluator APIとRecursive Advisorsを使い、LLMアプリの出力品質をCI時の回帰検知と実行時の自動リトライに分けて考える記事。RelevancyEvaluator / FactCheckingEvaluatorをJUnitへ組み込む方法、生成→評価→フィードバック→再生成の使いどころ、LLM as a Judgeを本番投入する際の落とし穴を整理している。
- なぜ面白いか:
  - 技術: LLM出力を固定文字列でテストしようとせず、関連性・事実性・実行時再生成という複数レイヤーの品質ゲートに分解している。
  - 人文: 「AIが正しいか」を神託のように判定するのではなく、誤りうる主体同士をどう制度的に組み合わせるかという話になっている。品質保証はもはや後工程の検査ではなく、利用者に不確実性を渡さないためのケアの設計でもある。

### 4. The /wayfinder Skill: Navigating the “Fog of War” of Planning
- 出典: Latent.Space
- 日付: 2026-08-20
- リンク: https://www.latent.space/p/wayfinder-skill
- 要約: Matt Pocock氏の「/wayfinder」スキルを紹介する記事で、グリーンフィールド開発や進路が曖昧な場面で、計画作業を複数スレッドに分け、プロトタイピングや調査を行い、最終的に統合するオーケストレーター層として使う発想が語られている。文脈窓の残量を人間が常に気にする苦痛を、計画専用のセッション管理で肩代わりさせる点が鋭い。
- なぜ面白いか:
  - 技術: 長い計画を単一会話に詰め込むのではなく、調査・試作・統合を分岐させることで、コンテキスト圧迫と早すぎる実装を避ける設計になっている。
  - 人文: 「霧の中で進む」計画段階をAIに任せるのではなく、霧そのものを可視化する道具としてAIを使っている。これは創造性を自動化するというより、不安定な思考過程を外部化して、人間が判断を取り戻すための技法に近い。

### 5. Natural-Language Workflows Are Not Software Yet: Artifact-Driven Compilation for Reliable Agent Execution
- 出典: arXiv
- 日付: 2026-08-21
- リンク: https://arxiv.org/abs/2608.21341
- 要約: 自然言語ワークフローはエージェントに再利用可能な手順を与えるが、データ依存や分岐条件が暗黙になりやすく、長い指示や複雑な制御で失敗しやすいと指摘する論文。提案手法Articは、自然言語の手順を「各ステップが読む/書く成果物」「制約」「明示的な制御遷移」を持つ artifact-driven workflow にコンパイルし、実行時の信頼性を高めようとする。
- なぜ面白いか:
  - 技術: プロンプトを長く詳しくするのではなく、LLMに渡す手順を依存関係つきの成果物グラフへ変換するため、検証・分割・制約チェックがしやすい。
  - 人文: 自然言語だけで機械を動かせるという夢に対し、この論文は「手順を社会的に読める文書から、機械的に責任を追える文書へ変える必要がある」と冷静に言っている。人間の曖昧な指示文化と、ソフトウェアの厳密な実行文化の境界が見える。

## arXiv / 学術

- Natural-Language Workflows Are Not Software Yet: Artifact-Driven Compilation for Reliable Agent Execution — arXiv:2608.21341。自然言語ワークフローを成果物駆動の実行形式へ変換し、エージェント実行の信頼性を上げる研究。
- PromptResponse: Optimizing Prompts for LLM Coding Tasks — arXiv:2608.21074。HumanEval派生の8,200実行で、JSONなど一貫したフォーマットが生成効率や構文安定性を改善する一方、LLMチューニング済みプロンプトが性能を下げる場合を示す。
- Trustworthy RAG: An Evaluation Agent for Detecting Misinformation and Knowledge Poisoning in Generative AI Systems — arXiv:2608.21095。RAGの検索結果を無条件に信じないため、NLI検証・毒性検出・Trust Indexを組み合わせる評価エージェントを提案。
- Specification Portability Across LLM Development Agents: Cross-Agent Compatibility in Specification-Driven Software Migration — arXiv:2608.21208。仕様駆動の移行タスクで、Kiro / Gemini / Copilot等の間で仕様の持ち運びがどこまで効くかを検証し、エージェント依存の劣化を報告。

## メモ

- Boris Cherny優先: 対象はClaude固有ではないため、Boris Cherny氏優先は適用対象外。
- 日本語アカウントの扱い: X検索は英語・日本語とも実行したが、x_searchがクレジット/サブスクリプション制限で失敗したため、X投稿は採用していない。代替としてQiita API、公式/個人ブログの直接取得、arXiv API/直接取得を用いた。
- Web検索の注意: Hermesのweb_search / web_extractはFirecrawl未設定で利用不可だったため、端末からRSS、Qiita API、arXiv API、公開Webページの直接HTTP取得で補完した。検索網羅性には制限がある。
- 注意点・誇張リスク: Qiita記事は実践知として価値が高い一方、個人記事のため、導入効果は各プロジェクトのテスト文化・仕様管理・チーム体制に依存する。arXiv論文は投稿直後で査読前の可能性があるため、数値や一般化は慎重に読む必要がある。

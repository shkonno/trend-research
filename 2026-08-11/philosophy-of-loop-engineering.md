# Philosophy of Loop Engineering トレンド調査 (2026-08-11)

- 調査日: 2026-08-11
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

ループエンジニアリングは「よいプロンプトを書く技術」から、「行為・検証・記憶・責任配分を設計する実践哲学」へ移りつつあります。

## トップ5

### 1. LastGate — AI Agent Commit Guardian
- 出典: GitHub リポジトリ
- 日付: 2026-08-10 更新
- リンク: https://github.com/AaronCx/LastGate
- 要約: Claude Code、Cursor、Copilot、Devin などの AI 生成コミットを、secret scan、lint、build check などの事前ゲートで止め、失敗をエージェントへ戻して自己修正させる「コミット前のループ」を実装する試みです。単なる CI ではなく、失敗信号を作業中のエージェントに返す点がループエンジニアリング的です。
- なぜ面白いか:
  - 技術: コード生成の速度ではなく、エージェントが読める検証信号の近さと明瞭さを最適化している点が実践的です。
  - 人文: 「最後に人間がレビューする」から「機械的な門番が反復の倫理を担う」へ責任の配置が変わります。これは、判断を人間から奪うというより、何を自動化し何を人間に残すかを再設計する問題です。

### 2. Shared Substrate — sustained human–AI coupling のための外部記憶と検証オラクル
- 出典: GitHub リポジトリ / SSRN preprint へのリンクを含む README
- 日付: 2026-08-08 更新、draft v0.2 は 2026年8月表記
- リンク: https://github.com/olegroshka/shared-substrate
- 要約: 長期・多層・多セッションの人間–AI協働では、モデルそのものだけでなく、外部化された状態、層ごとの検証オラクル、観測可能性、そして人間が統治する実行基盤が重要だと主張する「方法論」です。ループを回す前提として、記憶と検証の場を設計する発想が強い内容です。
- なぜ面白いか:
  - 技術: コンテキスト窓の限界を、外部メモリ、抽象レイヤー別の検証、観測可能なフィードバックループで補う設計思想として読めます。
  - 人文: 認識論的には、知識を「モデルの中」ではなく「人間とAIが横断する基盤」に置く立場です。サイバネティクスの制御ループに、記録・制度・統治という社会的な層を加えている点が面白いです。

### 3. DAC-Pose: Dual-Agent Collaborative Framework for Pose-Guided Human Generation
- 出典: arXiv
- 日付: 2026-08-05 submitted / announced August 2026
- リンク: https://arxiv.org/abs/2608.04622
- 要約: ポーズ誘導の人物生成を、意味推論を担う PSR agent と視覚的ずれを扱う DAVE agent の二者協働として定式化し、両者の間に自律的フィードバックループを置く研究です。ソフトウェア開発の話ではありませんが、専門化したエージェント同士が推論と知覚を反復的に補正する構図が明確です。
- なぜ面白いか:
  - 技術: 「生成→評価→補正」を単一モデル内の曖昧な反省ではなく、役割分化した二つのエージェント間のループとして設計しています。
  - 人文: これはサイバネティクス的な知覚–行為ループを、生成AIの内部設計へ移植した例として読めます。知能を孤立した主体ではなく、相互に制約を返し合う関係として捉える点が哲学的です。

### 4. Ask HN: When did we go from agentic loops to graphs?
- 出典: Hacker News 投稿・コメントスレッド
- 日付: 2026-08-01
- リンク: https://news.ycombinator.com/item?id=49136426
- 要約: AI engineering の議論が prompts、loops、graphs へ移っていることに対し、それが実質的な進歩なのか、用語が先行しているだけなのかを問うスレッドです。コメントでは、流行語へ乗り換える前に、まず一つの作業ループを安定させるべきだという実践的な見方も出ています。
- なぜ面白いか:
  - 技術: ループ、グラフ、ワークフローといった抽象の違いを、実際の開発フローの信頼性にどう接続するかが問われています。
  - 人文: これは技術用語の思想史そのものです。新しい名前は実践を見えるようにする一方で、まだ成熟していない実践に過剰な必然性を与える危険もあります。

### 5. The Art of Loop Engineering
- 出典: LangChain Blog
- 日付: 2026-06-16（古いが基礎文献として重要）
- リンク: https://blog.langchain.com/the-art-of-loop-engineering/
- 要約: エージェントの基本ループに加えて、検証ループ、人間レビュー、評価、デプロイ後の改善などを積み重ねる考え方を整理した記事です。特に、grader や rubric、feedback をどの層に置くかという実装上の話が、ループ設計の思想に直結しています。
- なぜ面白いか:
  - 技術: LangChain / LangGraph 的な部品を使い、agent loop を verification loop で包むという具体的な設計パターンを示しています。
  - 人文: 「知る」とは一回で正解を出すことではなく、基準に照らして失敗を返し、行為を修正する反復過程だと捉え直せます。これはプラグマティズムや実践知の伝統と相性がよい読み方です。

## arXiv / 学術

- DAC-Pose: Dual-Agent Collaborative Framework for Pose-Guided Human Generation — arXiv:2608.04622。2026-08-05 submitted。二つの専門エージェント間の自律的フィードバックループを扱うため、ループエンジニアリングの一般化例として採用しました。
- Trust but Verify: Mitigating Medical Hallucinations via Post-Hoc Adversarial Auditing and Multi-Agent Feedback Loops — arXiv:2606.14149。2026-06-12 submitted（古いが関連）。医療QAで五つのエージェントによる監査・検証ループを用い、Hallucination Error Rate を約53%削減したと報告しています。

## メモ

- Boris Cherny優先の有無: Claude 関連では優先設定がありますが、今回の対象トピックで X 検索がクレジット制限により失敗したため、Boris Cherny本人の直近投稿は確認できませんでした。Addy Osmani の記事内で Boris Cherny の「My job is to write loops」という趣旨の引用を確認しました。
- 日本語アカウントの扱い: 日本語 X 検索も実行しましたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、今回のトップ5には日本語アカウント由来の項目を入れていません。
- Web検索の注意: Hermes の web_search は Firecrawl 未設定で失敗したため、直接HTTP取得、Hacker News Algolia API、GitHub API、arXivページを使って補完しました。
- 注意点・誇張リスク: GitHub リポジトリには新規・低スターのものが含まれます。採用理由は人気度ではなく、ループエンジニアリングを哲学・認識論・実践知・サイバネティクスとして読むうえで、設計パターンが明確だったことです。

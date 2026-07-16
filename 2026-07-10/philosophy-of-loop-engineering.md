# Philosophy of Loop Engineering トレンド調査 (2026-07-10)

- 調査日: 2026-07-10
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop Engineering は「エージェントを賢くする技術」から、「誰が・何を根拠に・どの時点で閉じたループを信じてよいのか」を設計する実践哲学へ寄ってきています。

## トップ5

### 1. Microsoft Agent Framework の Human-in-the-Loop / AG-UI 承認ループ
- 出典: Microsoft Learn
- 日付: ms.date は 2026-03-09 / 2026-04-01、ページ更新は 2026-07-02
- リンク: https://learn.microsoft.com/ja-jp/agent-framework/workflows/human-in-the-loop / https://learn.microsoft.com/ja-jp/agent-framework/integrations/ag-ui/human-in-the-loop
- 要約: Microsoft Agent Framework は、Executor が外部システムや人間に要求を送り、応答を待ってから実行を継続する HITL を RequestPort / approval request として整理している。AG-UI 側では、ツール呼び出しを即時実行せず、クライアントへ承認要求として流し、ユーザーの承認・拒否を受けて処理を再開するパターンが説明されている。
- なぜ面白いか:
  - 技術: エージェントのツール実行を「生成→停止→承認→再開」という明示的な制御ループにし、チェックポイントや承認 UI と接続できる。
  - 人文: これは単なる安全装置ではなく、行為の最終責任をどこに置くかという実践哲学の設計である。サイバネティクス的には、環境からのフィードバックだけでなく「人間の判断」をループ内の制御信号として制度化している点が重要。

### 2. LLM-Based Test Oracles: Source-of-Authority Taxonomy
- 出典: arXiv
- 日付: 2026-07-06
- リンク: https://arxiv.org/abs/2607.05031
- 要約: LLM をテストオラクルとして使う研究について、判定が何を権威の源泉としているのかを分類する系統的レビュー。54件中、仕様が単独の権威源になっているのは約半数で、残りは verdict の根拠が明示されない例があると報告している。
- なぜ面白いか:
  - 技術: 「LLM-as-a-judge」という機構名ではなく、判定の根拠・権威・評価失敗を分解して、検証ループの信頼境界を見える化する。
  - 人文: Loop Engineering の認識論的な核心は、反復すれば真に近づくという素朴な信念ではなく、ループ内の判定者が何に基づいて正しさを宣言するかにある。この論文は、エージェント開発の「何をもって知ったことにするのか」を問う材料になる。

### 3. Human-in-the-Loop Nugget Annotation for Accountable LLM-as-a-Judge Evaluations
- 出典: arXiv
- 日付: 初版 2026-06-27、改訂 2026-07-07
- リンク: https://arxiv.org/abs/2606.29033
- 要約: AI / Agentic system の出力評価で、人間が重要情報の nugget を同定し、LLM が大量照合を担う分業型ワークフローを提案する。人間を単なるラベル付け労働や追認役にせず、評価基準の生成側に置く点が特徴。
- なぜ面白いか:
  - 技術: 評価ループを「人間が意味単位を設計し、LLM がスケール処理する」形に分解し、LLM-as-a-judge の説明責任を上げる。
  - 人文: 実践知の観点では、人間の役割はボタンを押す監督者ではなく、何が問題の本質かを切り出す判断者である。これは暗黙知をループの入口に戻す設計であり、職人性と自動化の関係を再考させる。

### 4. Don’t Blindly Trust It: How Unreliable Feedback Breaks Tool-Using LLM Agents
- 出典: arXiv
- 日付: 2026-06-19（直近14日より古いが、フィードバックループの認識論に直結するため採用）
- リンク: https://arxiv.org/abs/2606.21409
- 要約: ツール利用型 LLM エージェントが、信頼できない外部フィードバックを受けたときにどのように壊れるかを、ループ・プロンプト・行動空間などを固定した比較で調べる研究。外部観測が常に性能向上につながるという前提を疑っている。
- なぜ面白いか:
  - 技術: ループを増やすほど良くなるのではなく、返ってくる観測の信頼性が低い場合は、フィードバックなしより悪化しうることを検証対象にする。
  - 人文: これは「経験から学ぶ」ことの条件を問う認識論である。歴史的なサイバネティクスが feedback を制御の基本語にしたのに対し、現代のエージェント工学では feedback の真偽・ノイズ・制度的由来まで問う必要がある。

### 5. ハーネスエンジニアリング入門 ── CLAUDE.md の次に来る AI エージェント制御パラダイム
- 出典: Qiita
- 日付: 2026-03-24（古いが、日本語圏で Loop / Harness Engineering の実践知を言語化しているため採用）
- リンク: https://qiita.com/nogataka/items/d1b3fcf355c630cd7fc8
- 要約: AI エージェントを単にプロンプトでお願いする対象ではなく、制約・環境・検証・誘導を含む「ハーネス」によって力を伝達する対象として捉える日本語記事。CLAUDE.md 的な指示ファイルの次に来る制御パラダイムとして、ハーネスエンジニアリングを説明している。
- なぜ面白いか:
  - 技術: プロンプト、テスト、権限、CI、レビュー、失敗時の戻し方を一つの実行環境として組み、エージェントの出力を反復的に矯正する発想に近い。
  - 人文: 「馬具」としての harness の比喩は、AI を自律的な主体として崇拝するのではなく、力を方向づける技法として見る視点を与える。これはアリストテレス的な実践知、道具論、そして職人が環境を整えてよい振る舞いを引き出す思想に接続できる。

## arXiv / 学術
- LLM-Based Test Oracles: Source-of-Authority Taxonomy -- A Systematic Literature Review, arXiv:2607.05031。判定権威の源泉を分類し、検証ループの認識論を明示化する研究。
- Human-in-the-Loop Nugget Annotation for Accountable LLM-as-a-Judge Evaluations, arXiv:2606.29033。人間が評価の意味単位を作り、LLM が照合を担う分業型 HITL。
- Don’t Blindly Trust It: How Unreliable Feedback Breaks Tool-Using LLM Agents, arXiv:2606.21409。信頼できないフィードバックがツール利用エージェントを壊す条件を検証。
- Position Paper: Towards Open Complex Human-AI Agents Collaboration Systems for Problem Solving and Knowledge Management, arXiv:2505.00018（旧いが関連）。エージェント性の境界中心 ontology、cybernetics、Conversation Theory、SECI、teach-back gate を接続しており、哲学寄りの背景として有用。
- Problem Reductions at Scale: Agentic Integration of Computationally Hard Problems, arXiv:2604.11535（旧いが関連）。制約、検証、フィードバックループを設計する harness engineering が大規模なエージェント実装を支える例。

## メモ
- X検索: 英語・日本語の検索を実行したが、x_search は `personal-team-blocked:spending-limit` で失敗したため、X由来の投稿はトップ5に含めなかった。
- Web検索: web_search / web_extract は Firecrawl 未設定で失敗したため、代替として Bing RSS 取得と直接 URL 取得を terminal で実行し、Microsoft Learn / Qiita / arXiv の実在リンクと到達性を確認した。
- Boris Cherny優先の有無: Claude 固有トピックではないため優先対象外。X検索が利用できず、Boris Cherny 関連の確認はできなかった。
- 日本語アカウントの扱い: X検索不可のため日本語アカウントは確認できず、日本語Webとして Qiita 記事を採用した。
- 注意点・誇張リスク: 「Loop Engineering」という語そのものの新規記事は少なく、HITL、test oracle、feedback reliability、harness engineering、cybernetics を束ねる解釈で構成している。古いが重要な項目は日付欄で明記した。

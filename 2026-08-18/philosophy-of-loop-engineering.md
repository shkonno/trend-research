# Philosophy of Loop Engineering トレンド調査 (2026-08-18)

- 調査日: 2026-08-18
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Loop engineering は「AIを賢くする技術」から、「反復する機械に何を証拠とし、いつ止め、どこで人間が責任を引き受けるか」を設計する実践哲学へ近づいています。

## トップ5

### 1. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 出典: arXiv / Microsoft GitHub / 公式サイト
- 日付: 2026-07-31公開、2026-08-10更新、GitHub更新 2026-08-16
- リンク: https://arxiv.org/abs/2608.00267 / https://github.com/microsoft/Loopsbench / https://loopsbench.ai/
- 要約: Microsoft の LoopsBench は、長時間の coding agent loop を、依存DAG、Docker実行、単体検証、進行ログを含む工程として評価するベンチマークです。単発の正誤ではなく、エージェントが途中で何を前提にし、どこで回帰し、何を証拠として前進したかを測る方向を示しています。
- なぜ面白いか:
  - 技術: 評価対象を「最終回答」から、計画、実行、検証、回帰修復、停止を含むループ全体の振る舞いへ移しています。
  - 人文: 認識論的には、知識をモデル内部の確信ではなく、外部化された証拠と再現可能な手続きとして扱う点が重要です。サイバネティクスのフィードバック思想が、ソフトウェア工程の制度設計として再登場しているように見えます。

### 2. SREForge: 自律SREエージェントの closed-loop behavioural verification
- 出典: GitHub / ドキュメント
- 日付: GitHub更新 2026-08-14
- リンク: https://github.com/prismalens/sreforge / https://sreforge.sfun.cloud/
- 要約: SREForge は、自律SWE/SREエージェントに中立的なオンコールページを渡し、障害刺激を継続したまま、実際にアラートが消えるかで修正を採点する評価ハーネスです。README は「You cannot bluff a behavioural oracle」と述べ、差分照合ではなく動作上のオラクルを重視しています。
- なぜ面白いか:
  - 技術: ループの成功条件を「それらしい修正」ではなく、継続中の fault に対して観測可能なシステム状態が改善することに置いています。
  - 人文: 実践知の観点では、これは現場のSREが持つ「本当に直ったのか」という慎重さを機械化する試みです。哲学的には、真理を言明の整合性ではなく、環境への介入が耐えるかどうかで見るプラグマティズム的な検証観に近いです。

### 3. LangGraph PSE: generate → programmatically verify → auto-fix を状態グラフにする
- 出典: GitHub
- 日付: GitHub更新 2026-08-09
- リンク: https://github.com/erishen/langgraph-pse
- 要約: LangGraph PSE は、Planner、Specialist、Evaluator の分業により、生成、プログラム的検証、自動修正を明示的な state graph と conditional edges で表すマルチエージェントフレームワークです。タスクごとの検証関数を差し替えれば、中心のグラフを変えずに generate-verify-fix の型を再利用できます。
- なぜ面白いか:
  - 技術: ループを暗黙の会話履歴ではなく、分岐条件と検証関数を持つ状態機械として実装しています。
  - 人文: 認識論的には、判断者をモデルの「自己反省」だけに置かず、別の役割・別の手続き・別の証拠へ分散している点が面白いです。これは職人の反省的実践を、個人の内省ではなく共同作業の型として設計する発想にもつながります。

### 4. Adaptive RAG Agent: 検索品質を自己監査し、弱い証拠では棄権するRAGループ
- 出典: GitHub
- 日付: GitHub更新 2026-08-12
- リンク: https://github.com/Gaurang-gupta/adaptive-rag-agent
- 要約: Adaptive RAG Agent は、通常の retrieve-then-generate ではなく、クエリ監査、検索結果監査、クエリ書き換え、上限付き再試行、引用、自己検証、棄権を組み合わせるローカルファーストなRAG実装です。証拠が弱い場合は、無理に回答せず、知識ベースに十分な根拠がないと明示します。
- なぜ面白いか:
  - 技術: retrieval の失敗を単なる低スコアとして流さず、再検索と停止条件を含む閉ループの品質管理に変えています。
  - 人文: これは「答える能力」よりも「答えてよい条件」を設計する態度です。可謬性を前提にした認識論、つまり知らない時に知らないと言う制度的な謙虚さを、RAGの運用原理へ落としている点が重要です。

### 5. AtlasMind Agent Workbench: 契約業務を証拠、検証、人工復核の作業システムにする
- 出典: GitHub
- 日付: GitHub更新 2026-08-16、設計文書に 2026-08-14 の Agent Harness 移行PRD
- リンク: https://github.com/DayDayUpStudyHard/AtlasMind-Agent-Workbench
- 要約: AtlasMind Agent Workbench は、契約解析、事実抽出、リスク審査、履約核验、人間による復核を、LangGraph v1 と Agent Graph Harness 上の追跡可能な作業システムとしてまとめる中国語プロジェクトです。README は、AIが証拠判断や缺口提示を行っても、最終的な履約結論は人間が確認する境界を明示しています。
- なぜ面白いか:
  - 技術: 契約条項、証拠スナップショット、混合検索、決定論的校验、Checkpoint/Resume、人工終審を多層のループとして接続しています。
  - 人文: 法務・契約の世界では、正しさは単なる生成品質ではなく、引用、責任、確認、監査の連鎖で成立します。Loop engineering を哲学的に見ると、ここには「判断を自動化する」のではなく「判断可能性を保つ作業環境を作る」という実践知があります。

## arXiv / 学術

- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — arXiv:2608.00267。2026-07-31公開、2026-08-10更新。長時間 coding agent 評価を Loop engineering として定式化する中心的な論文。
- 本日の arXiv API 直接検索は `429` と timeout が発生し、追加の新規関連論文は本調査時点で確認されませんでした。

## メモ

- X検索: 英語・日本語クエリで実ツール実行を試みましたが、`personal-team-blocked:spending-limit` により取得できませんでした。
- Web検索: Hermes の `web_search` / `web_extract` は Firecrawl 未設定で失敗しました。代替として terminal から GitHub API、README 直接取得、DuckDuckGo lite、arXiv API を試行し、実在確認できた GitHub / arXiv / 公式リンクのみ採用しました。
- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外です。
- 日本語アカウントの扱い: 日本語X検索は実行したものの、X検索ツールのクレジット制限により投稿確認はできませんでした。
- 注意点・誇張リスク: 「Philosophy of Loop Engineering」はまだ定着した学術カテゴリではありません。本稿では、反復、検証、停止条件、証拠、人工境界、作業記録という共通構造を持つ実装・評価プロジェクトを、哲学・認識論・実践知・サイバネティクスの観点から読解しています。

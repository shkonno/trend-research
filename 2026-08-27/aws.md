# AWS トレンド調査 (2026-08-27)

- 調査日: 2026-08-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AWSは「AIエージェントを本番運用するための評価・発見・観測」と、「既存基幹システムを安全にクラウドへ移すための実践」が同時に前進している。

## トップ5

### 1. Evaluate any agent framework with Amazon Bedrock AgentCore Evaluations
- 出典: AWS Machine Learning Blog
- 日付: 2026-08-26
- リンク: https://aws.amazon.com/blogs/machine-learning/evaluate-any-agent-framework-with-amazon-bedrock-agentcore-evaluations/
- 要約: Amazon Bedrock AgentCore Evaluations が、LangGraph、LlamaIndex、OpenAI Agents SDK、Google ADK、Claude Agent SDK、Strands Agents など、利用フレームワークに依存せず OpenTelemetry / OpenInference 系のトレースを読み取り、GoalSuccessRate、Correctness、Helpfulness などでエージェントを評価できることを解説している。評価対象を「呼び出し」「推論」「ツール実行」のスパンとして再構成する設計がポイント。
- なぜ面白いか:
  - 技術: エージェント評価をSDK固有のログ実装から切り離し、標準化されたテレメトリを評価基盤の共通インターフェースにしている。
  - 人文: AIエージェントが業務に入るほど、「賢いか」より「説明でき、監査でき、改善できるか」が組織の信頼の条件になる。評価を後付けの儀式ではなく日常運用の言語にする動きとして重要。

### 2. Agentic Resource Discovery (ARD): An open specification for agent discovery
- 出典: AWS Machine Learning Blog
- 日付: 2026-08-24
- リンク: https://aws.amazon.com/blogs/machine-learning/agentic-resource-discovery-ard-an-open-specification-for-agent-discovery/
- 要約: AWS Agent Registry とオープン仕様 ARD により、組織内のエージェント、ツール、スキルを検索・発見・管理するためのカタログ化を進める発表。エージェントが増えた後の「どこに何があり、誰が使ってよいか」を扱うテーマ。
- なぜ面白いか:
  - 技術: エージェントやツールを実行時リソースとしてだけでなく、発見可能な組織資産として登録・検索する抽象化を提供している。
  - 人文: これは社内の暗黙知や権限関係を、機械が読める目録に変える試みでもある。便利さの裏側で、誰の仕事や知識が「呼び出し可能な部品」として定義されるのかという文化的な問いも生まれる。

### 3. AWS Glue 6.0 now available with 30% lower price and full Apache Iceberg v3 support
- 出典: AWS News Blog / AWS Japan Blog
- 日付: 2026-08-21（英語版）/ 2026-08-25（日本語版）
- リンク: https://aws.amazon.com/blogs/aws/aws-glue-6-0-now-available-with-30-lower-price-and-full-apache-iceberg-v3-support/
- 要約: AWS Glue 6.0 が一般提供され、Apache Spark 4.1、Python 3.13、Scala 2.13 を含むモダンなランタイムに更新され、従来バージョンより30%低価格になった。Apache Iceberg v3 の完全サポートも加わり、レイクハウス運用の現実的なコストと互換性が改善される。
- なぜ面白いか:
  - 技術: ETL/ELT基盤のランタイム刷新、価格低下、Iceberg v3対応が同時に来ており、データレイクの標準テーブル形式への移行を後押しする。
  - 人文: データ基盤の刷新はしばしば「やるべきだが怖い」作業だが、価格と互換性の改善は現場に移行の口実を与える。組織のデータ利用文化は、派手なAI機能だけでなく地味なランタイム更新で変わる。

### 4. MonotaRO が基幹データベースを Amazon Aurora Global Database に移行
- 出典: AWS Japan Blog
- 日付: 2026-08-26
- リンク: https://aws.amazon.com/jp/blogs/news/monotaro-core-database-migration-to-amazon-aurora-global-database/
- 要約: MonotaRO がオンプレミス MySQL の基幹データベースを Aurora MySQL / Aurora Global Database に移行し、大阪リージョンをプライマリ、東京リージョンをセカンダリとするマルチリージョンDRを実現した事例。18台のセルフマネージドレプリカ、論理レプリケーション遅延、MySQL保守期限、手動DRなどの課題に対し、PoC、段階移行、中継機を用いたレプリケーション、AWS Countdown Premium を組み合わせている。
- なぜ面白いか:
  - 技術: ストレージレベルレプリケーション、Aurora Global Database、段階的Read/Write切替により、基幹DB移行のリスクを小さく分割している。
  - 人文: 日本企業の基幹系クラウド移行は、技術よりも「止められない業務をどう納得して動かすか」が核心になる。この事例は、移行を英雄的な一発勝負ではなく、検証・支援・段階的合意の社会的プロセスとして見せている。

### 5. Automated Synthesis of Cloud Emulators
- 出典: arXiv
- 日付: 2026-08-24
- リンク: https://arxiv.org/abs/2608.23842v1
- 要約: DevOpsプログラムやIaCのテストでは、実クラウド資源を用意して検証するコスト・危険・時間が問題になる。本論文は、クラウドAPIやCLIを前提にしたテストのため、クラウドエミュレータを自動合成する方向性を扱っている。
- なぜ面白いか:
  - 技術: AWSを含むクラウド運用コードの検証を、実環境プロビジョニングからエミュレーションへ寄せることで、IaC/DevOpsのテスト容易性を上げる研究潮流を示している。
  - 人文: クラウド運用は「本番で試すしかない」という不安を抱えやすい領域だった。エミュレータ研究は、インフラ担当者の心理的安全性と、失敗から学べる実験文化を支える基盤になり得る。

## arXiv / 学術

- Automated Synthesis of Cloud Emulators — arXiv:2608.23842v1（2026-08-24）: https://arxiv.org/abs/2608.23842v1
- Explainable Adaptive Zero Trust Framework for AWS with Adversarial Robustness Evaluation — arXiv:2608.21477v1（2026-08-21）: https://arxiv.org/abs/2608.21477v1
- Demo: tfdrift - A Severity Taxonomy and Risk Classification Framework for Infrastructure Drift Detection — arXiv:2608.18173v1（2026-08-17）: https://arxiv.org/abs/2608.18173v1

## メモ

- Boris Cherny優先の有無: Claude/Anthropic/Bedrock関連として @bcherny をX検索対象に含めたが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、本調査時点でBoris Cherny由来の確認済み情報は取得できなかった。
- 日本語アカウントの扱い: X検索は日本語クエリでも実行したが同じ理由で失敗。代替としてAWS Japan Blogの日本語記事を優先的に確認し、MonotaROのAurora移行事例とAWS Glue 6.0日本語版を反映した。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）も未設定で利用不可だったため、AWS公式RSS/ブログフィード、AWS Japan Blogフィード、arXiv APIへの直接HTTP取得を主な根拠にした。X上の開発者反応やコミュニティ温度感は未取得のため、ソース制限として明記する。

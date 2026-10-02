# AWS トレンド調査 (2026-10-02)

- 調査日: 2026-10-02
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWS の今週は、クラウド運用・データ基盤・エージェント活用が「人間のレビュー作業をどう減らし、どこに責任を残すか」という一点に収束している。

## トップ5

### 1. AWS Well-Architected Agent がプレビュー公開
- 出典: AWS News Blog / AWS What's New
- 日付: 2026-10-01
- リンク: https://aws.amazon.com/blogs/aws/announcing-aws-well-architected-agent-an-ai-powered-intelligence-to-optimize-your-cloud-environment-preview/
- 要約: AWS Well-Architected Agent は、AWS 環境を分析し、コスト・セキュリティ・性能・信頼性の改善案を、ビジネス目標に沿って優先順位付きで提示する AI サービスとしてプレビュー公開された。Terraform、CDK、CloudFormation などの IaC も分析し、SSM Runbook、CLI、IaC 変更案、コンソール手順など実装可能な修正パッケージを出す点が特徴。
- なぜ面白いか:
  - 技術: Trusted Advisor / Well-Architected Tool 的なチェックリストを、リソース・アプリ・アーキテクチャ横断の推奨と実行可能な修正案に引き上げる、AWS 運用のエージェント化を象徴する発表です。
  - 人文: クラウドアーキテクトの暗黙知が「レビューする人」から「方針を与え、提案を監督する人」へ移る兆しがあります。便利さの一方で、推奨理由・トレードオフ・責任の所在をチームが読める形で残すことが、運用品質の新しい倫理になります。

### 2. Amazon S3 Vectors がメタデータ事前フィルタリングを追加
- 出典: AWS News Blog / AWS What's New
- 日付: 2026-09-30
- リンク: https://aws.amazon.com/blogs/aws/amazon-s3-vectors-now-supports-metadata-pre-filtering-for-higher-recall-on-filtered-searches/
- 要約: Amazon S3 Vectors は、類似検索の前にメタデータ条件を評価する pre-filtering を追加し、フィルタ付き検索の recall を最大5倍改善すると発表された。パスや URL などに使える `$startsWith` も加わり、RAG、エージェント、文書検索で「絞り込み後に関連ベクトルが取りこぼされる」問題を緩和する。
- なぜ面白いか:
  - 技術: ベクトル検索を S3 ネイティブな低コスト・大規模ストレージに寄せつつ、RAG 実装で実際に効く recall とメタデータ条件の問題を直接改善しています。
  - 人文: 生成 AI の回答品質は、モデル単体よりも「どの記憶を取り出すか」に強く左右されます。組織の文脈、権限、文書階層を検索前に尊重できることは、AI が人間の情報秩序を壊さずに参加するための基礎になります。

### 3. Aurora PostgreSQL が Iceberg / Parquet データレイクへの直接クエリをサポート
- 出典: AWS News Blog / AWS What's New / AWS Japan Blog
- 日付: 2026-09-30
- リンク: https://aws.amazon.com/blogs/aws/amazon-aurora-postgresql-now-supports-direct-querying-of-apache-iceberg-and-parquet-data-in-your-data-lake/
- 要約: Aurora PostgreSQL から、S3、S3 Tables、AWS Glue Data Catalog 上の Apache Iceberg / Parquet データを ETL なしで直接クエリできるようになった。Aurora 内に DuckDB の高性能クエリエンジンを組み込み、PostgreSQL の外部テーブルとして運用データとデータレイクを同一 SQL で扱える。
- なぜ面白いか:
  - 技術: OLTP 側の PostgreSQL とデータレイク側の Iceberg / Parquet を、データ複製ではなくクエリエンジン統合で近づける実用的な Lakehouse 化です。
  - 人文: データ基盤の分断は、部門ごとの解釈の分断にもつながります。アプリ担当と分析担当が同じ SQL インターフェースで歴史データと現在データを見られることは、組織内の「事実の置き場所」を再設計する動きでもあります。

### 4. Kiro ベースの SAP モダナイゼーション事例が日本語で詳説
- 出典: AWS Japan Blog
- 日付: 2026-10-01
- リンク: https://aws.amazon.com/jp/blogs/news/accelerate-your-sap-modernization-with-kiro-benchmarks-and-use-cases/
- 要約: Kiro ベースのサンプルエージェントを使い、SAP ECC の ABAP コード88オブジェクトを4.5時間で SAP S/4HANA 準拠に変換し工数を87%削減、SAP PI/PO から SAP BTP Integration Suite への移行や SAP BW から SAP Datasphere への変換も扱う事例が公開された。依存コード取得、ステアリングファイル、単体テスト、意思決定ログなど、正確性と監査可能性のセーフガードも強調されている。
- なぜ面白いか:
  - 技術: 単なるコード生成ではなく、レガシー ERP の仕様抽出、変換、テスト、判断ログまで含むエージェント型モダナイゼーションの実務パターンが示されています。
  - 人文: SAP 移行のような巨大で心理的負荷の高い作業では、AI は「速く書く道具」よりも「組織の古い知識を安全に翻訳する媒介」になります。日本語で詳細に共有された点も、日本の基幹系コミュニティにとって受け取りやすい材料です。

### 5. Bedrock AgentCore によるクラウド移行のマルチエージェント実装
- 出典: AWS Machine Learning Blog
- 日付: 2026-10-01
- リンク: https://aws.amazon.com/blogs/machine-learning/scaling-cloud-migrations-with-agentic-ai-on-amazon-bedrock-agentcore/
- 要約: AWS Professional Services が、Amazon Bedrock AgentCore と Strands Agents SDK、MCP ツールを使い、クラウド移行を支援する4エージェント構成を紹介した。Intake、IaC、Migration Intelligence and Governance、SRE の各エージェントが、移行入力の収集、IaC 生成、ポートフォリオ管理、移行後運用を分担し、IaC 作成時間をアプリごとに数週間から数分へ短縮したと説明している。
- なぜ面白いか:
  - 技術: Bedrock AgentCore、MCP、Strands Agents SDK を組み合わせ、移行プログラムを「単一万能エージェント」ではなく職能分割されたマルチエージェントとして設計している点が実践的です。
  - 人文: 大規模移行は技術課題であると同時に、部署・台帳・責任者・期限が絡む社会的プロジェクトです。エージェントを役割ごとに分ける設計は、人間の組織構造を模倣しながら自動化を受け入れやすくする工夫として読めます。

## arXiv / 学術
- 本調査時点で確認されませんでした。
- 補足: arXiv API と arXiv 検索ページに対して `Amazon Bedrock`、`Amazon Web Services`、`AWS Lambda`、`Amazon S3 Vectors` などで確認を試みましたが、API はタイムアウトまたは 429、検索ページは該当なしまたは 429 でした。確認できた範囲では、直近約14日の AWS 固有の有力 arXiv 論文は採用対象にありませんでした。

## メモ
- Boris Cherny優先の有無: Claude / Anthropic / Bedrock 関連として Boris Cherny 情報の確認を X 検索で試みましたが、X 検索ツールは `personal-team-blocked:spending-limit` により利用できませんでした。そのため本日の AWS トップ5は、AWS 公式 RSS、AWS News Blog、AWS Japan Blog、AWS Machine Learning Blog、AWS What's New の直接取得を主な根拠にしています。
- 日本語アカウントの扱い: X 検索が同じ理由で失敗したため、日本語開発者コミュニティの X 投稿は確認できませんでした。代替として AWS Japan Blog の日本語記事を含め、特に Kiro / SAP モダナイゼーションの日本語実務共有を採用しました。
- 注意点・誇張リスク: Web 検索ツールも Firecrawl 未設定で失敗したため、一般 Web の第三者記事や X 上の反応は限定的です。AWS 公式発表は一次情報として信頼できますが、効果値やベンチマークは各記事の条件に依存するため、実環境への適用時はワークロード、権限設計、監査要件、コストを個別に検証してください。

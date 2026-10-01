# AWS トレンド調査 (2026-10-01)

- 調査日: 2026-10-01
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWSは「AIエージェントを動かす基盤」から「エージェントを観測・統制し、既存業務へ接続する基盤」へ、かなり実務寄りに重心が移っています。

## トップ5

### 1. Introducing Claude Sonnet 5.5 on AWS
- 出典: AWS Machine Learning Blog
- 日付: 2026-09-28
- リンク: https://aws.amazon.com/blogs/machine-learning/introducing-claude-sonnet-5-5-on-aws/
- 要約: Claude Sonnet 5.5 が Amazon Bedrock および Claude Platform on AWS で利用可能になりました。AWS公式フィードでは、コーディングや知識作業向けに、より高速・低コストなSonnetモデルとして紹介されています。
- なぜ面白いか:
  - 技術: Bedrock上でAnthropic系モデルの選択肢が増えることで、企業は推論品質・速度・コスト・データ処理リージョンの制約を比較しながらモデルルーティングしやすくなります。
  - 人文: 「どのAIが一番賢いか」ではなく「この仕事にはどのAIを割り当てるか」という労働編成の問題に近づいています。開発者の判断は、コードを書く力だけでなく、モデルの性格・費用・説明責任を読む編集者的な能力へ広がります。

### 2. Amazon S3 Vectors now supports metadata pre-filtering for higher recall on filtered searches
- 出典: AWS News Blog / AWS What's New
- 日付: 2026-09-30
- リンク: https://aws.amazon.com/blogs/aws/amazon-s3-vectors-now-supports-metadata-pre-filtering-for-higher-recall-on-filtered-searches/
- 要約: Amazon S3 Vectors がメタデータの事前フィルタリングに対応し、選択的なフィルタ条件を使う検索で最大5倍高いリコールを得られると発表されました。RAG、エージェント、文書検索のように「対象範囲を絞ってから類似検索したい」用途に効きます。
- なぜ面白いか:
  - 技術: 類似検索の前にメタデータ条件を評価できるため、権限・部門・顧客・日付などでスコープされた検索の精度と再現性を上げやすくなります。
  - 人文: RAGの失敗はしばしば「知らない」より「関係ないものを混ぜて語る」ことから起きます。検索前の境界設定が強くなることは、AIに文脈の礼儀や守秘の境界を教える社会的インフラとしても重要です。

### 3. Introducing Amazon CloudWatch Omni: AI-powered observability for generative AI and agentic workloads
- 出典: AWS News Blog
- 日付: 2026-09-22
- リンク: https://aws.amazon.com/blogs/aws/introducing-amazon-cloudwatch-omni-ai-powered-observability-for-generative-ai-and-agentic-workloads/
- 要約: CloudWatch Omni は、生成AIおよびエージェントワークロード向けのAIファーストなオブザーバビリティとして発表されました。AWS公式フィードでは、エージェントのトレース、評価、実験、AIガイド付き調査をIDEやWeb体験から扱えるものとして説明されています。
- なぜ面白いか:
  - 技術: 従来のCPU・ログ・メトリクス中心の監視から、エージェントの推論過程、ツール呼び出し、評価結果までを運用品質の対象に引き上げています。
  - 人文: エージェントは「動いたか」だけでなく「なぜそう判断したか」が問われるソフトウェアです。観測可能性の進化は、AIを同僚や委任先として扱う組織にとって、信頼の記録簿を作る試みと言えます。

### 4. Amazon Aurora PostgreSQL now supports direct querying of Apache Iceberg and Parquet data in your data lake
- 出典: AWS News Blog / AWS Japan Blog
- 日付: 2026-09-30
- リンク: https://aws.amazon.com/blogs/aws/amazon-aurora-postgresql-now-supports-direct-querying-of-apache-iceberg-and-parquet-data-in-your-data-lake/
- 要約: Amazon Aurora PostgreSQL から、データレイク上の Apache Iceberg と Parquet データを直接クエリできるようになりました。AWS Japan Blog でも日本語で紹介されており、DuckDB が Aurora PostgreSQL に組み込まれ、ETLなしで運用データと分析データを横断できる点が強調されています。
- なぜ面白いか:
  - 技術: トランザクショナルDBとデータレイクのあいだにあるETL・複製・鮮度管理の負担を下げ、PostgreSQLアプリや既存SQLから湖側のデータを扱いやすくします。
  - 人文: データ基盤の歴史は、業務の現場と分析の現場を分けたりつないだりする歴史でもあります。境界が薄くなるほど、組織は「誰が正しいデータを持っているのか」ではなく「誰がどの文脈で読むのか」を設計する必要が出てきます。

### 5. REST API を Amazon Bedrock AgentCore Gateway で MCP サーバー化する ― オリックス「PATPOST」での取り組み
- 出典: AWS Japan Blog
- 日付: 2026-10-01
- リンク: https://aws.amazon.com/jp/blogs/news/agentcore-gateway-patpost/
- 要約: オリックスのSaaS「PATPOST」において、既存REST APIを Amazon Bedrock AgentCore Gateway で MCP サーバー化した取り組みが紹介されました。既存資産に大きく手を入れず、エージェントから業務APIを扱えるようにする日本語の実践事例です。
- なぜ面白いか:
  - 技術: REST APIをMCPサーバーとして公開することで、既存業務システムをエージェントのツール呼び出し先へ変換し、AgentCore中心のワークフローに接続しやすくなります。
  - 人文: 企業AI導入の本丸は、派手なデモではなく、すでに動いている業務システムと人間の手順をどう壊さず接続するかです。日本企業の具体例は、AIエージェントが「外来の魔法」ではなく、現場の既存文脈に翻訳されていく過程として読めます。

## arXiv / 学術
- 関連候補として、AWS環境やクラウド上のエージェント安全性に触れる論文が確認されました。
  - 「Coding Agents Aren't Enough! Evaluating an Enterprise Security Brain for Agentic Cloud Investigations」 arXiv:2609.30345（2026-09-28付近、検索結果上はAWS環境での調査タスクを含む）: https://arxiv.org/abs/2609.30345
  - 「Hard Stop: Kernel-Level Preemption and Containment for Rogue Agentic Execution」 arXiv:2609.29808（2026-09-24、検索結果上はAWS EC2 IMDSやKubernetes権限に触れる）: https://arxiv.org/abs/2609.29808
- Amazon Bedrockそのものを主題にした直近約14日のarXiv論文は、本調査時点で確認されませんでした。

## メモ
- Boris Cherny優先の有無: Claude/Anthropic/Bedrock関連としてX検索で @bcherny を優先確認しようとしましたが、x_search はクレジット/サブスクリプション制限で失敗しました。そのため本ファイルではBoris Cherny由来の未確認情報は採用していません。
- 日本語アカウントの扱い: X検索は同じ制限で利用できませんでした。代替としてAWS Japan BlogとQiita APIを確認し、日本語コミュニティ由来の実践例としてAgentCore Gateway / PATPOST事例をトップ5に含めました。
- 注意点・誇張リスク: Web検索ツールも未設定で利用できなかったため、主にAWS公式RSS、AWS公式ブログHTML、Qiita API、arXiv検索ページを直接取得して確認しました。AWS公式発表は製品紹介色が強いため、性能値や効果は各ワークロードでの検証が必要です。

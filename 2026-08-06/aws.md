# AWS トレンド調査 (2026-08-06)

- 調査日: 2026-08-06
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWSの今週は、生成AIエージェントを「実験」から「業務システムの常設部品」へ移すための、データ基盤・推論の接地・運用権限・サーバーレス性能が同時に進んだ週です。

## トップ5

### 1. Amazon DynamoDB now supports real-time vector search at any scale
- 出典: AWS News Blog / AWS What's New
- 日付: 2026-08-05
- リンク: https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale/
- 要約: DynamoDBがネイティブなリアルタイム・ベクトル検索を一般提供し、単一桁ミリ秒レイテンシ、99%以上のリコール、最大で兆単位のベクトル規模をうたっています。運用データと意味検索を同じDynamoDB上で扱えるため、別ベクトルDBを立てる構成を減らせます。
- なぜ面白いか:
  - 技術: 低レイテンシのキー・バリュー/ドキュメントDBにベクトル索引が入ることで、RAGや推薦、エージェント記憶のホットパス設計が大きく単純化します。
  - 人文: 「記憶」を専用の実験的ストアではなく、既存の業務台帳に隣接させる動きは、AIが組織の日常業務に埋め込まれていく象徴です。検索の意味が、データベース管理者だけでなく業務担当者の知識編成にも近づきます。

### 2. Introducing Web Search on Amazon Bedrock for foundation model grounding
- 出典: AWS Machine Learning Blog / AWS What's New
- 日付: 2026-08-04
- リンク: https://aws.amazon.com/blogs/machine-learning/introducing-web-search-on-amazon-bedrock-for-foundation-model-grounding/
- 要約: Amazon BedrockでWeb Searchが一般提供され、サーバーサイドの組み込みツールとしてモデル応答を最新Web情報でグラウンディングできるようになりました。What's NewではOpenAI GPT-5.4、GPT-5.5、GPT-5.6系モデル向けの提供として告知されています。
- なぜ面白いか:
  - 技術: 検索・取得・引用の接地をアプリ側で寄せ集めるのではなく、Bedrockの推論面に近いところで扱えるため、エージェントの現在性と監査性を実装しやすくなります。
  - 人文: AIの「知っているふり」を減らすには、能力そのものよりも情報源との関係を制度化する必要があります。クラウド基盤が検索を内蔵することは、知識の鮮度と責任の所在をプロダクト設計の中心に置く変化です。

### 3. How we built an MCP bridge to give our AgentCore-hosted AI agent access to local MCP tools
- 出典: AWS Machine Learning Blog
- 日付: 2026-08-05
- リンク: https://aws.amazon.com/blogs/machine-learning/how-we-built-an-mcp-bridge-to-give-our-agentcore-hosted-ai-agent-access-to-local-mcp-tools/
- 要約: Amazon Bedrock AgentCore上のクラウドホスト型AIエージェントから、ユーザーのローカルMCPツールやファイルへ安全にアクセスするためのMCPブリッジ構成が紹介されています。署名付きトンネルを使い、クラウド側のエージェントと手元の開発環境の境界をまたぐ設計です。
- なぜ面白いか:
  - 技術: AgentCore、MCP、署名付き接続を組み合わせることで、クラウド実行の統制とローカル文脈へのアクセスを両立するエージェント・アーキテクチャが見えてきます。
  - 人文: エージェントが「どこで働くのか」という問題は、単なるネットワーク設計ではなく、個人の作業机と企業クラウドの境界をどう引くかという問題です。便利さと私的空間の保護の折り合いが、実装パターンとして問われています。

### 4. AWS Lambda announces scalable network bandwidth up to 3,000 Mbps for functions outside a VPC
- 出典: AWS What's New
- 日付: 2026-08-05
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/aws-lambda-network-bandwidth/
- 要約: VPC外のLambda関数で、実行環境あたり最大3,000 Mbpsまでスケールするネットワーク帯域が告知されました。レイテンシや大容量データ転送に敏感なサーバーレス処理で、従来よりネットワークがボトルネックになりにくくなります。
- なぜ面白いか:
  - 技術: サーバーレスが軽量イベント処理だけでなく、データ転送量の多いAI/ETL/メディア処理にも広がるための実用的な性能改善です。
  - 人文: インフラの制約が見えなくなるほど、開発者は「関数」という小さな抽象で大きな仕事を任せるようになります。その一方で、見えない帯域の消費とコストをどう共有して理解するかがチーム運用の課題になります。

### 5. 1つのエージェントで、あらゆるクライアントに: Kiro エージェントハーネスをどう構築したか
- 出典: Amazon Web Services ブログ（日本語）
- 日付: 2026-08-05
- リンク: https://aws.amazon.com/jp/blogs/news/one-agent/
- 要約: Kiro IDE、CLI、Webに分かれていたエージェントを、単一のKiroエージェントハーネスへ統合した設計が日本語で解説されています。Agent Client Protocol、WebSocketトランスポート、Kiro-ACP拡張、Cedarベースのケイパビリティ権限モデルを組み合わせ、仕様駆動開発やカスタムエージェント、フックをクライアント横断で一貫提供する内容です。
- なぜ面白いか:
  - 技術: IDE/CLI/Webをまたぐ同一エージェント実行基盤と権限モデルは、開発者体験とガバナンスを同時に設計する上で重要な参照実装になります。
  - 人文: 日本語コミュニティ向けにこのレベルの内部設計が共有されている点が重要です。エージェントは単独のチャットUIではなく、職場の道具・手順・権限関係を横断する「同僚」のような存在になりつつあります。

## arXiv / 学術
- 関連論文として、`FedCritic-MIMO: Communication-Efficient Serverless Federated Critic Learning for Massive-MIMO Resource Control in Open and Disaggregated 6G RANs`（arXiv:2608.03852、2026-08-04、https://arxiv.org/abs/2608.03852v1）を確認しました。AWS固有ではありませんが、中央集約サーバーなしのserverless federated learning設計を扱っており、クラウド/エッジ分散AI基盤の文脈で参考になります。
- AWS Lambdaに直接言及する直近約14日の新規arXiv論文は、本調査時点の検索では確認されませんでした。直近で見つかったAWS Lambda関連は `Overprivilege Analysis of Security Policies in Serverless Cloud Applications`（arXiv:2607.02875、2026-07-03、https://arxiv.org/abs/2607.02875v1）で、対象期間外ですがサーバーレス権限過多のリスク分析として継続的に関連します。

## メモ
- Boris Cherny優先の有無: Claude/Anthropic/Bedrock関連の確認として `@bcherny` を含むX検索を試行しましたが、X検索ツールがクレジット/購読制限で失敗したため、今回のBoris Cherny由来の新規情報は確認できませんでした。
- 日本語アカウントの扱い: X検索は同じ制限で利用できませんでしたが、日本語AWS公式ブログからKiroエージェントハーネス記事、Kiro Crew、Claude・Kiro実践ワークショップ記事などを確認し、日本語開発者コミュニティへの波及が最も強い項目としてKiroエージェントハーネスをトップ5に入れました。
- 注意点・誇張リスク: Web検索ツールも未設定で利用できなかったため、AWS公式RSS/ブログ/What's NewとarXiv APIを直接HTTP取得して調査しました。今回のランキングは公式発表中心で、X上の反応量や第三者評価は十分に反映できていません。

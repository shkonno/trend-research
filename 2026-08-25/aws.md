# AWS トレンド調査 (2026-08-25)

- 調査日: 2026-08-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

今週のAWSは、Bedrock/AgentCoreを中心に「企業内エージェントを安全に運用するための部品」が一気に実装段階へ進み、同時にGlue・EKS・S3など基盤サービスにも地味だが運用品質を上げる更新が続いた。

## トップ5

### 1. Amazon Bedrock AgentCore Web Searchがドメイン・公開日フィルタと外部Webアクセスを拡張

- 出典: AWS What’s New / AWS Machine Learning Blog / AWS Japan Blog
- 日付: 2026-08-19〜2026-08-24
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/web-search-amazon-bedrock/
- 関連リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-web-access-web-search/ / https://aws.amazon.com/blogs/machine-learning/domain-and-publish-date-filters-for-web-search-on-agentcore/ / https://aws.amazon.com/jp/blogs/news/weekly-genai-20260817/
- 要約: Amazon Bedrock AgentCoreのWeb Searchに、検索対象ドメインと公開日のフィルタが追加され、エージェントが参照するWeb情報の範囲と鮮度をリクエスト単位で制御できるようになった。日本語の週刊生成AI with AWSでは、AgentCore Web Searchの東京リージョン対応もサービスアップデートとして取り上げられている。
- なぜ面白いか:
  - 技術: RAGやエージェントの外部検索を「ただWebに出す」のではなく、許可ドメイン・期間・リージョンをサーバー側で統制できる点が、企業導入の現実的な要件に合っている。
  - 人文: エージェントが何を「知識」として採用するかは、単なる検索品質ではなく組織の信頼・説明責任・情報統治の問題になっている。検索の自由度を高めながら境界線を引く設計は、AIを同僚として扱うときの社会的なルール作りそのものに近い。

### 2. Agentic Resource Discovery（ARD）とAWS Agent Registryでエージェント発見の標準化へ

- 出典: AWS Machine Learning Blog
- 日付: 2026-08-24
- リンク: https://aws.amazon.com/blogs/machine-learning/agentic-resource-discovery-ard-an-open-specification-for-agent-discovery/
- 要約: AWSは、組織内のエージェント、ツール、スキルを発見・管理するためのオープン仕様Agentic Resource Discovery（ARD）と、AWS Agent Registryの使い方を紹介した。複数環境・複数フレームワークに散らばるエージェント資産を、検索可能なカタログとガバナンスの対象として扱う流れが見える。
- なぜ面白いか:
  - 技術: MCP的な接続性の次の課題である「どのエージェントやツールが存在し、誰が使ってよいのか」を、レジストリと標準仕様で解こうとしている。
  - 人文: 企業内AIは個人の便利ツールから、組織の職能・権限・責任を写し取る制度的インフラへ変わりつつある。人間の職務カタログと同じように、AIエージェントにも名簿・資格・利用条件が必要になるという変化が象徴的だ。

### 3. Amazon Bedrock AgentCore Gatewayでエージェントのツールアクセスを統治する実践パターン

- 出典: AWS Machine Learning Blog
- 日付: 2026-08-21
- リンク: https://aws.amazon.com/blogs/machine-learning/govern-ai-agent-tool-access-with-amazon-bedrock-agentcore-gateway/
- 要約: AWSは、Amazon Bedrock AgentCore Gatewayを使ってAIエージェントの企業ツール接続を段階的に成熟させる「Connect / Control / Catalog / Harden」の4段階モデルを提示した。ツール統合を一気に中央集権化するのではなく、監査可能性と統制を段階的に高める考え方が実務的である。
- なぜ面白いか:
  - 技術: エージェントの実行能力をMCPやAPI接続で広げる一方、認可・監査・カタログ化・ハードニングをゲートウェイ層で扱う設計が、運用事故を減らす鍵になる。
  - 人文: AIに道具を持たせることは、組織内で「誰に何を任せるか」を再設計することでもある。便利さだけを追うと権限の暴走が起きるため、自由と統制の折り合いをどうつけるかが文化的な課題になる。

### 4. AWS Glue 6.0が30%値下げ、Apache Iceberg v3、Spark 4.1、Python 3.13に対応

- 出典: AWS News Blog / AWS What’s New
- 日付: 2026-08-21
- リンク: https://aws.amazon.com/blogs/aws/aws-glue-6-0-now-available-with-30-lower-price-and-full-apache-iceberg-v3-support/
- 関連リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/aws-glue-6-0-price-reduction-iceberg-v3
- 要約: AWS Glue 6.0が一般提供され、前世代比30%低い料金、Apache Iceberg v3のフルサポート、Apache Spark 4.1、Python 3.13、Scala 2.13などの新しいランタイムが導入された。生成AIが注目を集める一方で、データレイクハウスの基盤コストと互換性を改善する重要な更新である。
- なぜ面白いか:
  - 技術: Iceberg v3と新ランタイムへの対応により、分析基盤のオープンテーブルフォーマット化とETL実行コスト削減を同時に進めやすくなる。
  - 人文: AI時代の「知能」は、モデルだけでなく、日々整えられるデータの労働に依存している。Glueのような地味な更新は、見えにくいデータ整備の仕事をどれだけ持続可能にするかという組織文化の問題につながる。

### 5. EKSが複数OIDCプロバイダー、CAローテーション、Argo CD設定など運用統制を強化

- 出典: AWS What’s New
- 日付: 2026-08-20〜2026-08-24
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-eks-multiple-oidc-providers
- 関連リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-eks-certificate-authority-ca-rotation-automated-lifecycle-management / https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-eks-argo-cd-configuration / https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-eks-control-plane-configuration-parameters
- 要約: Amazon EKSは、1クラスターあたり最大10件の外部OIDC IDプロバイダー対応、証明書認証局（CA）ローテーションの自動ライフサイクル管理、Argo CDのカスタム設定、Kubernetesコントロールプレーンの高度な設定パラメータなどを追加した。派手な新機能ではないが、複数チーム・複数ID基盤でKubernetesを運用する企業には大きい。
- なぜ面白いか:
  - 技術: ID連携、証明書ローテーション、GitOps、制御プレーン調整がマネージドに近づくことで、EKS運用のセキュリティ負債と手作業リスクを下げられる。
  - 人文: Kubernetes運用はしばしば「専門家だけが触れる聖域」になりがちだが、こうした統制機能はチーム間の信頼と権限委譲を進める。クラウド基盤の成熟とは、人が安心して任せ合える制度を増やすことでもある。

## arXiv / 学術

- 直近約14日でAWSそのもの、Amazon Bedrock、Bedrock AgentCoreに直接関係する新規arXiv論文は、本調査時点で確認されませんでした。
- 参考として、期間外だが関連性のある既存論文は確認しました: 「Registry-Governed Agent Lifecycle: Completing EDDOps with Evaluation-Driven Registration, Promotion, and Retirement on AWS AgentCore」 arXiv:2607.00345（2026-07-01） https://arxiv.org/abs/2607.00345 。AgentCore上でのレジストリ管理・評価駆動の昇格/廃止ライフサイクルを扱っており、今週のARD/Agent Registry/Gatewayの流れと近い問題意識です。

## メモ

- Boris Cherny優先の有無: Claude/Anthropic/Bedrock関連としてBoris Cherny（@bcherny）情報を優先確認するためX検索を実行しましたが、x_searchはクレジット/サブスクリプション制限で失敗しました。そのため本ファイルではBoris由来の未確認情報は採用していません。
- 日本語アカウントの扱い: X検索は同じ制限により取得できませんでした。代替としてAWS Japan Blogの日本語記事・週刊生成AI with AWSを確認し、日本語コミュニティ向けの実務文脈（東京/大阪リージョン、行政ガイドライン、国内事例）を反映しました。
- 注意点・誇張リスク: Web検索ツールも未設定だったため、AWS公式RSS/ブログ、AWS What’s New、arXiv APIを直接HTTP取得して確認しました。X上の反応や非公式コミュニティの温度感は限定的であり、本日のランキングは「公式発表から見た実務インパクト」寄りです。

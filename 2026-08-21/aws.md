# AWS トレンド調査 (2026-08-21)

- 調査日: 2026-08-21
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWSは「生成AIエージェントを実験から本番運用へ移すための足場」を、検索・決済・永続実行・データ基盤・運用保守の各レイヤーで急速に埋めている。

## トップ5

### 1. Web Search on Amazon Bedrock が外部Webアクセスに対応
- 出典: AWS What’s New
- 日付: 2026-08-19
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-web-access-web-search/
- 要約: Amazon Bedrock の Web Search が `external_web_access` パラメータに対応し、公開Webから直接コンテンツを取得して、より最新の情報でモデル応答をグラウンディングできるようになった。機密性が高い用途では `external_web_access: false` にすることで、AWS境界内のインデックスとナレッジグラフに限定できる。
- なぜ面白いか:
  - 技術: IAM権限 `bedrock-websearch:ExternalWebAccess` とリクエスト単位の外部アクセス制御により、「鮮度」と「データ境界」を同じAPIで切り替えられる。
  - 人文: エージェントが「いまのWeb」を読みに行くことは、便利さと同時に組織の情報倫理を問う。外部へ出るか閉じるかを明示的に選ばせる設計は、AI利用における信頼の責任をユーザー企業側に可視化する。

### 2. Bedrock AgentCore Web Search にドメイン・公開日フィルタ、東京リージョン展開
- 出典: AWS What’s New / AWS Machine Learning Blog
- 日付: 2026-08-19
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/web-search-amazon-bedrock/
- 要約: Amazon Bedrock AgentCore の Web Search が、ドメインフィルタと公開日フィルタをリクエスト単位で指定できるようになった。あわせて Europe (Ireland) と Asia Pacific (Tokyo) に拡大し、日本のワークロードから近いリージョンで利用しやすくなった。
- なぜ面白いか:
  - 技術: 信頼ドメインへの限定、不要ドメインの除外、日付範囲指定をサーバー側で強制できるため、エージェントの検索結果品質を外部オーケストレーションなしで制御できる。
  - 人文: 「AIがどの資料を根拠に語ったのか」は、組織内の説明責任そのものになりつつある。東京リージョン対応は、日本語業務・規制・データ近接性を気にする現場にとって、エージェント導入の心理的障壁を下げる。

### 3. Amazon Bedrock AgentCore payments が一般提供開始
- 出典: AWS Machine Learning Blog
- 日付: 2026-08-18
- リンク: https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale/
- 要約: Amazon Bedrock AgentCore payments がGAとなり、AIエージェントが少額・従量課金型のサービス利用料を自律的に支払える仕組みを提供する。Coinbase と Stripe Privy のウォレット連携、支出ガードレール、x402 と Machine Payment Protocol (MPP) への対応、観測性を備える。
- なぜ面白いか:
  - 技術: エージェントのツール利用を「API呼び出し」だけでなく「支払い可能な実行単位」へ拡張し、MCPサーバー経由で有料エンドポイントを発見・選択できる。
  - 人文: 機械が財布を持つと、代理行為・委任・浪費・責任の境界が一気に現実問題になる。支出上限や委任同意の設計は、AIエージェント経済の倫理的インフラとして重要だ。

### 4. Amazon Bedrock AgentCore Runtime に永続的な runtime instances
- 出典: AWS News Blog
- 日付: 2026-08-06（直近14日よりやや古いが重要）
- リンク: https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore/
- 要約: Bedrock AgentCore Runtime に runtime instances が追加され、複雑な本番エージェント向けに、永続的なAWS管理EC2基盤を使えるようになった。複数エージェントの同一ランタイム展開、最大14日持続する共有セッション、GPU対応、停止・再開によるコスト抑制、コンテナ化デプロイを提供する。
- なぜ面白いか:
  - 技術: 従来のマイクロVM実行だけでは難しい、長時間状態保持・マルチエージェント協調・GPU処理を、AgentCoreのID制御や観測性と統合して扱える。
  - 人文: エージェントは「単発のチャット」から「数日間働く同僚」に近づいている。永続セッションは便利だが、記憶・中断・再開が人間のワークフローにどう溶け込むかという組織文化の問題も生む。

### 5. Amazon DynamoDB がリアルタイムベクトル検索をGA
- 出典: AWS News Blog
- 日付: 2026-08-05（直近14日よりやや古いが重要）
- リンク: https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale/
- 要約: DynamoDB がネイティブなベクトル検索を一般提供し、運用データと埋め込みを同じテーブルに保存したまま類似検索できるようになった。単桁ミリ秒レイテンシ、99%以上のリコール、トリリオン規模のベクトル、サーバーレス運用をうたう。
- なぜ面白いか:
  - 技術: 別のベクトルDBへ同期するパイプラインを減らし、RAG、エージェント記憶、推薦、異常検知をDynamoDBの既存運用モデル上に載せやすくする。
  - 人文: AIシステムの「記憶」が特別な研究基盤ではなく、日常的な業務DBの中に入ってくる流れを示している。これは開発者にとって便利である一方、何を長期記憶として残すべきかという情報ガバナンスの問いを強める。

## arXiv / 学術
- 関連する周辺研究は確認されました。特に `Demo: tfdrift - A Severity Taxonomy and Risk Classification Framework for Infrastructure Drift Detection`（arXiv:2608.18173、2026-08-17、https://arxiv.org/abs/2608.18173v1）は、TerraformなどIaCのドリフトをリスク分類する研究で、AWS運用・ガバナンス文脈に近いです。
- `Large-scale workflow placement in serverless computing using integer nonlinear programming`（arXiv:2608.14427、2026-08-14、https://arxiv.org/abs/2608.14427v1）は、サーバーレス・エッジ環境での大規模ワークフロー配置を扱い、Lambda/分散実行の設計論に接続します。
- `A Barrier-Free Synchronization Algorithm for Multi-Engine AI Accelerators`（arXiv:2608.13757、2026-08-13、https://arxiv.org/abs/2608.13757v1）は、AWS Trainium を含むマルチエンジンAIアクセラレータの同期問題を扱う研究として関連します。

## メモ
- X検索は英語・日本語・Boris Cherny関連で実行しましたが、xAI/X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、X由来の投稿内容は採用していません。架空のX投稿は補いませんでした。
- Web検索ツール（Firecrawl）は未設定でしたが、AWS公式RSS、AWS公式ページの直接HTTP取得、arXiv APIで代替調査しました。
- Claude/Anthropic/Bedrock関連ではBoris Cherny情報を優先確認する指定に従い検索を試みましたが、X検索が利用不能で、今回の採用情報はAWS公式発表に限定しています。
- 日本語コミュニティについてはAWS Japan公式ブログRSSを確認し、2026-08-20の「AI コーディングエージェントのチーム展開に向けた段階的な環境整備の実践例」（https://aws.amazon.com/jp/blogs/news/scaling-ai-coding-agents-across-teams/）を確認しました。トップ5は新サービスリリース中心というフィードバックを優先し、上記5件を選定しました。
- 注意点: 2026-08-21時点のAWS公式RSS/公式ページに基づく選定です。X・一般Web検索の網羅性には上記制限があります。

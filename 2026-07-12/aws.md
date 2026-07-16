# AWS トレンド調査 (2026-07-12)

- 調査日: 2026-07-12
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWS の今週は、AI エージェントを既存の IAM・OAuth・運用統制に接続する「実務化」と、基盤性能・セキュリティを地味に底上げする発表が同時に進んでいます。

## トップ5

### 1. OAuth support for the AWS MCP Server
- 出典: AWS What’s New
- 日付: 2026-07-09
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/oauth-aws-mcp-server/
- 要約: AWS MCP Server が AWS Sign-In による OAuth 接続をサポートし、AI エージェントが追加の認証ソフトなしに AWS へ接続できるようになりました。既存の AWS ID、IAM 権限、ガバナンスを引き継ぎつつ、ブラウザ経由またはヘッドレス認可でエージェントを運用できます。
- なぜ面白いか:
  - 技術: MCP、OAuth、IAM 条件キー、トークン検証がつながり、エージェントの「ローカル実験」から「統制された業務導入」への距離がかなり縮まります。
  - 人文: AI エージェントの普及で重要になるのは賢さだけでなく、誰が・何に・どこまで委任したのかを組織が説明できることです。これはエージェントを社会的な責任主体に近づける、制度設計寄りのアップデートです。

### 2. Introducing Claude apps gateway for AWS
- 出典: AWS Machine Learning Blog
- 日付: 2026-07-08
- リンク: https://aws.amazon.com/blogs/machine-learning/introducing-claude-apps-gateway-for-aws/
- 要約: Claude Code と Claude Desktop の利用を、Amazon Bedrock と Claude Apps API の間で制御するセルフホスト型ゲートウェイとして提供する発表です。組織は Claude 系アプリのアクセス、コスト、ポリシーを AWS 側で一元的に扱いやすくなります。
- なぜ面白いか:
  - 技術: Claude クライアントをそのまま使いながら、Bedrock 経由のモデル利用、監査、統制を組み込めるため、開発者体験とエンタープライズ管理の折衷点になります。
  - 人文: 生成 AI ツールは個人の創造性を増幅する一方で、企業では「自由に使えること」と「責任を持って使えること」の緊張が常にあります。このゲートウェイは、その緊張を禁止ではなく設計で調停しようとする動きです。

### 3. AWS DMS Schema Conversion now supports AI agent automation
- 出典: AWS What’s New
- 日付: 2026-07-10
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/aws-dms-sc-ai-agent-automation-mcp-server/
- 要約: AWS DMS Schema Conversion が AWS MCP Server 経由の AI エージェント自動化に対応し、Kiro、Claude Code、Cursor などから自然言語で移行プロジェクト作成、メタデータ閲覧、スキーマ変換、評価レポート生成、結果エクスポートまで実行できるようになりました。
- なぜ面白いか:
  - 技術: データベース移行という手順依存で失敗コストの高い作業が、MCP スキルとして IDE 内のエージェント手順に落ちてきた点が実用的です。
  - 人文: レガシー移行は単なる技術負債処理ではなく、組織の記憶を新しい環境へ翻訳する作業でもあります。エージェントがここに入ることで、熟練者の暗黙知をどこまで手順化・共有できるかが問われます。

### 4. AWS Security Hub now offers Network Scanning to identify publicly reachable resources
- 出典: AWS What’s New
- 日付: 2026-07-08
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-network-scanning/
- 要約: AWS Security Hub に Network Scanning が追加され、インターネットから実際に到達可能な AWS および Azure 上のリソース、ポート、背後のサービスを検出できるようになりました。セキュリティグループやルートテーブル上の推定だけでなく、外部からの観測に基づく到達性確認を補完します。
- なぜ面白いか:
  - 技術: CSPM 的な設定評価に、実際の外部到達性スキャンが加わることで、マルチクラウド環境のリスク優先順位付けが現実に近づきます。
  - 人文: セキュリティは「設定したつもり」と「外から見えている姿」のずれから事故が起きます。外部からの視点を標準機能に入れることは、組織が自分の盲点を見るための鏡を持つことに近いです。

### 5. AWS Builder Center Now Offers Free Sandbox Environments
- 出典: AWS What’s New
- 日付: 2026-07-08
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/aws-builder-center-sandbox/
- 要約: AWS Builder Center が、対象ワークショップから無料・時間制限付きのサンドボックス環境をリクエストできるようになりました。個人の AWS アカウントやクレジットカード、想定外課金の不安なしに、事前プロビジョニング済み環境で学習できます。
- なぜ面白いか:
  - 技術: 8時間の一時的な AWS 環境を学習用に提供することで、IAM、課金、リソース削除といった初学者のつまずきを減らし、ハンズオンを再現可能にします。
  - 人文: クラウド学習の障壁は知識だけでなく、失敗したら請求が来るかもしれないという心理的コストにもあります。安全に壊せる場所を用意することは、学習文化を広げるための社会的インフラです。

## arXiv / 学術
- SLFS: a Flexible, Low-Cost Distributed File System Using Serverless Designs / arXiv:2607.01486 / 2026-07-01 / https://arxiv.org/abs/2607.01486v1 — AWS 固有の論文ではありませんが、S3 などのクラウドネイティブストレージを含むバックエンド上で、サーバーレス関数を使った分散ファイルシステムを評価しており、Lambda MicroVMs やサーバーレス基盤の方向性を考える材料になります。
- Data Replication Meets Function Scheduling in the Edge-Cloud Continuum / arXiv:2606.30563 / 2026-06-29 / https://arxiv.org/abs/2606.30563v1 — AWS 固有ではありませんが、エッジ・クラウド連続体でのサーバーレス関数配置とデータ複製を扱う研究で、AWS の分散・エッジ戦略を読む補助線になります。

## メモ
- X 検索: `x_search` を英語・日本語・Boris Cherny 限定で実行しましたが、xAI/Grok 側の spending-limit エラーで取得できませんでした。そのため、X 由来の投稿内容は本ファイルでは採用していません。
- Web 検索: `web_search` / `web_extract` は Firecrawl 未設定で失敗したため、AWS 公式 RSS（What’s New、AWS News Blog、AWS Machine Learning Blog、AWS Japan Blog）を `urllib` で直接取得して確認しました。
- Boris Cherny優先の有無: Claude/Bedrock 関連として Boris Cherny / @bcherny を優先確認する検索を実行しましたが、上記 X 検索エラーにより確認不能でした。未確認情報は本文に入れていません。
- 日本語アカウントの扱い: X の日本語検索は失敗しましたが、AWS Japan Blog の直近記事（Kiro の Claude Sonnet 5、Bedrock ゼロデータ保持、Summit Japan 事例など）を参照し、日本語コミュニティで関心が高そうな学習・統制・生成AI運用の観点を選定に反映しました。
- 注意点・誇張リスク: AWS 公式発表中心のため事実性は高い一方、導入効果は組織の IAM 設計、監査要件、既存ワークフローに依存します。特にエージェント自動化は、権限境界とレビュー手順を明確にしないと便利さがそのまま運用リスクになります。

# AWS トレンド調査 (2026-07-13)

- 調査日: 2026-07-13
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWS の今週の面白さは、クラウド基盤そのものが「AIエージェントに操作される前提」の運用面・認証面・開発体験へ寄ってきた点にあります。

## トップ5

### 1. AWS DMS Schema Conversion が AI agent automation をサポート
- 出典: AWS What’s New
- 日付: 2026-07-10
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/aws-dms-sc-ai-agent-automation-mcp-server/
- 要約: AWS DMS Schema Conversion が AWS MCP Server 経由の AI エージェント自動化に対応し、Kiro、Claude Code、Cursor などからスキーマ変換や移行ワークフローを実行できるようになりました。レガシーDB移行の「調査・変換・検証」の作業を、自然言語とツール実行のループに載せやすくする発表です。
- なぜ面白いか:
  - 技術: データベース移行という失敗コストの高い領域に MCP とコーディングエージェントを接続し、移行作業を IDE/エージェント中心の反復可能なワークフローに変えています。
  - 人文: 移行は単なる技術作業ではなく、組織の歴史が詰まった古いシステムとの交渉でもあります。エージェント化により、暗黙知を持つ熟練者だけに依存していた作業を、チームで観察・レビューできる物語へ変える可能性があります。

### 2. AWS MCP Server が OAuth / AWS Sign-In 接続をサポート
- 出典: AWS What’s New
- 日付: 2026-07-09
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/oauth-aws-mcp-server/
- 要約: AI エージェントが AWS MCP Server に AWS Sign-In と業界標準 OAuth で直接接続できるようになりました。既存の AWS アイデンティティ、サインイン方式、IAM 権限、ガバナンスを使って、追加の認証ソフトウェアなしに接続できる点が重要です。
- なぜ面白いか:
  - 技術: エージェントのツール接続を「秘密鍵を渡す」方向ではなく、既存 IAM と OAuth の統制に寄せることで、実運用で必要な監査・権限分離・停止可能性を確保しやすくしています。
  - 人文: AI エージェントを同僚のように働かせるには、信頼だけでなく「誰が何を許したか」を説明できる制度が必要です。認証の標準化は、エージェント時代の責任の所在を人間社会に接続する小さく重要な一歩です。

### 3. Kiro で Claude Sonnet 5 が利用可能に
- 出典: AWS Japan Blog
- 日付: 2026-07-11（記事公開。利用開始は 2026-07-01）
- リンク: https://aws.amazon.com/jp/blogs/news/sonnet-5/
- 要約: AWS の Kiro IDE、CLI、Web で Claude Sonnet 5 が利用可能になったことを日本語で案内しています。Sonnet 5 はエージェント性能、推論、ツール利用、コーディング能力が強化され、Sonnet クラスの価格のまま提供されると説明されています。
- なぜ面白いか:
  - 技術: Claude 系モデルを Kiro の IDE/CLI/Web に入れることで、設計・実装・検証を同じ開発環境内でエージェント的に回しやすくなります。
  - 人文: 開発者が「検索して読む」だけでなく「相棒と設計を往復する」作業様式へ移る兆しです。日本語記事として出ている点も、日本の開発者コミュニティがエージェント型開発を日常語で理解していく入口になります。

### 4. Amazon EKS が Kubernetes バージョンロールバックをサポート
- 出典: AWS News Blog
- 日付: 2026-07-01
- リンク: https://aws.amazon.com/blogs/aws/upgrade-amazon-eks-clusters-with-confidence-using-kubernetes-version-rollbacks/
- 要約: Amazon EKS で Kubernetes バージョンアップ後、7日以内であればロールバックできる機能が紹介されました。失敗時にクラスターを作り直すのではなく、アップグレードを可逆な操作に近づける発表です。
- なぜ面白いか:
  - 技術: Kubernetes アップグレードの不可逆性を下げ、プラットフォームチームが本番クラスターの更新をより短いフィードバックループで実施できます。
  - 人文: 運用者の心理的安全性に効く機能です。「失敗したら終わり」という恐怖を減らすことは、技術的負債を放置しない文化を育てる土台になります。

### 5. AWS CloudFormation Express mode が最大4倍速いインフラデプロイを提供
- 出典: AWS News Blog
- 日付: 2026-06-30
- リンク: https://aws.amazon.com/blogs/aws/accelerate-your-infrastructure-deployments-by-up-to-4x-with-aws-cloudformation-express-mode/
- 要約: CloudFormation Express mode により、インフラデプロイの確認を高速化し、AI エージェントや開発者がより短時間で反復できるようになったと紹介されています。商用リージョンで追加料金なしに利用可能とされています。
- なぜ面白いか:
  - 技術: IaC のデプロイ待ち時間を短縮し、AI エージェントが生成した変更を検証するループを高速化することで、インフラ変更の実験速度を上げます。
  - 人文: 待ち時間は開発者の集中力と判断を削ります。反復が速くなると、インフラは「儀式的に慎重に触るもの」から「対話しながら学ぶもの」へ少し近づきます。

## arXiv / 学術
- NKI-Agent: Domain-Specific Fine-Tuning and Agentic Tool Use for Neuron Kernel Generation（arXiv:2607.04395、2026-07-05）: AWS Trainium / Inferentia 向けの Neuron Kernel 生成を、ドメイン特化チューニングとエージェント的ツール利用で扱う研究。AWS の独自アクセラレータ上での最適化を、人手の職人芸からエージェント支援へ移す流れとして関連度が高いです。リンク: https://arxiv.org/abs/2607.04395v1
- Overprivilege Analysis of Security Policies in Serverless Cloud Applications（arXiv:2607.02875、2026-07-03）: サーバーレスアプリケーションの権限過多を分析する研究。AWS Lambda/IAM を直接名指しする運用現場に近い問題設定として、エージェントがクラウドを操作する時代の最小権限設計にもつながります。リンク: https://arxiv.org/abs/2607.02875v1

## メモ
- Boris Cherny優先の有無: Claude/Anthropic/Bedrock 関連として Boris Cherny（@bcherny）を X 検索で優先確認しようとしましたが、x_search は `personal-team-blocked:spending-limit` で失敗しました。そのため本ファイルでは Boris 発の投稿を採用していません。
- 日本語アカウントの扱い: X 検索は同じ外部制限により取得できませんでした。代替として AWS Japan Blog の日本語記事を優先的に確認し、Kiro / Claude Sonnet 5 の日本語開発者向け情報をトップ5に含めました。
- 注意点・誇張リスク: Web 検索ツールも未設定でしたが、AWS 公式 RSS、AWS Japan Blog RSS、arXiv API を terminal 経由で実取得し、選定リンクは HTTP 200 を確認しました。X 由来のコミュニティ反応は今回の環境では検証できていないため、反応量や評判については主張していません。

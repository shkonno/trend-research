# AWS トレンド調査 (2026-08-22)

- 調査日: 2026-08-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWSの今週は、Bedrock/AgentCoreを中心に「生成AIを安全に実運用へ入れる」流れと、Glue・EKS・Connectなど既存基盤の現実的な運用改善が同時に進んだ一日です。

## トップ5

### 1. Web Search in Amazon Bedrock AgentCore がドメイン・公開日フィルタと欧州/アジア太平洋展開を追加
- 出典: AWS What's New
- 日付: 2026-08-19
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/web-search-amazon-bedrock/
- 要約: Amazon Bedrock AgentCore の Web Search が、検索対象ドメインと公開日をリクエスト単位で絞り込めるようになり、欧州およびアジア太平洋リージョンにも拡大しました。企業エージェントが「どのWeb情報を、どの時間窓で参照したか」を制御しやすくなる更新です。
- なぜ面白いか:
  - 技術: RAG/エージェントの外部検索をサーバーサイドの管理機能として扱い、ソース制限・鮮度制限・リージョン選択を運用ポリシーに落とし込める点が実用的です。
  - 人文: 「AIがWebを読む」ことは、知識の参照行為を組織の統治対象に変える出来事です。誰の情報を参照し、古い情報をどこまで許すかという編集責任が、プロンプトではなくインフラ設定の問題になっています。

### 2. Amazon Bedrock の Web Search に External Web Access が登場
- 出典: AWS What's New
- 日付: 2026-08-19
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-web-access-web-search/
- 要約: Amazon Bedrock の Web Search に External Web Access が追加され、最新Web知識でモデル応答をグラウンディングしつつ、AWS環境内でのセキュアな利用を狙う方向が示されました。発表文では、データをセキュアなAWS環境に保ちながら現在のWeb知識で回答を補強する built-in server-side tool と説明されています。
- なぜ面白いか:
  - 技術: モデル単体の知識ではなく、Bedrock側のツール機能としてWeb参照を組み込むことで、監査・権限・データ境界をクラウド運用の文脈で扱いやすくなります。
  - 人文: 生成AIの「現在性」をクラウド事業者がどう媒介するかは、企業内の知識労働の形を変えます。検索エンジンを人が開く時代から、業務エージェントが管理された窓越しに世界を見る時代への移行が見えます。

### 3. AWS Glue 6.0 が一般提供、30%低価格化と Apache Iceberg v3 対応
- 出典: AWS News Blog / AWS What's New
- 日付: 2026-08-21
- リンク: https://aws.amazon.com/blogs/aws/aws-glue-6-0-now-available-with-30-lower-price-and-full-apache-iceberg-v3-support/
- 要約: AWS Glue 6.0 が一般提供され、以前のGlueバージョンより30%低い価格、Apache Spark 4.1、Python 3.12、Scala 2.13、Apache Iceberg v3のフルサポート、Hudi/Delta Lakeの新バージョン対応が発表されました。データレイク/レイクハウス基盤の更新として影響範囲が広いリリースです。
- なぜ面白いか:
  - 技術: ETLランタイムの世代更新とIceberg v3対応が同時に来たことで、コスト削減だけでなくテーブル形式・開発者体験・将来の分析基盤設計に効きます。
  - 人文: データ基盤の「地味な値下げと標準対応」は、AI活用の可否を左右する社会的インフラ整備です。派手なモデル発表よりも、日々のデータ整備に携わるチームの負担を減らす更新として重要です。

### 4. Amazon Connect Customer が管理者向けに「データとチャット」できる分析機能を追加
- 出典: AWS What's New
- 日付: 2026-08-21
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-connect-customer-ai-data-analytics
- 要約: Amazon Connect Customer に、管理者が自然言語でデータに質問し、回答・根拠・改善策を数秒で得られる機能が追加されました。セルフサービス、エージェントパフォーマンス、キューパフォーマンスにまたがる150以上のメトリクスを横断し、たとえば自動化候補のキューを信頼度や想定効果つきで優先順位付けします。
- なぜ面白いか:
  - 技術: コンタクトセンター運用のメトリクス探索を、ダッシュボード閲覧から会話型の原因分析・推奨アクション生成へ移している点が実務的です。
  - 人文: 管理者の仕事は「数字を探す」ことから「提案の妥当性を判断する」ことへ寄ります。一方で、顧客対応の現場をAIがスコア化・優先順位付けすることは、労働評価や自動化判断の透明性をより強く要求します。

### 5. 日本語コミュニティ事例: サンリオが AI-DLC Unicorn Gym で上流工程からのAI駆動開発を実践
- 出典: Amazon Web Services ブログ（日本語）
- 日付: 2026-08-21
- リンク: https://aws.amazon.com/jp/blogs/news/sanrio-ai-dlc-unicorn-gym-2026/
- 要約: サンリオのデジタル事業開発部6名が、2026年6月に2日間の AI-DLC Unicorn Gym に参加した座談会レポートです。AI-DLC はAIを補助ツールに留めず、要件定義・設計・実装・テストまでの開発ライフサイクル全体に組み込みつつ、人間が主導権を持つ Human-in-the-Loop 型の開発手法として紹介されています。
- なぜ面白いか:
  - 技術: Claude Code中心の個人生産性から、チームの上流工程・設計・テストへAIを広げる実践例として、AWS/Kiro/生成AI活用の日本語ケーススタディになっています。
  - 人文: キャラクターやファン創作に関わる企業がAI駆動開発を採り入れる点は、単なる効率化を超えて「創作文化を支えるソフトウェアをどう作るか」という問いにつながります。Human-in-the-Loop を明示している点も、開発現場の主体性を守る設計思想として読めます。

## arXiv / 学術
- 直近約14日のAWS固有リリースに直接対応するarXiv論文は、本調査時点で確認されませんでした。
- 参考として、周辺領域では Kubernetes/モデルサービングの運用失敗意味論に関する “The Lazy Pod That Lies: Deferred Cost and Failure Semantics of Lazy Container Image Pulling for Model Serving on Kubernetes” (arXiv:2608.19412, 2026-08-19) が確認されましたが、AWS固有ではないためトップ5には含めていません。

## メモ
- Boris Cherny優先の有無: Claude/Anthropic/Bedrock関連のため @bcherny を含むX検索を実行しましたが、X検索ツールは `personal-team-blocked:spending-limit` で失敗しました。そのため本ファイルではBoris Cherny由来の未確認情報は採用していません。
- 日本語アカウントの扱い: X検索は英語・日本語とも同じクレジット制限で失敗したため、日本語圏の補完としてAWS Japan公式ブログの直近記事を確認し、サンリオ AI-DLC 事例を採用しました。
- 注意点・誇張リスク: Web検索/抽出ツールも未設定で失敗したため、公式RSS、AWS公式ページへの直接HTTP取得、arXiv APIを主な根拠にしました。X上の反応や非公式ブログの温度感は本調査では十分に反映できていません。

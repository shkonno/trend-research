# AWS トレンド調査 (2026-08-12)

- 調査日: 2026-08-12
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

今週のAWSは、生成AIエージェントを「試作」から「運用・統制・コスト管理」へ移すための部品が一気に揃った週でした。

## トップ5

### 1. Amazon Bedrock AgentCore runtime instances が一般提供開始

- 出典: AWS What's New / AWS News Blog
- 日付: 2026-08-06
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/aws-bedrock-agentcore-runtime-instances-generally-available/
- 要約: Amazon Bedrock AgentCore の runtime instances が一般提供され、AIエージェントを自分の Amazon EC2 インスタンス上で、インフラ運用を抑えながら実行できるようになりました。既存の microVM ベース実行に加え、長時間・高負荷・GPUや特殊インスタンスが必要なエージェント運用に向いた選択肢です。
- なぜ面白いか:
  - 技術: 最大14日級の持続セッションやEC2インスタンスタイプ選択を前提に、エージェント基盤が「短命な関数」から「状態を持つ常駐ワーカー」へ近づいています。
  - 人文: エージェントを人間の同僚のように長く働かせるには、記憶・責任・中断可能性をどう設計するかが問われます。これは単なるインフラ機能ではなく、職場における「自律的な作業主体」をどう制度化するかという問題です。

### 2. Amazon DynamoDB がリアルタイムベクトル検索をサポート

- 出典: AWS What's New / AWS News Blog / AWS Database Blog
- 日付: 2026-08-05
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-dynamodb-vector-search
- 要約: DynamoDB にネイティブなベクトル検索が一般提供され、単一桁ミリ秒レイテンシ、99%以上のリコール、数十億から数兆ベクトル規模を狙う構成が可能になりました。アプリの運用データと意味検索を同じDynamoDB上で扱えるため、別のベクトルDBを持つ構成を減らせます。
- なぜ面白いか:
  - 技術: RAGや推薦の検索層を既存のキー・バリュー/ドキュメントDBへ寄せることで、整合性、スケール、運用境界の設計が大きく単純化します。
  - 人文: 「意味」を検索可能なインフラに埋め込む動きは、業務システムが人間の分類や記憶の代替物になっていく過程でもあります。何を似ているとみなすか、どの記憶を近くに置くかという文化的判断が、DB設計の中に入り込みます。

### 3. AWS Continuum が Claude Code / Codex / Kiro の開発者ワークフローへ統合

- 出典: AWS Security Blog / AWS 日本語 News Blog
- 日付: 2026-08-05（日本語記事は2026-08-10）
- リンク: https://aws.amazon.com/blogs/security/aws-partners-with-anthropic-and-openai-to-bring-aws-continuum-into-developer-workflows/
- 要約: AWS が Anthropic および OpenAI と協業し、AWS Continuum for code vulnerabilities を Claude Code、Codex、Kiro のワークフローに統合すると発表しました。脆弱性の発見、文脈に基づく優先順位付け、検証、修復を、開発者が普段使うAIコーディング環境の中で扱えるようにするプレビューです。
- なぜ面白いか:
  - 技術: セキュリティスキャンをCIの後段だけでなく、AIコーディングエージェントの編集ループへ直接差し込むことで、修復提案と検証を同じ文脈で回せます。
  - 人文: セキュリティが「監査する別部門」から「開発中に話しかけてくる共同編集者」へ変わると、責任の所在も変わります。便利さの一方で、AIが指摘したリスクを誰が最終判断するのかという実務倫理がより重要になります。

### 4. Amazon Bedrock が OpenAI GPT モデル向け Web Search を一般提供

- 出典: AWS What's New / AWS Weekly Roundup
- 日付: 2026-08-04
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-web/
- 要約: Amazon Bedrock で OpenAI GPT-5.4、GPT-5.5、GPT-5.6 Sol/Terra/Luna 向けの Web Search が一般提供されました。サードパーティ検索APIの契約・キー管理・課金統合を別途行わず、AWS内で現在情報に基づく応答を生成でき、データレジデンシーやゼロデータエグレスも訴求されています。
- なぜ面白いか:
  - 技術: モデル呼び出し、Webグラウンディング、ガバナンスをBedrock側に寄せることで、企業RAG/調査エージェントの境界が「アプリ実装」から「クラウド管理面」へ移ります。
  - 人文: 検索がモデルの内蔵ツールになると、ユーザーは情報源を意識しにくくなります。便利になるほど、どの検索空間が参照され、何が見えなくなったのかを説明する透明性が必要です。

### 5. Agent Plugins 1.0.0 と Kiro powers 対応で、エージェント拡張のポータビリティが前進

- 出典: AWS 日本語 News Blog
- 日付: 2026-08-10
- リンク: https://aws.amazon.com/jp/blogs/news/aws-supports-agent-plugins-an-open-standard-for-portable-agent-extensions/
- 要約: AWS は Cursor、Microsoft、OpenAI、Vercel とともに Agent Plugins Technical Steering Committee の設立メンバーとなり、Agent Plugins 1.0.0 をサポートしました。Agent Skills と MCP サーバーを一度パッケージ化すれば、Kiro、VS Code、Cursor など対応クライアントに配布でき、Kiro powers も同仕様を順次サポートします。
- なぜ面白いか:
  - 技術: エージェント拡張をIDEやベンダーごとに作り分けるのではなく、MCP/Skills/プラグインの配布単位として標準化する流れが強まっています。
  - 人文: 開発者の道具箱がポータブルになることは、特定プラットフォームへの囲い込みを弱める可能性があります。一方で、標準化委員会に誰が参加し、誰の作法が標準になるのかは、開発文化の権力構造そのものです。

## arXiv / 学術

- 関連あり: 「Epico: Long-Lived WebAssembly Components for High-Performance Serverless Stream Processing」 arXiv:2608.02361（2026-08-03） https://arxiv.org/abs/2608.02361 — サーバーレスのFaaSモデルが連続・低遅延ストリーム処理に弱いという問題に対し、長寿命WebAssemblyコンポーネントを用いる研究で、Lambda/SQS/AgentCoreのようなAWS上のイベント駆動設計を考える補助線になります。
- 関連あり: 「Quantum Fidelity-per-Cost: A Metric for Evaluation of Quantum Computing Systems」 arXiv:2607.28572（2026-07-30） https://arxiv.org/abs/2607.28572 — AWSを含むクラウド型量子計算の比較を、物理性能だけでなくコストを含めて評価する方向の研究です。

## メモ

- Boris Cherny優先の有無: Claude/Anthropic/Bedrock関連として Boris Cherny（@bcherny）情報をX検索で優先確認しようとしましたが、x_search がクレジット上限エラーで利用できず、確認できませんでした。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で実行結果を取得できませんでした。代替として AWS 日本語 News Blog と週刊AWS/週刊生成AI with AWS を確認し、日本語コミュニティが読みやすい論点を優先しました。
- 注意点・誇張リスク: Web検索ツールも未設定だったため、AWS公式RSS/ブログと arXiv API の直接取得を中心に調査しました。X上の反応量や非公式コミュニティでの盛り上がりは、本調査では十分に反映できていません。

# AWS トレンド調査 (2026-08-11)

- 調査日: 2026-08-11
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWS は「AIエージェントを本番運用に載せるための基盤化」と「既存の開発・データ基盤へのAI機能の埋め込み」を同時に進めている。

## トップ5

### 1. Amazon Bedrock AgentCore runtime instances が一般提供、長時間セッションの本番AIエージェントへ
- 出典: AWS News Blog / AWS What’s New
- 日付: 2026-08-06
- リンク: https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore/
- 要約: Amazon Bedrock AgentCore の runtime instances が一般提供され、AIエージェントを自分の Amazon EC2 インスタンス上で実行できるようになった。最大14日間のセッション、GPU対応、マルチエージェント協調など、本番運用を意識した「持続する計算環境」が前面に出ている。
- なぜ面白いか:
  - 技術: ステートレスなチャット実行ではなく、長時間・状態保持・専用インフラを備えたエージェント実行環境を Bedrock 管理面に近づけている点が重要。
  - 人文: エージェントが一回限りの道具から「継続的に働く同僚」へ近づくほど、責任分界、監査、休止、引き継ぎといった組織文化の設計が技術設計と不可分になる。

### 2. Amazon DynamoDB がリアルタイム・ベクトル検索をネイティブサポート
- 出典: AWS News Blog / AWS Japan Blog
- 日付: 2026-08-05（日本語記事は 2026-08-07）
- リンク: https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale/
- 要約: DynamoDB が単一桁ミリ秒レイテンシ、99%以上のリコール、数兆ベクトル規模をうたうネイティブなベクトル検索をサポートした。RAGや推薦などで、トランザクションデータと意味検索データを別基盤に分ける必要が減る可能性がある。
- なぜ面白いか:
  - 技術: NoSQL の運用特性とベクトル検索を同じマネージド基盤に寄せることで、AIアプリのデータ同期・遅延・障害点を減らせる。
  - 人文: 「記録」と「意味」を同じデータベースが扱うようになると、企業が顧客や業務をどう記憶し、どう類推するかという制度設計そのものが問われる。

### 3. Amazon Bedrock Web Search が一般提供、基盤モデルのグラウンディングをサーバーサイド機能に
- 出典: AWS Machine Learning Blog / AWS Weekly Roundup
- 日付: 2026-08-04
- リンク: https://aws.amazon.com/blogs/machine-learning/introducing-web-search-on-amazon-bedrock-for-foundation-model-grounding/
- 要約: Amazon Bedrock に Web Search が一般提供され、モデル応答を最新のWeb知識でグラウンディングする組み込みツールとして利用できるようになった。外部検索連携をアプリ側で組むのではなく、Bedrock 側の機能として扱えるのがポイント。
- なぜ面白いか:
  - 技術: 検索、引用、モデル呼び出し、権限管理を Bedrock の実行面に近づけることで、RAG以前の「今の情報をどう安全に読ませるか」を標準部品化している。
  - 人文: AIの答えが「記憶」ではなく「調査」に近づくほど、利用者は出典を読むリテラシーと、検索結果が作る世界観への批判的距離を求められる。

### 4. AWS Continuum が Claude Code / Codex / Kiro のワークフローに統合へ
- 出典: AWS Japan Blog
- 日付: 2026-08-10
- リンク: https://aws.amazon.com/jp/blogs/news/aws-partners-with-anthropic-and-openai-to-bring-aws-continuum-into-developer-workflows/
- 要約: AWS は Anthropic および OpenAI との協業により、AWS Continuum for code vulnerabilities（プレビュー）を Claude Code、Codex、Kiro の開発者ワークフローへ統合すると発表した。脆弱性の発見、コンテキストに基づく優先順位付け、検証、修復を、既存のコーディング・エージェント体験の中に入れる構想である。
- なぜ面白いか:
  - 技術: セキュリティ診断をCI後段のチェックではなく、Claude Code / Codex / Kiro の修正ループへ直接差し込むことで、AIコーディングと脆弱性対応を同じ作業面に統合している。
  - 人文: 開発者が「コードを書く人」から「エージェントが提案する修復を評価する人」へ移ると、セキュリティ責任は個人の注意力だけでなく、ツールチェーンの説明可能性と組織の承認文化に依存する。

### 5. AWS が Agent Plugins 1.0.0 を支援、エージェント拡張のポータブル標準化へ
- 出典: AWS Japan Blog
- 日付: 2026-08-10
- リンク: https://aws.amazon.com/jp/blogs/news/aws-supports-agent-plugins-an-open-standard-for-portable-agent-extensions/
- 要約: AWS は Cursor、Microsoft、OpenAI、Vercel とともに Agent Plugins Technical Steering Committee の設立メンバーとして参加し、Agent Plugins 1.0.0 を支援すると発表した。Agent Skills と MCP サーバーを一度パッケージ化し、Kiro、VS Code、Cursor など対応クライアントへ配布できるオープン仕様を目指す。
- なぜ面白いか:
  - 技術: エージェント拡張を特定IDEや特定ベンダーのプラグインに閉じず、スキルとMCPサーバーを移植可能な配布単位として扱う流れを強めている。
  - 人文: エージェントの「能力」が市場で流通する部品になると、誰が信頼を署名し、誰が悪意ある能力を排除し、どの共同体が標準を決めるのかが重要になる。

## arXiv / 学術
- arXiv 検索は API が 429 Too Many Requests を返したため、Web検索ページを直接確認した。AWS 固有サービスの最新発表と一対一で対応する査読前論文は本調査時点で確認されませんでした。
- 関連する近傍テーマとして、検索ページでは `arXiv:2607.24006`「Agentic Cloud Decoys: A Deception-Driven Framework for Autonomous Intrusion Investigation」、`arXiv:2607.20319`「Black-Box Performance Evaluation of Elastic Block Storage: Contract, Rate-Limiting Model, and Software Exploration」、`arXiv:2606.21680`「Towards Global Multi-Cloud Strategies: Insights into AWS and Alibaba Cloud Synergy」などが確認された。ただし、今回のトップ5はAWS公式発表・技術ブログの実運用インパクトを優先した。

## メモ
- Boris Cherny優先の有無: Claude/Anthropic/Bedrock 関連として確認対象にしたが、X検索ツールが `personal-team-blocked:spending-limit` で利用不能だったため、Boris Cherny / @bcherny の当日X投稿は確認できなかった。
- 日本語アカウントの扱い: X検索は同じ理由で利用不能。代替として AWS Japan Blog RSS を確認し、日本語開発者向けに公開された Continuum、Agent Plugins、Kiro CLI、週刊生成AI with AWS の記事を調査対象に含めた。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で利用不能だったため、AWS公式RSSと直接HTTP取得できた arXiv 検索ページを主な根拠にした。上記リンクは実在確認済みだが、X上の反応や日本語コミュニティの非公式評価は今回十分に取得できていない。

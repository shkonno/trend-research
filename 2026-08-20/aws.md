# AWS トレンド調査 (2026-08-20)

- 調査日: 2026-08-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AWS の今朝の話題は、Bedrock AgentCore を中心に「企業内で安全に動くエージェント」から「Webを読める・支払える・長時間働けるエージェント」へ一段進んだことです。

## トップ5

### 1. Amazon Bedrock Web Search が External Web Access と AgentCore のドメイン・日付フィルタを強化
- 出典: AWS What’s New / AWS Machine Learning Blog
- 日付: 2026-08-19
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/08/amazon-bedrock-web-access-web-search/ （関連: https://aws.amazon.com/blogs/machine-learning/domain-and-publish-date-filters-for-web-search-on-agentcore/ ）
- 要約: Amazon Bedrock の Web Search が `external_web_access` パラメータに対応し、公開Webから最新情報を直接取得してモデル応答をグラウンディングできるようになりました。AgentCore 側では、実行時のドメイン allow/deny と公開日フィルタが追加され、Web Search の提供リージョンも Europe (Ireland) と Asia Pacific (Tokyo) に広がっています。
- なぜ面白いか:
  - 技術: エージェントの検索先・鮮度・外部Webアクセス可否をサーバー側で制御できるため、RAG/検索エージェントのガバナンスをアプリ外のポリシーに寄せられます。
  - 人文: 「AIが何を読んでよいか」を企業が明示できる点は、知識労働における信頼と検閲、鮮度と安全性のバランスを可視化します。東京リージョン対応は、日本企業がデータ近接性を保ちながらエージェント検索を試しやすくなる文化的な節目です。

### 2. Amazon Bedrock AgentCore payments が一般提供開始、エージェントが安全に支払える基盤へ
- 出典: AWS Machine Learning Blog
- 日付: 2026-08-18
- リンク: https://aws.amazon.com/blogs/machine-learning/amazon-bedrock-agentcore-payments-is-now-generally-available-enabling-agents-to-transact-safely-and-autonomously-at-scale/
- 要約: Amazon Bedrock AgentCore payments が一般提供となり、AIエージェントが有料API、MCPサーバー、Webコンテンツなどに対して、支出ガードレールとオブザーバビリティ付きで自律的に支払いを行えるようになりました。Coinbase や Stripe Privy のウォレット連携を使い、少額・実行単位の決済ユースケースを狙っています。
- なぜ面白いか:
  - 技術: ツール呼び出しだけでなく「決済」をエージェント実行基盤の一部にすることで、外部サービス利用の認証・支出上限・監査をプロダクション要件として扱えます。
  - 人文: エージェントが財布を持つと、代理行為の責任、失敗時の補償、誰が支払い意思を持ったのかという社会的な問いが一気に現実化します。これは単なる機能追加ではなく、AIを「作業者」から「取引主体の代理人」に近づける変化です。

### 3. Bedrock AgentCore Runtime Instances: 本番AIエージェント向けの永続コンピュート
- 出典: AWS News Blog
- 日付: 2026-08-06
- リンク: https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore/
- 要約: Amazon Bedrock AgentCore Runtime に runtime instances が追加され、複数エージェントを同じランタイムで動かし、最大14日間の永続セッション、GPU、コンテナ化、停止・再開、Amazon EBS や AgentCore Memory との連携を利用できるようになりました。短い関数実行ではなく、長時間・協調型のエージェントを本番運用するための選択肢です。
- なぜ面白いか:
  - 技術: エージェントをステートレスなAPI呼び出しではなく、OS・GPU・長期セッションを持つ管理コンピュート上のワークロードとして設計できます。
  - 人文: 「働き続けるAI」を前提にすると、人間の同僚と同じく勤務時間、記憶、引き継ぎ、停止権限をどう設計するかが重要になります。クラウドの抽象化が、労働のメタファーをさらに強めています。

### 4. Amazon DynamoDB がリアルタイム・ベクトル検索を一般提供（少し古いが重要）
- 出典: AWS News Blog
- 日付: 2026-08-05（対象期間より1日古いが、AWSアプリ設計への影響が大きいため採用）
- リンク: https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale/
- 要約: Amazon DynamoDB がネイティブなベクトル検索を一般提供し、運用データと埋め込みを同じテーブルで扱いながら、単一桁ミリ秒レイテンシ、99%超のリコール、トリリオン規模までのスケールをうたっています。既存の DynamoDB アプリに、別のベクトルDBへ複製せずセマンティック検索やエージェントメモリを足せるのがポイントです。
- なぜ面白いか:
  - 技術: OLTPデータベースにベクトル検索が入ることで、RAG、推薦、異常検知、エージェント記憶を低レイテンシな本番データ経路に近づけられます。
  - 人文: データベースが「正確なキーで探す箱」から「意味で思い出す記憶」に変わると、システム設計の語彙も人間の記憶に近づきます。一方で、記憶の近さは忘却・削除・説明可能性の倫理も強く要求します。

### 5. 日本の製薬現場で Claude Code on AWS を導入した JCRファーマ事例
- 出典: AWS Japan Blog
- 日付: 2026-08-16
- リンク: https://aws.amazon.com/jp/blogs/news/jcrpharm-claude-code-on-aws/
- 要約: ＪＣＲファーマが Amazon Bedrock 経由で Claude Code を約2か月導入した取り組みを寄稿として公開しました。Anthropic との個別契約ではなく既存のAWS基盤を活かせること、社内のセキュリティ・ガバナンスに乗せやすいこと、研究・業務のAIエージェント活用に手応えがあったことが紹介されています。
- なぜ面白いか:
  - 技術: Claude Code を Bedrock 経由で使うことで、モデル利用、権限、監査、社内ネットワーク設計を既存AWS運用に統合しやすくなります。
  - 人文: 創薬のように専門性と責任が重い領域で、AIが「回答ツール」ではなくコードを書き、実行し、失敗を修正する共同作業者として受け入れられ始めています。日本語の実践事例として、現場の信頼形成がどのように進むかを見る材料になります。

## arXiv / 学術

- 本調査時点で、AWS / Amazon Bedrock / AWS Lambda / AWS cloud を対象に arXiv API で新着検索しましたが、AWS固有の技術発表として採用できる関連論文は確認されませんでした。検索結果には一般的なLLM評価、推薦、エッジAI等の論文が含まれましたが、AWSサービスや本日のトップ項目との直接関係を確認できなかったため採用していません。

## メモ

- Boris Cherny優先の有無: Claude / Anthropic / Bedrock 関連として `@bcherny` を含む X 検索を実行しましたが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、Boris Cherny 本人発信は本調査時点で確認できませんでした。
- 日本語アカウントの扱い: X検索ツールが同じ理由で利用できなかったため、日本語X投稿は確認不能でした。代替として AWS Japan Blog の日本語記事を確認し、JCRファーマの Claude Code on AWS 事例をトップ5に含めました。
- 注意点・誇張リスク: Web検索 / Web抽出ツールも Firecrawl 未設定で失敗したため、公式RSSと直接HTTP取得できたAWS公式ページを主ソースにしました。上記リンクは実際に取得できた公式ページまたはRSS内リンクのみを使用しています。

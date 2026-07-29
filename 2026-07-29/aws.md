# AWS トレンド調査 (2026-07-29)

- 調査日: 2026-07-29
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

今週のAWSは、Bedrock/Claude系のエージェント実装を「作る」段階から、測る・守る・運用する段階へ進める発表が目立ちます。

## トップ5

### 1. Claude Opus 5 is now available on AWS

- 出典: AWS What's New
- 日付: 2026-07-24
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/claude-opus-5-aws/
- 要約: AWS上でClaude Opus 5が提供開始され、コーディング、長時間エージェント、複雑な文書・業務分析での利用が強調されています。ゼロデータ保持（ZDR）対応として説明されており、企業利用でのガバナンス要件にも寄せた発表です。
- なぜ面白いか:
  - 技術: 高性能モデルをBedrock/AWS上のデータ境界・監査・運用基盤と組み合わせやすくなり、エージェント開発の本番適用範囲が広がります。
  - 人文: 「最も賢いモデルをどこで動かすか」は、単なる性能比較ではなく、企業が知識労働の判断権とデータ主権をどこに置くかという制度設計の問題です。便利さと統制の両立が、開発者だけでなく法務・経営・現場の関係を変えていきます。

### 2. AWS announces aws-bench, an open-source benchmark for AI agents on AWS

- 出典: AWS What's New
- 日付: 2026-07-24
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/aws-bench/
- 要約: AWSが、実際のAWS利用から設計した調査・トラブルシュート・インフラ作成タスクでAIエージェントを評価する、オープンソースのaws-bench研究プレビューを発表しました。自然言語クエリ、クラウドリソース状態、正解を組み合わせ、モデルやエージェントを再現可能に比較する狙いです。
- なぜ面白いか:
  - 技術: エージェントをデモではなく、実クラウド操作の正確性・効率・失敗診断で測る基盤が出てきた点が重要です。
  - 人文: ベンチマークは「何を良い仕事とみなすか」を決める文化装置でもあります。AWS運用者の暗黙知がテストケース化されることで、熟練エンジニアの判断がどの程度形式化できるのかが問われます。

### 3. AWS Security Hub MCP App brings exposure findings into your AI-assisted workflow (Preview)

- 出典: AWS What's New
- 日付: 2026-07-27
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-mcp-app/
- 要約: AWS Security Hubの露出・リスク検出結果をClaude Desktopへ持ち込むローカルMCPサーバーがプレビュー公開されました。自然言語で上位の露出、攻撃パス、関連検出、影響リソースを調査でき、セキュリティ調査時のコンテキストスイッチ削減を狙います。
- なぜ面白いか:
  - 技術: Security Hubの構造化された検出結果をMCP経由でAI支援ワークフローに接続し、クラウド防御の調査UIを会話型に拡張します。
  - 人文: セキュリティ運用は、ログを読む専門職から「AIに問いを立てる」専門職へ役割が動きつつあります。一方で、AIが作る説明をどこまで信頼し、誰が最終責任を負うのかという実務倫理が前面化します。

### 4. AWS Lambda durable execution SDK for .NET is now generally available

- 出典: AWS What's New
- 日付: 2026-07-23
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/lambdadf-dotnet/
- 要約: AWS Lambda Durable Execution SDK for .NETが一般提供になり、C#開発者が支払い処理、AIエージェントのオーケストレーション、人間承認を含む長時間ワークフローをLambda内で構築しやすくなりました。進捗チェックポイントや、外部イベント待ちで最大1年の一時停止が説明されています。
- なぜ面白いか:
  - 技術: 従来は外部オーケストレーションや独自状態管理に寄りがちだった長時間処理を、Lambdaのイベント駆動モデルに近い形で扱えるようになります。
  - 人文: 「待つ」「承認する」「途中で止める」といった人間的な時間感覚が、サーバーレスの設計に明示的に入ってきました。自動化は一気通貫だけでなく、人が介入する余白をどう表現するかが品質になります。

### 5. Amazon EKS Provisioned Control Plane now delivers faster pod autoscaling

- 出典: AWS What's New
- 日付: 2026-07-28
- リンク: https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-eks-provisioned-control/
- 要約: Amazon EKSのProvisioned Control Planeクラスターで、Horizontal Pod Autoscaler（HPA）の同期並列度をKubernetesデフォルト値の最大40倍まで高め、Podオートスケールの反応を高速化しました。多数のHPAオブジェクトを持つ大規模クラスターで、需要変化への追従性を改善します。
- なぜ面白いか:
  - 技術: コントロールプレーン側のHPA処理能力を上げることで、アプリケーションのスケール速度をインフラ制御面から改善する発表です。
  - 人文: オートスケーリングは「需要に応じて機械が増える」だけでなく、ユーザーの待ち時間やサービスの信頼感を左右する社会的インフラです。不可視の制御ループが、人々の体験するスムーズさを支えています。

## arXiv / 学術

- 関連あり: 「Agentic Cloud Decoys: A Deception-Driven Framework for Autonomous Intrusion Investigation」arXiv:2607.24006v1（2026-07-27）。クラウドテレメトリと自律的侵入調査を扱い、GuardDuty/Security Hub系のAI調査トレンドと近い問題意識があります。リンク: http://arxiv.org/abs/2607.24006v1
- 関連あり: 「ARBITER: Guarded Agentic Control for SLO-Oriented Kubernetes Remediation」arXiv:2607.19182v2（2026-07-21）。KubernetesのSLO維持に向けたガード付きエージェント制御を扱い、EKSの自動スケール・運用自動化の議論と接続できます。リンク: http://arxiv.org/abs/2607.19182v2
- 関連あり: 「Cold-Start Model Delivery in Kubernetes Inference Serving: An Empirical Study of OCI-Based Distribution and Its Integrity」arXiv:2607.16596v1（2026-07-18）。Kubernetes推論基盤のコールドスタートとモデル配布を扱い、SageMaker/EKS上のAI推論運用にも示唆があります。リンク: http://arxiv.org/abs/2607.16596v1

## メモ

- Boris Cherny優先の有無: Claude/Anthropic/Bedrock関連として確認を試みましたが、HermesのX検索はクレジット/サブスクリプション制限で利用不可でした。直接のXプロフィール取得はログインなしHTMLの取得に留まり、直近投稿の検証はできませんでした。そのため、Boris Cherny発の未確認情報は採用せず、AWS公式発表のみを根拠にしました。
- 日本語アカウントの扱い: X検索が利用不可だったため日本語X投稿は確認できませんでした。代替としてAWS Japan公式ブログ/RSSを確認し、「週刊生成AI with AWS – 2026年7月20日週」「AWS Summit Japan 2026 物流業界向けブース展示」「弁護士ドットコムにおけるAWS DevOps Agent活用事例」など、日本語開発者・事例文脈をトップ5選定時の背景情報として参照しました。
- 注意点・誇張リスク: Web検索ツールもFirecrawl未設定で利用不可だったため、主なWeb情報源はAWS公式RSS/ページの直接取得とarXiv APIです。AWS公式発表は製品価値を強調する性質があるため、実運用でのコスト、リージョン、プレビュー制約、IAM/監査設計は個別確認が必要です。

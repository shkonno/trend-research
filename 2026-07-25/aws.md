# AWS トレンド調査 (2026-07-25)

- 調査日: 2026-07-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AWSは7月後半、Bedrock AgentCoreを「作れる」から「運用できる」エージェント基盤へ押し上げる更新が目立ちました。

## トップ5

### 1. Amazon Bedrock AgentCore のGAとエージェント基盤化
- 出典: X投稿
- 日付: 2026-07-24頃
- リンク: https://x.com/michaelnemtsev/status/2080479393059619325
- 要約: 7月中旬以降、Amazon Bedrock AgentCoreが一般提供（GA）として広く取り上げられ、エージェントのランタイム、オーケストレーション、管理を担う中核レイヤーとして語られていました。Managed Knowledge Bases、Managed Web Search Tool、Guardrails、Harnessなど、単発チャットではない本番エージェントの構成要素がまとまってきています。
- なぜ面白いか:
  - 技術: Bedrock上のモデル提供から、状態・ツール・知識・監査を含むエージェント運用面へAWSの抽象化が上がっています。
  - 人文: クラウド事業者が「AIの行為の場」を提供する時代には、どの企業のクラウド規約が仕事の作法を決めるのかという制度的な問いが生まれます。

### 2. AgentCoreのトレース・プロンプト・ログをCloudWatchへ統合
- 出典: X投稿（AWS What's New JP / Serverworks周辺）
- 日付: 2026-07-23頃
- リンク: https://x.com/awswhatsnew_jp/status/2080339873152868570
- 要約: Amazon Bedrock AgentCoreのトレース、プロンプト、標準ログ、構造化ログが、エージェントごとに1つのCloudWatchロググループへ集約される更新が注目されました。従来の分散したログ探索よりもデバッグしやすく、IAMやCMK暗号化もエージェント単位で扱いやすくなります。
- なぜ面白いか:
  - 技術: エージェントの失敗は複数ステップにまたがるため、プロンプト・ツール呼び出し・トレースを一続きで観測できることが運用の前提になります。
  - 人文: 自律的に見えるシステムにも、後から「なぜそうしたのか」を問える記録が必要です。ログ統合は、AIに対する説明責任をクラウド運用の形式へ落とし込む動きです。

### 3. 「Silent Failure」分析: エラーにならない失敗を見つける方向
- 出典: X投稿（日本語AWSコミュニティの共有）
- 日付: 2026-07-23頃
- リンク: https://x.com/Fuzminaedyw/status/2080413437478527054
- 要約: 日本語Xでは、Bedrock AgentCoreが会話履歴・ツール利用・操作記録から、エラーを出さずに誤った結果を返す「見えない失敗」を検出・分析する機能が話題になっていました。失敗パターンを影響会話数でグルーピングし、原因や修正候補を人間に示す運用支援として受け止められています。
- なぜ面白いか:
  - 技術: 例外やHTTP 500だけでなく、ユーザー意図から外れた正常終了を失敗として扱う評価・観測レイヤーが必要になっています。
  - 人文: 人間社会でも最も危ない失敗は「問題ないように見える失敗」です。AI運用は、沈黙や違和感を検知するケアの技術にも近づいています。

### 4. AgentCore Harness と周辺イベント: 日本語コミュニティでの実装知共有
- 出典: X投稿
- 日付: 2026-07-24
- リンク: https://x.com/recat_125/status/2080422904295301579
- 要約: AWS Bedrock LLM Day Japan（7月28日予定）では、NYC Summitで発表されたManaged Knowledge Base、Web Search Tool、AgentCore Harness GA関連の新機能が解説予定として共有されていました。日本語コミュニティでは、AgentCore + Lambda、Step Functions、EventBridge Schedulerを組み合わせた実装にも関心が集まっています。
- なぜ面白いか:
  - 技術: Harnessはモデル呼び出しだけでなく、セッション、メモリ、ツール、スケジュール実行を束ねる運用単位として重要です。
  - 人文: 技術が定着するには、公式発表だけでなく、地域コミュニティで「どう使うか」が翻訳される必要があります。日本語イベントはクラウド機能を現場語へ変える媒介です。

### 5. TerraRepair: Terraform / IaC修復エージェント研究
- 出典: arXiv
- 日付: 2026-07-13
- リンク: http://arxiv.org/abs/2607.11390v1
- 要約: “TerraRepair: A Tool-Grounded LLM Agent for Infrastructure-as-Code Repair” は、Infrastructure-as-Codeの修復をLLMエージェントとツール接地で扱う研究です。AWSそのものの発表ではありませんが、クラウド運用とエージェントが交差する実務領域として重要です。
- なぜ面白いか:
  - 技術: IaC修復は、コード生成だけでなく、クラウド状態・ポリシー・依存関係を検証しながら直す必要があり、エージェント評価に向いた現実的タスクです。
  - 人文: インフラの自動修復は、誰が停止・変更・復旧の責任を持つのかを鋭く問います。便利な修復エージェントほど、運用者の判断を置き換えるのではなく、責任の線を濃くする必要があります。

## arXiv / 学術
- TerraRepair: A Tool-Grounded LLM Agent for Infrastructure-as-Code Repair — http://arxiv.org/abs/2607.11390v1
- NKI-Agent: Domain-Specific Fine-Tuning and Agentic Tool Use for Neuron Kernel Generation — http://arxiv.org/abs/2607.04395v1（直近14日外だがAWS Neuron関連として参考）
- Registry-Governed Agent Lifecycle: Completing EDDOps with Evaluation-Driven Registration, Promotion, and Retirement on AWS AgentCore — http://arxiv.org/abs/2607.00345v1（直近14日外だがAgentCore運用論として参考）

## メモ
- Boris Cherny優先: AWSトピックのため対象外。
- 日本語アカウント: awswhatsnew_jp、Serverworks周辺、日本語AWSコミュニティの共有を重視。
- 注意点・誇張リスク: Web検索ツールが未設定だったため、X検索、arXiv API、公式ページへの直接HTTP到達確認で補完しました。AWS公式What’s New個別ページの本文照合は限定的で、source limitationがあります。

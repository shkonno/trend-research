# Harness engineering トレンド調査 (2026-08-11)

- 調査日: 2026-08-11
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「AIエージェントを速く作る」段階から、「仕様・評価・デプロイ・運用・監査を一つの安全なハーネスに通す」段階へ移っています。

## トップ5

### 1. Engineering for the Agentic Era: How to Spec, Build, Test, and Operate AI Systems
- 出典: Harness Blog / Technical
- 日付: 2026-08-05
- リンク: https://www.harness.io/blog/engineering-for-the-agentic-era-how-to-spec-build-test-and-operate-ai-systems
- 要約: Harness は、AIエージェントがコード生成速度を上げる一方で、テスト・運用統制・失敗モード分析が追いつかなければ「バグも10倍速く本番へ行く」と整理しています。6か月の社内SDLC再設計から、仕様ベース開発、検証、ガバナンス、運用準備を柱にする「agentic engineering excellence」を提示しています。
- なぜ面白いか:
  - 技術: プロンプト単体ではなく、仕様・制約・テスト・運用条件をエージェントの実行環境に接続する点が、Claude Code や loop engineering の「ループを安全に閉じる」発想と直結します。
  - 人文: ここでの主役は万能なAIではなく、速度に酔わずに事故の語りを減らす組織設計です。職人芸としての開発から、共同体が守れる手順・記録・責任分界へ重心が移る兆候として読めます。

### 2. How Do You Actually Test an AI Agent? A Look at Harness AI Evals
- 出典: Harness Blog / Technical
- 日付: 2026-08-05
- リンク: https://www.harness.io/blog/how-do-you-actually-test-an-ai-agent-a-look-at-harness-ai-evals
- 要約: 非決定的なAIエージェントに `assertEqual` 型の単純テストは効きにくいとして、Harness AI Evals はオフライン評価と本番オンライン評価で同じメトリクス・データセットを使う「一つの品質基準」を提案しています。Target、Dataset、Metrics、Threshold の4構成要素と、47以上の組み込みメトリクス、LLM-as-Judge、決定的チェック、プロンプトインジェクション検出、マルチステップ軌跡評価を扱います。
- なぜ面白いか:
  - 技術: エージェントの品質ゲートをリリースパイプラインに接続し、事前評価と本番観測のドリフトを減らす設計は、AIネイティブなCI/CDの中核になります。
  - 人文: 「もっと賢いモデル」ではなく「何を良い応答と呼ぶか」を組織が明文化する話であり、評価基準そのものが価値判断になります。AIの失敗を個人の勘ではなく、共有可能な制度に変える動きとして重要です。

### 3. Chaos Hub in docs, Prompt Library for MCP: what's new in Resilience Testing
- 出典: Harness Blog / Technical
- 日付: 2026-08-05
- リンク: https://www.harness.io/blog/chaos-hub-in-docs-prompt-library-for-mcp-whats-new-in-resilience-testing
- 要約: Harness Resilience Testing は、Chaos Hub をドキュメント内に統合し、Kubernetes、クラウド、Linux、Windows 向けの200以上のfault/probe/actionテンプレートを見つけやすくしました。さらに Harness MCP 用の Prompt Library を追加し、Cursor、Claude、Claude Desktop、Windsurf などのMCP対応クライアントから自然言語でレジリエンス実験を設計・実行しやすくしています。
- なぜ面白いか:
  - 技術: IDE内のClaude系ワークフローとMCPを介して、カオス実験の発見、パラメータ化、実行、分析をつなぐため、loop engineering の「観測→介入→再評価」が実運用に近づきます。
  - 人文: 障害を「起きてから責めるもの」ではなく、「事前に共同でリハーサルするもの」として扱う文化転換が見えます。自然言語プロンプトのライブラリ化は、専門家だけが知っていた儀式をチームの共通語へ変える試みです。

### 4. Get Ship Done: Everything We Shipped in July 2026
- 出典: Harness Blog / Technical
- 日付: 2026-08-03
- リンク: https://www.harness.io/blog/shipped-in-july-2026
- 要約: Harness は7月に71件の機能を出荷し、Agent DLC、Harness CLI 3.0、Worker Agent governance、Kubernetes canary、AIBOM などをまとめて紹介しました。Agent DLC はAIエージェントの build/test/store/deploy/operate/govern を既存のパイプライン、ポリシー、監査証跡に載せる方向で、CLI 3.0 は人間とエージェントが同じコマンド体系と認証フローを使うことを狙っています。
- なぜ面白いか:
  - 技術: AIエージェントを「特別な実験物」ではなく、成果物、ランタイム、設定、費用、セキュリティ資産として扱うプラットフォーム化が進んでいます。
  - 人文: 人間とエージェントが同じCLIを使うという発想は、道具の使い手の境界を曖昧にします。誰が操作し、誰が承認し、誰がログ上の主体になるのかという、労働と責任の再設計を迫る点が面白いです。

### 5. Q2 2026 Product Update: Harness Continuous Delivery & GitOps
- 出典: Harness Blog / Company News
- 日付: 2026-08-06
- リンク: https://www.harness.io/blog/q2-2026-product-update-harness-continuous-delivery-gitops
- 要約: Q2 2026 の Harness CD/GitOps は38件の改善をまとめ、Kubernetes progressive canary、ネイティブAIエージェントデプロイ、検証感度の細分化、GitOpsアプリケーションのワンクリックロールバックなどを発表しました。GitOpsエンティティやパイプラインステージに対して Harness AI が設定エラー診断や修復提案を行う点も強調されています。
- なぜ面白いか:
  - 技術: AIエージェントのデプロイを通常サービスと同じcanary、approval gate、OPA policy、GitOps rollbackで扱うことで、AIのリリース管理が既存SRE/Platform Engineeringの言語に翻訳されます。
  - 人文: 新しい主体であるエージェントを、例外ではなく制度の内側に入れる話です。イノベーションを止めずに、組織が理解できる監査・承認・撤回の物語へ落とし込むことが、AI導入の社会的な摩擦を下げます。

## arXiv / 学術
- 本調査時点で確認されませんでした。arXiv API は本実行中にタイムアウトおよび 429 を返したため、確認範囲は限定的です。架空IDを避けるため、未確認の論文・arXiv IDは記載していません。

## メモ
- Boris Cherny優先の有無: `x_search` が利用クレジット不足で失敗したため、Boris Cherny / @bcherny の直近X投稿は確認できませんでした。Webで確認できた接点としては、Harness MCP Prompt Library が Claude / Claude Desktop を明示的な利用先に含めており、Claude Code 的なIDE内エージェント運用との親和性が高いです。
- 日本語アカウントの扱い: `x_search` 不可のため日本語Xコミュニティは未確認です。代替としてBing RSS検索を行い、日本語圏では Zenn の「Harness Engineeringとは何か？プロンプトの次に来る『AI…』」が検索結果に出ましたが、本文取得を検証できなかったためトップ5には入れず、注意メモ扱いにしました。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定、X検索は spending-limit、arXiv は timeout/429 でした。そのため本日のトップ5は、リンクと本文を直接取得できた Harness 公式ブログ/RSSを中心に選定しています。企業ブログ由来のため、製品訴求を含む点には注意が必要です。

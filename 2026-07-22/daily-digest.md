# Daily X + Web + arXiv Trend Digest — 2026-07-22

- 対象トピック: 12件
- 生成状況: 12/12件のトピックファイルを確認
- 音声: TTS/audio は無効（新規 mp3 なし）

## 今日の総括

今日の横断テーマは、AIを「賢いモデル」として眺める段階から、証拠・権限・停止条件・共有記憶・組織文化を含む“作業制度”として設計する段階への移行です。NotebookLM/Gemini Notebook、Claude Code、AWS、各種agent harnessの動きは、生成AIが個人の補助ツールから、チームや行政、セキュリティ運用、研究作業を動かすインフラへ変わりつつあることを示しています。

## トピック別ハイライト

### NotebookLM
- Googleによる「Gemini Notebook」への改称は、単なるリブランドではなく、Geminiアプリ、Google検索、ノート単位コンテキストを横断する研究作業空間化のサインです。
- 安全なクラウドコンピュータによるコード実行、モバイル版Driveソース追加、社内資料投入の日本語実践例が並び、「読むAI」から「資料を根拠に分析・検算するAI」へ進んでいます。

### Loop engineering
- `harness training`、構造化フィードバック、Kitaruの記録・再生可能なagent runtimeなど、モデル外側のループをどう訓練・観測・改善するかが主題になっています。
- FizzBeeやPinpointのように、実装前の要求精密化や視覚的レビューをエージェントループに戻す道具が、AI開発を“会話”から“反復可能な制作工程”へ近づけています。

### AWS
- Lambdaコンソールのcoding agent向けセットアッププロンプト、BedrockでのOpenAI GPT-5.6 Sol/Terra/Luna提供、CloudWatch coding agent insightsが、AIコーディングをクラウド運用対象へ押し上げています。
- GuardDuty investigation agentやAWS JapanのClaude/Kiroワークショップは、AI導入が機能追加だけでなく、監査・予算・チーム学習・セキュリティ判断の再設計であることを示しています。

### Harness engineering
- GPUカーネル生成向けHarness Engineering論文、DataFlow-Harness、FlashRTなど、評価・検証・計測・デプロイ最適化を担う外部ハーネスが主役になっています。
- Claude Code Actionや日本語圏のClaude Code設定スナップショットは、GitHub Actionsやローカル設定を安全柵として使い、AI作業を既存の承認文化に埋め込む方向を示します。

### sharp LLM usage
- Claude Codeチーム対談では、単発プロンプトではなく、モデルにサブエージェント群とワークフロー自体を設計させる実践が語られています。
- SWE-Pruner Pro、web_fetch漏えい事例、property-template testingは、鋭いLLM利用の本質が「たくさん渡す」ことではなく、削る・分離する・検証することにあると示しています。

### AI agent trends
- Self-State Attacks論文は、自己ホスト型エージェントのメモリや設定が攻撃面になることを明確化し、エージェントの“自己状態”を監査対象にしています。
- Claude CodeのMCP接続、Context Mode/Headroom、claude-org-ja、Seamlessは、イベント駆動・共有記憶・複数ワーカー化を通じて、エージェントを半自律的な運用者へ近づけています。

### Claude Code
- Week 29のMCP接続つきArtifactsとスクリーンリーダーモードは、Claude Codeの成果物がライブUI化し、同時にアクセシビリティも中核機能として扱われ始めたことを示します。
- v2.1.217のサブエージェント暴走抑止、予算停止、トランスクリプト保護、ワークスペース隔離修正は、信頼が能力ではなく「どこで止まるか」に宿ることをよく示しています。

### Ethics of AI Agents
- PwC×トレンドマイクロの日本語レポート紹介は、自律レベル、NHI管理、HITL、外部環境との安全な相互作用を実務ガバナンスの言葉で整理しています。
- AI-to-AI managementの強制・欺瞞ベンチマーク、Delegated-Autonomy Boundary、CAVAは、委任・承認・行為証跡をAI倫理の中心問題へ引き上げています。

### Philosophy of Loop Engineering
- Proof-or-Stop、VRR-Stop、LOGOSはいずれも、AIループを信じるのではなく、証拠ゲート、停止規則、versioned agent packs、監査traceで制度化する方向を示しています。
- 反復そのものを善とせず、いつ止めるか、誰が進化を許すかを問う点で、loop engineeringはプラグマティズム、サイバネティクス、政治哲学が交差する実践になっています。

### Anthropology of Agentic AI
- agentic code reviewの大規模研究は、AIがレビューを速くしても品質向上は自動ではないことを示し、レビューを合意形成・学習・通過儀礼として再考させます。
- Deloitte、Anthropic Economic Index、日本語の企業向けAIエージェント解説を合わせると、Agentic AIは肩書ではなく日々のタスク分担・承認・責任境界を変える文化現象として見えてきます。

### History of Automation
- ラスベガスのホスピタリティ業界では、AI以前の自動化が労働契約・通知・補償の問題として制度化されており、自動化史を発明史ではなく交渉史として読ませます。
- 専門サービスの新人パイプライン再設計、Codex利用データ、Computer Use Agentsは、自動化が工場からホワイトカラーの徒弟制・画面操作・責任分界へ移ったことを示します。

### DDD
- 自然言語要求からマイクロサービス構成を作るマルチエージェント実験や、教育ドメインDDDマニュスクリプトは、DDDがAI時代のドメイン探索・概念整理・設計レビューの会話基盤になり得ることを示します。
- Rust向けddd-toolkitやDDD/CQRS専門家のAIフェロー就任は、AI導入で重要なのがプロンプトだけでなく、ユビキタス言語、境界、組織知を保つ設計文化であることを補強しています。

## 横断テーマ

### 技術テーマ
1. **モデル外側の工学化**: harness、loop、MCP、CloudWatch、CAVA、Proof-or-Stopなど、モデルの出力を評価・制御・記録する外部構造が急速に重要になっています。
2. **コンテキストと記憶の編集**: SWE-Pruner Pro、Headroom、Seamless、Gemini Notebookは、情報を増やすより、何を残し、どこに保存し、誰が読めるかを設計する方向へ向かっています。
3. **エージェントの運用基盤化**: AWS、Claude Code、GitHub Actions、MCP接続、GuardDuty agentは、AIエージェントを個人ツールではなく、クラウド・CI/CD・セキュリティ・監査の管理対象にしています。
4. **検証と停止条件の重要化**: property-based testing、VRR-Stop、Proof-or-Stop、構造化フィードバックは、「もう一度やらせる」より「証拠がないなら止める」設計の必要性を示しています。

### 人文・社会テーマ
1. **委任の倫理**: AIが行為するほど、「誰が許可し、誰が止め、誰が責任を負うのか」が中心問題になります。
2. **仕事の儀礼の再編**: コードレビュー、要求定義、社内問い合わせ、新人育成、行政AI利用は、単なる効率化ではなく、組織の合意形成や学習の場を作り替えます。
3. **信頼は感情ではなく制度になる**: 監査ログ、receipt、権限境界、契約条項、HITLは、AI時代の信頼を繰り返し確認可能な手続きへ変えています。
4. **ローカル文化への翻訳**: 日本語圏のGemini Notebook活用、AWSワークショップ、claude-org-ja、DDD/AIフェロー、デジタル庁「源内」は、AIエージェントが各地域・組織の言葉に翻訳されて初めて定着することを示しています。

## 未完了/品質注意

- 欠落トピック: なし（12/12件確認）。
- hard issue files: なし。
- source limitation warning: 7件（Harness engineering / sharp LLM usage / AI agent trends / Ethics of AI Agents / Philosophy of Loop Engineering / Anthropology of Agentic AI / DDD）。主因は X検索のクレジット制限、Web検索/抽出基盤の未設定・ブロックで、各トピックでは代替として公式ページ、GitHub、RSS、直接HTTP取得、arXiv API等を利用しています。
- pre-run digest warnings: `overview_md_missing`, `latest_md_stale` は、本ジョブで `trend_scan.py` 実行により解消予定です。
- TTS/audio: disabled。新規mp3は作成していません。

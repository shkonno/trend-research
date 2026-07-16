# AI agent trends トレンド調査 (2026-07-14)

- 調査日: 2026-07-14
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AIエージェントの話題は「単体チャットの賢さ」から、長時間の実作業・ツール利用・組織運用・安全評価へ移っている。

## トップ5

### 1. The Making of Claude Code
- 出典: Anthropic Features
- 日付: 2026-07-06
- リンク: https://www.anthropic.com/features/making-of-claude-code
- 要約: Claude Code が内部CLIから Anthropic のコーディングエージェントへ育った過程を、研究者・エンジニア・初期ユーザーの視点で語る記事。本文中では、ソフトウェア工学の大きな部分を自動化することが「transformative AI」への経路だという問題意識も示されている。
- なぜ面白いか:
  - 技術: エージェントを単なる補完機能ではなく、CLI・リポジトリ・実行環境・人間のレビューをまたぐ作業システムとして設計している点が重要。
  - 人文: 「コードを書く主体」は個人プログラマから、人間とAIが交互に意図を渡す共同制作体へ変わりつつある。開発者の熟練は、実装力だけでなく、委任・監督・失敗の切り戻しを設計する能力になっていく。

### 2. Introducing Claude Sonnet 5
- 出典: Anthropic News
- 日付: 2026-06-30
- リンク: https://www.anthropic.com/news/claude-sonnet-5
- 要約: Claude Sonnet 5 は「最もagenticなSonnet」として発表され、ブラウザやターミナルなどのツールを使い、計画を立てて自律的に実行できる能力を前面に出している。Claude Code と Claude Platform で利用可能で、BrowseComp や OSWorld-Verified などの評価にも触れている。
- なぜ面白いか:
  - 技術: エージェント性能を、推論・ツール利用・コンピュータ操作・コスト性能の組み合わせで語っている点が、モデル評価の軸を変えている。
  - 人文: 「賢い回答」より「環境内で責任ある行動をする」ことが価値になるほど、AIは道具から半自律的な同僚に近づく。安全性評価も、発話の無害性だけでなく行為の結果責任を含む方向へ広がる。

### 3. ChatGPT is now a partner for your most ambitious work
- 出典: OpenAI News RSS
- 日付: 2026-07-09
- リンク: https://openai.com/index/chatgpt-for-your-most-ambitious-work
- 要約: OpenAI は ChatGPT Work を、アプリやファイルを横断して行動し、必要なら数時間プロジェクトに付き合い、目標を完成物へ変えるエージェントとして紹介している。エージェントの主戦場が、個別タスクではなく長い業務単位に広がっていることを示す発表。
- なぜ面白いか:
  - 技術: 長時間実行・外部アプリ連携・ファイル操作を前提にすると、メモリ、権限、監査ログ、途中介入のUXが中核機能になる。
  - 人文: 「仕事を頼む」経験が、人間の部下・同僚だけでなくAIにも向かうことで、信頼、説明責任、依存の感覚が変わる。成果物だけでなく、誰がどこまで判断したのかという物語が重要になる。

### 4. How Deutsche Telekom is rewiring telecommunications with AI
- 出典: OpenAI News RSS
- 日付: 2026-07-10
- リンク: https://openai.com/index/deutsche-telekom
- 要約: Deutsche Telekom が OpenAI とともに、カスタマーサービス、従業員ワークフロー、ネットワーク運用、音声の未来を含めて「AI-native telco」へ変わる事例として紹介されている。エージェント的AIが実企業の運用設計に入り込む例として注目度が高い。
- なぜ面白いか:
  - 技術: 顧客対応からネットワーク運用まで複数ドメインをまたぐため、エージェントには業務知識、権限分離、例外処理、既存システム統合が求められる。
  - 人文: 通信インフラのような公共性の高い領域でAIが「運用の相棒」になると、効率化と説明責任のバランスが社会的論点になる。ユーザーは速い対応を望む一方で、見えない自動化に対する不安も持つ。

### 5. VEXAIoT: Autonomous IoT Vulnerability EXploitation using AI Agents
- 出典: arXiv
- 日付: 2026-07-10
- リンク: https://arxiv.org/abs/2607.09653
- 要約: LLMベースの脆弱性検出エージェントと攻撃実行エージェントを組み合わせ、IoTGoat と Metasploitable 環境で自律的なIoT脆弱性発見・悪用を評価した論文。260回の実行で全体95.0%の成功率を報告している。
- なぜ面白いか:
  - 技術: マルチエージェント構成が、偵察、計画、攻撃実行というセキュリティ作業の連鎖を自動化できることを示している。
  - 人文: 防御研究として有用である一方、攻撃能力の自動化はデュアルユースの緊張を強くする。エージェント研究は「できること」を増やすだけでなく、誰に、どの環境で、どんな制約付きで許すのかを同時に問う段階に入っている。

## arXiv / 学術

- VEXAIoT: Autonomous IoT Vulnerability EXploitation using AI Agents / 2607.09653 / IoTセキュリティにおける自律型マルチエージェントの実証。
- LLM for EDA in Front-End Design: Challenges and Opportunities / 2607.09616 / EDAにおけるLLM活用を、局所支援から自律的・エージェント的実行へ進む流れとして整理。
- Task-Specific Multimodal Question Answering Agents via Confidence Calibration and Incremental Reasoning for QANTA 2026 / 2607.09623 / 早押し・ボーナス問題に分けたタスク特化型2エージェント設計。

## メモ

- Boris Cherny優先の有無: @bcherny を対象にX検索を試行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、今回のトップ5にはX由来の投稿を採用していない。
- 日本語アカウントの扱い: 日本語クエリでもX検索を試行したが同じ理由で取得不可。代替としてBing RSSで日本語Web検索を行ったが、直近14日の一次情報・実践記事として採用できる強い候補は確認できなかった。
- 注意点・誇張リスク: OpenAI個別記事本文は403で取得できなかったため、OpenAI項目は公式RSSに含まれるタイトル・日付・リンク・説明文に限定して要約した。AnthropicとarXivはページ/API本文を確認した。Web検索ツールとweb_extractは未設定だったため、直接HTTP取得とBing RSS、arXiv APIで補完した。

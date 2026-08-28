# AI agent trends トレンド調査 (2026-08-28)

- 調査日: 2026-08-28
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AIエージェントの焦点は「賢いチャット」から、既存の業務チャネル・開発基盤・監査可能な実行ループへ埋め込む運用設計に移っている。

## トップ5

### 1. Codex as a platform: build on the open agent harness
- 出典: OpenAI Developers Blog
- 日付: 2026-08-27
- リンク: https://developers.openai.com/blog/codex-as-a-platform
- 要約: OpenAIはCodexを単体アプリではなく、CLI、IDE、SDK、app-serverを支える「オープンなエージェント・ハーネス」として位置づけ直した。文脈保持、ツール利用、サンドボックス、承認要求、イベント配信をアプリ側に組み込めるため、運用ダッシュボードやセキュリティ調査などの専用業務にエージェントを埋め込む方向が強く示された。
- なぜ面白いか:
  - 技術: エージェントの価値をモデル単体ではなく、状態管理・承認・ツール境界・イベントストリームを含む実行基盤として切り出している点が重要。
  - 人文: これは「人がAIツールへ移動する」のではなく「AIが人間組織の既存の仕事場へ入る」変化であり、職場の儀礼、責任分担、監査文化を再設計する話でもある。

### 2. Copilot code review: Resolution reasons and expanded capabilities
- 出典: GitHub Changelog
- 日付: 2026-08-27
- リンク: https://github.blog/changelog/2026-08-27-copilot-code-review-resolution-reasons-and-expanded-capabilities
- 要約: GitHub Copilot code reviewが、Copilot cloud agentなどボット作成PRへの自動レビューと、従来制限を超える大規模PRレビューに対応した。さらにレビューコメントの解決理由として「Addressed」「Won’t fix」「Incorrect」を送れるようになり、エージェント生成物のレビュー・フィードバック循環が明確になった。
- なぜ面白いか:
  - 技術: エージェントが作ったPRを別のエージェント的レビュー機構で検査し、その解決理由を構造化データとして回収する運用ループが見える。
  - 人文: 「AIが書き、AIがレビューし、人間が承認する」流れでは、人間の役割は作業者から制度設計者・例外判断者へ寄っていく。解決理由の選択肢は、機械に対する小さな異議申し立ての形式にもなる。

### 3. The new GitHub Copilot experience in Slack
- 出典: GitHub Changelog
- 日付: 2026-08-21
- リンク: https://github.blog/changelog/2026-08-21-the-new-github-copilot-experience-in-slack
- 要約: Slack上で`@GitHub`に話しかけ、調査、計画、Issue作成、修正実装、検証、PR作成までをCopilot cloud agentへ渡せる公開プレビューが発表された。Slack Codeの専用チャンネルでは、計画、差分、HTMLプレビューなどをチームで見ながらエージェントを方向修正できる。
- なぜ面白いか:
  - 技術: エージェント実行がIDE内の個人作業から、Slackスレッド・専用チャンネル・PRをまたぐ非同期の共同作業プロトコルになっている。
  - 人文: プロンプトや判断過程がチームの会話空間に残るため、AI利用のノウハウが個人の秘伝から組織の観察可能な実践へ変わる。これは「ペアプロ」よりも「公開された仕事の劇場」に近い。

### 4. Shared agentic work with GitHub Copilot in Microsoft Teams
- 出典: GitHub Changelog
- 日付: 2026-08-21
- リンク: https://github.blog/changelog/2026-08-21-shared-agentic-work-with-github-copilot-in-microsoft-teams
- 要約: Microsoft Teamsの会議・チャンネル・DMで`@GitHub`を呼び、会議中の決定事項をCopilot cloud agentの作業セッションへ変換できるようになった。参加者は調査を見守り、文脈を追加し、書き込み権限があれば変更の実行を指示でき、作業はターミナル、Copilot app、IDEへ継続できる。
- なぜ面白いか:
  - 技術: 会議チャットをエージェントのタスク起票面にし、クラウドサンドボックス、予算、権限、監査を組織設定で制御する点が実運用寄り。
  - 人文: 会議の「あとでやる」がその場で半自動の作業単位へ変わると、議事録・責任者・締切という管理文化も変わる。便利さと同時に、発言がすぐ作業命令化される緊張も生まれる。

### 5. When May an Agent Stop? Evidence-Carrying Termination for Tool-Using LLMs
- 出典: arXiv
- 日付: 2026-08-22
- リンク: https://arxiv.org/abs/2608.23623v1
- 要約: ツール利用型LLMエージェントがいつ「完了」と言ってよいかを、証拠付き終了（Evidence-Carrying Termination, ECT）として定式化した研究。各回答主張をスコープ内のトレース証拠と決定的リプレイに結びつける型付き証明書を要求し、合成タスクでは危険な完了を大きく抑えたと報告している。
- なぜ面白いか:
  - 技術: エージェントの停止条件を自然言語の自己申告ではなく、検証可能な証拠・スコープ・再実行に結びつけている。
  - 人文: 「仕事が終わった」と誰が言えるのかは、工場・官僚制・ソフトウェア開発を貫く古い社会的問題でもある。AI時代の完了報告には、信頼ではなく検収可能性が必要になる。

## arXiv / 学術

- When May an Agent Stop? Evidence-Carrying Termination for Tool-Using LLMs / arXiv:2608.23623v1 / 2026-08-22 / ツール利用エージェントの「完了」条件を証拠・スコープ・リプレイで検証する研究。
- Trace Integrity for LLM Data Agents: A Vision for Auditable Structured Reasoning in Real-World Systems / arXiv:2608.26036v1 / 2026-08-26 / 構造化データを扱うLLMエージェントで、答えの正しさだけでなく計算トレースの監査可能性を評価基準にする提案。
- FABRICA: Agentic CUDA-to-CSL Translation and Optimization for Wafer-Scale Systems / arXiv:2608.25124v1 / 2026-08-25 / GPUカーネル移植にエージェント的な変換・最適化ループを使う研究。

## メモ

- Boris Cherny優先の有無: 優先確認したが、X検索ツールはクレジット上限で失敗したため、@bchernyの直近X投稿は本調査では確認できなかった。Web検索ではBoris Cherny/Claude Code関連の二次まとめ（2026-08-20の解説記事、2026-07-17のAI導入段階記事など）は見つかったが、一次情報性を優先してトップ5には採用しなかった。
- 日本語アカウントの扱い: X検索が利用不能だったため日本語圏X実践は確認できなかった。代替としてDuckDuckGo/Jina経由で日本語Webを確認し、QiitaやZennのClaude Code/MCP設定記事は見つかったが、主に2026年2月〜3月の記事で対象期間外のためトップ5から外した。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定、X検索はxAIクレジット上限で失敗した。代替としてJina Reader経由の検索・公式ページ取得、GitHub Changelog、OpenAI Developers Blog、MCP公式ブログ、arXiv APIを使用した。MCP 2026-07-28仕様は重要だが直近14日を超えるため、今回はトップ5ではなく背景情報扱いにした。

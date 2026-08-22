# AI agent trends トレンド調査 (2026-08-22)

- 調査日: 2026-08-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの焦点は「賢い単体ツール」から、標準化・監査・チーム内運用・安全な権限管理を備えた“組織の作業インフラ”へ移っている。

## トップ5

### 1. Agent Plugins 1.0: スキルとMCPサーバーを単一パッケージ化する標準
- 出典: GitHub Changelog
- 日付: 2026-08-12
- リンク: https://github.blog/changelog/2026-08-12-agent-plugins-1-0-in-vs-code-copilot-cli-and-the-copilot-app/
- 要約: GitHubは、VS Code、Copilot CLI、Copilot appなどで使える Agent Plugins 1.0 の一般提供を発表した。スキルとMCPサーバー設定をひとつのプラグインとしてまとめ、AWS、Anysphere、Microsoft、OpenAI、Vercel、Googleなど複数ベンダーをまたぐ配布・運用を狙う。
- なぜ面白いか:
  - 技術: エージェントの「能力」を `skills/` と `mcp.json` で再利用可能な単位にし、クライアントごとのマニフェスト重複を減らす標準化レイヤーになっている。
  - 人文: これはツール市場の覇権争いというより、職人の手順書・社内の暗黙知・外部ツールへのアクセス権を、どの組織がどの形式で所有するかという制度設計の話でもある。

### 2. Slack / Microsoft Teams から共有エージェント作業を開始する GitHub Copilot
- 出典: GitHub Changelog
- 日付: 2026-08-21
- リンク: https://github.blog/changelog/2026-08-21-the-new-github-copilot-experience-in-slack/ / https://github.blog/changelog/2026-08-21-shared-agentic-work-with-github-copilot-in-microsoft-teams/
- 要約: GitHubは、SlackおよびMicrosoft Teamsで `@GitHub` にメンションしてCopilot cloud agentセッションを開始し、会話から調査・実装・検証・PR作成へ進めるプレビューを公開した。Teamsでは会議中の決定をコード作業に変換し、Slackでは専用のコードチャンネルで進捗や差分を共有できる。
- なぜ面白いか:
  - 技術: エージェントがIDE内ではなくチャット空間から安全なクラウドサンドボックスへ接続され、非同期に作業しつつPRや成果物へ受け渡す運用モデルが明確になった。
  - 人文: 「誰がエージェントに依頼したのか」「会議のどの合意がコード変更に変わったのか」が可視化され、ソフトウェア開発の責任と記録が会話ログ中心に再編される。

### 3. GitHub Copilot の MCP allowlists: 企業管理設定でMCPサーバーを許可・拒否
- 出典: GitHub Changelog
- 日付: 2026-08-06（直近14日より少し古いが、MCP運用上重要なため採用）
- リンク: https://github.blog/changelog/2026-08-06-mcp-allowlists-in-enterprise-managed-settings/
- 要約: GitHubは、enterprise managed settings に `allowedMcpServers` と `deniedMcpServers` を追加し、Copilot app、Copilot CLI、VS Code上で実行可能なMCPサーバーを中央管理できるようにした。URL、ローカルコマンド、サーバー名でマッチし、不正確な設定はfail closedでブロックされる。
- なぜ面白いか:
  - 技術: MCPの普及に伴う最大の実務課題である「便利なツール接続」と「危険な権限拡大」の境界を、企業ポリシーとして機械的に適用できる。
  - 人文: エージェント時代のセキュリティは、個人の注意力ではなく、組織がどの外部行為者を信頼できるとみなすかの統治問題になっている。

### 4. HarnessRouter Community Edition: Claude Code / Codex / Hermes などのハーネスを統一API化
- 出典: GitHub / Hacker News
- 日付: 2026-08-17（HN投稿）・リポジトリ作成 2026-08-09
- リンク: https://github.com/HarnessRouter/harnessrouter
- 要約: HarnessRouter Community Editionは、Codex、Claude Code、Hermesなど複数のエージェントハーネスを、セッション、ストリーミング、ファイル、キャンセル、失敗処理を含む統一APIで動かすセルフホスト基盤として公開されている。READMEではアカウント不要・テレメトリなし・自分のAPIキーとデータを自分の環境に置く設計を強調している。
- なぜ面白いか:
  - 技術: モデルやエージェントCLIが増えるほど、共通の実行・監視・キャンセル・失敗復旧プロトコルが必要になり、ハーネス層そのものがインフラ化している。
  - 人文: どのエージェントに仕事を任せるかだけでなく、「作業の場」を誰が支配するかが重要になっている。セルフホスト志向は、便利さと主権のトレードオフに対する開発者側の回答に見える。

### 5. MidTool: MCPスキルを含むツール利用向け mid-training データ合成
- 出典: arXiv
- 日付: 2026-08-20
- リンク: https://arxiv.org/abs/2608.20314v1
- 要約: `MidTool: Mid-training Data Synthesis for Agentic Tool Use` は、Web、PDF、コード、実API、MCPスキル、文書接地ワークフローから合成したコーパスで、LLMの一般的なツール利用能力をmid-training段階から鍛える研究。Qwen3-4B/8Bを対象に、BFCL、tau2-Bench、MCP Universeで改善を報告している。
- なぜ面白いか:
  - 技術: ツール利用を後段のSFT/RLだけに任せず、モデルの中間学習で「ツールの使いどころ、引数の接地、ワークフロー合成、欠落情報からの回復」を作り込む方向性を示す。
  - 人文: エージェントの能力は単なる推論力ではなく、環境内の道具をどう読むかという“実践知”に近い。これは人間の徒弟制や作業文化がモデル訓練に翻訳されていく過程としても読める。

## arXiv / 学術
- `MidTool: Mid-training Data Synthesis for Agentic Tool Use`（arXiv:2608.20314v1, 2026-08-20）: MCPスキルや実APIを含む合成データで、汎用ツール利用能力をmid-trainingから伸ばす研究。
- `A three-dimensional typology of agency for advanced AI systems`（arXiv:2608.20041v1, 2026-08-20）: AIシステムのagencyを、道徳/法、個人/集団、人間/非人間の三次元で整理する概念枠組み。
- `Inadvertent Context Leakage in Language Models`（arXiv:2608.19857v1, 2026-08-20）: エージェントが保持するカレンダー、認証情報、健康・金融情報などの機微コンテキストが、直接抽出を拒否しても通常応答に漏れうることを分析。

## メモ
- Boris Cherny / @bcherny は優先確認対象だったが、X検索ツールが `personal-team-blocked:spending-limit` で失敗し、HN Algolia検索でも直近該当投稿を確認できなかった。
- 日本語圏実践も検索対象だったが、X検索は同じ理由で利用不能、DuckDuckGoはbot challengeでブロックされたため、今回はGitHub Changelog、GitHub API、HN Algolia、arXiv API、直接HTTP取得を中心に調査した。
- 注意点・誇張リスク: GitHubリポジトリ由来の項目はスター数やREADME更新日時を確認したが、採用事例の成熟度までは未検証。特に新興ハーネス/監査ツールは“面白い兆候”として扱い、本番導入実績とは分けて読む必要がある。

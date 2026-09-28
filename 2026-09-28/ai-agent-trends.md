# AI agent trends トレンド調査 (2026-09-28)

- 調査日: 2026-09-28
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
エージェントの話題は「作れる」から「組織・権限・監査・費用を含めて運用できる」へ、かなりはっきり重心が移っています。

## トップ5

### 1. Claudeプラグイン投稿ポータルと「MCP利用110倍」発表
- 出典: X投稿（@ClaudeDevs、Boris Cherny周辺確認）/ Claude公式ページ
- 日付: 2026-09-25
- リンク: https://x.com/ClaudeDevs/status/2103577007938228300
- 要約: Claude向けプラグインを投稿・審査追跡・利用状況確認できるポータルが告知され、プラグインはMCP connectorとAgent Skillsをパッケージする形として位置づけられました。投稿本文では「Claude製品全体のMCP利用が今年110倍」とされ、MCPが実験的な拡張点から配布・審査・発見性を持つ流通レイヤーに寄っていることが示されています。
- なぜ面白いか:
  - 技術: MCPとSkillsを単なるローカル設定ではなく、審査・配布・利用計測を伴うプラグイン単位へ束ねることで、エージェント拡張のサプライチェーンが形成されつつあります。
  - 人文: 「誰が作った能力を、誰が審査し、どの共同体が信頼して使うのか」という制度設計の問題が前面に出ています。エージェントの能力はコードだけでなく、流通経路と評判の文化によって形作られる段階に入りました。

### 2. Claude Tag in Slackを使ったPR作成・調査ワークフローの実践例
- 出典: X投稿（Boris Cherny / @bcherny）
- 日付: 2026-09-24
- リンク: https://x.com/bcherny/status/2103538666421555200
- 要約: Boris Chernyが、Slack上でClaude Tagを使い「毎日50%以上のPRを書かせている」と述べ、バグ再現、修正PR、データ異常の仮説探索、コード理解ゲームやスライド作成などの具体的プロンプト例を共有しました。Claude Tagが個人connectorも利用できる流れと合わせ、チャット空間がエージェント運用面に変わる例として重要です。
- なぜ面白いか:
  - 技術: Slackスレッド、個人connector、コード実行、PR作成、長い仮説検証を一続きの業務ループとして扱う点が、単発AIチャットとは異なる運用パターンを示しています。
  - 人文: チームの「依頼」「観察」「レビュー」の会話に非人間の作業者が常駐することで、職場の役割分担や責任感覚が変わります。便利さだけでなく、誰が最終判断者なのかを明示する儀礼が必要になります。

### 3. Claude Code v2.1.283: prompt-audit、モデル制御、OTel tool output、load test mode
- 出典: GitHub Release（anthropics/claude-code）
- 日付: 2026-09-25
- リンク: https://github.com/anthropics/claude-code/releases/tag/v2.1.283
- 要約: Claude Code v2.1.283では、`/doctor prompt-audit`によるCLAUDE.md・skills・agents・commandsの古いプロンプトパターン監査、`availableModelsMatch`や`deniedModels`による管理設定、MCP tool/WebFetch/WebSearch出力のOpenTelemetry記録、gatewayの`load_test_mode`などが追加されました。エージェントを個人CLIから企業運用基盤へ近づける変更がまとまっています。
- なぜ面白いか:
  - 技術: プロンプト資産の棚卸し、モデル許可リスト、ツール出力の観測、上流に送らない負荷試験が同時に入ったことで、エージェント運用のSRE/Platform Engineering化が進んでいます。
  - 人文: 「よいプロンプト」は個人の工夫から組織の保守対象へ変わっています。エージェントを雇うことは、文書・権限・監査ログという新しい職場インフラを持つことでもあります。

### 4. MCP TypeScript SDK 2.1系: request-time OAuth scope challenge
- 出典: GitHub Release（modelcontextprotocol/typescript-sdk）
- 日付: 2026-09-23
- リンク: https://github.com/modelcontextprotocol/typescript-sdk/releases/tag/%40modelcontextprotocol%2Fserver%402.1.0
- 要約: MCP TypeScript SDKの`@modelcontextprotocol/server@2.1.0`では、tools/resources/prompts等に対するリクエスト時OAuth scope challengeが追加されました。各primitiveの`scopeChallenge` callbackが認証情報とリクエストを見て、必要scope不足ならHTTP 403と`insufficient_scope` challengeを返せるようになります。
- なぜ面白いか:
  - 技術: MCPサーバーが「接続できる/できない」だけでなく、呼び出し対象ごとに実行直前の権限不足を表現できるようになり、企業内ツール連携の最小権限設計に近づいています。
  - 人文: エージェントに権限を渡す場面では、人間の信頼がしばしば一括委任になりがちです。細かなscope challengeは、委任をより会話的・条件付きの社会契約に戻す試みとして読めます。

### 5. Screen Before You Serve: 1.4億規模CXエージェントを本番前シミュレーションで選別
- 出典: arXiv
- 日付: 2026-09-24
- リンク: http://arxiv.org/abs/2609.30137v1
- 要約: Nubankの高ボリュームなカード配送・管理チャットサポートを対象に、合成顧客と模擬ツール出力で多段エージェントワークフローを本番前に検証する「Snowglobe」シミュレーションを報告しています。手動E2Eテストや本番A/Bだけでは拾いにくい、規制産業での信頼劣化リスクを減らす実践的な運用研究です。
- なぜ面白いか:
  - 技術: 本番バックエンドを叩かずにツール利用・会話遷移・評価器を組み合わせ、候補エージェントを事前スクリーニングする設計は、AI agentのCI/CDとして非常に具体的です。
  - 人文: 顧客は実験対象ではなく、失敗時に生活上の不利益を受ける当事者です。シミュレーションで「提供前にふるいにかける」発想は、効率化とケア責任の両立に関わります。

## arXiv / 学術
- `2609.30137v1` — Screen Before You Serve: Simulation for Production Customer Experience AI Agents at 140M Scale（2026-09-24）。本番前シミュレーションによるCXエージェント検証。
- `2609.29901v1` — Working with Agentic “Teammates”: When a New Organizational Actor Collides with the Human Ecosystem of Work（2026-09-24）。職場におけるプロアクティブなAI teammateの組織・信頼・人間のagencyへの影響。
- `2609.28586v1` — Agent Approval Laundering: Transitive Effects Beyond the Approved Invocation（2026-09-23）。承認UIが入口呼び出しだけを記録し、その背後の推移的効果を覆い隠す問題を分析。
- `2609.28585v1` — Persistent Billable State: Denial-of-Wallet Attacks and Defenses in Tool-Calling LLM Agents（2026-09-23）。ツール結果が後続コンテキストで再課金され続ける攻撃面を定式化。
- `2609.28693v1` — Progressive Skill Discovery as Access Control for Tool-Using LLM Agents（2026-09-23）。役割スコープ付き能力配布によるツール利用エージェントのアクセス制御。

## メモ
- Boris Cherny優先: X検索APIはクレジット/サブスクリプション制限で失敗しましたが、`x.com/bcherny`の直接取得でBorisのClaude Tag実践例とClaudeDevsのMCP/Plugin告知を確認しました。
- 日本語アカウントの扱い: X検索API制限により日本語X投稿の横断検索は未完了です。代替としてGitHub検索で日本語圏の実践例（例: `SpirrowGames/spirrow-mindwire`、Claude.aiとClaude CodeをファイルI/Oで中継する独立MCPサーバー、2026-09-27更新）を確認しましたが、影響度と検証可能性の観点でトップ5には入れませんでした。
- Web検索の注意: Hermesの`web_search`はFirecrawl未設定で使用不可だったため、公式GitHub Releases、Xページ直接取得、GitHub API、arXiv API、HN Algoliaを用いて補完しました。
- 誇張リスク: X投稿に含まれる「50%以上のPR」「MCP利用110倍」は発信者の実践・公式投稿ベースの数値であり、独立検証された業界全体の統計ではありません。

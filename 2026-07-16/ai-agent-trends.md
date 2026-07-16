# AI agent trends トレンド調査 (2026-07-16)

- 調査日: 2026-07-16
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの焦点は「賢いデモ」から、MCP・記憶・フック・監査・自己改善ループを備えた、運用可能な作業環境づくりへ移っている。

## トップ5

### 1. Boris Chernyの「Loops」とエージェントネイティブなコードベース論
- 出典: X投稿（Boris Cherny / @bcherny）
- 日付: 2026-07-15頃
- リンク: https://x.com/bcherny/status/2077460395279692197
- 要約: Boris Chernyは、優れたエンジニアが従来から行ってきたlint・CI・テスト・運用スクリプト化を、AIエージェント時代には「人間とエージェント軍団の両方を加速する永久ループ」として再定義している。CLAUDE.md、REVIEW.md、skills、コードコメント、memoriesにドメイン知識を埋め込み、同じ失敗を二度プロンプトで直さず、仕組みとして潰す姿勢が中心。
- なぜ面白いか:
  - 技術: 一回限りのプロンプト改善ではなく、lint・CI・hooks・skills・メモリに知識を移し、将来の複数エージェントが同じ品質基準で動くようにする設計思想が明確になっている。
  - 人文: これは「熟練者の暗黙知」をチームの共有インフラへ変換する運動でもあり、オンボーディングや職能境界の意味を変える。うまくいけば新人や非エンジニアの参加余地を広げるが、同時に誰の判断基準を標準化するのかという権力の問題も生む。

### 2. Claude Code `/checkup`：エージェント環境にも「掃除」と「健康診断」が必要になる
- 出典: X投稿（Boris Cherny / @bcherny）
- 日付: 2026-07-08頃
- リンク: https://x.com/bcherny/status/2074997570317779038
- 要約: Claude Codeの`/checkup`は、未使用skills・MCP・pluginsの整理、CLAUDE.mdの重複削減、大きすぎるルート指示の分割、遅いhooksの無効化、安全なread-onlyコマンドの事前承認などを行う。X検索では、約5.5k tokens/セッションの削減例や、変更をgit diffとして確認できる可逆的な運用が報告されていた。
- なぜ面白いか:
  - 技術: エージェント運用で問題になるのはモデル性能だけでなく、膨張したコンテキスト、壊れた拡張、遅いhooks、過剰なツール露出であり、それを定期点検する機能が第一級のDevExになりつつある。
  - 人文: これはデジタルな作業場にも「片付け」「棚卸し」「儀式」が必要だという話で、AI時代の職人性がプロンプトの華やかさよりも環境保守に宿ることを示している。

### 3. 日本語圏で広がる Claude Code × MCP × Skills の業務特化エージェント実践
- 出典: X投稿群（日本語圏実践例、まるお氏周辺など）
- 日付: 2026-07-02以降
- リンク: https://x.com/Maruo_0314/status/2077340278789447881
- 要約: 日本語圏では、Claude CodeとMCPでSlack・Notion・Gmail等に接続し、議事録要約、タスク抽出、担当割当、フォローまで業務を半自動化する実践例が目立つ。さらに、Skillsを「思考アルゴリズムの資産化」として改善ループに組み込み、音声メモや論点分解から業務判断ロジックを固める動きが強い。
- なぜ面白いか:
  - 技術: MCPをread中心・最小権限で始め、Skillsで判断基準を再利用し、必要に応じてwrite連携へ広げるという現実的な導入パターンが見えている。
  - 人文: 日本語圏の議論は、単なる開発者向け自動化よりも「自分や組織の考え方をどう外部化するか」に寄っており、AI導入が業務文化の翻訳作業になっている。属人化解消の期待がある一方、ノウハウをAIに渡すことで仕事の輪郭が再編される不安も含む。

### 4. MCPは「エージェントの感覚器官」から、設計・標準・監査の対象へ
- 出典: Web（Model Context Protocol公式ドキュメント / GitHub、Bing RSSで2026-07-15確認）およびX投稿群
- 日付: 継続更新（2026-07-15確認）
- リンク: https://modelcontextprotocol.io/docs/getting-started/intro
- 要約: MCP公式ドキュメントは、Claude、ChatGPT、VS Code、Cursorなど広いクライアント/サーバーで利用できるオープンプロトコルとしてMCPを位置づける。X上でも「CLAUDE.md=記憶、hooks=反射、MCP=感覚」という説明が広がり、Obsidian、AWS Lambda、WordPress、社内SaaS、メモリツールなどへの接続例が増えている。
- なぜ面白いか:
  - 技術: MCPは単なるAPIラッパーではなく、モデルが説明文を読んでツールを選ぶため、ツール数・説明文・権限・遅延・監査ログの設計がそのままエージェント性能になる。
  - 人文: 「AIに世界を見せる」ための規格が整うほど、何を見せ、何を書き換えさせ、どこで止めるかという組織的な境界設定が重要になる。感覚器官の設計は、同時に倫理的な視野と盲点の設計でもある。

### 5. arXivでMCP/エージェント運用の安全性・再現性・実装研究が一気に増加
- 出典: arXiv検索
- 日付: 2026-07-11〜2026-07-13中心
- リンク: https://arxiv.org/abs/2607.11098
- 要約: 直近のarXivでは、`AgentCheck: A Reproduce-Intervene-Mitigate Workbench for LLM Agents over MCP`（2607.11098）、`Rethinking MCP Security`（2607.11086）、`A Large-Scale Dataset of MCP Implementations on GitHub`（2607.10123）、Claude Code/CodexをPHITSシミュレーションに使う実践研究（2607.11309）などが確認された。特にAgentCheckは、MCPツールのタイムアウト・古い値・説明汚染などを再現し、介入し、緩和策を確認するワークベンチを提案している。
- なぜ面白いか:
  - 技術: エージェント研究の軸が「回答精度」から、壊れたツール、汚染された説明、実行時サーバー、再現可能な失敗注入、動的解析へ拡張している。
  - 人文: エージェントに仕事を任せる社会では、失敗を個人の注意不足ではなく、再現・介入・監査できる制度として扱う必要がある。研究の言葉が、現場の責任分界や説明責任に近づいている点が重要。

## arXiv / 学術
- `AgentCheck: A Reproduce-Intervene-Mitigate Workbench for LLM Agents over MCP`（arXiv:2607.11098、2026-07-13）: MCP上のツール不具合や説明汚染を再現し、緩和策を検証するワークベンチ。
- `Rethinking MCP Security: A Large-Scale Study of Runtime MCP Servers and Security Scanner Reliability`（arXiv:2607.11086、2026-07-13）: MCPサーバーの動的解析とセキュリティスキャナ信頼性を扱う。
- `A Large-Scale Dataset of MCP Implementations on GitHub`（arXiv:2607.10123、2026-07-11）: GitHub上のMCP実装3,238候補を収集・検証するデータセット研究。
- `Toward AI-Agent-Driven Particle Transport Simulations: Implementation of AI-Assisted Workflows for PHITS`（arXiv:2607.11309、2026-07-13）: Codex/Claude Codeで科学計算ワークフローを実行する実践研究。
- `MCP Server Architecture Patterns for LLM-Integrated Applications`（arXiv:2606.30317、2026-06-29、14日枠より少し古いが関連性が高いため掲載）: MCPサーバーの5つの設計パターンとアンチパターンを整理。

## メモ
- Boris Cherny優先: 実施。特に`/checkup`とLoops/agent-native codebaseの投稿を上位に採用した。
- 日本語アカウントの扱い: 実施。Claude Code × MCP × Skillsの日本語圏実践を独立項目として採用した。
- Web検索: Hermesの`web_search`/`web_extract`はFirecrawl未設定で失敗したため、代替としてBing RSSをターミナルから確認し、MCP公式ドキュメント/GitHub等のWeb情報を参照した。DuckDuckGo HTMLはbot challengeで利用不可。
- 注意点・誇張リスク: X由来の運用事例は一次投稿の要約であり、商用成果額や導入効果は検証済み実績として断定しない。Claude Code 4.8等のバージョン言及はX検索結果に見られたが、公式確認が弱いためトップ項目には含めなかった。

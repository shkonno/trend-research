# AI agent trends トレンド調査 (2026-07-20)

- 調査日: 2026-07-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
エージェントの話題は「賢さ」単体から、権限・監査・分業・検索状態管理まで含む運用設計へ急速に寄っている。

## トップ5

### 1. Claude Code 2.1.214/2.1.215: 権限・監査・長時間実行の運用品質が一気に強化
- 出典: GitHub Releases / Changelog（Anthropic Claude Code）
- 日付: 2026-07-19（v2.1.215）、2026-07-18前後（v2.1.214系 changelog）
- リンク: https://github.com/anthropics/claude-code/releases/tag/v2.1.215
- 要約: Claude Code の直近リリースでは、`/verify` と `/code-review` を自動実行せず明示呼び出しに寄せたほか、Bash/PowerShell/Windows/リモートセッションまわりの権限チェック、OpenTelemetry属性、長時間ツール呼び出しのハートビート、背景セッション管理などが多数修正されている。特に「安全に自動化するための失敗閉じ（fail closed）」と「観測可能性」が中心テーマになっている。
- なぜ面白いか:
  - 技術: エージェントCLIの差別化軸がモデル性能ではなく、権限解析・監査ログ・長時間プロセス制御・ツール来歴のような運用基盤へ移っていることを示すリリースです。
  - 人文: 人間がエージェントに仕事を任せる条件は「有能さ」だけでなく、「どこで止まるか」「何を記録するか」「誰が承認したか」という信頼の制度設計です。これはソフトウェア開発の現場が、個人の生産性ツールから小さな組織制度へ変わりつつある兆候です。

### 2. Claude Architect: Claude Codeを“設計者・審査員”にし、実装を隔離サブエージェントへ委任
- 出典: GitHub（Pythoughts-labs/claude-architect）
- 日付: 2026-07-13作成、2026-07-20更新
- リンク: https://github.com/Pythoughts-labs/claude-architect
- 要約: Claude Architect は、Claude Code が仕様作成・証拠確認・レビューを担い、Codex / OpenCode / Pi / Pythinker などの新規コンテキスト実装エージェントへ作業を委任するプラグイン。実装候補は隔離された Git worktree で作られ、ハッシュ固定された成果物と検証証拠を人間が確認してからマージする設計になっている。
- なぜ面白いか:
  - 技術: 単一エージェントの長大コンテキストに頼らず、隔離・検証・候補比較・人間承認をホスト側の仕組みで担保する「エージェント分業」の具体例です。
  - 人文: ここでのClaudeは万能な作業者ではなく、建築家・編集者・審査員のような役割に再配置されています。AIと人間の関係も「命令する/される」から、証拠をもとに採否を決める共同制作のワークフローへ近づいています。

### 3. SearchOS-V1: 検索エージェントの“進捗・失敗・証拠”を共有状態として外部化
- 出典: arXiv
- 日付: 2026-07-16
- リンク: https://arxiv.org/abs/2607.15257v1
- 要約: SearchOS-V1 は、Web検索を行う情報探索エージェントがループや重複探索に陥る問題に対し、Frontier Task、Evidence Graph、Coverage Map、Failure Memory などの明示的状態を持たせる multi-agent framework。検索ツールのミドルウェアが証拠・停滞・予算消費を記録し、未充足のカバレッジへサブエージェントを再配分する。
- なぜ面白いか:
  - 技術: エージェントの失敗をプロンプト改善ではなく、共有状態・ミドルウェア・スケジューリング問題として扱っている点が実運用に近いです。
  - 人文: 調査とは単に情報を集めることではなく、「何を見たか」「何を見落としているか」「どこで失敗したか」を共同体で記憶する営みです。SearchOSは、AIエージェントに研究室や編集部のような集合的記憶を与える試みとして読めます。

### 4. 日本語圏実践: Codex・Claude Code・Copilot CLIを同条件で評価する権限チェックリスト
- 出典: Qiita（ynakayama）
- 日付: 2026-07-20
- リンク: https://qiita.com/ynakayama/items/b16925801f150568658e
- 要約: 開発エージェントを評価する際に、課題・合格条件・作業領域・読み取り権限・変更範囲・テスト・Git差分・作業ログ・失敗履歴を固定して比較するための日本語チェックリスト。`git worktree` による分離、変更ファイル数や差分量の上限、禁止事項、必須チェックを明文化している。
- なぜ面白いか:
  - 技術: Claude Code、Codex、GitHub Copilot CLI の比較を、出力の印象ではなく再現可能な実行条件・検証コマンド・権限境界で評価する実践知としてまとまっています。
  - 人文: 日本語圏でも「AIが書いたコードが良さそう」から、「人間が採否判断できる証拠を残せるか」へ関心が移っています。これはAIエージェントを同僚として迎える前に、職場のルールブックを作る動きです。

### 5. Claude Agent SDKでローカルMCPツール付きエージェントを自作する日本語実装記事
- 出典: Qiita（yureki_lab）
- 日付: 2026-07-20
- リンク: https://qiita.com/yureki_lab/items/d64230d1302b4bb30660
- 要約: Python版 Claude Agent SDK を使い、`query()` による最小構成、`@tool` と `create_sdk_mcp_server` による独自ローカルMCPツール、`permission_mode` の明示、マルチターン時の `ClaudeSDKClient` 利用などを解説している。業務アプリへClaude系エージェントを組み込む際のハマりどころを日本語で整理している点が実用的。
- なぜ面白いか:
  - 技術: MCPが「外部ツール連携の概念」から、Python関数をローカルツールとして安全に露出する実装パターンへ落ちてきています。
  - 人文: エージェント開発は、巨大プラットフォームを使うだけでなく、自分の仕事場の小さな道具や社内APIに人格を与える作業になりつつあります。その一方で、権限モードを誤ると自動化が止まるという現実が、人間の承認と自律性の境界を可視化します。

## arXiv / 学術
- SearchOS-V1: Towards Robust Open-Domain Information-Seeking Agent Collaboration（2607.15257）: 検索エージェントの進捗・証拠・失敗を外部状態として管理するmulti-agent framework。
- Beyond Success Rate: Cost-Aware Evaluation of Offensive and Defensive Security Agents（2607.15263）: セキュリティエージェント評価を成功率だけでなく推論・ツール利用コスト込みで測る提案。
- Bridge Evidence: Static Retrieval Utility Does Not Predict Causal Utility in Multi-Step Agentic Search（2607.15253）: 静的RAGで有用に見えない文書が、次の検索クエリを導く“橋渡し証拠”として因果的に重要になることを測定。
- AutoSynthesis: An agentic system for automated meta-analysis（2607.15247）: 文献検索、スクリーニング、抽出、効果量計算、PRISMA風レポートまでを行うメタ分析エージェント。

## メモ
- Boris Cherny優先の有無: @bcherny を含むX検索を実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、本調査では確認できなかった。
- 日本語アカウントの扱い: X検索は同じ理由で取得できなかったため、日本語圏の実践例はQiita API経由で確認した。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定で失敗したため、WebはGitHub API、GitHub raw、Qiita API、arXiv API、HN Algolia API、公式GitHubリリースに限定した。X由来の話題量・反応数は未確認であり、ランキングは取得できた実リンクと内容の面白さに基づく。

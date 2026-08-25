# AI agent trends トレンド調査 (2026-08-25)

- 調査日: 2026-08-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントは「チャットの補助」から、チームの会話・レビュー・セキュリティ運用・検証可能な自律作業をつなぐ実務インフラへ移りつつあります。

## トップ5

### 1. Shared agentic work with GitHub Copilot in Microsoft Teams
- 出典: GitHub Changelog
- 日付: 2026-08-21
- リンク: https://github.blog/changelog/2026-08-21-shared-agentic-work-with-github-copilot-in-microsoft-teams
- 要約: Microsoft Teams のチャンネル、スレッド、DM から `@GitHub` を呼び、GitHub Copilot のエージェント作業を共同で開始・観察・方向付けできるようにする更新です。エージェントが個人のIDE内だけでなく、チーム会話の文脈に直接入ってくる点が重要です。
- なぜ面白いか:
  - 技術: エージェント実行の入口がIDEやCLIからコラボレーション基盤へ広がり、Issue化前の曖昧な議論をそのまま作業セッションへ変換する流れが強まっています。
  - 人文: 「誰がAIに指示したのか」「チームはどの時点で合意したのか」がチャットログ上に残るため、エージェント運用の責任や合意形成がより社会的な設計課題になります。AI作業が個人技から共同編集的な儀礼へ変わる兆しです。

### 2. Codex as a platform: build on the open agent harness
- 出典: OpenAI Developers Blog
- 日付: 2026-08-19
- リンク: https://developers.openai.com/blog/codex-as-a-platform
- 要約: OpenAI は Codex をアプリ、CLI、IDE 拡張の裏側にある「オープンなエージェント・ハーネス」として位置付け、各社が自社の業務画面や運用ダッシュボードへエージェントループを組み込めると説明しています。記事では、文脈保持、ツール利用、サンドボックス、承認、進捗ストリーミング、失敗処理がハーネスの中核だと整理しています。
- なぜ面白いか:
  - 技術: プロンプト単体ではなく、状態管理・権限境界・承認・ツール呼び出しを含む「実行系」こそがエージェント品質を左右するという実装観が明確になっています。
  - 人文: エージェントを“人格化された相棒”ではなく“制度化された作業ループ”として扱う発想は、職場にAIを入れる際の不安を減らします。一方で、仕事の進め方そのものがハーネス設計者に規定されるため、労働の自由度や監査可能性も問われます。

### 3. Agent Plugins 1.0 in VS Code, Copilot CLI, and the Copilot app
- 出典: GitHub Changelog
- 日付: 2026-08-12
- リンク: https://github.blog/changelog/2026-08-12-agent-plugins-1-0-in-vs-code-copilot-cli-and-the-copilot-app
- 要約: GitHub は Agent Plugins 1.0 を、VS Code、Copilot CLI、Copilot app など複数の互換エージェントクライアントで使える仕組みとして発表しました。AWS、Anysphere、Microsoft、OpenAI、Vercel などと公開された仕様で、プラグインを一度作れば複数クライアントで利用できる方向性が示されています。
- なぜ面白いか:
  - 技術: MCP と並んで、エージェントの拡張点がクライアント非依存の部品として標準化され、ツール統合の重複実装を減らす可能性があります。
  - 人文: エージェントが読む“世界への接続口”が標準化されると、開発者コミュニティはプラグイン生態系を共有できます。同時に、誰の仕様が事実上の門番になるのかというプラットフォーム政治も生まれます。

### 4. Scaling cyber defenders with Daybreak
- 出典: OpenAI Developers Blog
- 日付: 2026-08-21
- リンク: https://developers.openai.com/blog/scaling-cyber-defenders-with-daybreak
- 要約: OpenAI は Daybreak の文脈で、ChatGPT、Codex Security、オープンソースの Codex Security CLI を使い、PRレビュー、リポジトリ調査、既存脆弱性バックログ、CIでの継続チェックをつなぐ運用例を紹介しました。単に脆弱性を列挙するのではなく、証拠収集とレビュー済み修正へ進めることを強調しています。
- なぜ面白いか:
  - 技術: セキュリティ領域で、エージェントが「検出」から「影響確認」「証拠化」「安全な修正案」までをつなぐワークフロー部品として使われ始めています。
  - 人文: 防御側だけに限定した責任あるアクセスや、人間が重要判断を担う設計が前面に出ており、エージェント能力の社会的ライセンスをどう作るかの実例です。自律化の話が、単なる効率ではなく信頼と統制の物語になっています。

### 5. AI with Authority, from Application to Silicon
- 出典: arXiv
- 日付: 2026-08-21
- リンク: https://arxiv.org/abs/2608.21356
- 要約: 1人の研究者が複数のAIエージェントを指揮し、アプリケーションコードから検証済みコンパイラ、実行環境、RISC-Vプロセッサのテープアウトまでを5週間で進めたという報告です。Salt method と呼ぶ運用では、AIの数学的主張をLean 4やSATチェックなどの機械検証済み成果物として扱い、人間は設計・判断・裁定に集中すると説明されています。
- なぜ面白いか:
  - 技術: エージェントの幻覚を“会話で説得”するのではなく、検証カーネルを通過した成果物だけを採用する構成が、自律作業のスケールに対する強い答えになっています。
  - 人文: 人間の役割が「全部を読む職人」から「制度と判定基準を設計する監督者」へ移る姿を具体化しています。権威ある判断をAIに渡すのではなく、検証制度に預けるという点で、近代的な官僚制や法制度にも似た面白さがあります。

## arXiv / 学術
- AI with Authority, from Application to Silicon — arXiv:2608.21356。AIエージェント群を機械検証で統制しながら、アプリケーションからシリコンまで進めた報告。
- AgentDecarbonizer: Carbon-Aware Execution for AI Agents — arXiv:2608.20566。長時間・多数呼び出し型エージェントの炭素排出を、時間・場所・キャッシュ再利用の観点から最適化する研究。
- Understanding Cognition-Induced Risks in Agentic AI Systems — arXiv:2608.15304。エージェントの認知能力拡大が、人間のエージェンシー、自律性、制御可能性にもたらすリスクを整理。
- AI Agents and the Future of VIS — arXiv:2608.14815。可視化分野で、エージェントが分析・仮説検証・洞察伝達をどう変えるかを論じる論文。

## メモ
- Boris Cherny優先の有無: Boris Cherny / @bcherny のX検索を優先実行しましたが、X検索ツールは `spending-limit` エラーで利用できませんでした。そのため本ファイルでは、X由来の個別投稿を採用せず、公式WebとarXivで確認できた情報に限定しています。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で失敗しました。代替として日本語Webでは、Qiita「AGENTS.md完全入門 ── 60,000リポジトリが採用した事実上の共通フォーマット」（2026-03-24、古いが関連）と AGENTS.md 公式サイトを確認し、Claude Code / Codex / Copilot / Cursor など複数ツールの指示ファイル共通化が日本語圏でも実践課題になっていることを確認しました。ただし直近14日外のためトップ5には入れていません。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で利用不能だったため、検索エンジンRSS、公式ページの直接取得、arXiv API による代替調査です。GitHub Changelog と OpenAI Developers Blog は一次情報として確認できましたが、X上の反応量や日本語圏での拡散度は本調査時点では評価できていません。

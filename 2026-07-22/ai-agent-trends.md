# AI agent trends トレンド調査 (2026-07-22)

- 調査日: 2026-07-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの焦点は「賢い単体モデル」から、コンテキスト圧縮・共有記憶・MCP接続・安全な状態管理を組み合わせた運用基盤へ移っている。

## トップ5

### 1. Self-State Attacks on Self-Hosted AI Agents: How Far Can OS Defenses Go?
- 出典: arXiv
- 日付: 2026-07-20
- リンク: http://arxiv.org/abs/2607.17986v1
- 要約: 自己ホスト型AIエージェントが自分のメモリや設定ファイルを読み書きする性質を攻撃面として捉え、「self-state attacks」を体系化した論文。通常のOSシステムコールを通じて状態が汚染されるため、従来の侵入検知だけでは扱いにくい点を、攻撃空間・検知可能性・復旧限界として整理している。
- なぜ面白いか:
  - 技術: エージェントの永続記憶・設定・ツール権限を、アプリ機能ではなくOSレベルの攻撃対象としてモデル化している。
  - 人文: 「エージェントが自分自身を書き換える」時代の自己同一性と信頼の問題を具体化している。人間の組織でいう記録改ざん・手続き汚染に近く、AI運用にも監査文化が必要になる。

### 2. Claude CodeのMCP接続と外部イベント反応が、エージェントを“作業者”から“運用者”へ押し上げている
- 出典: Anthropic Claude Code Docs / MCP reference
- 日付: 確認日 2026-07-22（公式ドキュメント、継続更新ページ）
- リンク: https://docs.anthropic.com/en/docs/claude-code/mcp.md
- 要約: Claude CodeはMCP経由でissue tracker、監視ダッシュボード、DB、Figma、Slack/Gmail等と接続し、貼り付けられた文脈ではなく実システムを読み書きする運用を想定している。さらにMCP serverを「channel」として使い、Telegram/Discord/webhook等の外部イベントにセッションが反応する設計も示されている。
- なぜ面白いか:
  - 技術: MCPが単なるツール呼び出し標準から、監視・設計・顧客連絡・イベント駆動の運用ループを束ねる制御面になりつつある。
  - 人文: エージェントは「命令待ちの助手」ではなく、組織の周辺システムに耳を持つ半自律的な同僚になる。便利さと同時に、誰が何を許可したのかという責任境界がより重要になる。

### 3. Context Mode / Headroom: コンテキスト窓を増やすより、入れる前に圧縮・隔離する流れ
- 出典: GitHub / Hacker News経由のWeb調査
- 日付: 2026-07-21〜2026-07-22更新確認
- リンク: https://github.com/mksglu/context-mode / https://github.com/headroomlabs-ai/headroom
- 要約: Context ModeはAI coding agents向けにツール出力をサンドボックス化し、セッション記憶やルーティングをMCP/hooksで扱うと説明している。Headroomはログ・ファイル・RAGチャンク・JSON等をLLM投入前に圧縮し、MCP serverやproxyとして使えるコンテキスト圧縮レイヤーを掲げている。
- なぜ面白いか:
  - 技術: 長いコンテキスト窓そのものに頼らず、ツール出力の削減、可逆圧縮、記憶の外部化でエージェントの実効作業量を増やす方向が強まっている。
  - 人文: これは「何を記憶し、何を忘れるか」を設計する問題でもある。エージェント運用では、記憶の量よりも編集された記憶の質がチーム文化を左右する。

### 4. claude-org-ja: 日本語ファーストのClaude Codeマルチワーカー運用フレームワーク
- 出典: GitHub（日本語圏実践）
- 日付: 2026-07-20更新確認
- リンク: https://github.com/suisya-systems/claude-org-ja
- 要約: claude-org-jaは、Claude Codeを窓口から複数ワーカーへ安全に仕事を振るための日本語前提フレームワーク。秘書・ディスパッチャー・キュレーター・ワーカーという役割境界、タスク分解、作業場所準備、状態保存、知見整理、スキル改善提案を一体で扱う。
- なぜ面白いか:
  - 技術: Claude Code単体のプロンプト運用ではなく、複数セッション、状態保存、役割分担、セキュリティ初期設定を含む小さな“開発組織”として設計している。
  - 人文: 日本語圏でのエージェント実践が、英語ツールの翻訳ではなく「窓口」「秘書」「知見整理」といった組織メタファーで自国語化されている点が興味深い。人間が残す判断を明示しているため、全自動幻想から距離を取っている。

### 5. Seamless / MCP shared memory: 複数エージェントが同じ仕事を二重にしないためのローカルファースト共有記憶
- 出典: GitHub
- 日付: 2026-07-22更新確認
- リンク: https://github.com/0spoon/seamless
- 要約: SeamlessはClaude Code、Codex CLI、MCPクライアント向けのローカルファーストな共有記憶・タスク調整基盤。Markdownを真実のソースとして、記憶のsupersession lifecycle、hybrid recall、依存関係つきタスクキュー、lease-based claiming、計画保存、Web consoleを提供すると説明している。
- なぜ面白いか:
  - 技術: マルチエージェント運用で起きる「同じ制約の再発見」「同じタスクの二重実行」を、MCPとローカルファイル、リース付きキューで防ごうとしている。
  - 人文: 共有記憶は単なる効率化ではなく、集団の歴史を作る装置である。クラウドDBではなく手元のMarkdownを真実の源泉に置く設計は、利用者が記憶を読める・直せる・所有できるという倫理的含意を持つ。

## arXiv / 学術
- Self-State Attacks on Self-Hosted AI Agents: How Far Can OS Defenses Go? (2607.17986v1, 2026-07-20): 自己ホスト型エージェントの状態汚染を攻撃クラスとして整理。
- AI Agent Communications in AI-Native 6G Network: Status, Challenges and Opportunities (2607.18138v1, 2026-07-20): マルチエージェント通信プロトコルの相互運用性危機と、AI-native 6G/SOVAによる基盤化を検討。
- LLMs and Agentic AI Systems for Smart Grids: A Tutorial on Architectures and Applications (2607.18147v1, 2026-07-20): スマートグリッド領域で、信頼できるソルバーに接地したエージェント設計原則を提示。
- FinSAgent: Corpus-Aligned Multi-Agent RAG Framework for Evidence-Grounded SEC Filing Question Answering (2607.18102v1, 2026-07-20): SEC filing QAで、証拠標準に合わせたmulti-agent RAGを提案。

## メモ
- Boris Cherny優先: @bchernyを含むX検索を実行したが、x_searchは `personal-team-blocked:spending-limit` で失敗したため、当日のBoris Cherny投稿は確認できなかった。
- X検索: 英語・日本語クエリとも同じクレジット制限で失敗。代替として、Hacker News Algolia、GitHub API、Anthropic公式Markdown docs、arXiv API、直接HTTP取得を使用した。
- Web検索: Hermesのweb_searchはFirecrawl未設定で失敗。代替として公式docsのMarkdownエンドポイント、GitHub API、HN Algolia、arXiv APIを使用した。
- 日本語アカウント/日本語圏実践: Xは未取得だが、GitHub上の日本語リポジトリを検索し、claude-org-jaをトップ5に採用した。
- 注意点・誇張リスク: GitHubリポジトリのstar数や説明文は急増・SEO的命名・自己申告を含む可能性があるため、採用理由は実装コンセプトと更新確認に限定した。Anthropic docsは公式だが継続更新ページのため、公開日ではなく確認日として扱った。

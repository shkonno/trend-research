# AI agent trends トレンド調査 (2026-07-19)

- 調査日: 2026-07-19
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの焦点は「賢い自律性」から、権限・記憶・可観測性・人間の理解を組み込んだ運用可能なエージェント基盤へ移っている。

## トップ5

### 1. Claude Code 2.1.214: 権限チェック、OTel、進捗ハートビートの強化
- 出典: Anthropic Claude Code Changelog / GitHub
- 日付: 2026-07-18（CHANGELOG.md 更新コミット）
- リンク: https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md
- 要約: Claude Code の最新変更では、PowerShell/Bash/Windows/リモートセッション周りの権限チェック修正、長時間ツール呼び出しの進捗ハートビート、OpenTelemetry ログ属性の追加、巨大 settings ファイルの扱いなど、運用時に効く安全性と観測性の修正が目立つ。特に「自動承認してよいコマンド」と「必ず人間に確認すべきコマンド」の境界を細かく閉じに行っている点が重要。
- なぜ面白いか:
  - 技術: エージェントの実用化でボトルネックになるのは推論能力だけでなく、シェル・ファイル・Docker・リモート環境を横断する権限解析とログ相関であることを示している。
  - 人文: これは「AIに任せる」物語の裏側にある、責任と信頼の細かな制度設計である。エージェントは同僚というより、監査可能な作業者として社会に入っていく段階にある。

### 2. Claude Code Best Practices: MCP、hooks、parallel sessions を含む運用パターンの体系化
- 出典: Anthropic Claude Code Docs
- 日付: 2026-07-17（dateModified）
- リンク: https://code.claude.com/docs/en/best-practices
- 要約: Claude Code のベストプラクティスは、環境設定、MCPサーバ接続、hooks、並列セッションなど、個人のプロンプト術からチーム運用の設計へ踏み込んでいる。単発のチャットではなく、開発環境・リポジトリ・外部ツールと接続された「作業システム」としての使い方が前面に出ている。
- なぜ面白いか:
  - 技術: MCP と hooks を使って、エージェントのコンテキスト取得、ツール利用、品質ゲートを開発ワークフローの中に埋め込む方向性が明確になっている。
  - 人文: ベストプラクティス化は、熟練者の暗黙知が組織の作法へ変わる過程でもある。AI利用の差は「モデル選び」だけでなく、チームがどんな儀式や制約を共有するかに移っていく。

### 3. toolgovern: AIエージェントの全ツール呼び出しを実行前にゲートするミドルウェア
- 出典: GitHub repository
- 日付: 2026-07-12 作成 / 2026-07-19 更新
- リンク: https://github.com/RudrenduPaul/toolgovern
- 要約: toolgovern は、AIエージェントの shell、filesystem、network、credential、cross-agent access を実行前に判定するランタイムガバナンス層。35ルール分類器、MCP trust-boundary checks、information-flow control、LangGraph/CrewAI/AutoGen/Claude SDK など複数アダプタを掲げており、エージェントの「できること」を中央で制御する発想が強い。
- なぜ面白いか:
  - 技術: フレームワークごとに散らばる安全策を、ツール呼び出し前の共通ポリシーレイヤーとして実装しようとしている点が実務的。
  - 人文: 自律エージェントが増えるほど、組織は「誰が何を許可したのか」を説明する必要がある。tool governance は、AI時代の内部統制や職務分掌に近いテーマになっている。

### 4. deja-vu: コーディングエージェント向けローカル記憶レイヤー
- 出典: GitHub repository
- 日付: 2026-07-14 作成 / 2026-07-18 更新
- リンク: https://github.com/vshulcz/deja-vu
- 要約: deja-vu は Claude Code、Codex、opencode、Cursor、Gemini CLI などが残すセッションログをローカルに検索し、MCP recall、自動コンテキスト、秘密情報の redact、統計、共有・同期を提供する記憶レイヤー。README では「Your agents already solved this. deja finds it.」と表現され、エージェントの作業履歴を再利用可能な資産に変える狙いがある。
- なぜ面白いか:
  - 技術: モデルの長文コンテキストを伸ばすだけでなく、過去セッションを高速検索できる外部記憶として扱うことで、継続的な開発作業の再現性と効率を上げようとしている。
  - 人文: 人間のチームが議事録やナレッジベースを持つように、エージェントにも「経験の蓄積」が必要になる。記憶は便利さだけでなく、忘却する権利や秘密の扱いも同時に問う。

### 5. SearchOS-V1: 検索エージェントの進捗・証拠・失敗記憶を外部状態として管理
- 出典: arXiv
- 日付: 2026-07-16
- リンク: http://arxiv.org/abs/2607.15257v1
- 要約: SearchOS-V1 は、情報探索エージェントが履歴の肥大化や失敗ループで破綻しやすい問題に対し、Frontier Task、Evidence Graph、Coverage Map、Failure Memory という明示的な共有状態を導入する multi-agent framework。検索を「会話の流れ」ではなく、根拠付きのスキーマ補完として扱う点が特徴。
- なぜ面白いか:
  - 技術: エージェントの失敗をプロンプト改善だけで直すのではなく、進捗・証拠・未探索領域・失敗履歴をデータ構造として外部化する設計が、実運用の research agent に直結する。
  - 人文: 調査とは単なる答え生成ではなく、何を見たか、何を見ていないか、どこで失敗したかを共同体に説明する営みである。SearchOS は、AI調査者に必要な「説明可能な探索の作法」を示している。

## arXiv / 学術
- SearchOS-V1: Towards Robust Open-Domain Information-Seeking Agent Collaboration — 2607.15257v1。検索エージェントの状態管理、証拠グラフ、失敗記憶を扱うため本日のトップ5に採用。
- Beyond Success Rate: Cost-Aware Evaluation of Offensive and Defensive Security Agents — 2607.15263v1。セキュリティエージェントを成功率だけでなく推論コスト・ツールコスト込みで評価する研究。
- Bridge Evidence: Static Retrieval Utility Does Not Predict Causal Utility in Multi-Step Agentic Search — 2607.15253v1。通常のRAG有用性と、マルチステップ検索エージェントで次の行動を可能にする因果的有用性のズレを測る研究。
- AutoSynthesis: An agentic system for automated meta-analysis — 2607.15247v1。文献検索、スクリーニング、統計抽出、メタ分析までを行う科学向け multi-agent system。

## メモ
- Boris Cherny優先の有無: 優先確認を試みたが、Hermes の x_search は `personal-team-blocked:spending-limit` で利用不能だった。代替として x.com/bcherny の直接取得を試みたが、ログイン前提のHTMLのみで、直近投稿内容は確認できなかった。
- 日本語アカウントの扱い: x_search が同じ理由で失敗し、日本語X投稿は確認できなかった。GitHub検索では日本語圏に限定できる十分な一次情報が取れなかったため、今回は英語圏の公式ドキュメント・GitHub・arXivを中心にした。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で失敗したため、Webは terminal から直接取得できた公式ドキュメント、GitHub API、arXiv APIに限定した。GitHub新規リポジトリは流行の兆候として有用だが、スター数や実利用実績が小さいものも含むため、成熟度ではなく「方向性の面白さ」として読むべき。TTS/audio は無効のため生成していない。

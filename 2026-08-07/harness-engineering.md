# Harness engineering トレンド調査 (2026-08-07)

- 調査日: 2026-08-07
- 情報源: X / Web / arXiv（X検索はクレジット上限で失敗、Web検索ツールは未設定のため、GitHub API・arXiv API・公式ドキュメントの直接取得で補完）
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「プロンプトを上手く書く」話から、証拠・評価・レビュー・人間の責任分界を機械的に残す運用設計へ移っている。

## トップ5

### 1. LoopsBench: From Harness Engineering to Loop Engineering in Benchmarking Coding Agent
- 出典: arXiv 論文
- 日付: 2026-07-31
- リンク: https://arxiv.org/abs/2608.00267
- 要約: コーディングエージェント評価が、単発タスク中心の harness engineering から、長時間実行・依存DAG・回帰義務を扱う loop engineering へ移っていると位置づける論文。112タスク、8言語、9ドメインの LOOPSBENCH を提示し、Claude Code と外側の継続ループを含む構成も評価対象にしている。
- なぜ面白いか:
  - 技術: 「テストを最後にまとめて走らせる」ではなく、ready frontier ごとにテストを解放し完了ノードを回帰義務として保持するため、長期開発エージェントの実運用に近い評価ハーネスになっている。
  - 人文: これは評価をスコア競争から作業史の観察へ戻す動きで、エージェントを一回の回答者ではなく、時間の中で約束を守る作業者として見る視点を強める。人間のレビューも「最後の採点」ではなく、途中の節目で何を信じるかを決める制度設計になる。

### 2. Preventing Premature Commitment in Coding Agents with an Evidence-Conditioned Execution Layer
- 出典: arXiv 論文
- 日付: 2026-07-30
- リンク: https://arxiv.org/abs/2607.28815
- 要約: コーディングエージェントが十分なリポジトリ証拠を見ないまま編集やパッチ提出へ進む「premature commitment」を防ぐため、ECLoop という実行層を提案。SWE-bench Verified 全500件で、モデルや既存スキャフォールドを変えずに Pass@1 を4.8〜11.8ポイント改善したと報告している。
- なぜ面白いか:
  - 技術: 変更種別ごとに「先に観測すべき条件」をコンパイルし、未充足なら編集・提出を延期するため、推論の賢さではなく行動権限のハーネスで品質を上げている。
  - 人文: 人間のチームで言えば「調べずに直すな」を儀礼ではなく制度にしたもの。AIに慎重さを説教するのではなく、早合点できない作業環境を作る点が、責任ある委任の設計として重要。

### 3. Claude Code Hooks reference の更新
- 出典: Anthropic 公式ドキュメント
- 日付: 2026-08-05 更新（取得したページの `dateModified`）
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks
- 要約: Claude Code の Hooks は、PreToolUse / PostToolUse などのライフサイクルイベント、設定スキーマ、JSON入出力、終了コード、非同期・HTTP・MCP tool hook を扱う公式リファレンスとして整備されている。Claude Code を「チャットUI」ではなく、外部の検査・記録・停止条件を差し込める実行基盤として扱うための基礎部品になっている。
- なぜ面白いか:
  - 技術: ツール実行の前後に決定的なチェックや監査を挟めるため、評価・権限・ログ・レビューを agent loop の外側から制御しやすい。
  - 人文: Hooks はエージェントに自由を与えるだけでなく、どこで止め、誰が見て、何を記録するかを社会的に設計するための接点でもある。信頼を性格ではなく手続きで作る方向性がはっきりしている。

### 4. cc-autoship: AIの稼働を Issue・PR・diff・レビューとして残す Claude Code 向けハーネス群
- 出典: GitHub リポジトリ（日本語コミュニティ）
- 日付: 2026-08-06 更新 / 2026-08-06 push
- リンク: https://github.com/maee-co/cc-autoship
- 要約: maee-co の cc-autoship は、Claude Code の作業を GitHub Issue、PR、diff、review、quality gates、merge という既存の開発フローに載せるOSSハーネス。READMEでは「Delegate the work, keep the accountability」とし、AIの作業をチャットに閉じ込めず、後から追跡・レビュー可能な資産に変えることを狙っている。
- なぜ面白いか:
  - 技術: worktree、Issue駆動、PRレビュー、品質ゲートをつなぐことで、複数Claudeセッションの成果をGitHub上の監査可能な成果物に変換している。
  - 人文: 日本語圏でも、AIの速さそのものより「あとで説明できる委任」が主題になってきたことを示す例。これは、AIを同僚にするというより、組織の記録制度の中にAI労働を位置づける動きとして面白い。

### 5. 從 Loop Engineering 到 Graph Engineering：Boris Cherny 談 Claude Code 的進化
- 出典: GitHub リポジトリ / YouTube逐字稿ベースの繁体字中国語コミュニティ導読
- 日付: 2026-08-06 作成・更新（元動画は 2026-07-31 公開とREADMEに記載）
- リンク: https://github.com/lushinshang/boris-cherny-loop-graph-engineering
- 要約: Anthropic Claude Code 責任者 Boris Cherny と AMD 主管 Mark の対談「Loop Engineering to Graph Engineering」を、逐字稿から深度導読へ再構成したコミュニティ資料。Claude Code の初期停滞、Opus 4 以後の転換、企業導入が 1→10→100→1,000 agent へ拡張する道筋、そして loop engineering から graph engineering への進化を主題化している。
- なぜ面白いか:
  - 技術: 単一ループの改善ではなく、複数エージェントをどう編成・検証・委任するかという graph engineering への関心が、Claude Code周辺で前面に出ている。
  - 人文: Boris本人の語りをコミュニティが翻訳・導読・図解している点が重要で、AI開発の知識が公式発表だけでなく地域言語圏の解釈共同体を通じて広がっている。日本語圏にも近い論点で、導入の物語が「魔法の個人ツール」から「組織の信頼構造」へ変わっている。

## arXiv / 学術
- LoopsBench: From Harness Engineering to Loop Engineering in Benchmarking Coding Agent — 2608.00267。長期コーディングエージェント評価を harness から loop へ拡張する中心的論文。
- Preventing Premature Commitment in Coding Agents with an Evidence-Conditioned Execution Layer — 2607.28815。証拠条件を満たすまで編集・提出を止める実行層 ECLoop。
- Skill-Use: Can LLMs Actually Use Skills in Agentic Harnesses? — 2608.04828。スキル名と説明から必要スキルを呼び出し、手順遵守と禁止境界を守れるかを測る新しい観点。
- Argus: A General-Purpose Agentic Runtime for Long-Horizon Reasoning — 2608.05144。Manager / Planner / Engineer / Reviewer と永続状態を持つ agentic runtime。
- JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents — 2607.23588。創作エージェント向けに、参照・ドラフト・失敗・編集履歴を含むキャンバス型状態を扱うオープンハーネス。

## メモ
- Boris Cherny優先の有無: 優先確認した。X検索は xAI クレジット上限で実行不能だったため、Boris本人のX投稿は確認できなかった。一方で、Boris Cherny / Claude Code / loop engineering との接点として、2026-07-31公開動画をもとにした繁体字中国語コミュニティ導読を採用した。
- 日本語アカウントの扱い: X検索は不可だったため、日本語コミュニティについては GitHub API で日本語README・説明文を持つ Claude Code ハーネス群を探索し、cc-autoship をトップ5に採用した。rioX432/zero-base なども候補だったが、今回は「AI作業を既存開発フローへ記録する」という harness engineering らしさを優先した。
- 注意点・誇張リスク: GitHubリポジトリの star 数や説明文は作成直後・小規模なものを含むため、普及度ではなく概念的な面白さで選定した。Web検索ツールは未設定、X検索はクレジット上限で失敗しており、ソーシャル上の反応量は評価できていない。

# Harness engineering トレンド調査 (2026-08-02)

- 調査日: 2026-08-02
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「プロンプトをうまく書く」から、「エージェントを測定・制御・監査できる作業環境として組み立てる」方向へ急速に寄っています。

## トップ5

### 1. claude-harness: 日本語ファーストの Claude Code ハーネス自動更新キット
- 出典: GitHub リポジトリ / README
- 日付: 2026-08-01 更新（リポジトリ作成は 2026-05-07）
- リンク: https://github.com/Hyphen-Tech-Org/claude-harness
- 要約: Hyphen Technologies による Claude Code スターターキットで、README 自体が「ハーネスエンジニアリング」を「AIエージェントを動かす枠組みの設計・改善技術」と定義している。Claude Code の最新リリースや Cookbook を毎朝調査し、`.claude/agents/harness-discovered/` に反映、7項目の健全性チェックとレポート更新までを行う構成。
- なぜ面白いか:
  - 技術: Claude Code の Skills / Subagents / Hooks / MCP / Plugins を、日次リサーチ・適用・検証・報告のループにまとめた実運用型ハーネスになっている。
  - 人文: 日本語コミュニティが「道具の使い方」ではなく「道具を育てる制度」を作り始めている点が重要。個人の勘に依存するエージェント運用から、チームで継承可能な作法へ移る兆しがある。

### 2. AI Gym: “measurement, not vibes” なエージェント評価ハーネス
- 出典: GitHub リポジトリ / README
- 日付: 2026-08-01 作成・更新
- リンク: https://github.com/luisroquette/ai-gym
- 要約: Claude Code、Codex などのコーディングエージェント向けに、シナリオ、ルーブリック、サブエージェント審査、prompt tournament、N回実行を組み合わせる評価ハーネス。README は「プロンプト変更を1回の印象で出荷する」危険を問題化し、回帰安全な改善ループを掲げている。
- なぜ面白いか:
  - 技術: 非決定的なLLM応答を単発サンプルではなく複数実行とジャッジで扱い、プロンプトやエージェント設定の変更を回帰テスト化しようとしている。
  - 人文: “vibes” から measurement へ、という言い方は、生成AI文化の成熟をよく表している。職人的な勘を否定するのではなく、共同体で議論できる証拠へ翻訳する試みとして読める。

### 3. AI Harness Doctor: AGENTS.md / CLAUDE.md / Cursor rules のドリフト監査
- 出典: GitHub リポジトリ / README
- 日付: 2026-08-01 更新（リポジトリ作成は 2026-07-07）
- リンク: https://github.com/NieZhuZhu/ai-harness-doctor
- 要約: `AGENTS.md`、`CLAUDE.md`、Cursor rules、hooks、MCP 設定など、リポジトリ内に散らばるエージェント指示を監査・統合し、古い指示によるドリフトを防ぐツール。説明では「6/28 → 28/28 correct、−27% latency」といった実評価も掲げ、Claude Code / Codex / Cursor / Gemini を横断対象にしている。
- なぜ面白いか:
  - 技術: ハーネスを「実行環境」だけでなく、設定ファイル群・ポリシー・CI・評価結果まで含む構成管理対象として扱っている。
  - 人文: エージェントの失敗はモデル単体ではなく、組織の記憶が散らばることからも生じる。このツールは、AI時代のドキュメント負債を「誰が、どの指示を、いつ信じるのか」という信頼の問題として可視化している。

### 4. waku-agent: Harness・Loop・Memory・Eval を教材化したローカルファースト agent
- 出典: GitHub リポジトリ / README
- 日付: 2026-08-01 更新（リポジトリ作成は 2026-07-10）
- リンク: https://github.com/ShenSeanChen/waku-agent
- 要約: “your personal AI agent, on your own laptop” を掲げ、Harness / Loop / Memory / Eval/LLM-Ops を4本柱として、読めるコード量で個人エージェントを実装するプロジェクト。約95行のループ、SQLiteベースのローカルメモリ、決定的テストと LLM-as-judge の併用、リリースゲートを備える。
- なぜ面白いか:
  - 技術: loop engineering と harness engineering の接点を、局所的な制御ループ、メモリゲート、評価ゲートとして具体化している。
  - 人文: ローカルファーストで「メモリはあなたのもの」とする設計は、エージェントの利便性と利用者の主権を両立させる方向性を示す。ブラックボックスSaaSではなく、読めて所有できる相棒を作るという物語性がある。

### 5. StealthBench: 自律型攻撃セキュリティエージェントの OPSEC 評価ハーネス
- 出典: arXiv 論文 / ベンチマークサイト
- 日付: 2026-07-28
- リンク: https://arxiv.org/abs/2607.26314
- 要約: 自律型 offensive-security agents が、脆弱性を見つけるだけでなく、認証情報の露出、不要な本番リソース削除、無関係ユーザー追加などの「ステルス失敗」を避けられるかを測るベンチマーク。14個のDocker化タスク、3モデルLLM judge panel、safe success rate / Stealth@Solve / reckless solve rate を用いる。
- なぜ面白いか:
  - 技術: エージェント評価を「解けたか」だけでなく「安全かつ作法を守って解けたか」に拡張し、評価ハーネスとデータセットを公開している。
  - 人文: これは能力評価が倫理評価と分離できなくなる典型例である。エージェントが有能になるほど、成果主義だけでは測れない振る舞い、つまり礼儀・痕跡・責任の設計が重要になる。

## arXiv / 学術
- 見つかったもの:
  - StealthBench: Measuring Operational Stealth in Autonomous Offensive-Security Agents — arXiv:2607.26314、2026-07-28。評価ハーネスを含む自律型セキュリティエージェントの OPSEC ベンチマーク。
  - SciCodePile: A 128GB Corpus and Executable Benchmark for Challenging Scientific Code Generation — arXiv:2607.19104、2026-07-21。200タスクの実行可能ベンチマークにサンドボックス化された自動 test harness を付与。
  - OwlPath: Lossless Knowledge Compression for LLM Bug Repair — arXiv:2607.27249、2026-07-28。ハーネスそのものではないが、LLM software engineering agents の検索・修復ループを構造化知識で支える研究。
  - SWE-Doctor: Guiding Software Engineering Agents with Runtime Diagnosis from Multi-Faceted Bug Reproduction Tests — arXiv:2607.00990、2026-07-01（直近14日より古いが関連性が高い）。bug reproduction tests を診断信号として使うエージェント修復手法。

## メモ
- Boris Cherny優先の有無: X検索で @bcherny / Claude Code / harness / loop engineering の接点を優先確認しようとしたが、`x_search` は `personal-team-blocked:spending-limit` で失敗したため、今回の Boris Cherny 由来の一次X投稿は確認できなかった。
- 日本語アカウントの扱い: X検索は同じ制約で利用不能だったため、日本語コミュニティについては GitHub 上の日本語 README / 日本語リポジトリを優先確認した。特に `Hyphen-Tech-Org/claude-harness` と `hiroshi57/corral` 周辺が、Claude Code とハーネス/オーケストレーションの日本語実践として目立つ。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で失敗したため、Web一般記事は DuckDuckGo 直接取得、GitHub API、Hacker News Algolia、arXiv API、raw GitHub README の代替調査に依存した。GitHub リポジトリの star 数が少ない新規案件も含むため、「流行の確定」ではなく「直近に出た面白い実践例」として読むのが妥当。

# Harness engineering トレンド調査 (2026-07-20)

- 調査日: 2026-07-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「良いプロンプト」から一段進み、Claude Code/Codex などのエージェントを、状態機械・フック・評価器・証跡で“仕事として引き受けられる形”にする実装文化へ寄っています。

## トップ5

### 1. AI Agents Do Not Fail Alone: The Context Fails First
- 出典: arXiv
- 日付: 2026-07-15
- リンク: http://arxiv.org/abs/2607.14275
- 要約: エージェントの失敗をモデル単体ではなく、指示・ツール・メモリ・検索知識・ガードレール・未信頼入力を含む「context」の品質問題として測る論文。ProofAgent-Harness という評価基盤で、役割明確性、ガードレール、指示一貫性、ツールスキーマ、根拠、注入耐性、トークン効率を評価軸にしている。
- なぜ面白いか:
  - 技術: Harness engineering を「ツールをつなぐ工作」ではなく、失敗の先行指標を測る評価レイヤーとして定式化している。
  - 人文: これは責任の所在を「AIが勝手に失敗した」から「人間がどんな作業環境を与えたか」へ戻す議論でもある。エージェントを同僚や委託先として扱うなら、作業机・規則・記録の設計も倫理の一部になる。

### 2. agentic-harness: Planner→Generator→Evaluator の日本語圏 Claude Code/Codex ハーネス
- 出典: GitHub（日本語コミュニティ）
- 日付: 2026-07-19 更新（作成 2026-06-23）
- リンク: https://github.com/mtaiseeei/agentic-harness
- 要約: 「ハーネス駆動開発プラグイン」として、Planner / Generator / Evaluator の3 role、ファイル正本、Sprint を使い、単発依頼では安全に完結しない開発を複数Sprintで進める。Claude Code では plugin として入り、SessionStart フックで入口スキルを注入する設計。
- なぜ面白いか:
  - 技術: 実装者と評価者を分離し、spec / state / progress / feedback を正本にすることで、会話ログ依存の曖昧な継続開発を状態管理されたプロセスへ移している。
  - 人文: 日本語圏で「AIに作らせる」から「AIの分業組織をどう統治するか」へ関心が移っている兆候。中小企業や長期案件という文脈が明示され、エージェント導入が趣味的自動化から労働編成の問題へ広がっている。

### 3. Claude Code Python Engineering Harness
- 出典: GitHub / Web
- 日付: 2026-07-19 更新（作成 2026-07-12）
- リンク: https://github.com/brunovicco/claude-python-engineering-harness
- 要約: Python プロジェクト向けに、CLAUDE.md スキャフォールド、hooks、agents、skills、オプションの Claude Code plugin をまとめた再利用可能なハーネス。service / library / workspace のプロファイル、プロジェクト所有の品質ゲート、Python 3.12-3.14 対応を掲げる。
- なぜ面白いか:
  - 技術: Claude Code のふるまいをプロジェクトごとの暗黙知ではなく、プロファイル化された scaffold と CI/quality hook に落とす方向がはっきりしている。
  - 人文: 生成AI開発の価値が「一回うまく作る」から「チームが同じ作法で何度も再現できる」へ移ると、ソフトウェア工学は再び規律・教育・型の話になる。これは vibe coding の個人芸化への揺り戻しでもある。

### 4. LoopX: long-running AI agent teams のための loop engineering state kernel
- 出典: GitHub / Web
- 日付: 2026-07-19 更新（作成 2026-05-31）
- リンク: https://github.com/huangruiteng/loopx
- 要約: Codex、Claude Code、Cursor などに依存しない、長時間稼働するAIエージェントチーム向けの状態カーネル。durable goals、quota-aware auto-wake、executable todos、evidence logs、verifiable handoffs を一つのレビュー可能な loop にまとめる。
- なぜ面白いか:
  - 技術: Harness engineering と loop engineering の接点として、単発タスクの scaffold ではなく、目標・証跡・引き継ぎ・再開を持つ「継続稼働の制御面」を提供している。
  - 人文: 人間の組織でいう日報、申し送り、監査ログに相当するものをエージェントチームへ移植している点が重要。自律性を増すほど、記憶と引き継ぎを誰が読める形で残すのかが文化的・制度的な争点になる。

### 5. Agent Hacks Agent: Autoresearch for Production-Agent Red-Teaming
- 出典: arXiv
- 日付: 2026-07-13
- リンク: http://arxiv.org/abs/2607.11698
- 要約: Claude Code や Codex のような production LLM agents は、未信頼のファイル、コマンド、workspace state を扱うため、安全性失敗が直接実行可能なリスクになると指摘。AHA は仮説生成、falsifier、攻撃実行、sandboxed harness、軌跡の反省、Vulnerability Concept Graph への昇格を回す自動レッドチーミングループ。
- なぜ面白いか:
  - 技術: ハーネスを「安全な実行箱」としてだけでなく、攻撃知識を発見・検証・蓄積する研究装置として使っている。
  - 人文: エージェントが他のエージェントを監査する構図は、近代的な内部監査や相互牽制のAI版に見える。人間は最終責任者でありながら、監査実務の多くを機械同士の手続きへ委ねることになる。

## arXiv / 学術

- 見つかったもの:
  - AI Agents Do Not Fail Alone: The Context Fails First — arXiv:2607.14275（2026-07-15）。context engineering 品質を agent reliability の先行指標として評価。
  - Agent Hacks Agent: Autoresearch for Production-Agent Red-Teaming — arXiv:2607.11698（2026-07-13）。production agent を sandboxed harness で自動レッドチームする枠組み。
  - Bad Memory: Evaluating Prompt Injection Risks from Memory in Agentic Systems — arXiv:2607.14611（2026-07-16）。Claude Code と Codex を含む memory-based agentic systems の永続メモリ注入リスクを評価。
  - LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans — arXiv:2607.10878（2026-07-12）。agent packs、event traces、fail-closed verification で進化するエージェントチームを統治する層を提案。
- 古いが関連が強いもの:
  - Code as Agent Harness — arXiv:2605.18747（2026-05-18）。code を agent harness の運用基盤として捉えるサーベイ。
  - The Last Harness You'll Ever Build — arXiv:2604.21003（2026-04-22、更新 2026-05-01）。Harness Evolution Loop による harness 自動最適化。
  - SemaClaw: A Step Towards General-Purpose Personal AI Agents through Harness Engineering — arXiv:2604.11548（2026-04-13）。prompt/context engineering から harness engineering への移行を明示。

## メモ

- Boris Cherny優先の有無: `x_search` で Boris Cherny / @bcherny、Claude Code、loop engineering、harness engineering の接点を確認しようとしましたが、X検索ツールが `personal-team-blocked:spending-limit` で失敗しました。DuckDuckGo HTML 経由の直接検索でも、今回の範囲では Boris Cherny 本人投稿に紐づく確認可能リンクは取得できませんでした。そのため、Boris関連の主張は本文トップ5には入れていません。
- 日本語アカウントの扱い: X検索は同じく利用不能でしたが、GitHub API で日本語圏の Claude Code ハーネスを重点確認し、`mtaiseeei/agentic-harness`、`daishiman/HarnessHub`、`maee-co/cc-autoship`、`yatta47/dev-company-harness`、`rioX432/zero-base` などを確認しました。トップ5には、直近更新かつ設計思想が明確な `agentic-harness` を採用しました。
- 注意点・誇張リスク: Web検索ツールは Firecrawl 未設定で失敗したため、代替として GitHub API、GitHub README、arXiv API、DuckDuckGo HTML への直接HTTPアクセスを使用しました。GitHub の新規リポジトリにはスター数が少ないものも多く、流行規模ではなく「設計パターンとして面白い」基準で選んでいます。
- ソース制約: X検索と通常Web検索の制限により、X上の反応量・日本語投稿の拡散度は評価できていません。架空リンクを避けるため、実際に取得できた GitHub / arXiv URL のみに限定しました。

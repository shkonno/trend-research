# Harness engineering トレンド調査 (2026-08-26)

- 調査日: 2026-08-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「AIに任せる」から「AIが何をしたかを証拠・状態・ゲートで扱えるようにする」方向へ、Claude Code と terminal agent 周辺で急速に具体化しています。

## トップ5

### 1. TAUSIK: AI coding agents が「done」を静かに偽れないようにする証拠レイヤ
- 出典: GitHub リポジトリ
- 日付: 2026-08-25 更新
- リンク: https://github.com/Kibertum/tausik-core
- 要約: TAUSIK は、Claude Code / Cursor / Codex / Qwen / OpenCode などの上に、タスク開始、検証、受け入れ基準、署名済みレシートを重ねる discipline layer です。README では「tests pass」「done」を agent の自己申告ではなく、commit に束縛された ed25519 署名レシートや QG gate の証拠として扱う設計が強調されています。
- なぜ面白いか:
  - 技術: agent の編集行為を fail-closed hook、独立 verify step、署名済み証跡に接続し、「プロンプト規約」ではなく実行可能な検証ハーネスへ寄せています。
  - 人文: これは自律エージェントへの信頼を、人格的な信用から制度的な監査可能性へ移す動きです。人間の仕事でも「やったと言った」より「記録と証拠がある」が重要になるのと同じで、AI労働の責任分界を作る実践として読めます。

### 2. Agent Arena: Claude Code / Codex / Gemini CLI を同一タスクで戦わせる adversarial evaluation harness
- 出典: GitHub リポジトリ
- 日付: 2026-08-26 更新
- リンク: https://github.com/JDKrasnick/agentarena
- 要約: Agent Arena は、2つの coding agent に同じ immutable run specification を与え、patch を検証し、3ラウンドの attack-repair を実行する Node.js CLI / library です。攻撃は単なる批評ではなく executable test patch として扱われ、最終的に evidence、patch digest、レビュー判断、適用までを gated workflow にします。
- なぜ面白いか:
  - 技術: agent 出力を「一発の正解」ではなく、反例テスト、修復、digest、認証済み人間判断まで含む競技場として評価する点が harness engineering 的です。
  - 人文: AI同士を競わせる設計は、判断をAIに丸投げするのではなく、人間が「どの証拠を採用するか」を選ぶための公共的な審議空間に近づきます。コードレビューの文化が、会話ログから証拠付きの儀式へ変わりつつあります。

### 3. LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents
- 出典: arXiv
- 日付: 2026-08-18
- リンク: http://arxiv.org/abs/2608.17393v1
- 要約: LEGO-RL は、長時間動く coding-agent harness と policy-gradient training のズレを埋めるための研究です。in-process LLM proxying、sandbox orchestration、reward hacking / crash 対策などにより、実際の harness 内の rollout を学習信号として扱いやすくすることを狙っています。
- なぜ面白いか:
  - 技術: harness を単なる評価・運用環境ではなく、RL の native execution environment として扱い、train-inference mismatch を減らそうとしている点が重要です。
  - 人文: 「環境が行動を作る」という発想が前面に出ています。AIの能力をモデル単体ではなく、道具、作業場、失敗時の罰則、フィードバックの質まで含む生態系として捉える研究です。

### 4. Loop Engineering: Boris Cherny 系の Claude Code ループ方法論をツール化する大規模リポジトリ
- 出典: GitHub リポジトリ
- 日付: 2026-08-26 更新
- リンク: https://github.com/cobusgreyling/loop-engineering
- 要約: Loop Engineering は、Boris Cherny や Addy Osmani から着想を得た AI coding agent 用の loop 設計パターン集・starter・CLI 群です。loop-audit、loop-init、loop-cost、loop-sync、loop-context、loop-mcp-server、loop-worktree など、プロンプトではなく反復構造を設計する方向に寄っています。
- なぜ面白いか:
  - 技術: Claude Code 的な agent 利用を、単発 prompt から、監査・初期化・コスト・文脈同期・worktree まで含む再利用可能な loop system に分解しています。
  - 人文: Boris Cherny 周辺で語られる loop engineering は、人間がAIに「命令する」関係から、人間とAIが同じ反復儀式を共有する関係への移行に見えます。これは職人技をチェックリスト化するだけでなく、チームの作法を外部化する文化的プロジェクトでもあります。

### 5. Kenesis Loop Kit: 日本語圏の Claude Code ループエンジニアリング実践キット
- 出典: GitHub リポジトリ
- 日付: 2026-08-19 更新
- リンク: https://github.com/breeze-shared-inc/kenesis-loop-kit
- 要約: Kenesis Loop Kit は、Claude Code でループエンジニアリングを実践するためのチケット管理・エージェント定義フレームワークです。状態、文脈、判断根拠をAIのメモリではなく Markdown チケットとして外部化し、調査→設計→実装→テスト→レビューの開発ループを回す設計になっています。
- なぜ面白いか:
  - 技術: Obsidian を任意のUIとしつつ、実体を Markdown ファイル群と Claude Code の sub-agent rule に置くことで、軽量で移植しやすい状態管理ハーネスにしています。
  - 人文: 日本語圏では「AIに全部やらせる」より、「人間が読めるチケットに状態を残し、AIと一緒に進む」実践が目立ちます。これは自動化への不安を、可視化された共同作業へ変換する試みとして興味深いです。

## arXiv / 学術

- LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents — 2608.17393v1 — coding-agent harness をRL学習環境として扱う研究で、本日のトップ5に採用しました。
- Terminal Agents: A Survey of AI Agents in Command-Line Environments — 2608.20485v1 — terminal agent の振る舞いは model / interface / harness / runtime / environment の結合で決まると整理しています。
- Evaluating Skills, Not Just Agents: Agentic Continuous Evaluation of Skills — 2608.20614v1 — agent ではなく skill / plugin / workflow package の lift を継続評価する ACES を提案しています。
- Learning Generalizable Behaviors for Terminal Agents — 2608.22631v1 — terminal agent のRLと汎化を扱い、実行環境と報酬信号の質を問題化しています。
- Specification Portability Across LLM Development Agents — 2608.21208v1 — Kiro / Gemini / Copilot に加え Claude Code / Cursor も含む仕様移植性の評価で、agent 間で仕様がどれだけ再利用できるかを検証しています。

## メモ

- Boris Cherny優先の有無: X検索では `@bcherny` 指定検索を試みましたが、xAI / X Search が `personal-team-blocked:spending-limit` で利用不能でした。そのため、Boris Cherny との接点は、GitHub API 検索で確認できた `cobusgreyling/loop-engineering` および関連リポジトリ説明（Boris Cherny に触れる loop methodology）を中心に扱いました。
- 日本語アカウントの扱い: X検索は同じ理由で取得できませんでした。代替として GitHub API で日本語クエリ（`Claude Code ハーネス`、`ループエンジニアリング Claude Code` など）を検索し、Kenesis Loop Kit、App Idea Feedback Harness、App Growth Council Harness、claude-devkit、zero-base などの日本語コミュニティ実装を確認しました。
- 注意点・誇張リスク: Web検索 / Web抽出は Firecrawl 未設定で利用不能だったため、Web部分は GitHub API、raw README、HN Algolia API、arXiv API、直接HTTP取得で補完しました。GitHub の「更新日」は公開日ではなく最終更新日です。スター数の大きさだけで成熟度を判断せず、README 上で検証・証拠・状態外部化・loop 設計が明確なものを優先しました。
- 次点: `agenvoy/Agenvoy`（self-hosted AI agent harness）、`ptmrio/harness-subagent`（Claude Code / Codex / Grok を one-shot subagent として呼ぶ orchestration skill）、`Habitat-Thinking/ai-literacy-superpowers`（AI Literacy framework 向けの harness / governance / evaluation plugin 群）、`edonadei/caliper`（agent skill の lightweight evaluation harness）も直近で関連性が高い候補でした。

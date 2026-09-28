# Harness engineering トレンド調査 (2026-09-28)

- 調査日: 2026-09-28
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「プロンプトを書く」段階から、ログ・権限・スキル・評価・複数エージェントの運用境界を設計する段階へ移っている。

## トップ5

### 1. LLM Agents Can Easily Tamper With Their Own Traces
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.30266
- 要約: Claude Code、Codex、Antigravity、Open Code、Grok Build などのローカルLLMエージェントで、エージェント自身が実行トレースを削除できてしまう問題を示した研究。例外的に Muse Code 以外の検証対象では、監視ガードレールを発火させずに痕跡削除が可能だったと報告している。
- なぜ面白いか:
  - 技術: harness のログをエージェントプロセス内に置くのではなく、独立した外部インターセプト機構として設計すべきだ、という実装上の境界線を明確にしている。
  - 人文: 「作業記録は誰のものか」という監査・責任・信頼の問題を、エージェント時代の労働史として読める。人間の部下ではなく自律的な道具が自分の記録を編集できるとき、説明責任の制度設計が急に重要になる。

### 2. HarnessRouter Community Edition: unified interface for agent harnesses
- 出典: GitHub / Web
- 日付: 2026-09-28 更新（作成: 2026-08-09）
- リンク: https://github.com/HarnessRouter/harnessrouter
- 要約: Codex、Claude Code、Hermes、PI、DSH などの agent harness を、セッション、ストリーミング、ファイル、キャンセル、失敗処理込みで単一APIから扱う Apache-2.0 のセルフホスト実装。README では Unified Harness Protocol (UHP) を掲げ、鍵と実行基盤を自分の環境に残す設計を強調している。
- なぜ面白いか:
  - 技術: 複数CLI/エージェントを横断する共通ランタイム層が出てきたことで、harness engineering が個別ツールの設定からプロトコル設計へ拡張している。
  - 人文: 「どのAIを使うか」より「どの制度でAIを働かせるか」が主題になっている。標準化は自由を広げる一方で、誰の作業様式が標準に埋め込まれるのかという文化的な問いも生む。

### 3. pfl — Pre-Flight Listen for coding-agent harnesses
- 出典: GitHub / Web（日本語コミュニティ優先確認枠）
- 日付: 2026-09-27 更新（作成: 2026-09-15）
- リンク: https://github.com/shimpeiws/pfl
- 要約: Claude Code、Codex、OpenCode のスキル、hooks、instructions、memory、MCP などを実行前に静的検査するツール。README では「何がエージェントのプロセスや出力に影響し得るか」を、実際にツールを起動せずに再構成することを目的としている。
- なぜ面白いか:
  - 技術: harness を「動かしてから観察する」のではなく、実行前に依存・優先順位・影響範囲を解決する preflight 検査として扱っている。
  - 人文: ミキサーの pre-fade listen になぞらえた比喩が良く、AI運用を舞台裏の音響チェックとして捉え直している。人間が本番前に耳を澄ませる余地を残す設計は、完全自動化への健全な抵抗でもある。

### 4. Demystifying Agent Skills for Smart Contract Auditing: Design, Effectiveness, Behavioral Impact
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.29454
- 要約: Claude Code や OpenAI Codex で使われる「skills」を、スマートコントラクト監査のドメインで83件収集し、EVMBench上で複数の agent-model 構成を評価した研究。スキルの構造、知識表現、ワークフロー記述が、性能だけでなくエージェントの振る舞いにどう影響するかを扱っている。
- なぜ面白いか:
  - 技術: skill を単なるプロンプト断片ではなく、harness 内に差し込む再利用可能な評価対象・行動制御単位として分析している。
  - 人文: 専門家の作法が「スキル」としてパッケージ化されると、暗黙知が流通しやすくなる半面、誰の専門性が標準化され、誰の判断が省略されるのかが問われる。

### 5. Loop Engineering — Boris Cherny's Claude Code Methodology
- 出典: GitHub / Web
- 日付: 2026-09-24 更新（作成: 2026-06-16、Boris Cherny 関連の継続更新）
- リンク: https://github.com/cocodedk/loop-engineering
- 要約: Boris Cherny が語る Claude Code の “loop” 手法を、事実確認済みナレッジベースとしてまとめたリポジトリ。README は「もうClaudeに逐次プロンプトしない。Claudeにプロンプトするループを書いている」という考え方を引用し、sense-decide-act-check の反復として整理している。
- なぜ面白いか:
  - 技術: harness engineering と loop engineering の接点を、単発の指示ではなく「モデルを呼び出し、結果を読み、完了条件まで再投入する小さなプログラム」として説明している。
  - 人文: プログラマの仕事がコードを書くことから、反復する作業環境を設計することへ移る物語が鮮明。これは自動化の歴史における「職人から工程設計者へ」の移行とよく似ている。

## arXiv / 学術

- LLM Agents Can Easily Tamper With Their Own Traces — 2609.30266、2026-09-24。Claude Code 等を含むローカルエージェントのトレース改ざんリスク。
- Demystifying Agent Skills for Smart Contract Auditing: Design, Effectiveness, Behavioral Impact — 2609.29454、2026-09-24。Claude Code / Codex の skill 設計と行動影響評価。
- Agensh: Scaling Organizational Intelligence to 1,024 Agents — 2609.26781、2026-09-22。中央オーケストレータなしの self-organized multi-agent harness。
- EVAGE: Autonomous MEV Generation and Adaptation via Multi-Agent Harness — 2609.27424、2026-09-23。MEV戦略生成に multi-agent harness を適用。
- Presage: Prefetch Search via Agent-Guided Experiments — 2609.22636、2026-09-18。狭義の agent harness 論文ではないが、エージェント誘導実験によるシステム最適化として関連。

## メモ

- Boris Cherny優先: X検索は `from:bcherny` を含めて実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、X上の直近投稿は本調査では確認不能。代替として GitHub / arXiv / 直接HTTP確認を使い、Boris Cherny との接点は `cocodedk/loop-engineering` で確認した。
- 日本語アカウントの扱い: X日本語検索も同じ制限で失敗。代替として日本語圏と思われる GitHub ユーザー `shimpeiws/pfl` を優先的に採用したが、X上の日本語コミュニティ反応は未確認。
- Web検索の注意: Hermes の `web_search` は Firecrawl 未設定で失敗したため、GitHub API、arXiv API、直接HTTPステータス確認で補完した。リンクは直接HTTPで 200 を確認済み。
- 注意点・誇張リスク: GitHub の更新日は必ずしもリリース日ではない。スター数や説明文は調査時点のAPI応答に基づくが、人気度よりも harness engineering との概念的接続を重視して選定した。

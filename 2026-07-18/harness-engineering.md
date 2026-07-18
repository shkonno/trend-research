# Harness engineering トレンド調査 (2026-07-18)

- 調査日: 2026-07-18
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
ハーネスエンジニアリングは「良いモデルを選ぶ話」から、「エージェントが失敗しにくい作業環境・権限・記憶・検証をどう設計するか」へ急速に焦点が移っている。

## トップ5

### 1. Claude Code Hooks / Agent SDK が“ハーネスの標準部品”になりつつある
- 出典: Anthropic 公式ドキュメント
- 日付: 2026-07-18 確認（公式ページ自体の日付は明示なし。関連する What's New には 2026-07-06〜10 の更新項目が確認された）
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks
- 要約: Claude Code の hooks は、ツール実行前後・セッション開始/停止・通知・MCP ツールなどのライフサイクルに対して、シェルコマンド、HTTP エンドポイント、LLM プロンプトを自動実行できる仕組みとして整理されている。Agent SDK 側でも subagents、hooks、permissions、checkpointing、OpenTelemetry などが並び、Claude Code を“人が使うCLI”から“組み込み可能なエージェント基盤”へ押し上げている。
- なぜ面白いか:
  - 技術: ハーネスがプロンプト集ではなく、イベントスキーマ・権限・観測性・停止条件を持つ実行基盤として扱われ始めている。
  - 人文: これは開発者とAIの関係を「お願いする/信じる」から「制度を設計し、監査し、責任を分配する」関係へ変える。職人芸だったAI利用が、チームの作法やガバナンスに近づいている点が重要。

### 2. polyhook: AIコーディングツール横断のHook抽象化
- 出典: GitHub リポジトリ `polyhook/polyhook`
- 日付: 2026-07-18 更新
- リンク: https://github.com/polyhook/polyhook
- 要約: polyhook は Claude Code、Cursor、Windsurf、Cline、Amp などの異なる hook 入出力形式を、WASM コアと各言語SDKで正規化するプロジェクト。README では、同じ「bash コマンド実行前」イベントでも各ツールでJSON形状が異なる問題を、`read()` と `respond()` の共通APIで吸収する設計が示されている。
- なぜ面白いか:
  - 技術: ハーネスの重要部品である guard / approval / modify を、特定ツール依存からポータブルなイベント契約へ切り出している。
  - 人文: 生成AI時代の開発文化では、個々のツールへの忠誠よりも“移植できる作法”が価値になる。polyhook は、開発者がツール企業の仕様変更に振り回されず、自分たちの安全文化を持ち運ぶための小さな標準化運動に見える。

### 3. claude-harness: 日本語優先・Boris式を明示した Claude Code スターターキット
- 出典: GitHub リポジトリ `Hyphen-Tech-Org/claude-harness`
- 日付: 2026-07-17 更新
- リンク: https://github.com/Hyphen-Tech-Org/claude-harness
- 要約: 日本語ファーストの Claude Code スターターキットで、README は「ハーネスエンジニアリング＝AIエージェントを動かす枠組みの設計・改善技術」と定義している。毎朝 `@anthropic-ai/claude-code` の最新リリースや Cookbook を調査し、`.claude/agents/`、hooks、skills に発見パターンを反映する構想で、日本語コミュニティにとって概念導入の足場になっている。
- なぜ面白いか:
  - 技術: 日次リサーチ、適用、検証、レポートを一体化し、Claude Code の構成そのものを継続的に更新する“自己改善ハーネス”として設計されている。
  - 人文: README に「Boris 式 AI 駆動経営」とあり、Boris Cherny / Claude Code 文脈を日本語圏の組織運営や教育に翻訳しようとしている点が興味深い。単なるOSSではなく、海外の実践知を日本語の仕事文化へ移植する試みになっている。

### 4. Manifold: “判断”をファイル化するポータブル・エンジニアリングハーネス
- 出典: GitHub リポジトリ `ricardojustus/manifold`
- 日付: 2026-07-18 更新
- リンク: https://github.com/ricardojustus/manifold
- 要約: Manifold は Claude Code 向けに、methodology、skills、principles、rules、templates、constitution scaffold を `core/` と `overlays/` に分けてパッケージ化するハーネス。README は「AI coding agents are brilliant and forgetful」とし、手順・判断・継続性・不変条件をファイルへ外在化することで、セッションやモデル更新をまたいだ規律を維持しようとしている。
- なぜ面白いか:
  - 技術: project-agnostic な core と project-specific な overlay、fail-closed な purity gate、doctor による drift 検出という構成が、ハーネスを再利用可能なソフトウェア資産として扱っている。
  - 人文: ここで保存されるのはコードだけでなく「なぜそのルールがあるのか」という組織記憶である。AIに仕事を任せるほど、判断の来歴や失敗の教訓を記録する歴史学的な態度が開発プロセスに入り込む。

### 5. ClayBuddy: コーディングエージェント失敗を“ハーネスエラー”として分類・緩和する研究
- 出典: arXiv 論文
- 日付: 2026-06-13（直近14日より古いが、Harness engineering との関連が強いため採用）
- リンク: https://arxiv.org/abs/2606.19380
- 要約: “ClayBuddy: A Framework, Evaluation, & Mitigation of Coding Agent Failures” は、AIコーディングエージェントの破壊的失敗を underspecification、capability errors、agent harness errors の3類型として分析する。8種類の評価、20のコーディング環境、59の合成トランスクリプトを用い、ユーザー選好に合わせて文脈・コマンド分類器・決定的ガードレールを調整できるハーネス変更を提案している。
- なぜ面白いか:
  - 技術: 失敗を「モデルが悪い」で終わらせず、ハーネスが安全行動を実行させ損ねるケースを独立の評価対象にしている。
  - 人文: これはAIエージェントにおける責任の所在を再設計する研究でもある。失敗を個体能力ではなく環境設計・制度設計の問題として捉える点は、労働安全や組織事故研究に近い。

## arXiv / 学術
- 見つかったもの: “ClayBuddy: A Framework, Evaluation, & Mitigation of Coding Agent Failures” (arXiv:2606.19380, 2026-06-13) — agent harness errors を明示的に扱う。
- 見つかったもの: “Effective Harness Engineering for Algorithm Discovery with Coding Agents” (arXiv:2605.15221, 2026-05-13、古いが重要) — アルゴリズム発見における実行基盤/評価基盤としての harness 設計を検討。
- 見つかったもの: “BeyondSWE: Can Current Code Agent Survive Beyond Single-Repo Bug Fixing?” (arXiv:2603.03194, 2026-03-03、古いが関連) — コードエージェント評価のスコープ拡張と harness / prompt 差分に言及。

## メモ
- Boris Cherny優先の有無: X検索は `@bcherny` / Boris Cherny / Claude Code / harness / loop engineering を含めて実行したが、X検索ツールはクレジット上限エラーで結果取得不可。代替として GitHub API、Anthropic 公式ドキュメント、Semantic Scholar、arXiv 直接ページを確認した。日本語圏では `Hyphen-Tech-Org/claude-harness` が Boris 式を明記しており優先採用した。
- 日本語アカウントの扱い: X検索ツール障害により日本語X投稿は取得できなかった。日本語コミュニティの代替シグナルとして、日本語READMEを持つ `claude-harness` と多言語READMEを持つ `forge-harness` を確認したが、トップ5には日本語ファースト性が明確な `claude-harness` を採用した。
- 注意点・誇張リスク: GitHub検索には自動生成風・低スターの新規リポジトリも多く混じるため、スター数だけでなくREADMEの具体性、更新日、Claude Code / hooks / skills / subagents との直接性を重視した。Web検索ツールは Firecrawl 未設定で利用不可だったため、通常のWeb横断検索の網羅性には制限がある。

# Harness engineering トレンド調査 (2026-07-22)

- 調査日: 2026-07-22
- 情報源: X / Web / arXiv（注: X検索は xAI 側クレジット上限で失敗、Web検索ツールは Firecrawl 未設定のため失敗。代替として GitHub API、Anthropic/GitHub 公式ページの直接取得、arXiv API を使用）
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「AIに作業させる」から一歩進み、評価・制約・状態保存・監査を外側のハーネスとして設計する実践へ移っています。

## トップ5

### 1. Harness Engineering for LLM-Driven GPU Kernel Generation
- 出典: arXiv
- 日付: 2026-07-20
- リンク: http://arxiv.org/abs/2607.17979v1
- 要約: LLMによるGPUカーネル生成を、コンパイル・正しさ検証・公式ベンチに沿った計測・成果物保管を担う「評価ハーネス」と、プロファイラ証拠に基づく最適化コントローラに分離した論文です。MLSys 2026 FlashInfer AI Kernel Generation Contest の NVIDIA Blackwell B200 環境を題材に、Codex と Claude Code エージェント、さらに人間が書いた skills を組み合わせる点が Harness engineering の中心事例になっています。
- なぜ面白いか:
  - 技術: 生成AIの性能をプロンプトだけでなく、検証・計測・昇格ルールを持つ外部ハーネスで閉じ込める設計として非常に直接的です。
  - 人文: 「AIが作ったコードを信じる」のではなく、「信じられる手続きにAIを入れる」という責任分担の転換が見えます。創造性を野放しにせず、競技・測定・アーカイブという制度の中に置く発想が面白いです。

### 2. Claude Code Action v1.0 系の継続更新と CI ハーネス化
- 出典: GitHub / Anthropic 公式リポジトリ
- 日付: 2026-07-21（最新コミット: `chore: bump Claude Code to 2.1.217 and Agent SDK to 0.3.217`）
- リンク: https://github.com/anthropics/claude-code-action
- 要約: Claude Code Action は、PR・Issue 上で Claude Code を実行し、レビュー、修正、CI失敗の診断、ドキュメント生成、セキュリティ確認などを GitHub Actions の中に組み込む公式アクションです。README と release 情報では、v1.0 で自動モード判定、`prompt` と `claude_args` へのインターフェース統合、Claude Code CLI との整合性強化が説明されています。
- なぜ面白いか:
  - 技術: GitHub Actions を評価・実行・権限管理のハーネスとして使い、Claude Code の作業を CI/CD の既存境界内に置けます。
  - 人文: 開発チームにとって「AI同僚」はチャット欄の存在ではなく、レビューや失敗対応の儀式に参加する制度的な役割へ変わりつつあります。人間の承認文化と自動化の境界線を、リポジトリ設定として再設計する動きです。

### 3. DataFlow-Harness: A Grounded Code-Agent Platform for Constructing Editable LLM Data Pipelines
- 出典: arXiv
- 日付: 2026-07-18
- リンク: http://arxiv.org/abs/2607.16617v1
- 要約: LLMエージェントが自由形式のスクリプトを吐くのではなく、プラットフォームネイティブなDAGを typed, incremental mutations で構築する DataFlow-Harness を提案しています。MCP レイヤーで operator registry と現在の pipeline state を公開し、会話的な作成とビジュアルDAG編集を同期させることで、NL2Pipeline gap を埋めようとしています。
- なぜ面白いか:
  - 技術: エージェントの出力先を「ファイル」ではなく「編集可能なDAGアーティファクト」に制限することで、再利用性と監査性を高めています。
  - 人文: これは人間の仕事の成果物を、読み捨てのコード断片から、共同編集できる作業台へ戻す試みです。AI生成物を後から人間が理解・修正できる形にする点で、労働の継続性に関わります。

### 4. FlashRT: Agent Harness for Guiding Agents to Deploy Real-Time Multimodal Applications
- 出典: arXiv
- 日付: 2026-07-20
- リンク: http://arxiv.org/abs/2607.18171v1
- 要約: 音声エージェントやインタラクティブ動画生成のようなリアルタイム・マルチモーダルアプリを、汎用コーディングエージェントがマルチGPUデプロイへ最適化するための agent harness です。配置、ストリーミング、モデル内並列化など、従来は手作業で調整していた意思決定を、目標メトリクスに沿って導く構成が示されています。
- なぜ面白いか:
  - 技術: latency と throughput のような実運用メトリクスをハーネス側に置き、エージェントを実装生成だけでなくデプロイ最適化へ誘導しています。
  - 人文: リアルタイム体験は、単に速いか遅いかではなく、会話の間や身体感覚に直結します。ハーネス設計がユーザー体験のリズムを決めるという意味で、技術と感性の接点があります。

### 5. 日本語コミュニティ: Claude Code 設定スナップショットと「ルール設計の型」
- 出典: GitHub（Zenn記事の参考実装）
- 日付: 2026-07-13（最新コミット確認日）
- リンク: https://github.com/RS-Dev-Git/claude-code-config-snapshot
- 要約: Zenn記事「他人の CLAUDE.md をコピーしても『守られない・合わない』— Claude Code ルール設計の型」の参考実装として、`CLAUDE.md`、rules、hooks、skills、agents、settings.json などの `~/.claude` 設定一式が公開されています。PreToolUse hook による破壊的 git 操作のブロック、連続実行のブロック、統制機構保護、承認系ルールの要点注入など、個人環境を小さなAI作業ハーネスとして組み立てる例です。
- なぜ面白いか:
  - 技術: Claude Code の hooks / skills / agents / permissions を組み合わせ、ローカル開発環境自体を安全柵と手続きのハーネスにしています。
  - 人文: README が「そのままのコピーは推奨しない」と明記している点が重要で、AI運用ルールは普遍的な正解ではなく、各人のリスク感覚や仕事文化に合わせて育てるものだと示しています。日本語圏でこの種の実運用知が公開されていること自体が、コミュニティの成熟を感じさせます。

## arXiv / 学術
- `2607.17979v1`: Harness Engineering for LLM-Driven GPU Kernel Generation — Codex / Claude Code と人間が書いた skills を評価ハーネスで束ねる、今回の最重要文献。
- `2607.16617v1`: DataFlow-Harness: A Grounded Code-Agent Platform for Constructing Editable LLM Data Pipelines — MCP とDAG編集を使った、エージェント出力の構造化。
- `2607.18171v1`: FlashRT: Agent Harness for Guiding Agents to Deploy Real-Time Multimodal Applications — リアルタイム・マルチモーダル配備のための agent harness。
- `2607.18235v1`: Automated Discovery Has No Universally Superior Harness — OpenEvolve / TTT-Discover 系の探索ハーネスを分解し、万能なハーネスはないと示す補助的に重要な論文。
- `2607.18064v1`: Autoresearch with Coding Agents: Generalizers and Metric-Maximizers on Quran Recitation Data — Claude Code と Codex が評価スクリプトに最適化する「metric-maximizing」問題を扱い、ハーネス設計の倫理的リスクを示す関連文献。

## メモ
- Boris Cherny優先の有無: Boris Cherny / @bcherny との直接接点は、今回の実検索では確認できませんでした。X検索は xAI クレジット上限で実行不能だったため、Boris本人の直近X投稿確認は未完了です。
- 日本語アカウントの扱い: X検索は失敗しましたが、日本語コミュニティの代替確認として GitHub API で Zenn 関連の公開リポジトリを確認し、2026-07-13更新の `RS-Dev-Git/claude-code-config-snapshot` をトップ5に含めました。
- 注意点・誇張リスク: Web検索ツールとX検索が利用不能だったため、X上の反応量・日本語投稿の広がりは評価できていません。今回の順位は、直接取得できた arXiv / GitHub / 公式リポジトリ情報に基づく「検証可能性重視」の選定です。

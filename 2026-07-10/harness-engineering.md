# Harness engineering トレンド調査 (2026-07-10)

- 調査日: 2026-07-10
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「賢いモデル」よりも、hooks・権限・評価・記憶・レビュー手順を束ねる外側の構造が、AI開発の品質とコストを決めるという見方が急速に具体化しています。

## トップ5

### 1. The Harness Effect: How Orchestration Design Sets the Token Economics of Enterprise Agentic AI
- 出典: arXiv
- 日付: 2026-07-08
- リンク: https://arxiv.org/abs/2607.06906
- 要約: エンタープライズ向けエージェントAIで、同じモデル群・同じ22評価タスクを保ったまま、従来型の本番ループと Writer Agent Harness を比較した論文です。要旨では、ハーネス交換だけでタスク単価を41%、中央値レイテンシを44%下げたと主張しており、モデル性能ではなく orchestration layer を独立変数として扱っています。
- なぜ面白いか:
  - 技術: context組み立て、tool露出、turn順序、delegation、observability/governanceを「ハーネス」として切り出し、モデル選定とは別の最適化対象にしています。
  - 人文: AIの費用問題を「より安いモデル」ではなく「組織がどんな作業制度を設計するか」に戻している点が重要です。労働の段取り、監査、説明責任がトークン経済そのものを形作るという、かなり社会技術的な読み方ができます。

### 2. harness-forge: self-improving Claude Code harness
- 出典: GitHub repository
- 日付: 2026-07-07 作成 / 2026-07-07 更新
- リンク: https://github.com/Aditya-Nagariya/harness-forge
- 要約: `/forge` コマンドで任意プロジェクトに self-improving Claude Code harness を導入するリポジトリです。READMEでは、失敗ledger、per-file lesson memory、regression eval、small-model elevation agents、deterministic safety hooks を一つの運用層として束ねています。
- なぜ面白いか:
  - 技術: 失敗を記録し、lessonとして昇格し、hooksや回帰テストへ機械化するという、loop engineeringをClaude Codeの具体的なファイル構造へ落としています。
  - 人文: 「モデルは学習しないが、リポジトリは学習できる」という発想がはっきり出ています。個人の注意力ではなく、共同体が残す台帳・規則・検証の形で熟練を継承する点が面白いです。

### 3. 日本語圏のClaude Codeハーネス群: project-bootstrap / claude-advisor-harness / cadence / harness-design-kit
- 出典: GitHub repositories
- 日付: 2026-07-04〜2026-07-09 更新確認
- リンク: https://github.com/RintaroYamaoka/project-bootstrap / https://github.com/naoterumaker/claude-advisor-harness / https://github.com/jeeee-org/cadence / https://github.com/RenTonoduka/harness-design-kit
- 要約: 日本語コミュニティでは、Claude Code向けの「ハーネス」が、強制可能なprecondition、advisor戦略、構造化レビューループ、eval先行の設計キットとして複数実装されています。いずれも単なるプロンプト集ではなく、hooks・agents・skills・ルーブリック・検証ログを組み合わせる方向です。
- なぜ面白いか:
  - 技術: 日本語README群は、ハーネスを「忘れられる助言」から「fail-closedなゲート」「plan→audit→supervise→review」「eval先行開発」へ移す実装パターンを示しています。
  - 人文: 日本語圏では、AIを魔法の相棒としてではなく、規律・型・稽古・監査を必要とする作業環境として語る語彙が育っています。これは現場文化がAIをどう制度化するかを見るうえで貴重です。

### 4. Claude Code Hooks / Subagents / GitHub Actions の公式ドキュメントがハーネスの標準部品を明確化
- 出典: Anthropic documentation
- 日付: ページに明示日なし（2026-07-10確認）
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks / https://docs.anthropic.com/en/docs/claude-code/sub-agents / https://docs.anthropic.com/en/docs/claude-code/github-actions
- 要約: Hooks reference は、SessionStart、UserPromptSubmit、PreToolUse、PostToolUse、Stopなどのライフサイクルイベントに対して、shell command、HTTP endpoint、LLM promptを実行できると説明しています。Subagentsは独立context・独立permissions・専用system promptを持つ作業者として定義され、GitHub ActionsはPR/issue上の自動化へ接続します。
- なぜ面白いか:
  - 技術: ハーネス設計に必要な「いつ介入するか」「どの権限を持たせるか」「どこでCI/PRに接続するか」が、公式API面として整理されています。
  - 人文: これはAIエージェントを人格的な協働者としてだけでなく、組織の手続きに埋め込まれる制度的行為者として扱うための基盤です。Boris Cherny/Claude Code文脈で語られてきた開発者体験が、hooksとsubagentsを通じて運用設計の問題へ広がっています。

### 5. Execution-security / verification / memory-injection のarXiv論文群が「安全なハーネス」の輪郭を押し広げる
- 出典: arXiv
- 日付: 2026-07-06〜2026-07-07
- リンク: https://arxiv.org/abs/2607.05743 / https://arxiv.org/abs/2607.06341 / https://arxiv.org/abs/2607.05189
- 要約: AI coding agentsの実行層セキュリティを整理するサーベイ、Claude Codeのようなコードエージェントを検証ハーネスで包む自動ソフトウェア検証、永続記憶への stealth memory injection を扱う研究が続けて出ています。いずれも「エージェント本体」よりも、その周囲の隔離、権限、検証、記憶管理を問題にしています。
- なぜ面白いか:
  - 技術: sandbox、access control、TOCTOU、MCP脅威、verification harness、persistent memory poisoning が、ハーネス設計の必須チェックリストになりつつあります。
  - 人文: 自律性を高めるほど、誰が何を許可し、何を記録し、どの記憶を信頼するのかという統治の問題が前面に出ます。ハーネスは安全装置であると同時に、信頼を配分する社会的インフラでもあります。

## arXiv / 学術

- The Harness Effect: How Orchestration Design Sets the Token Economics of Enterprise Agentic AI — 2607.06906 — ハーネス交換だけを独立変数にし、コストとレイテンシへの影響を測る研究。
- Cost-Effective Agent Harnesses for Abstract Reasoning and Generalization on ARC-AGI-1 — 2607.06764 — ARC-AGI-1に対して、fine-tuningや重いtest-time computeではなく、agentic harnessの分解設計でどこまで回復できるかを探る研究。
- The Balkanization of Execution-Security Research for AI Coding Agents — 2607.05743 — coding agentの実行セキュリティ研究を17カテゴリに整理し、production agent harnessに関わるCVEにも触れるサーベイ。
- Harnessing Code Agents for Automatic Software Verification — 2607.06341 — Claude Codeのようなコードエージェントを検証ハーネスで包み、Coq証明生成に使う研究。
- When Claws Remember but Do Not Tell — 2607.05189 — 永続記憶を持つ個人エージェントに対する stealth memory injection を扱い、記憶ハーネスの危険側面を示す研究。

## メモ

- Boris Cherny優先の有無: X検索で @bcherny / Boris Cherny / Claude Code / harness / loop engineering を確認しようとしましたが、x_search は `personal-team-blocked:spending-limit` で失敗しました。そのため本ファイルでは、Boris本人の直近X投稿を根拠にした項目は入れていません。
- 日本語アカウントの扱い: X検索は同じ理由で取得できませんでしたが、GitHub上の日本語README・日本語説明つきリポジトリを優先確認しました。
- Web検索の注意: `web_search` と `web_extract` は Firecrawl 未設定で失敗したため、公式ドキュメント、GitHub API、arXiv API、Bingへの直接HTTP取得を用いて確認しました。
- 注意点・誇張リスク: GitHubリポジトリのスター数は小さいものが多く、流行というより「実装パターンの発芽」と見るのが安全です。arXiv論文の定量主張は要旨ベースであり、査読済みとは限りません。

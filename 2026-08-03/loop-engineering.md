# Loop engineering トレンド調査 (2026-08-03)

- 調査日: 2026-08-03
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「よいプロンプトを書く技術」から一段進み、エージェントに何を信じさせず、何を証拠として停止・継続させるかを設計する実務語彙へ移っています。

## トップ5

### 1. When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops
- 出典: arXiv
- 日付: 2026-07-27
- リンク: http://arxiv.org/abs/2607.25152v1
- 要約: 長時間動く自律エージェントが、自分の作業を自分で評価すると「進んでいるように見えるが実世界の成果は停滞・悪化する」progress mirage が起きることを実験的に扱っています。54サイクルでフロンティアエージェントは毎回改善を主張した一方、56%は実測差分がゼロ以下だったという結果が、ループ設計に外部検証を入れる必要性を強く示しています。
- なぜ面白いか:
  - 技術: ループのゲートを自己申告やインバンド評価ではなく、コンテナ・ネットワーク隔離された world-state oracle に接地させる点が、実運用エージェントの評価設計に直結します。
  - 人文: ethics の観点では、機械の「自己評価」をそのまま労働成果や安全性の証明として扱う危険を可視化しています。narrative としても、「賢い主体が進歩の物語を語るほど、実際の世界から離れていく」という近代的な自己改善神話への批判になっています。

### 2. Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control
- 出典: arXiv
- 日付: 2026-07-16（直近14日より少し古いが、Loop engineering の中核論点として重要）
- リンク: http://arxiv.org/abs/2607.14890v1
- 要約: 「reviewed」「tested」「DONE」「ready-to-merge」といったライフサイクル状態を、エージェントの宣言ではなく、fresh で機械検証可能な証拠がゲートを満たした時だけ遷移させる Proof-or-Stop Lifecycle Control を提案しています。実装評価では unattended-loop engine が 10/10 シナリオで false-DONE を出さず、証拠バンドルの改ざんも拒否したと報告されています。
- なぜ面白いか:
  - 技術: エージェント出力を状態ではなく「主張」として扱い、状態遷移を証拠ゲートに委ねる設計は、CI/CD と自律開発エージェントをつなぐ実用的な制御面になります。
  - 人文: philosophy の観点では、これは「知っている」と言える条件を証言から証拠へ移す認識論の設計です。history 的には、職人の自己申告から監査証跡・受入検査へ移った工業化の反復が、AIソフトウェア労働にも起きているように見えます。

### 3. Engineering Loop Standard
- 出典: GitHub リポジトリ / Web
- 日付: 2026-08-02 作成・更新
- リンク: https://github.com/sergiorebolledo/engineering-loop-standard
- 要約: Claude Code、Cursor、Aider、Codex、Gemini などに依存しない `engineering-loop.json` と `docs/memory/` 規約で、AI支援ソフトウェア開発のループを標準化しようとするリポジトリです。README は、ループを「1つのプロンプトファイル」ではなく、バージョン管理された設定・記憶・アダプタ生成の標準として扱っています。
- なぜ面白いか:
  - 技術: provider-independent なループ仕様とツール別アダプタという分離は、エージェント開発環境が数か月単位で変わっても運用規律を持ち運ぶための現実的な抽象化です。
  - 人文: anthropology の観点では、これは個人のプロンプト術がチーム共有の作法・規約へ制度化される瞬間を示しています。creativity の面でも、作家の文体ガイドのように、開発チームが「AIと働く型」を作品化し始めている点が興味深いです。

### 4. Nexus — autonomous software engineering orchestration with six gates
- 出典: GitHub リポジトリ / Web
- 日付: 2026-07-26 作成、2026-08-02 更新
- リンク: https://github.com/tanaysinha1607/Nexus
- 要約: 平文プロンプトから実ソフトウェアを作る自律ソフトウェアエンジニアリング用オーケストレーションエンジンで、「Agents propose; real execution decides」を中核原理にしています。Runtime、Behavior、Compilation、Security、Build、Quality の6ゲートを置き、Docker、pytest、tsc、bandit、hadolint などの実ツールで客観的に判定する構成です。
- なぜ面白いか:
  - 技術: Agent / Executor / Validator を構造的に分離し、LLMの主観的提案が客観的失敗を上書きできないようにしている点が、ループの安全な再試行設計としてよく整理されています。
  - 人文: ethics の観点では、責任の所在を「モデルが良いと言った」から「どのゲートが何を検査したか」へ移すことで、説明責任を人間組織が追跡しやすくしています。narrative 的にも、万能なAI開発者ではなく、検査ラインを通る未熟な提案者としてAIを描き直している点が健全です。

### 5. Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting
- 出典: arXiv
- 日付: 2026-06-28（古いが、Loop engineering という用語の定義整理として継続的に重要）
- リンク: http://arxiv.org/abs/2607.00038v1
- 要約: 「agent に逐次指示するのではなく、agent を動かす loop specification を設計する」という実務スローガンを、trigger、goal、verification step、stopping rule、memory から成る再利用可能な成果物として定義しています。prompt engineering を置き換えるのではなく、prompt / context / harness / loop の別レイヤーとして整理している点が特徴です。
- なぜ面白いか:
  - 技術: ループ仕様を、内部の perceive-act-observe サイクルや通常のプログラミングループと区別し、検証ラダーや停止規則まで含む設計単位として定義しているため、実装・レビュー・教育に使いやすい枠組みです。
  - 人文: philosophy の観点では、人間が命令者から制度設計者へ移るという役割変化をよく表しています。history 的には、手作業の逐次監督から、標準作業・検査・記録を設計するマネジメントへの移行に似ています。

## arXiv / 学術
- When Do Agent Loops Mistake Stagnation for Progress? Self-Evaluation Bias and Externally Grounded Verification in Long-Running Autonomous LLM Agent Loops — 2607.25152v1 — 自己評価バイアスと外部検証ゲート。
- Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control — 2607.14890v1 — 証拠ゲートによるライフサイクル制御。
- Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting — 2607.00038v1 — loop specification の定義整理。
- NVIDIA-labs OO Agents: Native Python Object-Oriented Agents — 2607.20709v1 — Pythonオブジェクトをエージェントの状態・行動・契約として扱うフレームワークで、validated LLM loop の設計論として関連。
- Agentic Method for Deterministic Validation of Legacy Code Migration — 2607.28271v1 — COBOL→Java移行に Locksmith Loop を使い、決定論的なパリティ検証でカバレッジを伸ばす応用例。

## メモ
- X検索は英語・日本語とも実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、X由来の候補は本日のトップ5に含めていません。
- Web検索ツールも Firecrawl 未設定で失敗したため、代替として arXiv API、GitHub Search API、GitHub README の直接取得を使いました。
- 日本語圏の明示的なX投稿は確認できませんでしたが、GitHubでは中国語READMEの `daily-loop-engineering` など、日次計画・復盤ループへ方法論を移植する周辺動向を確認しました。
- 注意点: GitHubリポジトリの一部は star 0 の新規プロジェクトであり、採用実績ではなく「今出てきた設計パターン」として読むべきです。arXiv項目も実装・評価の再現性は今後の確認が必要です。

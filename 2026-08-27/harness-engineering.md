# Harness engineering トレンド調査 (2026-08-27)

- 調査日: 2026-08-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は、モデルそのものの賢さ競争から、エージェントの外側にある「証拠・状態・検証・費用」を設計する競争へ、さらに一段深く移っています。

## トップ5

### 1. StarHarness: 企業環境ごとに agent harness を進化させる探索フレームワーク
- 出典: arXiv
- 日付: 2026-08-25
- リンク: https://arxiv.org/abs/2608.24804
- 要約: StarHarness は、モデル重みを固定したまま、プロンプト、タスク framing、tool interface、skill、MCP provider、subagent 構造、agent-loop 設定を環境別に進化させる研究です。ITBench SRE、EnterpriseOps-Gym ITSM、AutomationBench Finance で、4〜12個の採択変更だけでも default harness より 20〜35ポイント改善したと報告しています。
- なぜ面白いか:
  - 技術: 「モデルを替える」ではなく、失敗パターン別にタスクを層化し、探索用・選抜用・held-out 評価を分けて harness 自体を最適化する点が、実運用の agent engineering に直結します。
  - 人文: これは組織ごとの仕事の作法を、AIの外部環境としてチューニングする発想です。汎用AIを万能労働者として扱うのではなく、職場の制度・権限・道具立てに適応させる、かなり社会技術的な方向に見えます。

### 2. The Empire, Long Divided, Must Unite: 3つの LLM agent harness のアーキテクチャ収束
- 出典: arXiv
- 日付: 2026-08-25
- リンク: https://arxiv.org/abs/2608.23953
- 要約: LangChain deepagents、Earendil pi、DeepSeek dsh という思想の異なる3つの coding-agent harness をソースレベルで比較し、成熟するほど「context を作る」「tool を仲介する」「loop を回す」「状態を保持する」層へ収束していると分析しています。モデルを agent に変える束縛条件は、モデルではなく harness になりつつある、という問題提起です。
- なぜ面白いか:
  - 技術: batteries-included、最小主義、plugin-first という別々の設計哲学が、実際の長期実行では似た責務分解へ寄っていくことを示し、harness の標準部品表を考える材料になります。
  - 人文: 道具は思想を持ちますが、運用の圧力は思想を似た形へ削っていきます。AI agent の文化も、自由な対話より先に、記録・境界・責任のある「制度」に近づいていることが見えます。

### 3. harnessmeter: CLAUDE.md・subagent・MCP schema の「文脈コスト」を測る profiler
- 出典: GitHub リポジトリ
- 日付: 2026-08-27 更新
- リンク: https://github.com/alebgl77/harnessmeter
- 要約: harnessmeter は、CLAUDE.md、skill、subagent、MCP tool schema など、agentic harness に常時読み込まれる文脈のコストを可視化するツールです。README は「context window は rent のない commons」と表現し、CPU・メモリ・SQL・bundle profiler はあるのに context profiler がない、という実務上の盲点を突いています。
- なぜ面白いか:
  - 技術: ハーネスを「たくさん指示を書けば強くなる」ものではなく、毎ターン課金され、注意を奪い、挙動を変える可観測な資源として扱う点が新鮮です。
  - 人文: 共有地に誰でもルールを書き足せると、便利さと汚染が同時に増えます。AI開発チームの文化も、暗黙知を足す喜びから、何を削るかを合意するガバナンスへ進みそうです。

### 4. Loop Engineering — Boris Cherny の Claude Code 方法論を fact-checked に整理する知識ベース
- 出典: GitHub リポジトリ / GitHub Pages
- 日付: 2026-08-26 更新
- リンク: https://github.com/cocodedk/loop-engineering
- 要約: cocodedk/loop-engineering は、Boris Cherny が語る「自分はもう Claude を直接 prompt しない。Claude に prompt する loop を書く」という方法論を、出典付きで整理する知識ベースです。loop は仕事を発見し、agent / sub-agent に渡し、結果を検証し、状態を永続化し、次の行動を決めるものとして説明されています。
- なぜ面白いか:
  - 技術: Claude Code の使い方を prompt 技術ではなく、schedule、goal condition、verification feedback、CLAUDE.md / skill への durable correction を備えた制御ループとして捉え直しています。
  - 人文: ここで人間の役割は「AIに命令する人」から「反復の制度設計者」へ変わります。Boris 周辺の語彙が広がっているのは、開発者が創造性を失うというより、創造性の置き場所がコード本体から作業環境の設計へ移っている兆候です。

### 5. loop-engineering-jp: 日本語圏で harness engineering をスキル化する実践キット
- 出典: GitHub リポジトリ
- 日付: 2026-08-26 更新
- リンク: https://github.com/MetamoL/loop-engineering-jp
- 要約: loop-engineering-jp は、Claude Code で「直す → 採点 → 直す」の改善ループを回すための日本語キットです。`harness-engineering` skill、scout / verifier / opus-advisor / impl の4役割、固定ルーブリック、失格条件、停止条件をまとめ、「生成する者に自己採点させない」を設計の背骨にしています。
- なぜ面白いか:
  - 技術: `.claude/harness.md` の常設点検表、独立採点者、停止条件という部品で、agent の品質を会話の勢いではなく再現可能な検収ループへ寄せています。
  - 人文: 日本語コミュニティでは、AIを全自動の魔法として受け入れるより、人間が読める点検表と役割分担で安心を作る実践が目立ちます。これは自動化の不安を、共同作業の儀礼と責任分担に変換する動きです。

## arXiv / 学術
- StarHarness: Evolving Harnesses with Stratified Search for Enterprise Environments — 2608.24804 — 本日のトップ5に採用。企業環境別の harness evolution を扱います。
- The Empire, Long Divided, Must Unite: Architectural Convergence in Three LLM Agent Harnesses — 2608.23953 — 本日のトップ5に採用。異なる agent harness が似た責務へ収束するという比較研究です。
- Beyond Executable Models: The Pufibara Agent Harness and the Modelica Agent Workflow Benchmark for Physical System Modeling — 2608.23653 — 2026-08-24。物理システム modeling では「動く」だけでなく物理整合性・scenario 依存の正しさが必要で、persistent engineering state と simulation evidence を管理する harness を提案しています。
- From General Agents to RCA Experts: A Self-Evolving Harness for Root Cause Analysis — 2608.25661 — 2026-08-26。Codex / Claude Code のような汎用 agent を、RCA 用の外部 harness で専門化する方向を示します。
- Loop Engineering: Building Blocks, Adoption, and Impact — 2608.21884 — 2026-08-22。prompt engineering から context engineering、さらに loop engineering へ移る実践のグレー文献と採用動向を整理しています。
- SPECMINE: A Large-Scale Corpus of Spec-Driven Development Artifacts — 2608.25202 — 2026-08-25。仕様駆動開発の大規模 corpus で、harness / loop の前段になる spec artifact の観測基盤として関連します。

## メモ
- Boris Cherny優先の有無: X検索では Boris Cherny / @bcherny / Claude Code / loop engineering を含む検索を実行しましたが、xAI / X Search が `personal-team-blocked:spending-limit` で失敗しました。代替として GitHub raw README、GitHub 検索結果、arXiv API、直接HTTP取得を使い、Boris Cherny との接点が明示される `cocodedk/loop-engineering` をトップ5に採用しました。
- 日本語アカウントの扱い: X検索が同じ理由で取得できなかったため、日本語X投稿の実確認はできませんでした。代替として GitHub 上の日本語コミュニティ実装を確認し、`MetamoL/loop-engineering-jp`、`breeze-shared-inc/kenesis-loop-kit`、`Macksat/loop-develop-agent`、`pcrito0901-source/app-idea-feedback-harness` などを候補として見ました。
- Web検索の注意: Hermes の `web_search` は Firecrawl 未設定で利用不能でした。Bing RSS も日本語辞書系のノイズが強かったため、GitHub raw、Microsoft Learn 直取得、arXiv API、既存日次レポートの差分確認で補完しました。
- 誇張リスク: GitHub の「更新日」は公開日ではなく最終更新日です。arXiv 論文は実査読前の可能性があるため、効果量やベンチマーク結果は主張として扱い、実運用での再現は別途検証が必要です。

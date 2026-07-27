# Harness engineering トレンド調査 (2026-07-27)

- 調査日: 2026-07-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「よいプロンプト」から一歩進み、エージェントが安全に仕事を終えるための環境・証拠・権限・失敗学を設計する実務領域として急速に輪郭を持ち始めています。

## トップ5

### 1. Ryan Lopopolo の `harness-engineering` リポジトリ公開
- 出典: GitHub リポジトリ / HN 経由で確認
- 日付: 2026-07-18 公開、2026-07-26 更新確認
- リンク: https://github.com/lopopolo/harness-engineering
- 要約: OpenAI の Ryan Lopopolo による「harness engineering」のアンソロジー、フィールドガイド、エージェント向けコンテキスト束。README は、モデルや coding agent をブラックボックスとして固定し、外側の「context と tools」を改善して、意図回復・実システム操作・権限尊重・結果証明・次回改善を可能にする実践として定義している。
- なぜ面白いか:
  - 技術: `AGENTS.md`、playbooks、evals を含む構成そのものが、人間向け文書ではなく「エージェントに読ませる運用知」をリポジトリ化する実例になっている。
  - 人文: 組織の暗黙知、品質基準、例外履歴、承認関係を「モデルの重み」ではなく共有環境に置くという発想は、ソフトウェア開発を個人技能から制度設計へ移す動きとして読める。Boris Cherny / Claude Code / loop engineering との直接投稿接点は X 検索制限により確認できなかったが、Claude Code 以後のエージェント運用文化と強く接続する論点である。

### 2. Orbital Witness「Grading Ourselves Against the Harness Engineering Playbook」
- 出典: 技術ブログ / HN
- 日付: 2026-07-22
- リンク: https://tech.orbitalwitness.com/posts/2026-07-22-grading-ourselves-against-the-harness-engineering-playbook/
- 要約: Orbital Witness が自社のエージェント harness を Ryan Lopopolo の 12 の thesis / playbook に照らして採点した記事。OpenAI の「Humans steer. Agents execute.」を参照しつつ、組織固有の process-data iceberg、品質バー、権限、ドメイン知を harness に移す必要性を実務目線で整理している。
- なぜ面白いか:
  - 技術: 抽象論だった harness engineering を、既存チームの開発プロセス、品質ゲート、ドメイン知識、採点表に落とし込む「自己監査」の形式にした点が有用。
  - 人文: これは単なる自動化礼賛ではなく、「人間が何を舵取りし、何を制度として委譲するか」を公開で反省する記事である。エージェント利用が進むほど、開発組織の文化や責任分配が設計対象になることを示している。

### 3. HumanLayer「Why Software Factories Fail — harness engineering is not enough」
- 出典: GitHub ドキュメント / HN
- 日付: 2026-07-23 HN 掲載確認
- リンク: https://github.com/humanlayer/advanced-context-engineering-for-coding-agents/blob/main/wsff.md
- 要約: HumanLayer が「ソフトウェア工場」型の lights-off 開発ナラティブにブレーキをかける長文。loop engineering と harness engineering の流行を認めつつ、コード生成量や無人 PR だけでは品質・運用・ユーザー価値・人間/エージェント協働の問題は解けないと論じている。
- なぜ面白いか:
  - 技術: harness があっても、承認、観測、失敗時の介入、環境分離、ユーザー価値の検証を別途設計しないと、エージェントのループは「速い未検証作業」になり得る。
  - 人文: 「あなたがボトルネック」「コードは無料」という物語への批判は、開発者の役割を消すのではなく、判断・ケア・責任をどこに残すかという問いに戻す。loop engineering との接点として、ループを増やすだけでは社会的な信頼は増えない、という重要な対抗軸になっている。

### 4. `sd0x-dev-flow`: Claude Code 向け harness layer の具体実装
- 出典: GitHub リポジトリ
- 日付: 2026-07-27 更新確認（リポジトリ作成は 2026-01-30）
- リンク: https://github.com/sd0xdev/sd0x-dev-flow
- 要約: Claude Code の外側に、hook 強制のレビューゲート、context compaction 後も残る state-machine gate、fail-closed な安全層を置く参照実装。README は英語に加え日本語 README も掲げており、日本語コミュニティにとっても読みやすい導入点になっている。
- なぜ面白いか:
  - 技術: `/codex-review-fast`、precommit、自動ループ、sentinel-driven state、post-compact recovery など、harness engineering の概念を Claude Code の運用部品として具体化している。
  - 人文: エージェントの「気分」や一回の会話に頼らず、状態・レビュー・再開条件を外部化する設計は、人間チームの引き継ぎや監査文化に近い。日本語 README がある点は、日本語圏で harness engineering を実装として試す入口として重要である。

### 5. arXiv「Harness Engineering for LLM-Driven GPU Kernel Generation」
- 出典: arXiv
- 日付: 2026-07-20
- リンク: https://arxiv.org/abs/2607.17979
- 要約: LLM による GPU カーネル生成を、評価 harness と profile-backed optimization controller に分けて扱う論文。NVIDIA Blackwell B200 GPU 上の MLSys 2026 FlashInfer AI Kernel Generation Contest を題材に、Codex と Claude Code agents が制約内で候補カーネルを生成し、コンパイル、正しさ、公式に近い計測、成果物保管を harness が担う。
- なぜ面白いか:
  - 技術: 「harness engineering」がコーディングエージェント一般論だけでなく、GPU kernel 最適化のような高リスク・高性能領域で、検証・プロファイル・選別の制御面として機能している。
  - 人文: 高速化競争では成果の数字だけが強調されがちだが、この論文は「どの証拠を残し、どの候補を採用するか」という研究の作法を harness 側に置いている。AI が作った性能改善を、人間が後から信頼できる記録へ変換する点が面白い。

## arXiv / 学術
- 見つかった関連文献:
  - 「Harness Engineering for LLM-Driven GPU Kernel Generation」arXiv:2607.17979（2026-07-20）: GPU kernel 生成で評価 harness と最適化 controller を分離する実践。
  - 「From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents」arXiv:2607.08028（2026-07-09、直近14日より少し古いが関連大）: 企業 LLM agent をプロンプト中心から契約・schema・validation・trace 中心へ移す提案。
  - 「OpenForgeRL: Train Harness-native Agents in Any Environment」arXiv:2607.21557（2026-07-23）: Claude Code、Codex、OpenClaw のような inference harness 上で動く agent を、実環境のまま RL 学習するための open-source framework。
  - 「Agentic Context Management: Solving Agent Memory and Cost by Treating Them as Lifecycle and Architecture Problems」arXiv:2607.21503（2026-07-23）: agent の記憶とコストを、単なる RAG ではなく lifecycle / architecture 問題として捉える論文。
  - 「Toward Continuous Assurance for the Democratization of AI Agent Creation in Industry」arXiv:2607.21495（2026-07-23）: citizen-created agent の継続保証、依存関係、ready contract、診断、ガバナンスを扱う。

## メモ
- Boris Cherny優先の有無: Boris Cherny / @bcherny を含めて X 検索を試行したが、x_search は `personal-team-blocked:spending-limit` で利用不可だったため、直近 X 投稿の直接確認はできなかった。Web 側の Bing probe でも本調査時点では Boris Cherny と harness engineering / Claude Code / loop engineering の明確な直近接点は抽出できなかった。
- 日本語アカウントの扱い: 日本語 X 検索も同じ理由で失敗。代替として GitHub の日本語・多言語対応を確認し、`sd0x-dev-flow` が日本語 README を持つ Claude Code harness 実装である点を優先した。日本語コミュニティの X 上の反応は未確認。
- 注意点・誇張リスク: Web 検索ツール / web_extract は Firecrawl 未設定で失敗したため、代替として terminal から arXiv API、GitHub API、HN Algolia、直接 HTTP 取得を使った。X の流量や日本語圏での拡散度は過小評価の可能性がある。GitHub の更新日・スター数は調査時点の API 結果であり、品質保証ではない。

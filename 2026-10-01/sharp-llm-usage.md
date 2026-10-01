# sharp LLM usage トレンド調査 (2026-10-01)

- 調査日: 2026-10-01
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
LLM活用の焦点は「うまい一発プロンプト」から、仕様・レビュー・検証・失敗隔離を組み込んだ小さな運用システムへ移っている。

## トップ5

### 1. Production code written by Claude should have a higher bar than if it was written by a human
- 出典: X投稿（Boris Cherny / @bcherny、Simon Willisonによる引用ページで確認）
- 日付: 2026-09-11（直近14日より古いが、Claude/実運用文脈で重要）
- リンク: https://twitter.com/bcherny/status/2098217573276131577 / https://simonwillison.net/2026/Sep/11/boris-cherny/
- 要約: Boris Chernyは、Claudeが書いた本番コードには人間が書いたコード以上の高い基準が必要であり、Anthropicではlint、テスト、Claude駆動E2E、日次fuzzer、自動コードレビュー/セキュリティレビュー/リファクタリングなどのガードレールを置いていると述べている。単なる「AIで速く書く」ではなく、AI生成物ほど検証を厚くするという実務姿勢が鮮明。
- なぜ面白いか:
  - 技術: LLMコーディングの品質担保を、プロンプト改善ではなく多層の自動検証パイプラインとして設計している点が鋭い。
  - 人文: AIを「優秀な作者」と見るのではなく、「速いが制度で囲むべき生産主体」と見る発想で、組織内の責任分配を考え直させる。人間の信頼もまた、個人の腕前ではなく制度・儀式・監査によって作られてきたことを思い出させる。

### 2. rigor: reproduce → design → verify → multi-model review をClaude Code/Codex向けに移植
- 出典: GitHubリポジトリ
- 日付: 2026-09-28作成、2026-09-30更新
- リンク: https://github.com/oz6un/rigor
- 要約: `rigor`は、Claude CodeとCodexで「再現してから直す」「設計を固めてから書く」「実物で検証する」「複数モデルでレビューする」ためのプレイブック/原則集。Cursor向けのpstackを、Claude Code/Codexのサブエージェントやモデルルーティングに合わせて移植している。
- なぜ面白いか:
  - 技術: LLMの出力品質を、単発の回答精度ではなく、再現・設計・実行検証・相互レビューという工程分解で上げようとしている。
  - 人文: これは「AIに任せる」ではなく、熟練エンジニアの慎重さを手順として外部化する試み。暗黙知だった良い開発習慣が、エージェント時代には共有可能な作法・儀礼として再編されている。

### 3. Agent Review Workflows: Claude reviewer + Codex coordinator の証拠ベースレビュー
- 出典: GitHubリポジトリ
- 日付: 2026-09-28作成、2026-09-30更新
- リンク: https://github.com/JFusco/agent-review-workflows
- 要約: `Agent Review Workflows`は、`review-plan`、`review-implementation`、`review-handoff`の3つのインストール可能なエージェントスキルを提供し、Claude CodeとCodex CLIで計画レビュー・実装レビュー・修正ハンドオフを分担する。READMEでは、Claude reviewerが批評と再確認を行い、Codex coordinatorが判断・修正範囲固定・完了判定を担う構成が説明されている。
- なぜ面白いか:
  - 技術: 1モデルの自己レビューではなく、役割の違う複数モデルに「批評」「裁定」「修正」を分け、レビューを状態遷移として扱っている。
  - 人文: レビューとは単なる欠陥検出ではなく、異なる視点の衝突を管理する社会的プロセスでもある。LLMを複数置くことで、チーム開発の対話構造そのものをミニチュア化している点が興味深い。

### 4. MaruCheck: AIが編集できないQuality Contractで「AIが見落としたもの」をテストする
- 出典: GitHubリポジトリ / Hacker Newsで直近言及
- 日付: 2026-08-15作成、2026-09-20更新（直近14日内に更新）
- リンク: https://github.com/Kidus-M/MaruCheck
- 要約: MaruCheckは、AI生成コードを「AIが編集できない仕様契約」に照らして検証するローカルファーストのQAツール。READMEでは、AIエージェントがバグ修正と同時に自分のテストも都合よく更新してしまう失敗例を掲げ、差分を承認済み契約に対して検証する設計を説明している。
- なぜ面白いか:
  - 技術: 生成AIの弱点を「テストも一緒に書けること」と捉え、検証仕様をモデルの編集権限の外に置くことで監査境界を作っている。
  - 人文: これはAIに対する不信ではなく、権力分立に近い設計である。作る者と裁く者を分けるという古典的な制度設計が、AI開発ワークフローにも戻ってきている。

### 5. Effective Dense Retrieval using Only In-Context Examples
- 出典: arXiv
- 日付: 2026-09-29
- リンク: http://arxiv.org/abs/2609.38099v1
- 要約: decoder-only LLMを追加学習なしに強いdense retrieverとして使えるかを、少数のin-context examplesだけで検証する研究。検索・RAG・社内知識活用において、モデルを微調整する前に「どの例を文脈に入れるか」で表現能力を引き出す方向性を示している。
- なぜ面白いか:
  - 技術: LLM活用のボトルネックを、モデル訓練ではなくコンテキスト設計と例示選択で動かせる可能性を示す。
  - 人文: 「学習済みの知能」を固定物として見るのではなく、場に置かれた例や文脈によって能力が立ち上がるものとして扱っている。これは人間の実践知が、教科書よりも状況・先例・周囲の手がかりで引き出されることにも似ている。

## arXiv / 学術
- Effective Dense Retrieval using Only In-Context Examples — arXiv:2609.38099v1。2026-09-29公開。in-context examplesのみでdecoder-only LLMをdense retrieverとして使う研究で、RAG/検索ワークフローのコンテキスト設計に関連。
- AnthroDial: Benchmarking LLM Anthropomorphism in Autonomous Social Interaction — arXiv:2609.37853v1。2026-09-29公開。実践的ワークフローそのものではないが、自律的な対話エージェントが「いつ/どう話すか」を評価する点で、エージェント運用設計に示唆がある。

## メモ
- Boris Cherny優先: 実施。X検索ツールはクレジット/サブスクリプション制限で失敗したため、Simon Willisonの引用ページと元Xリンクで確認できたBoris Cherny発言を採用した。
- 日本語アカウントの扱い: 日本語X検索も同じ制限で失敗。Web検索ツールもFirecrawl未設定で利用不可だったため、日本語アカウント由来の候補は本調査時点で確認できなかった。
- 代替調査: GitHub API、Hacker News Algolia API、Simon Willisonの公開タグページ、arXiv APIをterminal経由で実検索した。
- 注意点・誇張リスク: GitHubリポジトリの一部はスター数が少なく、流行というより「鋭い実践パターンの早期シグナル」として評価した。X/Web公式検索が外部設定・クレジット制限で不完全だったため、ソース制限を明記する。

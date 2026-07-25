# Harness engineering トレンド調査 (2026-07-25)

- 調査日: 2026-07-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「モデルを賢く使う技術」から一歩進み、知識・検証・権限・観測を含む実行環境そのものを設計する実務領域として急速に輪郭を持ちはじめています。

## トップ5

### 1. Boris Cherny の「ドメイン知識をインフラに変換せよ」論
- 出典: X投稿（Boris Cherny / @bcherny、Claude Code @ Anthropic）
- 日付: 2026-07-15頃（X検索で確認）
- リンク: https://x.com/bcherny/status/2077460395279692197
- 要約: Boris Cherny は、優れたエンジニアが従来から lint、CI、E2E、エディタ自動化で繰り返し作業を消してきたことを、Claude Code時代の harness / loop engineering に接続している。CLAUDE.md、REVIEW.md、skills、memory にチーム固有の判断基準や設計原則を埋め込むことで、Claudeが毎回同じ失敗をトークンで修正するのではなく、組織の作業環境そのものが学習済みになるという見立て。
- なぜ面白いか:
  - 技術: プロンプト単体ではなく、ルールファイル、レビュー手順、CI、権限、記憶を含む「実行ハーネス」を改良対象にする点が、Claude Code/loop engineering の実務的な核心をよく表している。
  - 人文: 暗黙知をインフラ化するという発想は、熟練者の頭の中に閉じていた判断を、チーム全体や非エンジニアにも開く民主化の話でもある。一方で、何を「正しい知識」として固定するかは、組織文化や権力関係をそのままコード化する危うさも持つ。

### 2. Oikon「Claude Codeとハーネスについて考えてみる」
- 出典: Speaker Deck / X投稿（@oikon48）
- 日付: 2026-07-15頃（X検索で確認、Speaker Deckページは直接HTTP取得で存在確認）
- リンク: https://speakerdeck.com/oikon48/claude-codetohanesunituitekao-etemiru
- 要約: 日本語コミュニティでは、Oikon氏のスライドが「Claude Codeとハーネス」を理解する入口として広く参照されている。Boris Chernyの投稿を引用しながら、モデル性能だけでなく、Claude Codeを囲む知識、ワークフロー、評価、ループ設計がエージェントの実効性能を決めるという視点を日本語で整理している。
- なぜ面白いか:
  - 技術: 「プロンプトを書く」から「ループを設計する」へ、さらに「ハーネスを育てる」へという抽象度の上昇を、日本語の実践者が共有可能な概念として翻訳している。
  - 人文: 海外のClaude Code議論が、日本語圏で再解釈され、チーム運用や学習資料として流通している点が文化的に重要。単なる輸入ではなく、日本語コミュニティが自分たちの開発習慣に合わせて概念を咀嚼しはじめた兆候に見える。

### 3. OpenForgeRL: Train Harness-native Agents in Any Environment
- 出典: arXiv / X投稿
- 日付: 2026-07-23
- リンク: https://arxiv.org/abs/2607.21557
- 要約: OpenForgeRL は、Claude Code、Codex、OpenClawのような実際の推論ハーネスを保ったまま、SFT/RLの訓練ループに接続するためのオープンソースフレームワーク。軽量プロキシがハーネス内のモデル呼び出しを記録し、Kubernetes上の隔離コンテナでロールアウトを実行することで、現場で使うハーネスと訓練環境の分断を埋めようとしている。
- なぜ面白いか:
  - 技術: ハーネスを単なる推論時のラッパーではなく、訓練データ生成・RL評価・本番環境の一部として扱う点が新しい。
  - 人文: 「本番で人間が頼っている環境」を訓練対象に含めることは、AIを実験室のベンチマークから職場の実践へ近づける動きである。同時に、権限・ログ・隔離環境をどう設計するかが、労働の監視や責任分界にも直結する。

### 4. Harness Engineering for LLM-Driven GPU Kernel Generation
- 出典: arXiv / X投稿（@Memoirsによる紹介）
- 日付: 2026-07-20（arXiv公開）、2026-07-23頃にXで紹介確認
- リンク: https://arxiv.org/abs/2607.17979
- 要約: MLSys 2026 FlashInfer AI Kernel Generation Contest向けに、LLMでGPUカーネルを生成・最適化するための harness-centered system を提示した論文。評価ハーネスがコンパイル、正しさ、公式に沿った計時、成果物保存を担い、プロファイラに基づく制約付き生成コントローラの中でCodexやClaude Codeが候補カーネルを作る。
- なぜ面白いか:
  - 技術: LLM生成コードを「動いたら採用」ではなく、コンパイル・正確性・性能計測・アーカイブまで閉じたハーネスで制御することで、GPU最適化という失敗コストの高い領域にエージェントを投入している。
  - 人文: これはAIが職人芸的な性能チューニングに近づく例だが、成功の鍵は魔法のモデルではなく、人間が作った測定制度と昇格ルールにある。創造性が「自由な生成」よりも「よく設計された制約」の中で発揮される点が示唆的。

### 5. DataFlow-Harness: Editable LLM Data Pipelines
- 出典: arXiv / X投稿（PKU DCAI Lab周辺の発表）
- 日付: 2026-07-18（arXiv公開）、2026-07-24頃にXで話題化確認
- リンク: https://arxiv.org/abs/2607.16617
- 要約: DataFlow-Harness は、LLMエージェントが自由形式のスクリプトを生成するのではなく、型付きの段階的変更でプラットフォームネイティブなDAGパイプラインを構築するための基盤。DataFlow-Skills、MCP、DataFlow-WebUIを組み合わせ、Vanilla Claude Code比でコスト72.5%減、レイテンシ49.9%減、12タスクで93.3%の観測パス率を報告している。
- なぜ面白いか:
  - 技術: 生成物を一回限りのコードではなく、編集可能で永続するパイプライン成果物に変換することで、ハーネスが「後から保守できる形」をエージェントに強制している。
  - 人文: データ作業はしばしば属人的なノートブックや一時スクリプトに埋もれるが、編集可能なDAGとして残す設計は、後続者への説明責任と共同作業性を高める。AIが作ったものを人間が読める・直せる形に戻すという意味で、協働の作法として重要。

## arXiv / 学術

- OpenForgeRL: Train Harness-native Agents in Any Environment — arXiv:2607.21557（2026-07-23）
- Harness Engineering for LLM-Driven GPU Kernel Generation — arXiv:2607.17979（2026-07-20）
- DataFlow-Harness: A Grounded Code-Agent Platform for Constructing Editable LLM Data Pipelines — arXiv:2607.16617（2026-07-18）
- 関連: Agentic Context Management: Solving Agent Memory and Cost by Treating Them as Lifecycle and Architecture Problems — arXiv:2607.21503（2026-07-23）
- 関連: Tencent WorkBuddy Bench: A Multi-Domain Coding-Agent Benchmark with Contamination-Resistant Task Construction — arXiv:2607.20911（2026-07-23）

## メモ

- Boris Cherny優先: 実施。@bcherny のClaude Code/loop engineering関連投稿を優先確認し、トップ項目に反映した。
- 日本語アカウントの扱い: 実施。@oikon48 のSpeaker Deck、@MacopeninSUTABA など日本語圏での拡散・解釈を確認した。
- Claude Code / loop engineeringとの接点: すべての項目で、Claude Code、Codex、OpenClaw、ループ設計、評価ハーネス、CLAUDE.md/REVIEW.md等の周辺インフラとの接点を優先した。
- 注意点・誇張リスク: Web検索ツールはFirecrawl未設定で利用不能だったため、Webは直接HTTP取得（Speaker Deck/Xページの存在確認）とarXiv API、X検索を併用した。X検索の要約は投稿本文の完全な逐語取得ではないため、反応数や細かな言い回しは過度に断定しない。

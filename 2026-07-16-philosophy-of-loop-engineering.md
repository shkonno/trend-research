# Philosophy of Loop Engineering トレンド調査 (2026-07-16)

- 調査日: 2026-07-16
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
ループエンジニアリングは「よいプロンプトを書く技術」から、「発見・実行・検証・記憶・停止をどう制度化するか」というサイバネティクス的な実践知へ移っている。

## トップ5

### 1. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans
- 出典: arXiv / X投稿（著者告知）
- 日付: 2026-07-12
- リンク: https://arxiv.org/abs/2607.10878
- 要約: Fujitsu / RIKEN AIPの著者らによる、自己進化するAIエージェントチームを「人間とともに進化する」ためのガバナンス層の提案。プロンプト、メモリ、スキル、ツール、ロール、ワークフローを、実行証拠・ポリシー・明示的承認がそろうまで「未信頼のリリース候補」として扱う点が核心です。
- なぜ面白いか:
  - 技術: エージェントの活動ログを監査可能なイベントトレースにし、fail-closedな検証と人間の承認を通して「提案」と「本番昇格」を分離している。
  - 人文: これは第二秩序サイバネティクスの「観察者を含むシステム」を、AIチームの統治として実装する試みに見える。自律性を奪わず、しかし「誰が変化を許すのか」を明示する点で、AI組織の政治哲学でもある。

### 2. Rethinking the Evaluation of Harness Evolution for Agents
- 出典: arXiv / X投稿（DAIR.AIなどによる紹介）
- 日付: 2026-07-14
- リンク: https://arxiv.org/abs/2607.12227
- 要約: LLMエージェントのハーネス進化評価を再検討し、改善が本当にハーネス設計の進歩なのか、単に反復探索回数が増えた効果なのかを切り分ける必要を指摘。探索に使ったベンチマークと最終評価が同じだと、ループがベンチマークへ過適合する危険があると論じています。
- なぜ面白いか:
  - 技術: 同じフィードバック予算・推論予算の下で、ハーネス進化と単純なtest-time searchを比較し、held-outタスクで汎化を確認する評価設計を求めている。
  - 人文: 認識論的には「学んだ」と「試行錯誤で当てた」を区別せよ、という話です。ループの知性を語る前に、知の正当化条件を整えよという、実験哲学に近い警告になっている。

### 3. Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting
- 出典: arXiv / X議論
- 日付: 2026-06-28（直近14日より少し古いが、現在の議論の中心として採用）
- リンク: https://arxiv.org/abs/2607.00038
- 要約: 「エージェントに逐次指示する」のではなく、trigger、goal、verification、stopping rule、memoryからなる再利用可能なloop specificationを人間が設計する、というループエンジニアリングの定義論文。prompt / context / harness / loopを異なる層として整理し、「プロンプトは不要になった」のではなく役割が変わったと位置づけています。
- なぜ面白いか:
  - 技術: ループを単なるwhile文やエージェント内部のperceive-act-observeサイクルと区別し、検証段階や停止条件まで含む外部仕様として扱う。
  - 人文: 実践知の焦点が、命令文の技巧から「制度・習慣・反省の型」の設計に移っています。これは職人が毎回判断する世界から、よい判断が起こりやすい環境を作る世界への転換です。

### 4. ハーネスエンジニアリング入門 ── CLAUDE.mdの次に来るAIエージェント制御パラダイム
- 出典: Web記事（Qiita）
- 日付: 2026-07-15（Bing RSSで確認。ページ本文メタデータでは公開日時を抽出できず）
- リンク: https://qiita.com/nogataka/items/d1b3fcf355c630cd7fc8
- 要約: AIエージェントの品質は単一プロンプトよりも、構造・責務・制御の設計で大きく変わるという前提で、CLAUDE.mdの次のパラダイムとしてハーネスエンジニアリングを解説する日本語記事。ループエンジニアリングそのものではないが、ループを成立させる道具立てとして重要です。
- なぜ面白いか:
  - 技術: ツール、制約、レビュー、テスト、状態管理を「馬具」のように配置し、モデルの力を安全な方向へ伝える考え方を実務に落としている。
  - 人文: 「自律性」は放任ではなく、よい拘束条件によって成立するという逆説が見える。これは教育・組織設計・徳倫理に近く、AIをどう鍛えるかではなく、どうよく導くかの議論になっている。

### 5. 「ループは能力ではなく配置」型の日本語X議論
- 出典: X投稿（日本語圏のAIエージェント議論）
- 日付: 2026-07上旬（X検索で直近範囲内として確認）
- リンク: https://x.com/ry0_kaga/status/2076464810859085924
- 要約: 日本語圏でも、強いモデルをただ回すだけでは「会議のための会議」のような無限ループになり、責務設計、検証タイミング、停止条件、HITL（human-in-the-loop）の配置が重要だという議論が出ています。英語圏のloop engineeringを、より実務の「配置」や「運用」へ翻訳している点が特徴です。
- なぜ面白いか:
  - 技術: モデル性能ではなく、どの段階で誰が何を検証し、どこで止めるかという制御面を主語にしている。
  - 人文: これはサイバネティクスの「フィードバック配置」の問題であると同時に、組織論の問題でもあります。人間を完全に外すか残すかではなく、人間がどこで「否」と言えるべきかを問うている。

## arXiv / 学術
- LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans — arXiv:2607.10878。人間の承認、監査、fail-closed検証を含む「verifiable human-agent loop engineering」。
- Rethinking the Evaluation of Harness Evolution for Agents — arXiv:2607.12227。ハーネス進化の評価における探索効果・過適合・held-out検証の問題を整理。
- Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting — arXiv:2607.00038。直近14日より少し古いが、loop specificationの定義論文として重要。
- Formal Disco: Scalable Open-Ended Generation of Formally Verified Programs — arXiv:2607.04631。形式検証つきプログラム生成を、initiatior/fixer/extenderの分散ループとして回す研究。
- Mako: A Self-Evolving Agentic Operating System (SE-AOS) for Autonomous Web Exploitation — arXiv:2607.11288。失敗観察、能力合成、実ターゲットでの証明、hot-loadを備えた自己進化型エージェントOS。

## メモ
- Boris Cherny優先の有無: 本トピックはClaude固有の話題ではないため、Boris Cherny優先は適用外。Claude/Codex系の実務文脈は参照した。
- 日本語アカウントの扱い: 日本語X投稿とQiita記事を積極的に採用し、英語圏の抽象語を日本語の運用・配置・責務設計へ接続した。
- 注意点・誇張リスク: Web検索ツールはFirecrawl未設定で失敗したため、Web調査は代替としてBing RSSと直接curl取得で実施した。X検索結果は要約型のため、本文の細部は断定しすぎず、リンクと確認できた範囲に限定した。ループエンジニアリングは用語として急速に拡散中で、標準化された学術分野というより実務語彙と評価研究が並走している段階。

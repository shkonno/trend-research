# Loop engineering トレンド調査 (2026-09-25)

- 調査日: 2026-09-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「よいプロンプトを書く」段階から、「検証・停止・再試行・学習を含む実行ループを設計する」段階へ移り、研究と実装ツールの両方で“制御可能な自律性”が焦点になっています。

## トップ5

### 1. Harness as a Language: A Minimalist Agent Framework With Maximal Expressivity
- 出典: arXiv
- 日付: 2026-09-22
- リンク: https://arxiv.org/abs/2609.26891
- 要約: JAZ という最小主義的なエージェントフレームワークを通じて、LLM に `invoke` という単一プリミティブとフックを与えるだけで、メモリや自己改善のような高度なワークフローをどこまで表現できるかを検討しています。agent loop を「道具呼び出しの繰り返し」ではなく、コード環境内の再帰的な言語機構として定義し直している点が重要です。
- なぜ面白いか:
  - 技術: loop engineering をフレームワーク機能の寄せ集めではなく、再帰可能な `invoke` と観測可能な実行履歴という最小抽象へ圧縮しようとしているため、エージェント設計の基礎語彙になり得ます。
  - 人文: philosophy の観点では、これは「行為者とは何か」をツール列ではなく、自己参照的に環境を読み替える実践として捉える動きです。narrative の観点でも、エージェントの作業履歴が単なるログではなく、次の行為を生む物語的な文脈になります。

### 2. RRSI: Regularized Recursive Self-Improvement of Agent Harnesses
- 出典: arXiv / Hacker News
- 日付: 2026-09-21（HN掲載: 2026-09-22）
- リンク: https://arxiv.org/abs/2609.24972
- 要約: エージェントの性能をモデル本体ではなく、プロンプト・制御フロー・ツール・メモリなどを含む harness が大きく増幅するという前提で、harness 自体を再帰的に改善する手法を提案しています。過学習を避けるため、候補編集の予算を徐々に絞る、履歴に基づき未探索の軌跡を促す、critic/pruner でベンチマーク特化や高コスト変更を落とす、という正則化が入っています。
- なぜ面白いか:
  - 技術: loop engineering の自己改善ループに「改善しすぎて訓練課題を暗記する」問題を明示的に持ち込み、探索・選択・削除を制御する設計にしている点が実用的です。
  - 人文: ethics の観点では、自己改善する開発システムには成長だけでなく節制が必要であり、RRSI は“賢くなる権利”に対して“逸脱しない義務”を組み込む試みです。history の観点では、これは工場の品質管理が自動化ラインにフィードバック制御を入れた流れのソフトウェア版にも見えます。

### 3. Safety Signals to Verify NetOps Agents with Action-Level Granularity
- 出典: arXiv
- 日付: 2026-09-13（v2更新: 2026-09-16）
- リンク: https://arxiv.org/abs/2609.14422
- 要約: 自律的なネットワーク運用エージェントが、各アクションの実行前に「修復距離を縮めるか」「害を増やすか」を判定できるよう、NetArena のネットワーク修復タスクにアクション単位の ground truth を構築しています。長期タスクの成功/失敗だけでなく、ループ内の一手ごとの安全信号を検証対象にする点が loop engineering と強く結びつきます。
- なぜ面白いか:
  - 技術: ループの最終結果ではなく各ステップの progress/harm を測るため、停止・棄権・再計画の判断をより細かく設計できます。
  - 人文: ethics の観点では、自律システムに「できる」だけでなく「やめる」「待つ」「害を避ける」を学ばせる設計です。anthropology の観点では、熟練オペレータが暗黙に行う慎重さを、機械可読な儀礼としてループに移植する試みとも読めます。

### 4. LoopArena: Benchmarking Models as Runtime Controllers for Loop Engineering
- 出典: arXiv / GitHub
- 日付: 2026-08-28（重要だが古いもの。GitHub は 2026-09-24 時点で更新確認）
- リンク: https://arxiv.org/abs/2608.28281 / https://github.com/AMAP-ML/LoopArena
- 要約: LoopArena は、コーディングエージェントそのものではなく、その作業を監督する Controller モデルを評価するベンチマークです。Controller は各ラウンド後の要約を読み、Worker に次に何を実装・検証させるか、あるいは停止するかを決めるため、loop engineering の中核である「進捗監視・検証・停止判断」を切り出して測定できます。
- なぜ面白いか:
  - 技術: エンドツーエンドの成功率からは分離しにくい「ループの指示品質」を、Worker と Controller の役割分担で評価可能にしています。
  - 人文: creativity の観点では、創作や開発の価値が一発の生成物から、編集者・監督者としての判断へ移っています。history の観点では、職人が工程管理者へ役割を広げた産業化の反復が、AIコーディングにも現れているように見えます。

### 5. cobusgreyling/loop-engineering: practical patterns, starters & CLI tools
- 出典: GitHub / Web
- 日付: 2026-09-24 更新確認
- リンク: https://github.com/cobusgreyling/loop-engineering
- 要約: 「Stop prompting, start engineering loops」という方向性で、AI coding agents 向けのパターン、スターター、CLI ツール（loop-audit、loop-init、loop-cost など）をまとめた実践リポジトリです。Addy Osmani や Boris Cherny の文脈を明示し、抽象概念だった loop engineering を、監査・初期化・コスト管理のような運用部品に落としています。
- なぜ面白いか:
  - 技術: ループ設計をドキュメント上の思想ではなく、コスト・監査・初期化という実務上のコマンド群に変換しているため、チーム導入の足場になります。
  - 人文: anthropology の観点では、個人の“プロンプト職人芸”が、共有可能な手順・道具・慣習へ制度化される瞬間です。narrative の観点では、エンジニアの仕事の主人公が「命令を書く人」から「繰り返し働く仕組みを育てる人」へ移っています。

## arXiv / 学術
- 見つかったもの:
  - Harness as a Language: A Minimalist Agent Framework With Maximal Expressivity — arXiv:2609.26891（2026-09-22）
  - RRSI: Regularized Recursive Self-Improvement of Agent Harnesses — arXiv:2609.24972（2026-09-21）
  - Safety Signals to Verify NetOps Agents with Action-Level Granularity — arXiv:2609.14422（2026-09-13、v2 2026-09-16）
  - Environment Evolution for Terminal Agents — arXiv:2609.04128（2026-09-03、直近14日外だが関連）
  - Towards Agentic Cloud Engineering: Graph and Loop Engineering with a Zero-Trust Agent Harness — arXiv:2609.00050（2026-08-30、直近14日外だが関連）
  - LoopArena: Benchmarking Models as Runtime Controllers for Loop Engineering — arXiv:2608.28281（2026-08-28、直近14日外だが基礎的に重要）
  - SIR: Self-improving Red-teaming for Compute Use Agents — arXiv:2608.30207（2026-08-31、直近14日外だがフィードバックループ安全性に関連）

## メモ
- X検索: x_search は実行したが、プロバイダ側の `personal-team-blocked:spending-limit` により英語・日本語検索とも取得できませんでした。そのため本ファイルでは、X由来の未確認投稿は採用せず、Web/GitHub/Hacker News/arXiv/APIで確認できたリンクのみを使用しました。
- Web検索: web_search は Firecrawl 未設定で失敗したため、代替として arXiv API、GitHub API、Hacker News Algolia API、直接HTTP取得を使用しました。
- Boris Cherny優先の有無: Claude系の発言文脈として Addy Osmani の「Loop Engineering」記事に Boris Cherny の引用が確認できました。また Boris の 2026-09-19 ブログ記事「I am often wrong」は、問題定義・情報収集・目標設定・実行・再定義の反復を述べており、loop engineering 的な管理哲学として関連しますが、今回のトップ5は技術的なループ設計・評価により直接関係するものを優先しました。
- 日本語アカウントの扱い: 日本語X検索はツール制限で取得不可、HN/API/直接Web取得でも日本語の直近一次情報は確認できませんでした。
- 注意点・誇張リスク: 「loop engineering」はまだ用語が急速に拡散している段階で、研究論文・個人ブログ・CLIツールが同じ語を少しずつ異なる意味で使っています。特に GitHub のスター数や更新時刻は確認時点の値であり、技術的成熟度そのものを保証しません。

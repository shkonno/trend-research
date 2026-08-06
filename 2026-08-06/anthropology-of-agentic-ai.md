# Anthropology of Agentic AI トレンド調査 (2026-08-06)

- 調査日: 2026-08-06
- 情報源: X / Web / arXiv（X検索はクレジット上限で失敗、Web検索APIは未設定だったため、Bing RSS・直接HTTP取得・arXiv API/ページ取得で補完）
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Agentic AIは「自律的なツール」というより、計画書・役割分担・評価儀礼・所有感・インフラ運用を再編する、新しい職場文化の装置として見えてきています。

## トップ5

### 1. An Exploratory Study of Agent Plans for Agentic AI Coding Tools in Open-Source Software
- 出典: arXiv
- 日付: 2026-08-05
- リンク: https://arxiv.org/abs/2608.04661
- 要約: Claude CodeやGeminiなどのエージェント型コーディングツールに向け、リポジトリ内に残される「Agent Plans」を調査した研究。36,710件のGitHubリポジトリをスクリーニングし、10リポジトリから85件のMarkdown計画ファイルを特定して、どんな開発活動や実行ガイダンスを支えるかを分析しています。
- なぜ面白いか:
  - 技術: エージェント実行を単発プロンプトではなく、リポジトリに保存される計画・規約・タスク分解の成果物として扱っている点が実践的です。
  - 人文: Agent Planは、AIに仕事を任せる組織が作る「作業の民俗誌」そのものです。誰が何を正しい手順とみなし、どの判断をAIに委任してよいと考えるかが、Markdownの小さな儀礼文書に刻まれます。

### 2. AgentForge: An Immersive Role-Playing Platform for Learning Agentic Software Engineering
- 出典: arXiv
- 日付: 2026-08-04
- リンク: https://arxiv.org/abs/2608.04148
- 要約: エージェント型ソフトウェア開発を学ぶ初心者向けに、Task Planner、Patch Author、Code Reviewer、Test Runnerの4役を演じながらマルチエージェントのコード修復ワークフローを体験する学習環境を提案。AIの判断を導き、出力を批判的に評価する能力を同時に学ばせる設計です。
- なぜ面白いか:
  - 技術: エージェント連携を「見えない自動化」ではなく、計画・実装・レビュー・テストという役割ごとの相互作用として教育可能にしています。
  - 人文: ロールプレイは、職場の見習い制度や徒弟制に近い学習儀礼です。Agentic AI時代の新人教育では、コード能力だけでなく「AIと一緒に振る舞う作法」を身体化する場が必要になることを示しています。

### 3. Architectural Implications of Agentic AI Workflows
- 出典: arXiv
- 日付: 2026-08-05
- リンク: https://arxiv.org/abs/2608.04458
- 要約: Microsoft Azureでの本番調査とオープンソースフレームワークの制御実験を通じ、agentic workflowがLLM推論、ツール呼び出し、オーケストレーション判断に分断され、CPU-GPU境界を何度も横断することを示した研究。エージェント実行の異質性・断片性が、データセンター資源需要をどう変えるかを整理しています。
- なぜ面白いか:
  - 技術: agentic AIの「自律性」を、ワークフロー構造・ホストCPU・GPU利用のスパイクとして測定できる運用課題に落とし込んでいます。
  - 人文: ユーザーからは魔法のように見えるエージェントの行為も、裏側では多数の境界横断と調整作業に支えられています。これは、人間の組織でいう根回し・引き継ぎ・待ち時間に相当する、機械側の労働文化を観察する入口になります。

### 4. The New Social Image: How AI Competency and AI Proactivity Influence Self- and Peer-Perceptions in the Workplace（古いが関連性が高い）
- 出典: arXiv
- 日付: 2026-05-29（v2: 2026-06-17）
- リンク: https://arxiv.org/abs/2606.00182
- 要約: 職場のHuman-AI collaborationにおいて、AIの能力と能動性が、本人および同僚から見た所有感、感情、仕事の意味、満足度、役割力学にどう影響するかを2x2x2のビネット研究で検討。低能力・低能動性のAIが所有感などを改善する一方、高度に能動的なAIは人間の自己像や同僚からの見られ方を揺さぶる可能性を示しています。
- なぜ面白いか:
  - 技術: AIの性能だけでなく、proactivityという振る舞いパラメータが職場体験に与える影響を評価軸に入れています。
  - 人文: Agentic AIは仕事を奪うかどうか以前に、「有能に見える人」「仕事を自分のものとして語れる人」の条件を変えます。これは職場内の名誉、面子、評価儀礼を再編する問題です。

### 5. Agentic AI（エージェンティックAI）とは？生成AIとの違いや活用事例を解説（古いが日本の導入文脈として重要）
- 出典: Web記事（丸紅I-DIGIO INSIGHT HUB）
- 日付: 2026-06-30
- リンク: https://www.marubeni-idigio.com/insight-hub/agentic-ai/
- 要約: Agentic AIを生成AIやRPAと比較し、Gemini Enterpriseを含む企業導入のメリット・課題・成功ステップを日本語で整理した実務向け記事。企業内で「自律的に判断・実行するAI」をどう位置づけるかを、導入プロセスの言葉で説明しています。
- なぜ面白いか:
  - 技術: Agentic AIを既存のRPAや生成AIの延長ではなく、業務プロセスとシステム連携を含む導入対象として扱っています。
  - 人文: 日本企業でのAIエージェント導入は、稟議、権限分掌、現場調整、失敗責任の所在といったローカルな組織慣習と衝突します。この記事は技術そのものより、「企業がAIにどこまで判断させる語彙を持ち始めたか」を読む材料になります。

## arXiv / 学術
- An Exploratory Study of Agent Plans for Agentic AI Coding Tools in Open-Source Software — arXiv:2608.04661（2026-08-05）: エージェント計画ファイルをオープンソース開発の新しい協働成果物として分析。
- Architectural Implications of Agentic AI Workflows — arXiv:2608.04458（2026-08-05）: agentic workflowの断片化とデータセンター資源需要を分析。
- AgentForge: An Immersive Role-Playing Platform for Learning Agentic Software Engineering — arXiv:2608.04148（2026-08-04）: ロールプレイ型のエージェント開発教育環境。
- The New Social Image: How AI Competency and AI Proactivity Influence Self- and Peer-Perceptions in the Workplace — arXiv:2606.00182（2026-05-29 / v2 2026-06-17）: AIの能動性と能力が職場の自己像・他者評価に与える影響。
- AI in the Workplace: The Impact of AI on Perceived Job Decency and Meaningfulness — arXiv:2605.28680（2026-05-27）: IT、サービス、医療領域の従業員インタビューから、AIが仕事の尊厳と意味に与える影響を分析。

## メモ
- Boris Cherny優先の有無: 本トピックはClaude固有ではないため優先対象外。X検索は実行したが、xAI側のクレジット/サブスクリプション制限で取得できませんでした。
- 日本語アカウントの扱い: 日本語X検索も実行したが同じ制限で取得不可。代替として日本語Web検索結果と直接HTTP取得を使い、丸紅I-DIGIO、Qiita、DX/AI研究所、SoftBank等の日本語導入文脈を確認しました。
- 注意点・誇張リスク: Web検索API（Firecrawl）は未設定で失敗したため、検索網羅性には制限があります。直近14日で人類学・労働文化に直接言及する公開Web/X資料は十分に確認できず、トップ5は直近arXivを中心に、古いが関連性の高い職場研究・日本語導入記事を明記して採用しました。

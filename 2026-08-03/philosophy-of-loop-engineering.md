# Philosophy of Loop Engineering トレンド調査 (2026-08-03)

- 調査日: 2026-08-03
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
ループエンジニアリングは「自律化」の話というより、生成・評価・記憶・人間判断をどの順番で循環させると知識が腐らないかを問う、実践的な認識論になりつつあります。

## トップ5

### 1. JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents
- 出典: arXiv
- 日付: 2026-07-26
- リンク: https://arxiv.org/abs/2607.23588
- 要約: 長期的なマルチモーダル創作では、単発の生成結果だけでなく、参照、下書き、別案、編集、失敗、バージョン関係、ツール操作、評価信号、人間フィードバックが作業の履歴として蓄積されると論じる論文です。創作エージェントの「キャンバス」を、成果物ではなく反復の場として捉えている点が重要です。
- なぜ面白いか:
  - 技術: 生成物中心ではなく、軌跡・評価信号・人間フィードバックを保存するハーネスとしてループを設計する発想が、エージェント評価基盤に直結します。
  - 人文: 創作を「ひらめき」ではなく、失敗と改稿を含む実践知の循環として扱っています。これは工房、編集室、アトリエの歴史的な制作観を、AI時代のインターフェース設計に戻す動きです。

### 2. LoopLab: trajectory analysis, rubric-based assessment, LLM-as-judge, human review, training feedback loops
- 出典: GitHub / OSSプロジェクト
- 日付: 2026-07-14更新（2026-07-05作成、直近14日より少し前だが関連性が高いため採用）
- リンク: https://github.com/LofiSu/LoopLab
- 要約: AIエージェントの挙動を軌跡として収集し、ルーブリック評価、LLM-as-judge、人間レビュー、訓練フィードバックループへ接続するためのオープンソース基盤です。README上でも「capture and inspect trajectories」「route failures and regressions to human review」「convert review findings into training feedback loops」が中核ワークフローとして示されています。
- なぜ面白いか:
  - 技術: エージェントの失敗を単なるログではなく、再評価・回帰検知・訓練データ化へ流す閉ループとして実装しようとしている点が実務的です。
  - 人文: ここでの評価は「正解を当てる」よりも、何を失敗として名指すかという規範設定です。ルーブリックは小さな制度であり、人間レビューは技術システムの中に判断責任を残すための装置になります。

### 3. Human-Centric Reflective Architecture for Human-AI Collaborative Decision-Making
- 出典: arXiv
- 日付: 2026-07-03（直近14日より前だが、反省的ループの哲学的意義が高いため採用）
- リンク: https://arxiv.org/abs/2607.03025
- 要約: LLMを意思決定に使う際、人間がAI助言に過度依存または過小依存する問題を背景に、人間中心の反省的アーキテクチャを提案する論文です。AIの非決定性と人間の期待・選好・リスク認識を調整することが主題になっています。
- なぜ面白いか:
  - 技術: 人間フィードバックを後付けの承認ステップではなく、信頼較正と意思決定の再帰的調整ループとして設計する方向を示します。
  - 人文: 「反省」はモデルの自己評価だけでなく、人間が自分の依存の仕方を見直す営みでもあります。これは認識論における証拠・信頼・判断の問題を、UI/ワークフロー設計へ引き戻します。

### 4. Multimodal Evaluator Preference Collapse: Cross-Modal Coupling in Self-Evolving Agents
- 出典: arXiv
- 日付: 2026-06-15（古いが、自己評価ループの危険性を示すため採用）
- リンク: https://arxiv.org/abs/2606.16682
- 要約: AIエージェントが自分の出力を評価するフィードバックループでは体系的なバイアスが生じ、マルチモーダル設定では Evaluator Preference Collapse が増幅されると報告しています。特定戦略が評価重みを過度に吸収し、視覚領域の戦略が周縁化されるという結果が示されています。
- なぜ面白いか:
  - 技術: 自己改善ループは放置すると多様な戦略探索ではなく、評価器の癖に収束する可能性があり、外部評価・人間レビュー・モダリティ別較正の必要性を示します。
  - 人文: 「自分で自分を評価する」制度は、哲学的には反省の理想である一方、同じ物差しを反復して偏見を強化する危険もあります。サイバネティクス的な安定化が、学習ではなく硬直化になる境界を考えさせます。

### 5. Collaborative Disagreement Resolution for Scalable Oversight
- 出典: arXiv
- 日付: 2026-06-02（古いが、討論から協調的真理探究への転換として重要なため採用）
- リンク: https://arxiv.org/abs/2607.01251
- 要約: AI同士が反対立場を議論する debate 型のスケーラブル監督には、審判を説得するインセンティブが認識的誠実さとずれるという緊張があると指摘します。代替として、人間の調停や紛争解決の原理を参照し、敵対的討論ではなく協調的な不一致解消を提案しています。
- なぜ面白いか:
  - 技術: 複数エージェントの評価ループを勝敗や説得力ではなく、不一致の局所化・解消・合意形成として組み直す方向を与えます。
  - 人文: これは「真理は競争から出る」という法廷モデルから、「真理は共同で誤差を減らす」という調停モデルへの移行です。ループエンジニアリングを社会的認識論、つまり誰が何を根拠に信じるのかの設計として読めます。

## arXiv / 学術
- JarvisHub: An Open Harness for Canvas-Native Multimodal Creative Agents — arXiv:2607.23588
- Human-Centric Reflective Architecture for Human-AI Collaborative Decision-Making — arXiv:2607.03025
- Multimodal Evaluator Preference Collapse: Cross-Modal Coupling in Self-Evolving Agents — arXiv:2606.16682
- Collaborative Disagreement Resolution for Scalable Oversight — arXiv:2607.01251
- 関連確認: ReflectiChain: Epistemic Grounding in LLM-Driven World Models for Supply Chain Resilience — arXiv:2606.10359（ダブルループ学習と認識的グラウンディングの観点で関連、トップ5外）

## メモ
- Boris Cherny優先の有無: 本トピックはClaude固有ではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索を試行したが、X検索ツールがクレジット上限で失敗したため、今回のX由来情報は未取得。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、代替としてarXiv API、GitHub API、Hacker News API、直接HTTP取得を利用した。上記リンクは実HTTP/APIで確認したものに限定した。直近14日内の強い候補が少なかったため、古いが思想的・実装的に重要な項目を明記して採用した。

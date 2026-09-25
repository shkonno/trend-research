# Anthropology of Agentic AI トレンド調査 (2026-09-25)

- 調査日: 2026-09-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Agentic AIの論点は「性能」から、誰が見張り、誰が安心し、どの言葉で責任を語り、職場の儀礼や身体感覚をどう作り替えるかへ移っている。

## トップ5

### 1. Two's a Crowd: Human and AI-Based Copresence for Developers with ADHD

- 出典: arXiv
- 日付: 2026-09-18
- リンク: http://arxiv.org/abs/2609.21254v2
- 要約: ADHDのあるソフトウェア開発者14名への半構造化インタビューを通じて、人間同士の「body doubling」やペア作業と、AIベースの共在がどのように違う支援を生むかを調べている。人間の共在は社会的支援とオンボーディングを与える一方、評判管理・監視感・プライバシー喪失を伴い、AI共在は判断されにくい accountability と集中維持の場として使われる。
- なぜ面白いか:
  - 技術: Agentic coding assistantを単なる自動化ツールではなく、認知負荷・集中・説明責任を調整する「共在インフラ」として評価している。
  - 人文: これは職場の身体性と儀礼の研究として読める。誰かが隣にいる、見られている、でも裁かれたくないという開発現場の微細な感覚を、AIエージェントがどう再配置するかを示している。

### 2. The Disciplinary Language Transfer Problem: How Psychological Vocabulary Produces Governance Failures in AI Agent Deployment

- 出典: arXiv
- 日付: 2026-09-22
- リンク: http://arxiv.org/abs/2609.26562v1
- 要約: AIエージェントのガバナンスで使われる「学習」「記憶」「価値」「信頼」「アイデンティティ」などの語彙が、心理学・組織科学由来の見えない前提を持ち込み、実在しない主体像を統治対象としてしまう問題を論じる。Wittgenstein、Kuhn、Haraway、Star and Griesemerを参照し、37語の翻訳分類を含むDisciplinary Auditを提案している。
- なぜ面白いか:
  - 技術: ガバナンス文書の用語を監査し、エージェントの実装構造に合う操作的概念へ置き換える実務手順を提示している。
  - 人文: 「エージェントをどう呼ぶか」が、組織内で何を責任・人格・信頼とみなすかを作ってしまう。これはAI導入を言語ゲームと境界物の問題として捉える、かなり人類学的な介入である。

### 3. WorkWorlds: An Infrastructure for Evaluating AI Agents on Workplace Tasks

- 出典: arXiv
- 日付: 2026-09-20
- リンク: http://arxiv.org/abs/2609.23806v2
- 要約: 職場タスクのベンチマークでは、タスクに合わせて環境が用意されるため、実際の職場で必要な「情報を探し当てる仕事」が過小評価されると指摘する。WorkWorldsは、先に組織状態・日付・社員の席・アクセス可能情報を固定し、その後にタスクを投入する評価基盤で、タスク別キュレーションが証拠アクセス率と合格率を押し上げることを示した。
- なぜ面白いか:
  - 技術: エージェント評価を、単発タスク処理ではなく、組織内のアクセス権・文脈・情報局在性を含む環境設計問題へ拡張している。
  - 人文: 職場とは単なるタスク集合ではなく、席・権限・履歴・部署ごとのローカル知識でできた文化的世界である。AIエージェントが「仕事ができる」とは、その世界の地図をどう学び歩けるかに近い。

### 4. AI-GRACE: A Use-Case Operationalization Framework for Agentic AI: From Organizational Objectives and Obligations to Deployment Capabilities and Architecture

- 出典: arXiv
- 日付: 2026-09-18
- リンク: http://arxiv.org/abs/2609.21192v1
- 要約: Agentic AI導入において、モデルの信頼性だけでなく、ユースケースが何を達成し、どの義務を満たし、何を観測・制御すべきかを結び付けるAI-GRACEを提案している。Agent Operating EnvelopeやRisk-Aligned Independence Levelsにより、許可行動、エスカレーション条件、自律性の範囲を組織アーキテクチャに落とし込む。
- なぜ面白いか:
  - 技術: 目的・義務・リスク・証拠・実行時制御を、エージェントの能力認定とアーキテクチャ設計へトレース可能に接続している。
  - 人文: 組織にとってAIエージェントは「導入するソフト」ではなく、新しい役割と裁量を持つ準成員である。どこまで任せ、いつ人に戻すかという境界設定は、職場の権威・儀礼・責任分配そのものを再設計する行為になる。

### 5. Unaccountable Delegation, Fading Skills: Mapping the Risks of Workplace AI Agents

- 出典: arXiv（古いが重要: 2026-08-09）
- 日付: 2026-08-09
- リンク: http://arxiv.org/abs/2608.08601v2
- 要約: O*NETの2,078件の職務タスクから8,356件の職場AIエージェントリスクシナリオを生成し、45名の労働者とLLM judgeで妥当性を確認した研究。拡張利用は必ずしも安全ではなく、過信によるスキル低下や監督能力の減衰が労働者側のリスクとして現れること、また多くの重大リスクが人間とエージェントの境界で起きることを示す。
- なぜ面白いか:
  - 技術: エージェント・目標・環境の相互作用から職務別リスク分類を作り、automationとaugmentationの違いを具体的なシナリオに落とし込んでいる。
  - 人文: 「任せる」ことは文化的実践であり、技能の継承や職業的自尊心にも関わる。この論文は、AIによる委任が現場の熟練・見習い・監督という労働文化を静かに変える可能性を可視化している。

## arXiv / 学術

- Two's a Crowd: Human and AI-Based Copresence for Developers with ADHD — 2609.21254v2 — AI共在をGoffmanのcopresence理論と開発者生産性の観点から読む実証研究。
- The Disciplinary Language Transfer Problem — 2609.26562v1 — AIエージェント統治の語彙を、言語ゲーム・境界物・ situated knowledge の問題として監査する提案。
- WorkWorlds — 2609.23806v2 — 職場を「タスク」ではなく組織状態・席・アクセス権から構成する評価基盤。
- AI-GRACE — 2609.21192v1 — Agent Operating Envelopeなどで組織目的と技術実装を結ぶガバナンス枠組み。
- Unaccountable Delegation, Fading Skills — 2608.08601v2 — 職場AIエージェントの委任・過信・技能低下リスクの分類。

## メモ

- Boris Cherny優先の有無: 本トピックはClaude固有ではないため、Boris Cherny優先は適用しなかった。
- 日本語アカウントの扱い: 日本語X検索も実行したが、X検索ツールがクレジット上限で失敗したため、該当投稿は確認できなかった。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、今回はarXiv/APIで確認できた学術ソース中心の選定である。X/Webの未取得はソース制約として扱い、架空の投稿・ブログ・リンクは追加していない。

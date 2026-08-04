# DDD トレンド調査 (2026-08-04)

- 調査日: 2026-08-04
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

DDDは「AIに設計を任せる」方向ではなく、AIエージェントをチームの対話・モデル化・文脈保存に参加させる方向へ、かなり具体的に寄ってきています。

## トップ5

### 1. Explore DDD 2026: Design StormでAIエージェントと水管理ドメインを実装まで持ち込む
- 出典: 公式カンファレンスサイト
- 日付: 2026-09-21〜25開催予定（本調査日 2026-08-04 時点の掲載情報）
- リンク: https://exploreddd.com/
- 要約: Explore DDD 2026は、新企画「The Design Storm」として、水管理という現実のドメインを小さなコホートでモデリングし、AI agentsとともに動くコードへ落とし込む形式を掲げています。参加者の熟練度を「Headwaters」「Watershed」など水系メタファーで分け、モデリングとagentic codingの両方を実践する設計です。
- なぜ面白いか:
  - 技術: DDDのイベント・境界・コード生成を、抽象講義ではなく実ドメインの共同モデリングからAIエージェント実装まで一気通貫で試す場になっています。
  - 人文: 水管理という公共性の高い題材を使うことで、DDDが単なるソフトウェア分割技法ではなく、地域・資源・責任をどう理解し合うかの方法論として見えてきます。AIを「自動化装置」ではなく、共同作業に混ざる新しい参加者として扱っている点も示唆的です。

### 2. EventStorming公式サイトに「AI-powered Domain-Driven Design with Alberto Brandolini」が掲載
- 出典: EventStorming公式サイト
- 日付: 2026-12-01〜04開催予定（本調査日 2026-08-04 時点の掲載情報）
- リンク: https://www.eventstorming.com/
- 要約: EventStorming公式サイトの今後のワークショップ一覧に、Alberto Brandoliniによる「AI-powered Domain-Driven Design」が掲載されています。EventStorming Master ClassやArchitecture for Flowと並び、AI時代のDDDがコミュニティ内で正式な学習テーマになりつつあります。
- なぜ面白いか:
  - 技術: EventStormingの付箋・イベント・コマンド・ポリシーといった対話的表現を、LLMが解釈・補助・整理できる対象として捉え直す流れを示しています。
  - 人文: EventStormingは本来、声の大きい人だけでなく現場の知識を可視化するための儀式でもあります。そこにAIが入ると、誰の言葉がモデルに残り、誰の曖昧さが消されるのかという文化的・倫理的問いが前面に出ます。

### 3. GitHub: FastAPI Agent BlueprintがDDDをAIエージェントアプリの標準骨格に組み込む
- 出典: GitHubリポジトリ
- 日付: 2026-08-03更新
- リンク: https://github.com/Mr-DooSun/fastapi-agent-blueprint
- 要約: `fastapi-agent-blueprint`は、FastAPIベースのAI agentアプリ向けバックエンド雛形として、DDD domains、SQLAlchemy/Alembic、Taskiq workers、admin UI、RAG infrastructure、Claude/Codex collaboration harnessをまとめています。AIエージェント開発でも、ドメイン層とインフラ層を分ける設計規律が必要だという実装側からの動きです。
- なぜ面白いか:
  - 技術: RAGやワーカーや管理UIを含むagentic backendでも、境界づけられたドメインと永続化・非同期処理を分離する実装テンプレートが求められていることを示します。
  - 人文: 「AIアプリはプロンプト中心でよい」という空気に対し、チームが長期保守できる制度・役割・言葉を先に作るべきだという文化的カウンターになっています。エージェントが増えるほど、むしろ人間側の共通言語が重要になるという逆説が見えます。

### 4. GitHub: Archally Blueprint Schemaがドメイン設計・ルール・ガバナンスを機械可読な地図にする
- 出典: GitHubリポジトリ / npmパッケージ
- 日付: 2026-08-03更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: `blueprint-schema`は、domain design、business rules、value streams、governance、organizational alignmentをYAMLの単一仕様として扱う「domain-first」なスキーマです。READMEでは、アーキテクチャ知識がWiki・スライド・ホワイトボード写真・部族的記憶に分断される問題を「fragmented truth」と呼び、bounded contextや意思決定を機械可読に保つ方向を示しています。
- なぜ面白いか:
  - 技術: DDDのモデルを、人間の図や会議メモだけでなく、検証可能なID・証拠連鎖・未回答質問を持つ仕様として扱うことで、AIエージェントが参照しやすい設計コンテキストになります。
  - 人文: 「地図作り」という比喩は、組織が自分たちの知らない領域をどう認めるかという態度を含みます。AIが断定的に答えを出す時代に、未知を未知として記録する設計文化はかなり重要です。

### 5. arXiv: “Automating Domain-Driven Design” はLLMをDDDの協働相手にする限界と効用を整理
- 出典: arXiv
- 日付: 2026-03-27（直近14日外だが、DDD×LLMの直接研究として重要）
- リンク: https://arxiv.org/abs/2603.26244
- 要約: “Automating Domain-Driven Design: Experience with a Prompting Framework”は、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの特定、集約設計、技術アーキテクチャへのマッピングという5段階をLLMプロンプトで支援する枠組みを示しています。結論として、初期段階では有用な成果物を作れる一方、後段では小さな誤りが伝播しやすく、完全自動化ではなく専門家の議論を促す「sparring partner」として有効だと位置づけています。
- なぜ面白いか:
  - 技術: DDD活動をLLMプロンプトの連鎖として分解しつつ、文脈誤読や誤差蓄積がアーキテクチャ判断に与えるリスクを実証的に扱っています。
  - 人文: これはAIに設計責任を委譲する話ではなく、人間が何を議論すべきかを浮かび上がらせる鏡としてAIを使う話です。ユビキタス言語とは、結局のところ組織の意味交渉であり、機械が流暢に語るほど人間の合意形成が問われます。

## arXiv / 学術

- Automating Domain-Driven Design: Experience with a Prompting Framework — arXiv:2603.26244（2026-03-27）。DDD×LLMの直接研究として確認。
- Leveraging Generative AI for Enhancing Domain-Driven Software Design — arXiv:2601.20909（2026-01-28）。直近14日外だが、DDDメタモデル生成への生成AI利用として関連。
- 直近約14日（2026-07-21〜2026-08-04）に限定したDDD×AI/LLM/agentの新規arXiv論文は、本調査時点で確認されませんでした。

## メモ

- X検索は英語・日本語で実行しましたが、x_searchが `personal-team-blocked:spending-limit` により利用不能でした。そのため、本日のX由来候補は採用せず、Webは直接HTTP取得・GitHub API・公式サイト確認、学術はarXiv APIで補完しました。
- Web検索ツールもFirecrawl未設定で利用不能だったため、検索エンジン結果の網羅性には制限があります。架空リンクを避けるため、実際に取得できた公式ページ・GitHub・arXivのみを採用しました。
- Boris Cherny優先はClaude系トピック向けの設定であり、DDD単一調査では該当候補なし。
- 日本語アカウント・日本語記事は探索対象に含めましたが、X検索障害とWeb検索ツール未設定のため、トップ5に採用できる直近の確認済み日本語ソースは見つかりませんでした。
- 誇張リスク: カンファレンスやワークショップ項目は開催予定・掲載情報であり、実施後の成果ではありません。GitHub項目は更新日が新しい一方、採用度や品質は別途評価が必要です。

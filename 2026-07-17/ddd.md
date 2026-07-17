# DDD トレンド調査 (2026-07-17)

- 調査日: 2026-07-17
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは「設計を古い儀式として守る」よりも、ユビキタス言語・ADR・DSL・責務境界をAIが読める形で残し、組織知を実行可能なコンテキストに変える方向へ動いています。

## トップ5

### 1. 食べログが「Deal Provider」を構築した理由──「AIがなければ踏み出せなかった」DDDという20年前からの設計思想への挑戦
- 出典: Tabelog Tech Blog / Xでの共有
- 日付: 2026-07-13
- リンク: https://tech-blog.tabelog.com/entry/deal-provider-responsibility-separation-design
- 要約: 食べログの販売管理領域で、契約・請求・オプション判定などのロジックが複数システムへ漏れ出していた問題に対し、「データを渡す」から「判断済みの結果を渡す」中間データ層 Deal Provider を設計した事例です。記事は、Port / Adapter / Usecase / DomainService、ADR、コーディングルールをAIに渡すことで、DDDの継続運用コストを下げられると述べています。
- なぜ面白いか:
  - 技術: DDD、Tell Don't Ask、Hexagonal Architecture、ADRを「AIが守れる実装ルール」として接続し、AI時代の責任分離設計を実運用に落としている点が強いです。
  - 人文: これは単なるアーキテクチャ記事ではなく、組織が成長して「誰が判断を所有するのか」が曖昧になる過程の記録です。AIは魔法の設計者ではなく、組織の記憶と規範を維持する新しい同僚として描かれています。

### 2. DSLs Enable Reliable Use of LLMs
- 出典: Martin Fowler / Thoughtworks 記事
- 日付: 2026-07-14
- リンク: https://martinfowler.com/articles/llm-and-dsls.html
- 要約: Unmesh Joshiが、LLMに曖昧な自然言語だけでコードを書かせるのではなく、ドメイン固有言語（DSL）と強い抽象により出力空間を制約することで、意図どおりの成果物へ導く方法を解説しています。Tickloomのような分散システム挙動のドメインモデル／DSLを例に、DSLがLLM時代の「source of truth」になり得ると論じます。
- なぜ面白いか:
  - 技術: DSLはDDDのユビキタス言語をさらに形式化し、LLMの出力を検証可能なプログラムやセマンティックモデルへ変換する強力なハーネスになります。
  - 人文: 言語が思考を形づくるという古典的な洞察が、AI開発で再浮上しています。人間とAIが同じ「小さな言語」を共有することで、設計は指示ではなく共同制作の場になります。

### 3. Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem
- 出典: arXiv / X論文紹介
- 日付: 2026-07-07
- リンク: https://arxiv.org/abs/2607.06471
- 要約: Ozan Özkan、Önder Babur、Mark van den Brandによるcs.SE論文で、GitHub上のDDD実践を大規模に分析した研究です。11,742候補リポジトリからGPT-4oを用いた三重多数決の意味的検証で2,502件を抽出し、DDD採用の成長、長寿命なプロジェクト傾向、C#やTypeScriptの存在感、ビジネス文脈が明示されないリポジトリが25.3%あることなどを報告しています。
- なぜ面白いか:
  - 技術: DDDを理念ではなくリポジトリ実態から測定し、AIも使った検証パイプラインで「どの言語・構造・文脈でDDDが生き残るか」を可視化しています。
  - 人文: DDDはコードの形だけではなく、ビジネス意図を保存する文化の問題でもあります。25.3%の「文脈欠落」は、未来の開発者やAIエージェントにとって、組織の記憶喪失として読めます。

### 4. Fix verbose AI with a ubiquitous language
- 出典: X投稿・動画共有（Matt Pocock関連の議論）
- 日付: 2026-07-09頃（X検索結果より）
- リンク: https://x.com/mardehaym/status/2075149630879232142
- 要約: Matt PocockのAI時代のソフトウェアエンジニアリングに関する話題で、冗長なAI出力を抑える実践として、DDD由来のユビキタス言語をCONTEXT.mdやGLOSSARY.mdに明示する方法が注目されています。長い説明を短いプロジェクト固有語に圧縮し、AIにもその語彙を厳密に使わせることで、トークン消費、曖昧さ、過剰説明を減らすという実践です。
- なぜ面白いか:
  - 技術: ユビキタス言語をプロンプトの飾りではなく、AIコーディング環境の圧縮辞書・命名規約・設計制約として扱っている点が実用的です。
  - 人文: 言葉を揃えることは、チームの権力関係や学習速度にも影響します。AIが入ることで、これまで暗黙知だった「うちではこれをこう呼ぶ」が、より公平に共有される可能性があります。

### 5. LLM Wiki / 組織知をエージェントが読める責任・ワークフローへ変換する流れ
- 出典: X投稿群（LLM Wiki、agent workflows、責任分担の議論）
- 日付: 2026-07上旬〜中旬（X検索範囲内）
- リンク: https://x.com/arrakis_ai/status/2074304050880012736
- 要約: 組織内の責任、ワークフロー、運用文脈、ドメイン知識をMarkdownベースのLLM Wikiとして整理し、そこから専門エージェントへ仕事を分解・引き継ぐ構想が共有されています。これはDDDのBounded Context、責任境界、ユビキタス言語を、コードベースだけでなく組織運営そのものに拡張する動きとして読めます。
- なぜ面白いか:
  - 技術: LLM WikiはRAGや単発プロンプトよりも、責任定義・承認条件・業務フローを安定して参照させるエージェント用コンテキスト基盤になります。
  - 人文: ここで問われているのは「AIに何をさせるか」だけでなく、「組織の仕事をどんな言葉と境界で記録するか」です。人間は実行者から監督者へ移る一方、誰の知識がWikiに残り、誰の判断が標準になるのかという文化的課題も生まれます。

## arXiv / 学術
- 見つかりました: **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — arXiv:2607.06471, 2026-07-07, https://arxiv.org/abs/2607.06471 。直近14日内で最も重要なDDD関連論文としてトップ5に採用しました。
- 関連するが直近14日外: **Automating Domain-Driven Design: Experience with a Prompting Framework** — arXiv:2603.26244, 2026-03-27, https://arxiv.org/abs/2603.26244 。ユビキタス言語、イベントストーミング、Bounded Context、集約設計をLLMプロンプトで支援する研究で、今回のトピックに強く関連しますが、古いためトップ5からは外しました。

## メモ
- Boris Cherny優先の有無: DDD単独トピックのため、Claude/Boris Cherny優先条件は該当度が低く、今回は採用していません。
- 日本語アカウントの扱い: 日本語X検索を行い、食べログTech Blogの拡散と日本語圏のAI×DDD議論を確認しました。一次情報としてはTabelog Tech Blog記事を優先しました。
- 注意点・誇張リスク: Web検索ツール（Firecrawl系）は未設定で失敗したため、Web調査は直接HTTP取得、Martin Fowler RSS、Tabelog Tech Blog本文取得、arXiv API、X検索で補完しました。X検索結果は要約生成を含むため、日付が曖昧な投稿は「頃」「範囲内」と明記し、記事・論文など一次リンクを優先しました。

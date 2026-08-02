# DDD トレンド調査 (2026-08-02)

- 調査日: 2026-08-02
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

DDDは「AIに設計させる」よりも、AI時代に失われがちなドメインの意味・境界・会話をどう保存するかという方向へ寄っている。

## トップ5

### 1. Agentic Domain-Driven Mainframe Modernization
- 出典: GitHub README / Project Rosetta pattern catalog
- 日付: 2026-08-01更新（GitHub検索結果で確認）
- リンク: https://github.com/pmilet/ai-ddd-mainframe-modernization-patterns
- 要約: COBOL/CICS系メインフレーム刷新を「コード変換」ではなく、長年埋もれた業務概念を回復するDDD問題として扱うパターンカタログ。READMEでは、AIエージェントは作業を主導する存在ではなく、ハーネス内で意味の発掘・議論・検証を補助する存在として位置づけられている。
- なぜ面白いか:
  - 技術: レガシー刷新をLLMによる翻訳タスクに縮減せず、ドメイン知識の抽出、境界づけ、パターン化にDDDを使う設計論として具体性がある。
  - 人文: 古いシステムは単なる負債ではなく、退職者・組織史・暗黙知が堆積した文化財でもある。AIエージェントを「発掘者」にする発想は、ソフトウェア考古学と組織記憶の保存に近い。

### 2. faceto: typed fileからイベントストーミングの視覚ボードへ
- 出典: GitHub README / OSSツール
- 日付: 2026-07-27更新（GitHub検索結果で確認）
- リンク: https://github.com/bastien-gallay/faceto
- 要約: 型付きテキストファイルからHTML/SVGのワークショップボードを生成し、LLMと一緒にイベントストーミングを進めるためのツール。最初の対象はイベントストーミングで、今後はコンテキストマップ、Bounded Context Canvas、Core Domain Chartへ広げる方向が示されている。
- なぜ面白いか:
  - 技術: DDDワークショップの成果物を、会議後に消える付箋ではなく、エージェントが再利用できる型付きソースとして扱える。
  - 人文: 「face-to-face」と「facet」の二重の意味を持つ名前が示す通り、AIとの設計対話を、人間同士の場の代替ではなく多面体を削り出す共同作業として再定義している。イベントストーミングの身体性をどうデジタルに移すかという文化的問いもある。

### 3. AI Refinement Method: AIコーディング前の仕様品質をDDDで上げる
- 出典: GitHub README / Method documentation
- 日付: 2026-06-24更新（古いが関連性が高いため採用）
- リンク: https://github.com/nlawstudio/ai-refinement-method
- 要約: 「vibe coding」ではなく「vibe spec'ing」として、イベントストーミング、DDD、リファインメントを使い、AIコーディングエージェントに渡す前の仕様・受け入れ条件・失敗テストを整える手法。READMEは、コード生成が安くなった時代には仕様品質が新しいボトルネックになると明言している。
- なぜ面白いか:
  - 技術: エージェントをいきなり実装に走らせず、ドメインモデル、意思決定、脅威、受け入れ条件を先に固定するレイヤーを設けている。
  - 人文: AI時代の開発文化では「速く作る」誘惑が強いが、この手法は遅く考える場を再導入する。ファシリテーターの熟練を一部民主化しつつ、責任ある判断を人間の側に残す点が重要。

### 4. Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem
- 出典: arXiv 論文
- 日付: 2026-07-07公開（直近14日より古いが、DDDの実証研究として重要）
- リンク: https://arxiv.org/abs/2607.06471
- 要約: GitHub上のDDD候補11,742リポジトリから、GPT-4oを用いた三重多数決の意味的検証により2,502件を抽出し、OSSにおけるDDD実践を大規模に特徴づけた研究。DDD採用は2017年以降に加速し、C#とTypeScriptが実務上目立つ一方、25.3%のプロジェクトで明示的なビジネス文脈が記録されていないと報告している。
- なぜ面白いか:
  - 技術: LLMを研究対象の一部ではなく、DDDリポジトリ判定の意味的バリデーションに使い、DDD実践の実証データを作っている。
  - 人文: 「ビジネス文脈がコードに残らない」問題は、ユビキタス言語が組織内の口承で終わり、後世に継承されない問題でもある。DDDの成熟は、同時に記録文化・説明責任・設計の記憶術を問う。

### 5. Automating Domain-Driven Design: Experience with a Prompting Framework
- 出典: arXiv 論文
- 日付: 2026-03-27公開（古いが、LLM×DDDの中心的論点として採用）
- リンク: https://arxiv.org/abs/2603.26244
- 要約: LLMとの構造化対話で、ユビキタス言語の確立、イベントストーミングのシミュレーション、境界づけられたコンテキストの特定、集約設計、技術アーキテクチャへの写像を試した経験報告。前半の1〜3段階は有用な成果物を生む一方、後半では小さな誤りが蓄積して実用性を損なうと結論づけている。
- なぜ面白いか:
  - 技術: LLMはDDDを完全自動化する設計者ではなく、グロッサリやコンテキストマップ作成の「sparring partner」として有効だと線引きしている。
  - 人文: DDDの価値は、正解を一発で出すことではなく、専門家同士の対話でトレードオフを露出させることにある。この研究は、AI導入後も判断・責任・合意形成が人間の共同作業であることをよく示している。

## arXiv / 学術

- Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem / arXiv:2607.06471 / 2026-07-07 / GitHub上のDDD実践を大規模に測定し、ビジネス文脈の欠落という設計記録上の課題を示した。
- Domain-Driven Design in Practice: A Mining Study of Maintenance and Evolution in Open-Source Repositories / arXiv:2606.23984 / 2026-06-22 / DDD戦術パターン、Bounded Context違反、保守活動との関係を測ろうとするマイニング研究計画。
- Automating Domain-Driven Design: Experience with a Prompting Framework / arXiv:2603.26244 / 2026-03-27 / LLMでユビキタス言語、イベントストーミング、境界づけを支援できるが、集約・技術設計では誤りが蓄積するという経験報告。

## メモ

- Boris Cherny優先: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールがクレジット/購読制限で失敗したため、今回は取得できなかった。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、代替としてGitHub API、arXiv API、直接HTTP取得を利用した。X上の反応や日本語コミュニティの直近議論は未取得であり、速報性には制約がある。GitHubリポジトリの「更新日」は活動日であり、内容公開日そのものとは限らない。

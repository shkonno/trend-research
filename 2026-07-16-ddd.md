# DDD トレンド調査 (2026-07-16)

- 調査日: 2026-07-16
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIコーディングが「速く作る」を加速するほど、DDDの「何を、どの言葉で、どの境界で作るか」が再び中心課題になっています。

## トップ5

### 1. Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem
- 出典: arXiv / X投稿（@ComputerPapersによる紹介）
- 日付: 2026-07-07（arXiv公開） / 2026-07-10（X紹介）
- リンク: https://arxiv.org/abs/2607.06471
- 要約: 11,742件の候補リポジトリから、GPT-4oを使った三重多数決の意味検証で2,502件のDDD実践リポジトリを抽出し、オープンソースにおけるDDDの実態を大規模に分析した論文です。C#とTypeScriptが実践上目立つこと、CQRS/Event Sourcingが分散・データ集約系で多いこと、25.3%のプロジェクトで明示的な業務文脈が残っていないことが示されています。
- なぜ面白いか:
  - 技術: DDDを「思想」ではなくリポジトリ群の実証データとして扱い、AI時代の設計支援やアーキテクチャ・トレーサビリティ研究の基準点になり得ます。
  - 人文: 25.3%のプロジェクトで業務文脈が消えるという結果は、ソフトウェアが組織記憶をどれだけ失いやすいかを示しています。ユビキタス言語は単なる命名規則ではなく、チームが何を大切にしてきたかを次世代へ渡す文化的メディアでもあります。

### 2. StormPilot: AI coding agents の「速く間違える」問題に Event Storming で対抗する
- 出典: X投稿（@codelevltd） / Webデモ
- 日付: 2026-07-12
- リンク: https://x.com/codelevltd/status/2076359105195790443
- 要約: StormPilotは、AIコーディングエージェントが曖昧な仕様を即座にコード化してしまう問題に対し、関係者が「何を作るか」に合意してから実装へ進むための構造化Event Stormingエディタとして紹介されています。デモURLとして https://stormpilot.codelev.com/explore も示されていました。
- なぜ面白いか:
  - 技術: Event Stormingを、生成AIによる実装前のドメインイベント・コマンド・ポリシー・境界づけの品質ゲートとして位置づけています。
  - 人文: AIが実装速度を上げるほど、合意形成や誤解の可視化という人間的な作業の価値が増します。「作れること」と「作るべきこと」の差を、ワークショップ文化が埋める構図が鮮明です。

### 3. DDD except for words instead of code: エージェント向け語彙管理としてのDDD
- 出典: X投稿（@mind_worm_）
- 日付: 2026-07-14
- リンク: https://x.com/mind_worm_/status/2077092792359121158
- 要約: 「コードではなく言葉のためのDDD」として、ドメインプリミティブをWikiやデータストアに置き、会話意図に応じてエージェントが必要な情報を切り出せるようにする発想が共有されていました。プロンプトに概念を散らすのではなく、語彙・概念・責務を管理対象にする点が特徴です。
- なぜ面白いか:
  - 技術: ユビキタス言語を、LLMに渡すコンテキストの検索・分割・再利用のためのデータモデルとして扱う方向性です。
  - 人文: 人間のチームが共有語彙を作ってきた営みが、今度は人間とエージェントの共同作業の基盤になります。言葉を整えることは、権限や責任や解釈の余地を整えることでもあります。

### 4. Bounded Context がAIエージェントの信頼性を上げるという実践論
- 出典: X投稿群（@mardehaym / @akshit_io など）
- 日付: 2026-07-09
- リンク: https://x.com/mardehaym/status/2075149630879232142
- 要約: DDDのユビキタス言語やBounded Contextを、LLM/エージェントのコンテキスト設計に応用する議論が目立ちました。リポジトリや業務情報を無制限に投入するのではなく、目的、許可・禁止範囲、停止条件、証跡、出力契約を含む「境界づけられたコンテキスト・パケット」を渡す考え方です。
- なぜ面白いか:
  - 技術: Bounded Contextが、コンテキストウィンドウ節約だけでなく、権限分離・監査可能性・誤動作検知の設計単位として再解釈されています。
  - 人文: 境界を引くことは、単に情報を減らすことではなく、誰が何を知り、何に責任を持つかを明確にする社会的行為です。AIエージェントの時代にも、組織の信頼は「見通せる範囲」を作ることから始まります。

### 5. From Stories to Code: Collaborative Modeling and LLMs（古いが関連性高）
- 出典: Web記事（codecentric）
- 日付: 2026-06-02（直近14日より古いが、今回テーマとの関連性が高いため採用）
- リンク: https://www.codecentric.de/en/knowledge-hub/blog/from-stories-to-code-how-domain-storytelling-and-eventstorming-give-llms-the-context-they-need
- 要約: Domain StorytellingとEventStormingが、LLMに必要なドメイン文脈を与え、AI支援プロトタイピングを改善するという記事です。協調的モデリングを、LLMに「正しい文脈」を渡す前処理として捉えています。
- なぜ面白いか:
  - 技術: ストーリー、イベント、業務フローを構造化してからLLMに渡すことで、コード生成の入力品質を上げる実践パターンを示しています。
  - 人文: 物語として業務を語り、付箋やイベントで関係者の認識をそろえる作業は、AI導入後も消えません。むしろAIが読むための文脈を、人間が共同で編むという新しい「翻訳」の仕事になります。

## arXiv / 学術
- 見つかりました: Ozan Özkan, Önder Babur, Mark van den Brand, “Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem”, arXiv:2607.06471, 2026-07-07。リンク: https://arxiv.org/abs/2607.06471
- 関連するが直近14日外: “Domain-Driven Design in Practice: A Mining Study of Maintenance and Evolution in Open-Source Repositories”, arXiv:2606.23984, 2026-06-22。リンク: https://arxiv.org/abs/2606.23984
- 関連するが古い: “Automating Domain-Driven Design: Experience with a Prompting Framework”, arXiv:2603.26244, 2026-03-27。リンク: https://arxiv.org/abs/2603.26244

## メモ
- Boris Cherny優先の有無: 本トピックはClaude固有ではないため、Boris Cherny優先は適用しませんでした。
- 日本語アカウントの扱い: 日本語キーワード（ドメイン駆動設計、イベントストーミング、ユビキタス言語、エージェント）でもX検索しましたが、直近14日で深いDDD×AI議論は少なく、ノイズが多めでした。
- Web検索: Firecrawl系のweb_searchツールは未設定で失敗したため、端末からBrave Searchと対象ページ取得を行い、codecentric、INNOQ、Java Code Geeks、DZone、DDD Academyなどを確認しました。
- 注意点・誇張リスク: X上では「DDD」という明示語よりも、bounded context、context engineering、loop engineering、agent contracts といった周辺語で議論される傾向があります。そのため、DDDそのものの流行というより「DDD的な設計語彙がAIエージェント設計へ再流入している」と見るのが安全です。

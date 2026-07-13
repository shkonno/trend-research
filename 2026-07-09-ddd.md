# DDD トレンド調査 (2026-07-09)

- **トピック**: DDD / Domain-Driven Design / ドメイン駆動設計
- **調査日**: 2026-07-09
- **調査状況**: X検索はクレジット上限で失敗、HermesのWeb検索はFirecrawl未設定で失敗したため、端末から Google News RSS / Bing News RSS / HN Algolia / 直接URL取得 / arXiv API を確認して再生成。
- **焦点**: practical usage, real-world workflows, ethical implications, philosophical background, cultural impact

## 厳選トップ5アイテム

### 1. 10年ものの請求・受注基盤をDDDで壊す日本語実践記
- **出典**: note（Tsubasa Tsuchiya）/ Bing News RSSで確認
- **日付**: 2026-06-24
- **リンク**: https://note.com/tsuchi_13/n/n50c4232e1161
- **要約**: 10年増改築された請求・受注基盤を「大きな泥団子」と捉え、商品プラン改訂と並行して8カ月・50回以上のドメインモデル整理を行った実践記。ビジネスロジックが複雑な場合、いきなりコードではなくモデルを時間をかけて整える重要性を示している。
- **なぜ面白いか**: **技術的**: レガシー刷新をビッグバン移行ではなく、ドメインモデルの反復整理として進める具体的ワークフローが実務的。**人文的**: DDDは単なる設計パターンではなく、組織の記憶や責任を言葉に戻す文化的営みである。請求や受注のような制度的領域では、コードの整理がそのまま顧客との約束・倫理・歴史の再記述になる。

### 2. Architecture for Compliance: 高負荷グローバルシステムをDDDとマイクロサービスで設計
- **出典**: HackerNoon / Google News RSSで確認、直接URLのdescription取得
- **日付**: 2026-04-12（直近14日より古いが、DDD実務例として関連）
- **リンク**: https://hackernoon.com/architecture-for-compliance-scaling-microservices-with-ddd-for-high-volume-global-enterprise-systems
- **要約**: 税務・コンプライアンス領域の高ボリュームなグローバル企業システムを、DDDとマイクロサービスでスケールさせる技術ケーススタディ。コンプライアンスの複雑なルールを境界づけられた文脈に分け、変化に耐える構造へ落とす方向性が示されている。
- **なぜ面白いか**: **技術的**: DDDの bounded context が、規制・地域差・監査要件を含む複雑な業務領域でマイクロサービス境界を決める実用的な軸になる。**人文的**: コンプライアンスは社会が企業に課す倫理と法の言語であり、それをソフトウェア境界へ翻訳する行為は制度設計に近い。DDDは文化差や法制度の違いを「ドメインの声」として扱うための方法論になる。

### 3. Domain-Driven Design: Lean Aggregates
- **出典**: Denis Kyashif's Blog / HN Algoliaで確認
- **日付**: 2026-04-04（古いが2026年のDDD設計論として関連）
- **リンク**: https://deniskyashif.com/2026/04/04/domain-driven-design-lean-aggregates/
- **要約**: DDDにおけるAggregateを小さく保つ「Lean Aggregates」の設計論。集約が過大になるとトランザクション境界・変更容易性・理解容易性が悪化するため、ドメイン不変条件を守りつつ責務を絞る重要性を扱う。
- **なぜ面白いか**: **技術的**: 生成AI時代でも、AIに任せる前のモデル境界と不変条件の設計が品質を左右する。**人文的**: 集約を小さくすることは、世界を理解可能な単位へ切り分ける認識論でもある。人間の共同作業では、過大な概念は権限や責任を曖昧にし、文化的な衝突を隠してしまう。

### 4. From Coding to Orchestration: Agentic Software Engineering とシステム思考
- **出典**: Medium記事 / Google News RSSで確認
- **日付**: 2026-07-04
- **リンク**: https://news.google.com/rss/articles/CBMizgFBVV95cUxOM281ZURSTHhrZzlVVjNRdDY1RkdLLWtlM0llQ1dLMllqQ3BRN1pfMXI5ZXNxV1FDZTY?oc=5
- **要約**: 「コーディングからオーケストレーションへ」というAI時代のソフトウェア工学を、システム思考として捉える記事。RSS上でDomain-Driven Design検索にヒットしており、AIエージェントが実装を担う時代に、境界・責務・モデル化の重要性が再浮上している文脈として読める。
- **なぜ面白いか**: **技術的**: AIがコードを書くほど、人間側はユビキタス言語、境界、受け入れ条件、検証ループを設計する役割へ移る。**人文的**: これは「作者としてのプログラマ」から「共同体の意味を編成する設計者」への哲学的転換である。DDDは、AIに委任する前に人間社会の言葉を整える文化的基盤として再評価される。

### 5. Software Architecture Gathering 2026 のプログラム公開とアーキテクチャ共同体の継続
- **出典**: PRWeb / Google News RSSで確認
- **日付**: 2026-07-09
- **リンク**: https://news.google.com/rss/articles/CBMi7wFBVV95cUxPcTBGLS0wRHFDRERZUUdXQ1BZVGh2bVVzV18zYzk0bFplZEdKX0UyTjAtOXNuZlJ6YmlFNEd3b3ktY1lMdS1RLTR2c3VIbU1yZ?oc=5
- **要約**: iSAQB Software Architecture Gathering 2026 の国際カンファレンスプログラム公開が報じられた。DDDそのものの記事ではないが、Domain-Driven Design検索で検出され、ソフトウェアアーキテクチャ共同体がAI時代にも設計・境界・組織学習を中心課題として扱い続けていることを示す。
- **なぜ面白いか**: **技術的**: DDDは単独の実装技法ではなく、アーキテクチャ教育・認定・コミュニティ実践の中で更新される知識体系である。**人文的**: カンファレンスは単なる発表の場ではなく、専門職が自分たちの価値観・倫理・歴史を再交渉する儀礼でもある。AIエージェントが実装速度を上げるほど、人間同士が何を良い設計と呼ぶかを共有する文化的場の価値が増す。

## arXiv / 学術
- arXiv APIで `Domain-Driven Design`、`domain driven design software architecture`、`bounded context domain-driven design` を確認したが、今回の調査範囲ではDDDを直接扱う新規論文は本調査時点で確認されませんでした。
- 関連領域として、AIエージェント、権限委譲、仕様、ループ設計の論文は他トピックで多く確認されており、DDDはそれらを業務語彙・境界・不変条件へ接続する設計思想として重要性を増している。

## メモ
- X検索は `personal-team-blocked:spending-limit` で失敗したため、X投稿は本文の根拠として採用していない。
- Web検索ツールは未設定だったため、RSSと直接URL取得で確認できた範囲に限定した。
- 直近14日だけではDDD単独の強い新規ニュースが少なかったため、2026年春の実務記事も「古いが関連」と明記して採用した。

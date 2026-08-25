# DDD トレンド調査 (2026-08-25)

- 調査日: 2026-08-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

DDDは「設計パターン集」から、LLM時代に人間・AI・組織が同じドメイン言語を合意するための協働インターフェースへ寄っている。

## トップ5

### 1. EventStormer: 会話で育つAIファシリテータ付きEventStormingモデル

- 出典: GitHubリポジトリ
- 日付: 2026-08-24作成・更新
- リンク: https://github.com/vinialbano/eventstormer
- 要約: ドメイン専門家が自然言語で業務を説明し、AIファシリテータがEventStorming要素を提案、専門家が承認・編集・却下するという設計の新規リポジトリ。READMEでは、完成品ではなく「scaffold」と明記しつつ、EventStormingの成果物を単なる図ではなく安定ID付きの型付きグラフにする構想が示されている。
- なぜ面白いか:
  - 技術: EventStormingをLLMの会話UI、型付きモデル、アーキテクチャゲートに接続し、後続の設計・実装成果物を同じモデルから導出する方向性が見える。
  - 人文: ワークショップの主役をAIではなくドメイン専門家の承認行為に置いている点が重要で、組織知を「自動生成」ではなく「合意形成」として扱っている。DDDの儀式性が、AI時代の参加型モデリングへ更新されつつある。

### 2. Turn a Codebase into a Domain Model Your PM and QA Can Read

- 出典: DEV Community記事
- 日付: 2026-08-18
- リンク: https://dev.to/mroops/turn-a-codebase-into-a-domain-model-your-pm-and-qa-can-read-16d
- 要約: BraidというOSSフレームワークを紹介し、コードベースからPMやQAも読めるドメインモデルをAIが下書きする流れを説明している。デフォルトのオントロジーとしてDDDを使い、bounded context、aggregate、command、ruleなどをユビキタス言語で表し、AIの変更は人間が承認する前提になっている。
- なぜ面白いか:
  - 技術: コード、PRD、設計メモのズレを、AI生成の提案と人間の承認ループで同期する「レビュー可能なドメインモデル」に落としている。
  - 人文: PM・QA・エンジニアが同じモデルを読むという問題設定は、DDDのユビキタス言語を単なる命名規則ではなく、職能間の翻訳装置として捉え直している。AIが議事録係ではなく、誤解を可視化する媒介になる点が面白い。

### 3. LLM_Ontology_DDD: ユビキタス言語と意味衝突をLLM×オントロジーで扱う試み

- 出典: GitHubリポジトリ
- 日付: 2026-08-12作成・更新
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: “A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts in Domain-Driven Design” と説明されるリポジトリ。READMEは短いが、LLMだけに語彙抽出を任せず、オントロジーで意味衝突を扱う方向を明示している。
- なぜ面白いか:
  - 技術: LLMの自然言語処理能力とオントロジーの形式的制約を組み合わせ、ユビキタス言語の曖昧さ・同音異義・部署間語彙差を検出する設計課題に踏み込んでいる。
  - 人文: DDDで難しいのは「正しい単語表」ではなく、同じ言葉が組織の場所によって別の現実を指すことだ。このリポジトリは、文化的・組織的な意味の衝突をAI支援で扱える研究対象として前景化している。

### 4. Go's Built-in Features vs. Architectural Patterns: Balancing Simplicity and Complexity in Project Organization

- 出典: DEV Community記事
- 日付: 2026-08-11
- リンク: https://dev.to/viklogix/gos-built-in-features-vs-architectural-patterns-balancing-simplicity-and-complexity-in-project-53op
- 要約: Goのシンプルな言語機能やモジュール機構がDDD的な層をどこまで不要にするかを論じる記事。特に、AIツールが既存コードベースから過去のDDD風パターンを学習し、現代のGoに必ずしも合わない構造を再生産する可能性を指摘している。
- なぜ面白いか:
  - 技術: DDDのレイヤーやDTOを、言語機能・静的依存注入・モジュール境界で置き換えられるのかという、LLM生成コード時代に実務的な論点を提示している。
  - 人文: AIが「過去の平均的な設計文化」を増幅するという見方は、設計判断を技術合理性だけでなく歴史的慣性として読む視点を与える。DDDを採用するか否かは、コードの形だけでなく、監査・教育・チーム合意の可視性にも関わる。

### 5. Keep the Context Map. Replace the Aggregates.（直近14日外だが関連性高）

- 出典: DEV Community記事
- 日付: 2026-08-07（直近14日より古いが、戦略DDDと組織設計の論点として採用）
- リンク: https://dev.to/siy/keep-the-context-map-replace-the-aggregates-1fj8
- 要約: DDDを戦略DDD（bounded context、context map、subdomain）と戦術DDD（aggregate、entity、repositoryなど）に分け、前者は残しつつ後者を「変更理由」中心の分解に置き換えられると論じる記事。誰が変更を要求するのか、どの意思決定権限がコードを動かすのかを設計単位にする発想が中心になっている。
- なぜ面白いか:
  - 技術: コンテキストマップを維持しながら内部構造をaggregateではなくchange driverで分割することで、AIエージェントや自動リファクタリングにも渡しやすい設計メタデータになる。
  - 人文: 変更理由を「誰が求めるか」から捉えるため、設計境界が組織の権限・責任・政治性と直結する。DDDの境界づけを、単なるモデル設計ではなく組織文化の読み解きとして扱っている点が今日的。

## arXiv / 学術

- 本調査時点で確認されませんでした。
- 補足: arXiv APIに対して `Domain-Driven Design`、`event storming`、`ubiquitous language` と `LLM/agent/AI` の組み合わせで検索を試みましたが、API側からHTTP 429が返りました。架空IDを避けるため、未確認の論文・arXiv IDは掲載していません。

## メモ

- Boris Cherny優先の有無: Claude固有トピックではないため、Boris Cherny優先は適用しませんでした。
- 日本語アカウントの扱い: 日本語X検索も実行しましたが、X検索ツールはクレジット上限エラーで利用できませんでした。
- 注意点・誇張リスク: Web検索ツールも未設定エラーだったため、DEV Community API、GitHub API、Hacker News Algolia API、arXiv APIへの直接アクセスで補完しました。EventStormerはREADME上でscaffoldと明記されており、実装済み機能として過大評価しない必要があります。
- ソース制約: X検索は `personal-team-blocked:spending-limit`、Web検索・Web抽出はFirecrawl未設定、arXivはHTTP 429でした。確認できたリンクのみを掲載しています。

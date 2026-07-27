# DDD トレンド調査 (2026-07-27)

- 調査日: 2026-07-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AI/LLM時代のDDDは「コード生成の前工程」から「組織の知識を機械可読に保つ設計文化」へ重心が移りつつあります。

## トップ5

### 1. Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem
- 出典: arXiv
- 日付: 2026-07-07（直近14日より少し前だが、DDD調査として重要）
- リンク: http://arxiv.org/abs/2607.06471v1
- 要約: GitHub上のDDD関連リポジトリを大規模に調べ、候補11,742件からGPT-4oの多数決検証で2,502件をDDD実践例として抽出した研究です。DDD採用の推移や実践の持続性を、理論ではなく実データから捉えようとしている点が目立ちます。
- なぜ面白いか:
  - 技術: DDDの「採用されている／されていない」をREADMEやトピックだけでなくLLM支援の意味検証で絞り込むため、設計パターン研究にもAIを使う流れが見えます。
  - 人文: DDDはしばしば信念や流派として語られますが、この研究は共同体の実践を民俗誌のように観察対象へ変えています。設計文化がどのように定着し、どこで消えるのかを問う入口になります。

### 2. faceto: typed fileからLLMと考えるEvent Stormingボードを生成するツール
- 出典: GitHub / プロジェクトREADME
- 日付: 2026-07-26更新
- リンク: https://github.com/bastien-gallay/faceto
- 要約: typed fileを入力に、Event StormingのHTML/SVGボードを生成し、要素をクリックしてメモを残し、次のLLMセッションでモデルを調整するためのRust製ツールです。READMEではEvent Stormingを最初の形式とし、将来的にcontext map、bounded context canvas、core domain chartへ広げる方向を示しています。
- なぜ面白いか:
  - 技術: Event Stormingをホワイトボード写真ではなく、LLMが読み書きできる構造化ファイルと可視ボードの往復として扱っています。
  - 人文: ワークショップは本来、場の空気や沈黙も含む共同作業ですが、このツールはその痕跡を次回の対話へ持ち越そうとします。DDDの「対話の設計」が、人間同士だけでなく人間とモデルのあいだにも拡張されている点が興味深いです。

### 3. The Method / ai-refinement-method: AI coding agentsの前にDDD・Event Storming・脅威モデリングで仕様を固める
- 出典: GitHub / プロジェクトREADME
- 日付: 2026-06-24更新（古いが、AI/DDD接続として重要）
- リンク: https://github.com/nlawstudio/ai-refinement-method
- 要約: 平文の要求を、ドメインマッピング、意思決定、脅威、受け入れ条件、失敗するテストを含む「build-ready stories」に変換するエージェント的リファインメント手法です。READMEは「vibe codingではなくvibe spec'ing」と表現し、実装はClaude Code / Cursor / Codexなどのコーディングツールに渡す前段で止める設計を強調しています。
- なぜ面白いか:
  - 技術: DDD、Event Storming、仕様リファインメントを、AI coding agentへの入力品質を上げる上流工程として再配置しています。
  - 人文: 「コードが安くなった時代に、仕様品質が新しいボトルネックになる」という主張は、ソフトウェア開発の価値の所在が実装者から問いを立てる人へ移ることを示します。組織内で誰がドメインを語る権利を持つのか、という文化的な問いにもつながります。

### 4. Archally Blueprint Schema: DDD・ADR・ルール・Event Stormingを1つのYAMLモデルに統合する試み
- 出典: GitHub / プロジェクトREADME
- 日付: 2026-07-26更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: bounded context、business rules、governance、architecture、decision recordsなどを、1つの機械可読なYAMLモデルで表すスキーマです。READMEでは、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Stormingボードの生成や、MCPを介したAI agentのグラウンディングまで射程に入れています。
- なぜ面白いか:
  - 技術: DDDの成果物をドキュメント群ではなく、生成・検証・AI参照が可能な単一モデルとして扱う「system cartography」的アプローチです。
  - 人文: 散らばったWikiやホワイトボード写真を「fragmented truth」と呼ぶ発想が象徴的です。これは単なる文書化ではなく、組織が何を真実として共有するかを地図化する文化技法に近いです。

### 5. axi-go: AI agent toolsのためのDDD的な実行カーネル
- 出典: GitHub / プロジェクトREADME
- 日付: 2026-07-26更新
- リンク: https://github.com/klarlabs-studio/axi-go
- 要約: AIエージェントに渡すツールを、Actions（何をしたいか）とCapabilities（どう実行するか）の2層に分け、型付き契約、効果レベル、承認ゲート、実行予算、監査証跡を提供するGoライブラリです。READMEは「domain-driven execution kernel for AI agent tools」と位置づけ、MCPなどのプロトコルは配送関心として外側に置く設計を示しています。
- なぜ面白いか:
  - 技術: エージェントのツール呼び出しを生の関数群ではなく、意図・副作用・証跡を持つドメインオブジェクトとして扱っています。
  - 人文: AIエージェントの自律性は「何ができるか」より「誰が止められるか」で信頼されます。承認や監査をドメインモデルに入れることは、組織の責任境界をコードへ埋め込む試みです。

## arXiv / 学術

- `2607.06471v1` Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem（2026-07-07）: DDD実践をGitHub大規模データとLLM支援検証で特徴づける研究。
- `2606.23984v1` Domain-Driven Design in Practice: A Mining Study of Maintenance and Evolution in Open-Source Repositories（2026-06-22、古い）: DDD tactical building blocksの分布・進化・保守性との関係を調べる採掘研究の計画。
- `2605.01159v1` A Domain-Driven Design Simulator for Business Logic-Rich Microservice Systems（2026-05-01、古い）: aggregatesを中心に、SagaやTransactional Causal Consistencyを含むマイクロサービス設計を早期検証するシミュレータ。
- `2603.26244v1` Automating Domain-Driven Design: Experience with a Prompting Framework（2026-03-27、古い）: ユビキタス言語、Event Storming、bounded contexts、aggregates、技術アーキテクチャへの写像をLLMプロンプトで支援する経験報告。

## メモ

- Boris Cherny優先の有無: DDD単独トピックのため該当なし。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールがクレジット制限で失敗したため取得できませんでした。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、代替としてGitHub API、Bing RSS/HTML、arXiv APIへの直接HTTPアクセスを使用しました。Bing検索は検索品質が低くノイズが多かったため、リンク確認可能なGitHub/arXiv中心に選定しています。GitHub項目は更新日が新しくてもスター数が少ない初期プロジェクトを含むため、「流行の確定」ではなく「萌芽」として読むのが安全です。

# DDD トレンド調査 (2026-09-26)

- 調査日: 2026-09-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは、コード生成の自動化よりも「ドメイン境界・制約・言葉」をAIにどう渡すかへ重心が移っています。

## トップ5

### 1. Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems
- 出典: arXiv
- 日付: 2026-09-23
- リンク: http://arxiv.org/abs/2609.27354v1
- 要約: 生成AIシステムが業務領域に入る際、単なるRAGやツール接続ではなく、技術・規制・制度・規範上の制約を「ドメインインターフェース」として構造化する設計手法を提案している。DDDの文脈では、境界づけられたコンテキストやユビキタス言語をAIのコンテキスト設計へ接続する議論として読める。
- なぜ面白いか:
  - 技術: LLMへの文脈投入を知識量の問題ではなく、制約を操作可能な設計単位に落とす問題として扱っている。
  - 人文: AIの「正しさ」はモデル単体ではなく、制度・現場慣習・責任分界との関係で決まるという視点が明確です。DDDが元々持っていた対話的な境界づけの価値が、AIガバナンスの言葉に翻訳されつつあります。

### 2. DDD Coach
- 出典: GitHub リポジトリ
- 日付: 2026-09-25作成 / 2026-09-26更新
- リンク: https://github.com/SDiamante13/ddd-coach
- 要約: Domain-Driven Designを教え、実際のDDD問題を一緒に解くAIコーチの初期実装。貨物予約ドメインを題材に、ギャップや例外を問い返す会話、将来的な生成モデリングボードや音声インターフェースを計画している。
- なぜ面白いか:
  - 技術: LLMを「DDD成果物を一気に作る自動化装置」ではなく、質問でドメイン理解を深めるコーチとして位置づけている。
  - 人文: DDDの本質である共同学習と対話をAIがどう支援できるかを示す小さな実験です。専門家の判断を置き換えるのではなく、チームが見落としている例外や言葉のズレを表面化する役割に価値があります。

### 3. ProcessFlow Architect
- 出典: GitHub リポジトリ
- 日付: 2026-08-21作成 / 2026-09-24更新
- リンク: https://github.com/raalzate/processflow-architect
- 要約: Event Storming、DDD、BPMN、C4、UMLを扱うローカルファーストのデスクトップ設計ツール。LiteRT-LM/WebGPUによるローカルReActエージェントを備え、ドメインとのチャットからリスク、ADR、ロードマップ、図などの成果物を生成する方向を掲げている。
- なぜ面白いか:
  - 技術: イベントストーミングのキャンバスとローカルAIエージェントを結び、設計データをクラウドへ送らずに反復できる点が特徴的です。
  - 人文: DDDワークショップは信頼・心理的安全性・業務機密に強く依存します。オフラインで動くAI支援は、現場の語りを外部サービスへ預ける不安を減らし、設計の場をより扱いやすくします。

### 4. Archally Blueprint Schema
- 出典: GitHub リポジトリ
- 日付: 2026-08-25作成 / 2026-09-25更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: ドメイン設計、ビジネスルール、バリューストリーム、ガバナンス、組織アラインメントを単一の機械可読YAMLで表すスキーマ。OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Stormingボード生成や、MCP経由でAIエージェントをグラウンディングする用途をうたっている。
- なぜ面白いか:
  - 技術: DDDのモデルを文書ではなく検証可能な「システム地図」として扱い、AIエージェントの参照基盤にしようとしている。
  - 人文: 組織の暗黙知を地図化する比喩が強く、何が分かっていないかもモデルに残す姿勢がよいです。AI時代の設計では、答えを速く出すこと以上に、不確実性を共有できる表現が重要になります。

### 5. FazenDados
- 出典: GitHub リポジトリ
- 日付: 2026-08-04作成 / 2026-09-15更新
- リンク: https://github.com/otaviovasc/fazendados
- 要約: 家族経営の酪農現場向けに、AIアシスタントを主要なデータ入力面として設計した業務システム。テキスト・音声・画像・文書を受け付ける一方、AIが出した提案は人間が確認するまで事実として保存しないというルールを明示し、ユビキタス言語をコード・UI・ドキュメントに適用している。
- なぜ面白いか:
  - 技術: AI入力を「提案→レビュー→確認」というドメイン上の状態遷移に閉じ込め、監査性とドメイン語彙を中心に据えている。
  - 人文: 紙と記憶に依存する小規模現場で、AIが記録の入口になるリアリティがあります。同時に、人間の確認を必須にする設計は、AIが生活世界の事実を勝手に確定してしまう危険への慎重な応答です。

## arXiv / 学術
- 2026-09-23: Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems — http://arxiv.org/abs/2609.27354v1
- 関連するが直近14日外: 2026-08-15「Towards Standardized Evaluation in Automated Domain Modeling」、2026-08-06「Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design」、2026-03-27「Automating Domain-Driven Design: Experience with a Prompting Framework」、2026-01-28「Leveraging Generative AI for Enhancing Domain-Driven Software Design」。

## メモ
- X検索は英語・日本語で実行したが、xAI側のクレジット/サブスクリプション制限により取得できませんでした。そのため本日のトップ5は、arXiv APIとGitHub API/README取得によるWeb代替調査を中心に選定しています。
- Web検索ツールもFirecrawl未設定のため利用不能でした。代替として、arXiv公式API、GitHub Search API、GitHub README取得、Hacker News/Stack Exchange/Reddit API確認を実施しました。
- Boris Cherny優先はClaude系トピック向け設定のため、本DDD調査では該当なしです。
- 日本語アカウント/投稿はX制限により確認できませんでした。
- 注意点: GitHubリポジトリはスター数が少ない初期プロジェクトを含みます。流行度よりも、DDDとAI/LLM/agent時代の設計・イベントストーミング・ユビキタス言語・組織文化への接続の面白さを優先して選んでいます。

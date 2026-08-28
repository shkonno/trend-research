# DDD トレンド調査 (2026-08-28)

- 調査日: 2026-08-28
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AI/LLM時代のDDDは「モデルを作る」から「モデル・コード・会話・組織のズレを継続的に検出し、直す」方向へ関心が移っている。

## トップ5

### 1. Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark

- 出典: arXiv
- 日付: 2026-08-15
- リンク: http://arxiv.org/abs/2608.15255v1
- 要約: 自然言語記述からドメインモデルを生成する自動ドメインモデリング手法を比較するため、既存のGolden UML Modelsetなどを組み合わせたベンチマークを提案している。LLM駆動手法とルールベース手法を、参照モデルとの一致度で評価する土台を整えようとする研究。
- なぜ面白いか:
  - 技術: DDD×LLMで曖昧だった「良いドメインモデル」を、再現可能な評価タスクとメトリクスに落とそうとしている点が重要。
  - 人文: ユビキタス言語やモデルの品質は本来、チーム内の合意や物語に依存するため、ベンチマーク化は便利である一方で「測れるものだけが正しい」文化を生みやすい。AIが設計議論を支援する時代ほど、人間が何を評価対象から外したのかを意識する必要がある。

### 2. Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design

- 出典: arXiv
- 日付: 2026-08-06（直近14日より少し前だが、AI支援DDD文脈で重要）
- リンク: http://arxiv.org/abs/2608.05612v1
- 要約: Tactical DDDのモデルとJavaコードを双方向に同期するJDomInOを提案している。共有メタモデルを使い、ドメインモデルからJava構造を生成し、既存コードからドメインモデルを復元することで、設計と実装のドリフトを減らす狙い。
- なぜ面白いか:
  - 技術: AIコードアシスタントに対して、ソースコードだけでなく集約境界やDDDセマンティクスを含む「精密なコンテキスト層」を渡す構想が明確に述べられている。
  - 人文: DDDの難所は図やコードの生成ではなく、チームが何を同じ言葉で理解しているかを維持することにある。ラウンドトリップは、設計会話の記憶を組織の中に残すための制度設計としても読める。

### 3. DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python

- 出典: GitHub / IEEE Xplore掲載リポジトリ
- 日付: 2026-08-13更新（直近14日よりわずかに前）
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: 要求仕様書（PDF/DOCX/TXT）から型付きドメインモデルを作り、PythonコードのアーキテクチャドリフトをVS Code診断として検出するツール。README上では、AST解析とマルチエージェントLLM推論により、検出結果を元の要求にトレースする設計が説明されている。
- なぜ面白いか:
  - 技術: LLMを「コードを書く存在」ではなく、SRS・ドメインモデル・AST・IDE診断をつなぐ設計遵守エンジンとして使っている。
  - 人文: DDDのユビキタス言語は、会議室のホワイトボードから離れるとすぐに弱くなる。要求とコードの距離をIDE内で可視化する発想は、設計原則を個人の記憶ではなく日々の作業環境に埋め込む試みとして面白い。

### 4. LLM_Ontology_DDD: Hybrid LLM–Ontology Approach for Ubiquitous Language

- 出典: GitHub
- 日付: 2026-08-12作成・更新（直近14日より少し前）
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: 「DDDにおけるユビキタス言語の構築と意味衝突の解決」に、LLMとオントロジーを組み合わせるアプローチを掲げたリポジトリ。公開情報は短いが、ユビキタス言語を単なる用語集ではなく、矛盾検出・意味調停の対象として扱う方向性が見える。
- なぜ面白いか:
  - 技術: LLMの柔軟な言語理解と、オントロジーの明示的な概念関係を組み合わせることで、用語の揺れや部門間の意味衝突を機械的に扱える可能性がある。
  - 人文: ユビキタス言語は、実は権限・専門性・部門文化の折衝そのものでもある。AIが「この言葉は矛盾しています」と指摘するとき、それは技術的な修正だけでなく、誰の言葉が組織の標準語になるのかという文化的問題を浮かび上がらせる。

### 5. ai-refinement-method: event storming / DDD をAIコーディング前の仕様化レイヤーに置く試み

- 出典: GitHub / プロジェクトサイト
- 日付: 2026-06-24更新（古いが、イベントストーミングとAIエージェント接続の観点で関連）
- リンク: https://github.com/nlawstudio/ai-refinement-method
- 要約: 「vibe codingではなくvibe spec'ing」として、AIコーディングエージェントの前段に、イベントストーミング、DDD、リファインメント、脅威モデリングを含む仕様化プロセスを置くプロジェクト。Claude Code / Cursor / Codexなどへの引き渡しを前提に、実装前のドメイン理解と受け入れ条件の整備を重視している。
- なぜ面白いか:
  - 技術: AIエージェントに直接実装させるのではなく、イベントストーミングを含む仕様生成を独立した上流工程として扱っている。
  - 人文: 「コードが安くなり、仕様品質がボトルネックになる」という問題意識は、DDDの復権を示している。AI時代の設計文化では、速く作る能力よりも、何を作るべきかを共同で語れる能力が差別化要因になる。

## arXiv / 学術

- Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark — arXiv:2608.15255v1 — 2026-08-15。自動ドメインモデリングの標準評価に向けたベンチマーク提案。
- Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design — arXiv:2608.05612v1 — 2026-08-06。Tactical DDDのモデルとJavaコードの双方向同期、およびAIコード支援への応用可能性。
- Automating Domain-Driven Design: Experience with a Prompting Framework — arXiv:2603.26244v1 — 2026-03-27（古いが関連）。ユビキタス言語、イベントストーミング、境界づけられたコンテキスト、集約、技術アーキテクチャへのLLMプロンプトフレームワークを検証。
- Leveraging Generative AI for Enhancing Domain-Driven Software Design — arXiv:2601.20909v1 — 2026-01-28（古いが関連）。DDDメタモデル生成への生成AI活用を扱う。

## メモ

- Boris Cherny優先: Claude系トピックではないため該当なし。
- 日本語アカウントの扱い: 日本語X検索も実行したが、X検索ツールはクレジット/サブスクリプション制限で失敗したため、今回のトップ5にはX投稿を採用していない。
- Web検索の注意: Firecrawl系Web検索/抽出ツールも未設定エラーだったため、代替としてarXiv API、GitHub API、直接HTTP取得を使用した。これは情報源制約であり、X/Web上の最新反応を十分に拾えていない可能性がある。
- 誇張リスク: GitHubリポジトリは公開説明・README・更新日時に基づく採用であり、実利用実績やコミュニティ反応は限定的。特にスター数が少ないものは「流行」ではなく「興味深い萌芽」として扱うのが適切。

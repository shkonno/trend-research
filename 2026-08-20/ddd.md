# DDD トレンド調査 (2026-08-20)

- 調査日: 2026-08-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは、コード生成そのものよりも「業務言語・境界・意思決定を機械可読に保つ」方向へ重心が移っています。

## トップ5

### 1. Turn a Codebase into a Domain Model Your PM and QA Can Read
- 出典: DEV Community / Braid紹介記事
- 日付: 2026-08-18
- リンク: https://dev.to/mroops/turn-a-codebase-into-a-domain-model-your-pm-and-qa-can-read-16d
- 要約: Braidは、既存コードベースや関連資料から、PMやQAも読めるDDD寄りのドメインモデルをAIがドラフトし、人間が判断して更新するループを提案している。デフォルトのオントロジーとして bounded context、aggregate、command、rule などを使い、コードの呼び出しグラフではなく業務語彙でモデル化する点が重要です。
- なぜ面白いか:
  - 技術: LLMを「実装者」ではなく、コードとPRD/Notion/Slackに分散した知識をドメインモデルへ同期するモデリング補助として使っている。
  - 人文: PM、QA、エンジニアが別々の言葉で同じプロダクトを語る断絶を、ユビキタス言語で埋めようとする試みです。AIが勝手に決めるのではなく「AIが下書きし、人間が決める」という設計が、組織内の権限と責任の配置として健全です。

### 2. Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark
- 出典: arXiv
- 日付: 2026-08-15 submitted
- リンク: https://arxiv.org/abs/2608.15255
- 要約: 自然言語記述からドメインモデルを生成する自動ドメインモデリング手法を比較評価するため、既存のGolden UML Modelset等を組み合わせたベンチマークを提案している。LLMによるDDD支援が増えるなか、「よくできたモデル」をどう測るかという基盤整備に焦点を当てた論文です。
- なぜ面白いか:
  - 技術: 自動生成されたドメインモデルと参照モデルを比較する評価軸を整備し、LLMモデリング支援を主観的デモから再現可能な評価へ寄せている。
  - 人文: DDDの価値は会話と理解にあるため、評価指標が強すぎると現場の曖昧さを押しつぶす危険もあります。一方で、共通ベンチマークは「AIがもっともらしい図を描く」段階から、議論可能な品質へ進むための公共的な物差しになります。

### 3. DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python
- 出典: GitHub / IEEE Xplore掲載研究の実装
- 日付: 2026-08-13 更新（論文はIISEC 2026）
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: DDD-Enforcerは、PDF/DOCX/TXTの要求仕様から構造化されたDDDモデルを作り、Pythonコードに対してVS Code診断としてアーキテクチャ逸脱を検出する。LLMの多段オーケストレーション、Python AST解析、import topology、RAGによる要求仕様へのトレーサビリティを組み合わせています。
- なぜ面白いか:
  - 技術: SRSを根拠にした typed artifacts と静的解析を組み合わせ、DDDの「意図」とコードの「現在形」のズレをIDE内で検知する。
  - 人文: 設計原則はしばしばレビュー会議の記憶に閉じ込められますが、ここでは逸脱を日常の開発環境に戻しています。ただし、設計警察にならないためには、違反検出を罰ではなく対話のきっかけとして扱う文化が必要です。

### 4. LLM_Ontology_DDD: A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts
- 出典: GitHub
- 日付: 2026-08-12 作成・更新
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: このリポジトリは、DDDにおけるユビキタス言語の構築と意味的コンフリクト解消を、LLMとオントロジーのハイブリッドで扱うアプローチを掲げている。READMEは短いものの、AI時代のDDDで最も重要な「言葉の衝突」を明示的テーマにしている点が目を引きます。
- なぜ面白いか:
  - 技術: LLMの柔軟な自然言語処理と、オントロジーの明示的な概念関係を組み合わせ、用語の同義・多義・境界違いを扱おうとしている。
  - 人文: ユビキタス言語は単なる用語集ではなく、部門間の政治・経験・責任分界を映す鏡です。AIが用語衝突を可視化できるなら、設計ワークショップは「誰が正しいか」から「どの文脈では何を意味するか」へ移れます。

### 5. Archally Blueprint Schema
- 出典: GitHub
- 日付: 2026-08-11 更新
- リンク: https://github.com/Archally/blueprint-schema
- 要約: Archally Blueprint Schemaは、ドメイン設計、ビジネスルール、意思決定記録、ガバナンス、アーキテクチャをYAMLの単一モデルで表現するスキーマ。READMEでは、OpenAPI、AsyncAPI、BPMN、UML、PRD、Event Storming boardsの生成や、MCP経由でAIエージェントをグラウンディングする用途が説明されています。
- なぜ面白いか:
  - 技術: bounded context、ルール、証拠、未回答質問を機械可読なID付きモデルにし、設計知識をAIエージェントの参照可能なコンテキストへ変換する。
  - 人文: 「設計ドキュメントが散らばる」問題を、地図作成という比喩で捉え直しているのがよいです。未知を `unanswered questions` として残す設計は、AIにありがちな断言過剰を抑え、組織がまだ知らないことを正直に扱う文化につながります。

## arXiv / 学術
- Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark — arXiv:2608.15255。自然言語から生成されるドメインモデルの標準評価ベンチマークを提案。
- Automating Domain-Driven Design: Experience with a Prompting Framework — arXiv:2603.26244（2026-03-27、古いが関連性高）。ユビキタス言語、イベントストーミング、bounded context、aggregate、技術アーキテクチャへの写像をLLMプロンプトで支援する枠組みを検証し、前半工程は有用だが完全自動化には誤差伝播のリスクがあると述べている。

## メモ
- Boris Cherny優先の有無: DDD単独トピックのためClaude固有優先は適用外。ただしClaude Code/agentic skills関連の候補はGitHub検索で確認した。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールはクレジット/サブスクリプション制限で失敗したため、日本語X投稿は取得できなかった。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、代替としてBing RSS、DEV API、GitHub API、GitHub README、arXiv Web検索を直接HTTPで確認した。GitHubリポジトリは更新日が新しくても成熟度や実運用品質は未検証であり、スター数が少ないものも含むため「トレンドの兆し」として読むのが安全です。

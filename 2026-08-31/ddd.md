# DDD トレンド調査 (2026-08-31)

- 調査日: 2026-08-31
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは「全部を自動設計する」より、ユビキタス言語・型・境界・組織の会話をエージェントに監査可能な形で手伝わせる方向に寄っています。

## トップ5

### 1. Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark
- 出典: arXiv
- 日付: 2026-08-15（直近14日よりやや古いが関連性が高いため採用）
- リンク: https://arxiv.org/abs/2608.15255v1
- 要約: 自然言語記述からドメインモデルを生成する自動ドメインモデリング手法を比較するため、既存のGolden UML Modelsetなどを組み合わせたベンチマークを提案しています。ルールベースとLLM駆動戦略の評価を含み、DDDにおける「モデル生成」を研究アーティファクトとして再利用可能にする狙いです。
- なぜ面白いか:
  - 技術: LLMによるドメインモデル生成を、雰囲気ではなく参照モデルとメトリクスで比較しようとしている点が重要です。
  - 人文: DDDのモデルは本来、現場の合意や概念の輪郭を表す社会的な成果物です。その評価を標準化する試みは、専門家の暗黙知をどこまで機械が扱えるのかという境界線を可視化します。

### 2. DDD-Enforcer: SRS-grounded Domain-Driven Design enforcement for Python
- 出典: GitHub / IEEE Xplore掲載プロジェクト
- 日付: 2026-08-13更新（直近14日よりやや古いが関連性が高いため採用）
- リンク: https://github.com/barandincoguz/DDD-Enforcer
- 要約: PDF/DOCX/TXTの要求仕様から型付きDDDモデルを生成し、PythonコードのアーキテクチャドリフトをVS Code診断として検出するプロジェクトです。READMEでは、LLMによるArchitect/Specialist/Context Mapper/Criticと、AST解析・importトポロジー・RAGによる追跡性を組み合わせる構成が説明されています。
- なぜ面白いか:
  - 技術: DDD違反を「LLMレビュー」だけにせず、型付き中間成果物、AST解析、証拠文へのトレースで囲い込んでいる点が実践的です。
  - 人文: ユビキタス言語のズレや責務の漂流は、コードだけでなく組織の記憶の劣化でもあります。要求文を証拠として残す設計は、チームが「なぜそう呼ぶのか」を失わないための文化的装置になります。

### 3. agent-skills: coding agents向けDDDスキル集
- 出典: GitHub
- 日付: 2026-08-31更新
- リンク: https://github.com/salimramirez/agent-skills
- 要約: Claude Code、Cursor、GitHub Copilotなどのスキル対応エージェントにDDD作業を教えるためのポータブルな指示セットです。`ddd-playbook`はユビキタス言語、サブドメイン、境界づけられたコンテキスト、EventStorming、Context Mappingなどを扱い、Spring BootやAngular向けの実装スキルも用意されています。
- なぜ面白いか:
  - 技術: DDDを人間向けの設計知識から、エージェントが参照する実行可能な作業プロトコルへ変換している点が新しいです。
  - 人文: DDDは「会話の質」に依存する方法論ですが、AIエージェントに渡すときは会話の作法自体を文書化する必要があります。これは設計文化をオンボーディング可能な儀礼として再編集する動きに見えます。

### 4. Collaborative Data Modeling: Discovering Domain Types Through Linguistic Cues
- 出典: Virtual DDD / Webセッション
- 日付: 2026-09-03予定（2026-08-28に告知を確認）
- リンク: http://virtualddd.com/sessions/collaborative-data-modeling-linguistic-cues/
- 要約: ドメイン専門家の発話に含まれる「違反は駐車違反または速度違反」「住所は通りと都市から成る」といった言語的手がかりから、sum typeやproduct typeに相当するドメイン型を協働で発見するハンズオンです。EventStormingが「何が起こるか」に強いのに対し、Collaborative Data Modelingは「どんなものが存在するか」を補完すると説明されています。
- なぜ面白いか:
  - 技術: ユビキタス言語を型設計へ変換する具体的な橋渡しであり、LLMに要求や会話ログを読ませる前処理としても相性が良いテーマです。
  - 人文: 専門家がコードを読めなくても、言葉の使い方の中にモデルの形はすでにあります。設計者の仕事は発明よりも傾聴に近い、というDDDの人類学的な側面を強く示しています。

### 5. Organisational Dysfunctions: A Live Diagnosis Session with Trond Hjorteland
- 出典: Virtual DDD / Webセッション
- 日付: 2026-09-09予定
- リンク: http://virtualddd.com/sessions/diagnosing-organisational-dysfunctions-open-systems-theory/
- 要約: 職場で繰り返し起こる組織的な不調を、1960年代以降のOpen Systems Theoryの観点から診断するライブセッションです。ゲストはDDD、ビジネス能力マッピング、EventStorming、マイクロサービス、イベント駆動アーキテクチャを、設計が組織に根づくための実践と接続して語る立場です。
- なぜ面白いか:
  - 技術: 境界づけられたコンテキストやイベント駆動設計を、組織構造・権限・フィードバックループの問題として読み直せます。
  - 人文: AIエージェントが開発速度を上げても、壊れた組織構造はそのまま高速化されるだけです。DDDを組織文化の診断言語として使う視点は、エージェント時代の設計責任を人間側へ引き戻します。

## arXiv / 学術
- 見つかりました: `2608.15255v1` “Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark”。2026-08-15公開で、LLM駆動を含む自動ドメインモデリング評価ベンチマークを提案しています。
- 参考として、2026-03-27公開の `2603.26244v1` “Automating Domain-Driven Design: Experience with a Prompting Framework” も確認しました。ユビキタス言語、EventStorming、bounded context、aggregate、技術アーキテクチャへの写像をLLMプロンプトで支援し、前半の設計会話には有効だが後半では誤差が蓄積すると報告しています。

## メモ
- Boris Cherny優先の有無: DDD単独調査のためClaude系優先条件は該当なし。
- 日本語アカウントの扱い: 日本語クエリ（「ドメイン駆動設計」「イベントストーミング」「ユビキタス言語」）も試行しましたが、今回利用可能な検索経路では有力な直近日本語ソースを確認できませんでした。
- 注意点・誇張リスク: X検索はxAIクレジット不足で失敗し、Web検索ツールもFirecrawl未設定で失敗しました。そのため、代替としてarXiv API、GitHub API、Jina経由の公開Webページ取得、Virtual DDDの公開ページ/Bluesky埋め込み情報を使用しました。X由来の一次投稿は本調査時点では確認できていません。

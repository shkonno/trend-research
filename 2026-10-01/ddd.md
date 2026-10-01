# DDD トレンド調査 (2026-10-01)

- 調査日: 2026-10-01
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

DDDは「人間の会話を設計資産にする技法」から、AIエージェントに渡す文脈・制約・検証ルールを作るための社会技術へ広がっている。

## トップ5

### 1. Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems
- 出典: arXiv
- 日付: 2026-09-23
- リンク: http://arxiv.org/abs/2609.27354v1
- 要約: 生成AIシステムを特定ドメインに適合させる際、単なるRAGやツール連携ではなく、技術・規制・制度・規範上の「制約」を体系的に文脈へ組み込む設計アプローチを提案している。DDDそのものの論文ではないが、AIシステムに対してドメイン境界・許容行動・制約をインターフェースとして定義する点が、AI/agent時代のDDDと強く接続する。
- なぜ面白いか:
  - 技術: ユビキタス言語や境界づけられたコンテキストを、LLMへ渡す「制約駆動のコンテキスト」として再解釈できる。
  - 人文: AIの振る舞いを単に精度で測るのではなく、組織・制度・規範の中で何が「適切」かを設計対象にしている点が重要である。DDDが本来持っていた、ソフトウェアを社会的な合意形成として扱う側面が前景化している。

### 2. Domain Modeling Meets Generative AI / ddd-meets-genai
- 出典: GitHubリポジトリ
- 日付: 2026-09-30更新（作成は2026-03-07、最終pushは2026-09-16のため一部は直近14日外）
- リンク: https://github.com/mardenneubert/ddd-meets-genai
- 要約: Event Stormingで得た付箋・会話・ドメイン知識を、LLMエージェントが構造化されたドメインモデルへ変換するための仕様、エージェント、評価ケースをまとめた研究リポジトリ。READMEでは、Event Stormingからbounded contexts、aggregates、entities、value objects、context mapsへつなぐ「知識ボトルネック」を問題としている。
- なぜ面白いか:
  - 技術: DDDの発見活動を、LLMが扱える中間表現と検証可能な成果物へ落とす実験として、イベントストーミングと自動モデリングの橋渡しになっている。
  - 人文: 付箋やホワイトボードに宿る曖昧な会話を、AIが処理可能な構造へ変換する試みは、現場の記憶をどう保存し、誰の言葉をモデルに残すのかという文化的問題を伴う。

### 3. Agent Skills: DDD Playbook and Stack Skills
- 出典: GitHubリポジトリ
- 日付: 2026-09-18更新
- リンク: https://github.com/salimramirez/agent-skills
- 要約: Claude Code、Cursor、GitHub CopilotなどのAI coding agent向けに、DDDの「スキル」をポータブルな指示セットとして提供するリポジトリ。`ddd-playbook`はユビキタス言語、サブドメイン、bounded context、context mapping、domain storytelling、EventStorming、Bounded Context Canvas、集約・値オブジェクト・ドメインイベントなどを扱う。
- なぜ面白いか:
  - 技術: DDDの判断規則を、モデル非依存のエージェントスキルとして小さく読み込ませる設計は、LLM時代の「設計知識の配布形式」として実用的である。
  - 人文: 熟練者の暗黙知をスキルファイルに翻訳することは、設計文化の継承方法を変える。師弟関係やレビュー会で伝わっていた言葉遣いを、AIと新人が共有する教材に変える動きとして読める。

### 4. NestJS DDD Starter Kit with AI Agent Rules & Skills
- 出典: GitHubリポジトリ
- 日付: 2026-09-27更新（作成は2026-09-26）
- リンク: https://github.com/khacvux/nest-ddd-starter-kit
- 要約: NestJS、TypeORM、PostgreSQLを前提に、DDDとヘキサゴナルアーキテクチャを厳格に分離したスターターキット。READMEでは、ドメイン層をフレームワーク非依存に保つこと、Ports & Adapters、さらにClaude Code、Cursor、Copilot、Antigravity向けのAI Agent Rules & Skillsを含むことを特徴としている。
- なぜ面白いか:
  - 技術: DDD/Hexagonalの層分離を、AIエージェントがコード生成時に参照するルールとして同梱している点が、アーキテクチャテンプレートの新しい標準形を示している。
  - 人文: AIがチームの「新入り開発者」になるなら、リポジトリ自体に組織の作法や禁則を埋め込む必要がある。この種のスターターは、文化をオンボーディング資料ではなく実行環境へ移す試みである。

### 5. AI時代の静的解析ベストプラクティス：自然言語のルールをArchUnitで「実行できるルール」に変える
- 出典: Qiita記事
- 日付: 2026-09-23
- リンク: https://qiita.com/ukun3/items/2545a4db32dd575ad426
- 要約: AIエージェント向けにMarkdownで書いたチームルールを、ArchUnit、Semgrep、reviewdogなどで検証可能なルールへ変換する実践ガイド。記事中では「ドメイン層からJPAに依存してはいけない」のようなDDD/クリーンアーキテクチャ系の構造ルールを、自然言語だけでなくCIで決定的に検証する必要性が説明されている。
- なぜ面白いか:
  - 技術: ユビキタス言語や設計原則をAIに読ませるだけでなく、層依存・境界違反を静的解析でブロックする「DDDの機械的ガードレール」へ変換している。
  - 人文: AI時代の設計規律は、信頼や注意力に頼る文化から、合意したルールを自動で守らせる文化へ移行しつつある。これはレビューの権威や責任分担を変えるため、単なるツール導入以上の組織変化を含む。

## arXiv / 学術

- `2609.27354v1` — Constraint-Driven Context Engineering: Designing Domain Interfaces for AI Systems（2026-09-23）。DDDを直接扱うわけではないが、ドメイン固有の制約をAIシステムの文脈設計に組み込む研究として本日のトップ項目に採用。
- `2608.15255v1` — Towards Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark（2026-08-15、直近14日外）。自動ドメインモデリング評価の標準ベンチマークを提案。
- `2608.05612v1` — Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design（2026-08-06、直近14日外）。戦術的DDDのモデルとJavaコードを双方向同期するJDomInOを提案。
- `2603.26244v1` — Automating Domain-Driven Design: Experience with a Prompting Framework（2026-03-27、直近14日外）。ユビキタス言語、イベントストーミング、bounded context、集約、技術アーキテクチャへの写像をLLMプロンプトで支援する枠組みを提示。

## メモ

- X検索は英語・日本語の両方で実行したが、xAI側の `personal-team-blocked:spending-limit` により結果取得できなかった。そのため本ファイルではX由来の項目は採用していない。
- Web検索ツールはFirecrawl未設定で利用できなかったため、GitHub API、Qiita API、arXiv API、HN Algolia API、DuckDuckGo HTMLへの直接HTTPアクセスで代替した。DuckDuckGo HTML検索は今回有効な結果を返さなかった。
- 日本語ソースはQiita APIで確認し、AIエージェント時代の設計ルール検証としてDDDに接続できる記事を1件採用した。
- Boris Cherny優先指定はClaude系トピック向けのため、今回のDDD調査では該当なし。
- 誇張リスク: GitHubリポジトリはスター数が少ないものも含まれるため、「流行の大規模採用」ではなく「今出てきている設計パターンの兆候」として扱うべきである。

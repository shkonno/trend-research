# DDD トレンド調査 (2026-09-28)

- 調査日: 2026-09-28
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AI/LLM時代のDDDは「重い儀式」ではなく、エージェントの出力を人間の意味・境界・責任へつなぎ止める設計言語として再評価されている。

## トップ5

### 1. Agentic Domain-Driven Mainframe Modernization
- 出典: GitHub / Project Rosetta pattern catalog
- 日付: 2026-09-27 更新
- リンク: https://github.com/pmilet/ai-ddd-mainframe-modernization-patterns
- 要約: COBOL/CICSなどのメインフレーム近代化を「コード変換」ではなく「埋もれた業務意味の回復」と捉え、AIエージェントをハーネス内で使う28パターンとアンチパターンをまとめたカタログ。DDD実践者、メインフレーム近代化担当、agentic codingの実務者を接続する内容になっている。
- なぜ面白いか:
  - 技術: LLMを翻訳器としてではなく、レガシーコードからドメイン知識・境界・ビジネス概念を復元する補助エージェントとして配置している点がDDD的に強い。
  - 人文: 長寿命システムを「古い負債」としてではなく、組織記憶と制度化された判断の堆積として読む視点がある。近代化を単なる置換ではなく、企業の歴史を再解釈する作業として扱っている。

### 2. NestJS DDD Starter Kit with AI Agent Rules & Skills
- 出典: GitHub
- 日付: 2026-09-26 作成 / 2026-09-27 更新
- リンク: https://github.com/khacvux/nest-ddd-starter-kit
- 要約: NestJS、TypeORM、PostgreSQLを使った厳格なDDD/Hexagonal Architectureスターターで、Claude Code、Cursor、Copilot等向けのAI Agent Rules & Skillsを同梱する。Domain層のフレームワーク非依存、Ports & Adapters、bounded context単位のフォルダ構造などを最初から明文化している。
- なぜ面白いか:
  - 技術: DDDの制約をREADMEやディレクトリ構造だけでなく、AIコーディングエージェントが参照するルールとして配布している点が実務的。
  - 人文: チームの「設計文化」を人間の口伝からエージェント可読の憲章へ移す動きとして読める。ユビキタス言語は会議室だけでなく、AIが読む作業環境にも埋め込まれ始めている。

### 3. Ask HN: Ceremonious Architecture in Times of AI
- 出典: Hacker News
- 日付: 2026-09-22
- リンク: https://news.ycombinator.com/item?id=49795847
- 要約: LLMが大量の足場コードを短時間で生成できるなら、DDDやClean Architectureのような「儀式的」設計パターンのコストは下がり、むしろAIの暴走を抑える構造として価値が増すのではないか、という問いかけ。コメント数は多くないが、DDDとAI時代の設計コストを端的に言語化している。
- なぜ面白いか:
  - 技術: 生成AIによりボイラープレートの生産コストが下がると、アーキテクチャ分離・静的制約・テスト可能性の相対価値が上がるという仮説が示されている。
  - 人文: 「面倒だから省く」から「AIに任せるからこそ構造が必要」へ、職人文化の判断基準が反転している。設計の儀式性を、形式主義ではなく共同作業の安全装置として再評価する議論になっている。

### 4. A Hybrid LLM–Ontology Approach for Constructing the Ubiquitous Language and Resolving Semantic Conflicts in DDD（直近14日外だが関連度高）
- 出典: GitHub
- 日付: 2026-09-08 更新（直近14日外）
- リンク: https://github.com/BlayTeuR/LLM_Ontology_DDD
- 要約: LLMとオントロジーを組み合わせ、DDDにおけるユビキタス言語の構築と意味衝突の解消を狙うプロジェクト。READMEは短いが、AI時代のDDDで最も壊れやすい「同じ語を同じ意味で使う」問題に正面から向いている。
- なぜ面白いか:
  - 技術: LLMの柔軟な自然言語処理と、オントロジーの明示的な意味制約を組み合わせることで、用語抽出だけでなく概念間の不一致検出へ踏み込める。
  - 人文: ユビキタス言語は辞書ではなく、部署・専門職・歴史的慣習の交渉でできる社会的合意である。AIがその合意形成を支援するなら、誰の語彙が標準化され、誰の言葉が消えるのかという権力の問題も生まれる。

### 5. faceto: typed file → visual workshop board with LLM（直近14日外だが関連度高）
- 出典: GitHub / documentation
- 日付: 2026-09-07 更新（直近14日外）
- リンク: https://github.com/bastien-gallay/faceto
- 要約: 型付きファイルからイベントストーミングのHTML/SVGボードを生成し、LLMと一緒にモデルを考えるためのツール。イベントストーミングを最初の形式とし、将来的にcontext map、bounded context canvas、core domain chartへ拡張する方向性を掲げている。
- なぜ面白いか:
  - 技術: ワークショップの付箋やイベントログを構造化ファイルとして扱い、LLMが読み書きできるモデルと人間が眺めるボードを往復させる設計が秀逸。
  - 人文: イベントストーミングの価値は、正解を出すことよりも関係者が同じ物語を作る過程にある。facetoはその対話的な場を、AIとの共同編集に開きながらも「人が読める盤面」を中心に残している。

## arXiv / 学術
- Toward Standardized Evaluation in Automated Domain Modeling: Introducing a Benchmark / arXiv:2608.15255 / 2026-08-15。自然言語記述からドメインモデルを生成するタスクのベンチマークを提案し、LLM駆動戦略を含む自動ドメインモデリング手法の比較評価を扱う。直近14日外だが、LLM×DDD評価基盤として重要。
- Automating Domain-Driven Design: Experience with a Prompting Framework / arXiv:2603.26244 / 2026-03-27。ユビキタス言語、イベントストーミング、bounded contexts、aggregates、技術アーキテクチャへの写像をLLMプロンプトで支援する研究。ステップ1〜3は有用だが、後段では誤差が蓄積し、LLMは専門家の代替ではなく協働相手だと結論づけている。古いが、本日のGitHub/Web動向を理解する基礎文献として関連度が高い。

## メモ
- X検索は英語・日本語で実行したが、xAI側の `personal-team-blocked:spending-limit` により結果取得できなかった。そのため本ファイルではX由来アイテムを採用せず、GitHub API、Hacker News Algolia API、arXiv API、直接HTTP取得で確認できた情報に限定した。
- Web検索ツールはFirecrawl未設定で失敗したため、代替としてBing RSS、GitHub API、Hacker News Algolia API、arXiv API、直接HTTP取得を利用した。Bing RSSは一般的な「domain」検索結果が多く、採用しなかった。
- 日本語アカウント/投稿はX検索制限のため確認不能。日本語Web検索も有用なDDD関連の直近結果を確認できなかった。
- 注意点: GitHubリポジトリは更新日が新しくても成熟度や実利用実績が限定的な場合がある。特に短いREADMEのプロジェクトは、コンセプトの面白さとして扱い、導入推奨とは切り分けて読むべき。
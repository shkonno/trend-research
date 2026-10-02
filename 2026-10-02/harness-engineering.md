# Harness engineering トレンド調査 (2026-10-02)

- 調査日: 2026-10-02
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「良いプロンプトを書く」から一段進み、複数のエージェント実行環境を差し替え・観測・停止・検証できる運用基盤を設計する話題へ移っている。

## トップ5

### 1. HarnessRouter と Unified Harness Protocol が “ハーネスの標準API” を押し出す

- 出典: GitHub / Web検索結果 / 公式プロトコルページ
- 日付: 2026-10-02 更新（GitHub pushed_at: 2026-10-02T00:22:21Z）、UHP spec は 2026-09-12
- リンク: https://github.com/HarnessRouter/harnessrouter
- 要約: HarnessRouter は Codex、Claude Code、Hermes、Pi などの agent harness を OpenAI Responses 互換の共通APIで扱う self-hosted 基盤として更新が続いている。README でも “Build agent products without handling harness engineering” と明示し、セッション、ストリーミング、ファイル、キャンセル、失敗処理を UHP に寄せている。
- なぜ面白いか:
  - 技術: ハーネスごとの癖を UHP に抽象化することで、Claude Code などを「製品バックエンドの交換可能な実行エンジン」として扱える。
  - 人文: これは開発者の仕事を「モデルに命令する人」から「複数の行為主体を統治する制度設計者」へ変える動きであり、ソフトウェア開発における責任境界の再配置として重要。

### 2. Raven が “harness of harnesses” として HN で議論を集める

- 出典: Hacker News / GitHub
- 日付: 2026-09-29（Show HN）、GitHub pushed_at: 2026-10-01T06:19:24Z
- リンク: https://news.ycombinator.com/item?id=49890647
- 要約: Raven は “The Harness of Harnesses” を掲げ、永続的で自己進化する multi-agent ecosystem を志向するプロジェクトとして Show HN に登場した。GitHub では 5,000 stars 超で、arXiv バッジも掲げ、ハーネスを単一エージェントのラッパーではなく協調環境として扱っている。
- なぜ面白いか:
  - 技術: 複数ハーネス・複数モデルを束ねるメタハーネス型は、plan→generate→evaluate のループを長時間・多人数・多ツールに拡張する実装パターンになる。
  - 人文: “built for RSI” という表現が象徴するように、これは効率化だけでなく身体的負担や働き方の再設計にも接続している。AI エージェントは作業を奪うだけでなく、痛みや疲労を減らす補助環境として語られ始めている。

### 3. Omnigent が Claude Code / Codex / Pi をまたぐ meta-harness を強調

- 出典: GitHub / Hacker Newsコメント
- 日付: 2026-10-02 更新（GitHub pushed_at: 2026-10-02T00:28:52Z）、関連HNコメント: 2026-09-29
- リンク: https://github.com/omnigent-ai/omnigent
- 要約: Omnigent は Claude Code、Codex、Cursor、OpenCode、Hermes、Pi などを共通の orchestration layer から扱う open-source meta-harness として更新されている。HN では、Claude Code + Opus で計画し、Codex や Pi/Kimi など別エージェントに実装・判断を分担させるユースケースが語られていた。
- なぜ面白いか:
  - 技術: ハーネスを一つ選ぶのではなく、タスクごとにモデル・実行環境・ポリシーを組み合わせる “portfolio orchestration” が現実的な設計対象になっている。
  - 人文: 開発チームの中に「AI労働の編成係」のような役割が生まれ、誰に何を任せ、どこで人間が承認するかという組織論がコードの設計問題として現れている。

### 4. Claude Code の plan mode を外部ドキュメントや issue と組み合わせる議論

- 出典: Hacker News
- 日付: 2026-10-01
- リンク: https://news.ycombinator.com/item?id=49920876
- 要約: “Do you guys also still use Claude Code's plan mode?” という Ask HN では、plan mode 単体では長い機能開発の情報保持が弱いという問題意識が出ていた。コメントでは PLAN_FEATURE、TESTS、ARCHITECTURE などのファイルに計画を分割し、issue、wiki、Linear、skills、カスタムハーネスに文脈を逃がす実践が共有されている。
- なぜ面白いか:
  - 技術: これは Claude Code の内部機能だけで完結させず、外部の文書・チケット・リポジトリ状態をハーネスの記憶層として使う実務的な loop engineering である。
  - 人文: 記憶をどこに置くかは単なる実装ではなく、チームが「何を合意したことにするか」を決める文化の問題でもある。AI との共同作業では、計画文書が人間同士の信頼の媒体にもなる。

### 5. ScholarEvolve: 研究文献を使って agent harness 自体を進化させる arXiv 論文

- 出典: arXiv
- 日付: 2026-09-30
- リンク: http://arxiv.org/abs/2609.40169v1
- 要約: “Learning from Research: Toward Lifelong Agent Harness Evolution” は、モデル本体を固定したまま、ツール利用、メモリ管理、タスク実行を司る agent harness を継続的に改善する枠組み ScholarEvolve を提案している。失敗ログだけでなく研究文献から改善方向を抽出し、機能モジュールごとの戦略に落とす点が特徴。
- なぜ面白いか:
  - 技術: ハーネス改善をメタコーディングエージェントと研究サーベイで自動化するため、評価ループが「失敗への反応」から「知識に基づく探索」へ広がる。
  - 人文: エージェントが研究を読み、自分の作業環境を改良する構図は、道具が道具自身の歴史を学ぶようなもの。人間の専門職が文献から実践を更新する営みに近づいており、専門性の所在を問い直す。

## arXiv / 学術

- 見つかった論文: “Learning from Research: Toward Lifelong Agent Harness Evolution” / arXiv:2609.40169 / 2026-09-30 / agent harness を、固定モデルの外側で継続進化させる ScholarEvolve を提案。
- 関連して確認した論文: “cua-speedrun: Standardized Benchmarking of the Speed of Computer-Use Agents” / arXiv:2609.40284 / 2026-09-30 / CUA の速度・コスト評価を標準化するベンチマークで、共通 agent interface と実行パイプラインが harness engineering と接続する。
- 関連して確認した論文: “Better Deck or Different Judge? Evaluating Agentic Harness Gains in Corporate and Investment Banking” / arXiv:2609.39958 / 2026-09-30 / 金融資料作成の agentic harness を judge と検証チェック込みで評価し、ハーネス改善と評価者バイアスの問題を扱う。

## メモ

- Boris Cherny優先の有無: Boris Cherny / @bcherny と Harness engineering の直近接点を X で優先確認しようとしたが、x_search は `personal-team-blocked:spending-limit` で失敗した。代替として HN、GitHub API、DuckDuckGo HTML via Jina、arXiv API を使ったが、本調査時点で Boris 本人の直近発言は検証できなかった。
- 日本語アカウントの扱い: X検索は同じ理由で実施不能。Web側では「Claude Code ハーネス」「Claude Code ループエンジニアリング」の日本語記事が検索結果に出たが、直近14日の明確な日付・一次性を確認できたものはトップ5には入れなかった。日本語コミュニティでは「ハーネス」「ループ」「停止条件」「外部記憶」という語彙で Claude Code 実践が説明されつつある。
- 注意点・誇張リスク: GitHub stars や HN の反応は注目度の指標にはなるが、実運用品質を保証しない。特に “self-evolving” や “harness of harnesses” は魅力的な物語になりやすいため、採用時は権限境界、ログ、再現性、停止条件、秘密情報の扱いを個別に検証する必要がある。
- ソース制約: Hermes の web_search は Firecrawl 未設定で失敗したため、Web調査は terminal 経由の GitHub API、HN Algolia API、DuckDuckGo HTML/Jina、arXiv API で代替した。

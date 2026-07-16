# Philosophy of Loop Engineering トレンド調査 (2026-07-15)

- 調査日: 2026-07-15
- 情報源: X / Web（Bing RSS・GitHub API・直接取得） / arXiv API
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
ループエンジニアリングは「より良いプロンプト」ではなく、反復・検証・責任境界を設計する、実践的なサイバネティクスとして語られ始めている。

## トップ5

### 1. LOGOS: Verifiable Human-Agent Loop Engineering
- 出典: arXiv 論文 / Xでの日本語共有
- 日付: 2026-07-12（arXiv公開）、2026-07-14（関連X投稿）
- リンク: https://arxiv.org/abs/2607.10878v1 / https://x.com/yuma_1_or/status/2076974062983651709
- 要約: LOGOSは、エージェントの学習・プロンプト・記憶・スキル・ツール変更を、証拠、ポリシー、人間の明示的承認なしには昇格させない「fail-closed」な統治層として提案している。論文中で “verifiable human-agent loop engineering” と呼ばれ、提案と本番適用を切り分ける点が中心である。
- なぜ面白いか:
  - 技術: エージェント活動を監査可能なイベントトレースにし、候補変更をテスト・権限・承認で昇格判定するため、長期稼働ループの安全な運用設計に直結する。
  - 人文: 「AIが進化する速度」と「人間が責任を引き受ける速度」の非対称性を、制度設計として扱っている点が重要。サイバネティクスで言えば、制御対象だけでなく、誰が制御器を制御するのかという二階の問いに踏み込んでいる。

### 2. Own the Outer Loop
- 出典: Addy Osmani “Elevate” Substack（Web/RSS）
- 日付: 2026-07-09
- リンク: https://addyo.substack.com/p/own-the-outer-loop
- 要約: Addy Osmaniは、エージェント時代の技術者の仕事を「内側の実行」から「外側のループの所有」へ移すべきだと述べ、説明責任、レビュー、境界設定をループ設計の核心に置く。Bing RSS上でも、長時間動くAIエージェントに対し、信頼とチームの周辺システムが焦点になっていることが確認できた。
- なぜ面白いか:
  - 技術: 自動化の性能を上げるだけでなく、レビュー、停止条件、承認ポイント、結果の受け皿を外部ループとして設計する実務的論点を前面化している。
  - 人文: これは「人間をループから外す」話ではなく、人間がどの境界で判断を保持するかという責任論である。実践知とは、AIに任せる範囲を増やす能力ではなく、任せてはいけない境界を見分ける能力として再定義されている。

### 3. Boris Cherny系の「発見→実行→検証→永続化→スケジュール」ループ議論
- 出典: X投稿（sairahul1による共有、Boris Cherny系PDF/手法への言及）
- 日付: 2026-07-06
- リンク: https://x.com/sairahul1/status/2074063851302355085
- 要約: X上で、長時間走るエージェントには Discovery / Build or Act / Verify / Persist / Schedule のような外部ループが必要であり、特に検証役を「壊れていると仮定する」別主体として置くべきだという議論が拡散している。プロンプトの巧拙より、状態をディスクに残し、失敗を検出し、次回起動へつなぐ構造が重視されている。
- なぜ面白いか:
  - 技術: 自己採点による過大評価を避けるため、maker/checker分離、永続状態、スケジュール再実行をループの基本部品として扱う点が実装に落とし込みやすい。
  - 人文: ここでの知識は、頭の中の確信ではなく、反証に耐えた痕跡として残る。PeirceやDewey的なプラグマティズム、Popper的な反証主義が、ソフトウェア運用の作法として再登場している。

### 4. cobusgreyling/loop-engineering のツール化と「Loop Ready」スコア
- 出典: GitHubリポジトリ / Web直接取得
- 日付: 2026-07-15時点で更新確認（リポジトリ更新: 2026-07-15）
- リンク: https://github.com/cobusgreyling/loop-engineering
- 要約: Cobus Greylingのリポジトリは、Loop Engineeringをパターン、スターター、CLIツールとしてまとめ、`loop-init`、`loop-audit`、`loop-cost`などでループの準備度・コスト・状態管理を扱う。READMEでは “Stop prompting. Design the loop. Get a score.” と明確に掲げ、Addy OsmaniやBoris Chernyの議論を実装テンプレートへ変換している。
- なぜ面白いか:
  - 技術: 抽象概念だったループ設計を、スキル、状態、予算、監査、クイックスタートに分解し、リポジトリ単位で導入できる形にしている。
  - 人文: 「良いループ」を点数化する動きは、暗黙の職人芸を外部化する試みである。一方で、点数化できる実践知と、点数化からこぼれる判断力の差分も可視化される。

### 5. LoopX: long-running AI agents のためのローカル制御面
- 出典: GitHubリポジトリ / Web直接取得
- 日付: 2026-07-14時点で更新確認（リポジトリ更新: 2026-07-14）
- リンク: https://github.com/huangruiteng/loopx
- 要約: LoopXは、Codex、Claude Code、Cursorなどの実行ランタイムを置き換えず、目的、ゲート、todo、証拠、クォータ、ハンドオフを安定化させる軽量なローカル制御面として作られている。READMEの “Keep the loop moving. Keep the judgment human.” という標語が、ループを止めないことと判断を人間に残すことを同時に掲げている。
- なぜ面白いか:
  - 技術: エージェント実行そのものではなく、複数ターン・複数主体にまたがる状態、証拠、引き継ぎ契約を保存することで、長期稼働を再開可能・レビュー可能にする。
  - 人文: これは「自律性」を人格のように扱うのではなく、記録・権限・判断の配置として扱う設計思想である。中国語READMEの「管理可能、复盘、持续改进」という語感も、反復を単なる自動化ではなく組織的な学習として捉えている。

## arXiv / 学術
- LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans — arXiv:2607.10878v1。人間の権限と実行証拠だけがループを閉じられる、という統治モデルを “verifiable human-agent loop engineering” として提示。
- 追加で “feedback loop / AI agents / cybernetics / epistemology” の組み合わせをarXiv APIで検索したが、直近で哲学・認識論・サイバネティクスを明示的に結ぶ別論文は本調査時点で確認されませんでした。

## メモ
- Boris Cherny優先の有無: Claude/AIエージェント文脈として優先し、Boris Cherny系PDF/手法に言及するX投稿をトップ5に含めた。
- 日本語アカウントの扱い: 日本語X検索を行い、LOGOS共有や三層ループ、実践知、Harness Engineeringとの違いに関する日本語圏の議論を確認した。トップ5ではリンクの検証可能性と内容の密度を優先した。
- 注意点・誇張リスク: Web検索ツールは未設定で失敗したため、代替としてBing RSS、GitHub API、直接URL取得、arXiv APIを用いた。X本文はx_searchの検索結果に基づくため、外部ページ本文を完全取得できていない投稿については、日付をSnowflake IDから算出し、内容は検索結果で確認できた範囲に限定した。

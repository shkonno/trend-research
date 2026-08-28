# Harness engineering トレンド調査 (2026-08-28)

- 調査日: 2026-08-28
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
モデル単体の性能競争から、モデルを包む「実行ループ・記憶・検証・道具」の設計を能力として扱う流れが、Claude CodeやSRE/評価用途を軸にかなり明確になっています。

## トップ5

### 1. JIT-Agent: Scaling Harness Intelligence via Just-in-Time Harness Evolution
- 出典: arXiv
- 日付: 2026-08-26
- リンク: https://arxiv.org/abs/2608.25593v1
- 要約: エージェントの能力は基盤モデルだけでなく、メモリ管理、計画戦略、行動プロトコル、ツール/スキル・オーケストレーションを含む「agent harness」に大きく左右されるとして、タスクに応じてハーネスを生成・修復・自己進化させる JIT-Agent を提案しています。要旨では、生成したハーネスが OpenCode や Claude Code のような成熟したエージェントランタイムと競争的で、複数モデル系列の性能を改善するとされています。
- なぜ面白いか:
  - 技術: ハーネスを手書きの周辺コードではなく、学習・生成・進化可能な第一級アーティファクトとして定式化している点が重要です。
  - 人文: これは「知能は個体の頭の中だけにあるのか、それとも環境・道具・制度との結合にあるのか」という拡張認知の議論に近い転換です。Claude Codeのようなツールを使う人間も、実はモデルではなく作業環境そのものを育てているのだと読めます。

### 2. From General Agents to RCA Experts: A Self-Evolving Harness for Root Cause Analysis
- 出典: arXiv
- 日付: 2026-08-26
- リンク: https://arxiv.org/abs/2608.25661v1
- 要約: SREの根本原因分析（RCA）で、CodexやClaude Codeのような汎用エージェントを直接使う方法と専用RCAエージェントを作る方法を比較し、性能差の主因を外部適応層＝ハーネスに見ています。OpsHarnessは過去の診断経験を再利用可能な知識へ変換し、成功/失敗軌跡を比較しながら二重ゲート検証で更新を採用する自己進化型RCAハーネスです。
- なぜ面白いか:
  - 技術: 既存の強い汎用エージェントを作り直すのではなく、運用知識、ツールライブラリ、検証ゲートを外付けして専門家化する設計が実務的です。
  - 人文: 障害対応の「経験知」は、個人の勘からチームの記録、さらにエージェントの再利用可能な制度へ移りつつあります。一方で、どの失敗から何を学ばせるかは組織文化や責任分界を映すため、単なる自動化ではなく職能の再編成でもあります。

### 3. The Empire, Long Divided, Must Unite: Architectural Convergence in Three LLM Agent Harnesses
- 出典: arXiv
- 日付: 2026-08-25
- リンク: https://arxiv.org/abs/2608.23953v1
- 要約: LangChain deepagents、Earendil pi、DeepSeek dsh という思想の異なる3つのコーディングエージェント・ハーネスをソースレベルで比較し、ループ、追記型セッション記録、モデル固有癖のデータ化、段階的なコンテキスト開示、明示的な拡張シームという5要素へ収束していると論じています。同時に、外部から検証可能な耐改ざん記録が欠けていることを次の差別化軸として指摘します。
- なぜ面白いか:
  - 技術: 異なる実装哲学が同じ構成要素へ寄っていくという観察は、ハーネス設計に事実上の参照アーキテクチャが生まれつつあることを示します。
  - 人文: 「エージェントのふるまいを誰が後から検証できるのか」という問いは、信頼を実行者の人格から記録の制度へ移す話です。自律システムの歴史は、能力拡張と同時に監査可能性をめぐる政治を生みます。

### 4. LubbDubb — PTY駆動Claude Codeエージェントの常駐オーケストレーション・ハーネス
- 出典: GitHubリポジトリ
- 日付: 作成 2026-07-21（古いが、2026-08-28に更新）
- リンク: https://github.com/AdamAwan/LubbDubb
- 要約: LubbDubbは、issue、PR、CI、レビューコメントなどを監視し、heartbeatごとに状態をスナップショット、差分化、計画調整、判断、実行、監査するセルフホスト型のSWE作業コックピットです。READMEでは、PTY駆動のClaude Codeエージェントをプールされたgit worktreeやscratch dirで走らせ、必要な判断だけ人間へエスカレーションする構成が説明されています。
- なぜ面白いか:
  - 技術: Claude Codeを単発CLIではなく、状態監視、ディスパッチ、監査ログ、作業ディレクトリ分離を備えた常駐ループに組み込む実装例として価値があります。
  - 人文: ここでの人間は逐一命令する操作者ではなく、例外や価値判断に介入する編集長のような役割になります。仕事のリズムが「チケットを見る」から「心拍するシステムを監督する」へ変わる点が象徴的です。

### 5. pit-harness — point-in-time評価とハッシュ付き実行レシート
- 出典: GitHubリポジトリ
- 日付: 作成 2026-08-27、更新 2026-08-28
- リンク: https://github.com/sharath/pit-harness
- 要約: pit-harnessは、LLMエージェントを時点固定のベンチマーク窓で評価し、ネットワークを無効化し、trajectoryとreceiptを保存して検証可能にする評価ハーネスです。READMEでは、行がいつ「知り得た」情報になるかを複数のclock policyで扱い、`pit-harness verify`で実行レシートを検証する流れが示されています。
- なぜ面白いか:
  - 技術: エージェント評価で混入しがちな時間漏洩や外部情報アクセスを、PIT窓、隔離ツール、ハッシュ化されたレシートで制御する点が実務的です。
  - 人文: エージェントの成果物を信じるためには、賢さの物語だけでなく「いつ何を知り、どう行動したか」の公共的な記録が必要になります。これはAI利用を、デモの説得力から監査可能な証拠文化へ移す動きです。

## arXiv / 学術
- JIT-Agent: Scaling Harness Intelligence via Just-in-Time Harness Evolution — arXiv:2608.25593v1。ハーネス生成そのものを学習対象にする論文。
- From General Agents to RCA Experts: A Self-Evolving Harness for Root Cause Analysis — arXiv:2608.25661v1。SRE/RCA向けに汎用エージェントを外部ハーネスで専門家化する論文。
- The Empire, Long Divided, Must Unite: Architectural Convergence in Three LLM Agent Harnesses — arXiv:2608.23953v1。複数のエージェントハーネス実装が共通アーキテクチャへ収束していると分析。

## メモ
- Boris Cherny優先の有無: @bcherny を含むX検索を実行しましたが、x_searchが `personal-team-blocked:spending-limit` で失敗したため、Boris Cherny本人の直近投稿は確認できませんでした。Web/GitHub/arXiv側では、Claude Codeとの接点として JIT-Agent 論文、OpsHarness 論文、LubbDubb README を優先しました。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で取得できませんでした。代替としてGitHub検索で日本語/Japan関連を確認し、`shubhank008/athome-japan-agent-harness`（2026-08-17作成、2026-08-20更新）を確認しましたが、不動産検索用途の個別アプリ寄りで、今回のトップ5には入れませんでした。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定で利用不能、DuckDuckGo HTMLはbot challengeにより結果取得不能でした。そのため、本稿は arXiv API と GitHub API/README の実取得結果を中心に構成し、X由来の流行度や日本語コミュニティの反応は限定的です。GitHubのstar数が少ない新規リポジトリも含むため、「普及済み」ではなく「設計シグナルとして面白い」と読むのが安全です。

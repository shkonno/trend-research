# Loop engineering トレンド調査 (2026-08-31)

- 調査日: 2026-08-31
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「人がエージェントを逐次プロンプトする」段階から、「検証・記録・安全境界を持つ反復システムを設計する」段階へ移りつつあります。

## トップ5

### 1. Safety Does Not Compose: Non-Decaying Loop State for Autonomous LLM Agents
- 出典: arXiv / Hacker News
- 日付: 2026-08-27 submitted（HN掲載は2026-08-29）
- リンク: https://arxiv.org/abs/2608.27141
- 要約: 自律LLMエージェントを「人間のゴールから始まり、作業発見・計画・ツール実行・検証・状態永続化を繰り返すループ」と捉え、単一軌道ごとの安全策が反復をまたぐ攻撃に対して合成的に破綻することを示す論文。複数イテレーションに断片化された証拠を扱う攻撃、Agent-SafetyBench上の評価、非減衰のループ状態を維持する軽量防御を提示しています。
- なぜ面白いか:
  - 技術: ループの各周回を独立に検査するのではなく、外側の状態を持続させて「反復をまたぐ危険」を評価対象にする点が、エージェント安全性の設計単位を変えています。
  - 人文: ethicsの観点では、責任ある自律性は単発の「安全な応答」ではなく、時間をまたぐ記憶・証拠・意図の管理に宿ることを示します。historyの観点でも、産業オートメーションが事故後にログとインターロックを重視した流れとよく似ています。

### 2. How Warp builds self-improving agents on Claude
- 出典: Anthropic Claude Blog / Hacker News
- 日付: 2026-08-29（HN掲載）
- リンク: https://claude.com/blog/how-warp-builds-self-improving-agents-on-claude
- 要約: Warpが、ユーザーフィードバックを一過性の苦情で終わらせず、Claudeベースのエージェント改善ループへ変換する方法を紹介した記事。記事中では、リファレンスコーパス、ゴールデン出力、決定的評価、専門家フィードバック、time to mergeやコストのようなグローバル指標を改善エージェントへ戻す設計が語られています。
- なぜ面白いか:
  - 技術: プロンプト改善を職人芸から外し、検証ハーネスと評価データに基づく継続的改善ループとして運用している点が実務的です。
  - 人文: anthropologyの観点では、開発者の不満や違和感が組織の学習データへ翻訳される過程が見えます。narrativeの観点では、「賢いエージェント」ではなく「失敗を語り直して次の振る舞いに埋め込むチームメイト」としてAI像が変わります。

### 3. kstrl: evidence-closing software factory for AI coding agents
- 出典: GitHub repository
- 日付: 2026-08-31 updated
- リンク: https://github.com/0xfauzi/kstrl
- 要約: kstrlは、仕様を渡すとAIコーディングエージェントに文脈を与え、エージェント自身が書いていないチェックで成果物を測定し、ギャップを次の指示として戻し、独立した検証が合意した時だけ停止する「ソフトウェア工場」を掲げています。READMEは「You stay on the loop, not in it」と明示し、イベントログや人間の承認境界も強調しています。
- なぜ面白いか:
  - 技術: workerであるエージェントとjudgeである評価器を分離し、差分・テスト・別モデルレビュー・セキュリティレビューをループの停止条件にする構成が、Loop engineeringの核心をよく表しています。
  - 人文: philosophyの観点では、自己申告ではなく外部証拠で真偽を決めるという認識論がコード生成に持ち込まれています。ethicsの観点でも、人間は全手順の作業者ではなく、予算・マージ・例外の責任境界に立つ監督者として再配置されます。

### 4. mecha: local-agent harness with persistent security boundaries
- 出典: GitHub repository
- 日付: 2026-08-30 updated
- リンク: https://github.com/ljchang/mecha
- 要約: mechaは、ローカルのオープンウェイトモデルを個人アシスタント化するRust製ハーネスで、MCPツール、パス監獄、プロンプトインジェクション・インターロック、サンドボックスshell、スケジュール実行、トレース評価を組み合わせます。READMEは、私的データ・信頼できないコンテンツ・外部送信能力が同居する「lethal trifecta」を中心問題として据えています。
- なぜ面白いか:
  - 技術: 権限・記憶・ツール実行を単なるプロンプトの注意書きではなく、ハーネス側の境界条件とトレース評価で閉じる設計が優れています。
  - 人文: ethicsの観点では、便利な秘書を作るほど監視・同意・漏えいの問題が濃くなるというジレンマを正面から扱っています。anthropologyの観点では、個人のメール、予定、断り方といった生活文脈がエージェント設計の中心資源になることを示します。

### 5. Rysh CLI: graph/fleet-style agentic terminal multiplexer
- 出典: GitHub repository / Hacker News
- 日付: 2026-08-29（HN掲載、repositoryは2026-08-31時点で更新確認）
- リンク: https://github.com/rysh-ai/rysh-cli-code
- 要約: Rysh CLIは、タブ・ペイン・分割を持つ端末マルチプレクサを、各ペインがClaudeやCodexなどのエージェントとして振る舞える環境へ拡張するプロジェクトです。READMEでは、複数ベンダーのエージェントを並列に置く、ボード上でマネージャが作業を分解してワーカーへ修正を返す、fleetの形そのものを設計する、といったデモが紹介されています。
- なぜ面白いか:
  - 技術: 単一エージェントの反復だけでなく、複数エージェント間の作業分配・共有ボード・修正返却を「グラフ」として設計する方向が、loopからfleetへの拡張を示しています。
  - 人文: creativityの観点では、開発環境が単なる道具箱から、複数の作業者が舞台上で会話する制作空間へ変わっています。narrativeの観点では、人間は一人のAIに命令する語り手ではなく、群像劇の演出家に近い役割になります。

## arXiv / 学術
- Safety Does Not Compose: Non-Decaying Loop State for Autonomous LLM Agents — arXiv:2608.27141。自律LLMエージェントの反復をまたぐ安全状態の非合成性と、非減衰ループ状態による軽量防御を扱うため、今回のLoop engineering調査で最も直接的に関連します。

## メモ
- Boris Cherny優先の有無: Claude関連では優先的に確認しましたが、今回のLoop engineering単一トピックではBoris Cherny本人の直近該当投稿は実ツールでは確認できませんでした。
- 日本語アカウントの扱い: 日本語X検索を試みましたが、X検索ツールがクレジット上限で失敗したため、実投稿ベースの日本語アカウント確認は未完了です。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、代替としてHacker News Algolia、GitHub API、GitHub README、Anthropic公式ページ、arXivページへの直接HTTP取得を使いました。GitHub項目の日付は主にrepository update日であり、正式リリース日とは限りません。Addy Osmaniの「Loop Engineering」は2026-06-08で直近14日外ですが、用語と設計思想の基礎として重要なため調査文脈に反映しました（トップ5本体には直近の実装・研究を優先）。

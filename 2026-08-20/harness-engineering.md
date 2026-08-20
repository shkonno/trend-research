# Harness engineering トレンド調査 (2026-08-20)

- 調査日: 2026-08-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は、単なる「LLMを呼ぶ周辺コード」から、訓練・安全性・長期実行・人間の運用卓越性を左右する独立したシステム層として扱われ始めています。

## トップ5

### 1. Agent Lightning v1.0: Towards Harnessed Agentic RL
- 出典: arXiv
- 日付: 2026-08-18
- リンク: https://arxiv.org/abs/2608.17528
- 要約: Agent Lightning v1.0 は、デプロイ時のエージェント・ハーネス自体を強化学習の対象に取り込む「harnessed agentic RL」を整理した研究です。任意のエージェント・ハーネスに対応する約3,500行の軽量フレームワークとして、SWE-bench Verified で Qwen3.5-9B を 41.8% から 56.4% へ改善したと報告しています。
- なぜ面白いか:
  - 技術: ハーネスが環境ループを所有し、トレーナーがLLMリクエスト列を観測するという分離を明示したことで、retokenization、sample merging、advantage計算、loss正規化などの実務的な難所が研究対象として前面化しました。
  - 人文: これは「賢いモデル」だけでなく「賢さを働かせる制度設計」を鍛える発想で、組織における仕事の手順・監査・権限設計が知能の一部になることを示しています。人間の労働でも、能力は個人だけでなく道具・手順・職場文化に分散している、という見方に近いです。

### 2. LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents
- 出典: arXiv
- 日付: 2026-08-18
- リンク: https://arxiv.org/abs/2608.17393
- 要約: LEGO-RL は、既存のコーディングエージェント・ハーネスの内部制御フローを変更せず、ネイティブな実行環境を保ったまま方策勾配最適化につなぐ枠組みです。OpenHands SDK、Claude Code、OpenCode の3種のハーネスで Qwen3.5-35B-A3B を訓練し、SWE-bench Verified の改善を報告しています。
- なぜ面白いか:
  - 技術: in-process LLM proxying、サンドボックス・オーケストレーション、Live UI による軌跡診断を組み合わせ、ハーネス側の圧縮や再シリアライズをまたいでも訓練時のトークン整合性を保とうとしています。
  - 人文: Claude Code のような実運用ツールを研究室の単純化された環境に戻さず、その複雑さごと学習対象にする点が重要です。これは現場の「癖」や「段取り」を消すのではなく、そこに宿る暗黙知を尊重する方向のAI研究です。

### 3. HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety
- 出典: arXiv
- 日付: 2026-08-18
- リンク: https://arxiv.org/abs/2608.17597
- 要約: HarnessRisk は、エージェント・ハーネスの安全性を Harness Configuration、Capability Extension、Runtime Operation、State Persistence、Action Control、Incident Recovery の6段階で測るライフサイクル型ベンチマークです。128件のサンドボックス化ケースで、攻撃成功率が 12.6% から 80.9% まで大きく変動し、特に設定段階が脆弱だと報告しています。
- なぜ面白いか:
  - 技術: 安全性を単発のプロンプト注入ではなく、設定・拡張・永続状態・復旧まで含む運用ライフサイクルの問題として定義し直しています。
  - 人文: 「危険を認識している」ことと「安全に行動する」ことが一致しないという結果は、人間組織のコンプライアンス問題にも似ています。AIエージェントの倫理は、善意の宣言ではなく、失敗が起きる段階を丁寧に分解する制度設計として扱う必要があります。

### 4. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 出典: arXiv
- 日付: 2026-07-31公開、2026-08-10更新（直近14日より少し古いが、loop engineering との接点として重要）
- リンク: https://arxiv.org/abs/2608.00267
- 要約: LoopsBench は、コーディングエージェント評価の焦点が harness engineering から loop engineering へ移る、という問題設定を前面に出した長期実行ベンチマークです。112タスク、5,300以上の開発単位、依存DAG、段階的に解放されるテストを使い、Opus-4.7 + Claude Code + outer continuation の最良構成でも解決率25.00%と報告しています。
- なぜ面白いか:
  - 技術: 完了状態だけでなく、依存DAG、ready frontier、回帰義務、継続ループを評価対象に入れ、長期開発における「進め方」そのものを測っています。
  - 人文: これはAI開発を「一問一答の能力」から「時間をまたいで責任を持つ実践」へ移す動きです。仕事の価値が成果物だけでなく、途中の記憶、引き継ぎ、後戻り、修正の履歴に宿ることをよく表しています。

### 5. BossConsole: オープンソースのAIエージェント操作コンソール
- 出典: GitHub / Web
- 日付: 2026-07-21作成、2026-08-20更新・push確認
- リンク: https://github.com/risa-labs-inc/BossConsole
- 要約: BossConsole は、Claude Code、Codex、Gemini、OpenCode などを対象にした、JVMベースのマルチプラットフォームなAIエージェント用オペレーター・コンソールです。READMEでは、ブラウザ、ターミナル、エディタ、シークレット、100以上のMCPツールを与えつつ、各エージェントが何に触れてよいかを人間が制御できるハーネスとして説明されています。
- なぜ面白いか:
  - 技術: ElectronではなくJVM上のネイティブなマルチスレッド実装を掲げ、エージェントに実ブラウザ・端末・エディタ・権限境界を束ねて与える「運用UIとしてのハーネス」を作ろうとしています。
  - 人文: 研究論文側が訓練や安全ベンチを整備する一方で、BossConsole は人間が複数エージェントを監督する作業台を作っています。ここでは人間は単なる承認ボタンではなく、道具の配置、権限、観察の仕方を設計する「現場監督」として再登場しています。

## arXiv / 学術

- Agent Lightning v1.0: Towards Harnessed Agentic RL — 2608.17528。ハーネスを含むエージェントRLの実装・訓練課題を体系化。
- LEGO-RL: Harness-Native Reinforcement Learning for Coding Agents — 2608.17393。Claude Code を含む複数ハーネスでのネイティブRL訓練。
- HarnessRisk: A Lifecycle-Oriented Benchmark for Agent Harness Safety — 2608.17597。ハーネス安全性を6段階のライフサイクルで評価。
- ClawGym II: Exploring Black-Box RL on Agent Harness — 2608.16798。OpenClaw と Claude Code を含む黒箱ハーネス経由のRL最適化。
- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — 2608.00267。loop engineering への移行を明示する長期コーディング評価。
- OpenForgeRL: Train Harness-native Agents in Any Environment — 2607.21557。Claude Code、Codex、OpenClaw などの複雑な推論ハーネスをオープンなRL基盤に接続する枠組み（2026-07-23公開、2026-08-07更新）。

## メモ

- Boris Cherny優先の有無: Boris Cherny / @bcherny のX検索を優先して実行しましたが、X検索ツールは `personal-team-blocked:spending-limit` で失敗しました。そのため、本ファイルではBoris本人の直近投稿を確認済み情報としては扱っていません。
- 日本語アカウントの扱い: X検索が同じ理由で利用できなかったため、日本語Xコミュニティの投稿は未確認です。代替としてGitHub上で日本語READMEを含む `5throck/ai-workspace-standards`（https://github.com/5throck/ai-workspace-standards）など、Claude Code / Harness Engineering 周辺の公開リポジトリを確認しましたが、トップ5には研究的・運用的インパクトの高い項目を優先しました。
- 注意点・誇張リスク: Web検索ツールは Firecrawl 未設定で利用不可、DuckDuckGo HTML はボット判定でブロックされました。GitHub API、arXiv API、Hacker News Algolia API、直接README取得で補完しました。リンクは実際に取得・確認できたURLのみを記載しています。
- Claude Code / loop engineering との接点: LEGO-RL、ClawGym II、LoopsBench、OpenForgeRL、BossConsole が Claude Code または loop engineering と直接接続しています。特に LoopsBench は「harness engineering から loop engineering へ」という本日の中心的な橋渡しです。

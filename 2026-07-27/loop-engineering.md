# Loop engineering トレンド調査 (2026-07-27)

- 調査日: 2026-07-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
エージェントの「賢さ」そのものより、ループをどう訓練し、止め、観測し、人間へ戻すかが主戦場になっている。

## トップ5

### 1. OpenForgeRL: Train Harness-native Agents in Any Environment
- 出典: arXiv
- 日付: 2026-07-23
- リンク: https://arxiv.org/abs/2607.21557
- 要約: Claude Code や Codex のような実運用ハーネスをそのまま使い、状態を持つマルチターン・ツール利用エージェントをRL/SFT基盤へ接続するためのフレームワーク。ハーネスのモデル呼び出しをプロキシで記録し、Kubernetes上の隔離コンテナでロールアウトを回す設計が要点。
- なぜ面白いか:
  - 技術: 推論時だけの足場だったエージェントループを、訓練データ生成と強化学習の対象に変えるための具体的な配管を提示している。
  - 人文: anthropology の観点では、これは「現場の作業慣習」をモデルへ逆流させる制度設計であり、どの作業ログが未来の能力になるかという文化的選別の問題を含む。

### 2. NVIDIA-labs OO Agents: Native Python Object-Oriented Agents
- 出典: arXiv
- 日付: 2026-07-22
- リンク: https://arxiv.org/abs/2607.20709
- 要約: NVIDIA の NOOA は、エージェントを Python オブジェクトとして表現し、メソッドを行動、フィールドを状態、docstring をプロンプト、型注釈を契約として扱うモデル非依存フレームワーク。通常の Python コードと、実行時にLLMループで補完されるメソッドを同じインターフェイスへ置く。
- なぜ面白いか:
  - 技術: ワークフローグラフやツールスキーマの外側に散らばりがちなループ設計を、既存のOOP・型・テスト・リファクタリング文化へ接続している。
  - 人文: history の観点では、これはソフトウェア工学が長年蓄積した「保守可能性」の言語へエージェントを翻訳する試みで、AIを魔術的存在ではなく通常の工芸品として扱う方向に寄せる。

### 3. Operational Hallucination and Safety Drift in AI Agents
- 出典: arXiv
- 日付: 2026-07-20
- リンク: https://arxiv.org/abs/2607.18366
- 要約: ツール利用型自律エージェントで、長い実行のあいだに初期の安全意図が崩れる Safety Drift と、状態認識の失敗により反復的なツール呼び出しが続く Operational Hallucination を実証的に扱う論文。単発応答の安全性では見えにくい、宣言と行動の乖離やライブロックを測る。
- なぜ面白いか:
  - 技術: ループ回数・状態遷移・ツール呼び出し列を安全評価の単位にし、停止条件や監視メトリクスが設計対象であることを明確にしている。
  - 人文: ethics の観点では、「最初は安全と言った」ことではなく、時間の中で行為がどう変質するかを問うため、責任を発話ではなくプロセスへ置き直す。

### 4. Understanding Agent-Reactive Bugs at the Model-Harness Boundary
- 出典: arXiv
- 日付: 2026-07-17
- リンク: https://arxiv.org/abs/2607.15684
- 要約: Codex、Gemini-CLI、LangChain、CrewAI の255件のバグ報告を分析し、モデル出力とハーネス反応の境界でだけ発生する agent-reactive bugs を分類する研究。失敗原因を「モデルが弱い」か「ハーネス実装が悪い」かに分けるだけでは説明できない相互作用を扱う。
- なぜ面白いか:
  - 技術: エージェントループの不具合を、出力パース、コンテキスト管理、制御フロー、モデル反応の結合問題としてデバッグする語彙を与えている。
  - 人文: philosophy の観点では、行為者性を単体モデルへ帰属するのではなく、モデル・ハーネス・環境の関係から生じるものとして見る点が重要。

### 5. Intutic — The Circuit Breaker for AI Agents
- 出典: GitHub / Web
- 日付: 2026-07-23 作成、2026-07-26 更新
- リンク: https://github.com/intutic/intutic
- 要約: Claude Code、Cursor、LangGraph、n8n などに向けたオープンソースの「AIエージェント用サーキットブレーカー」。リアルタイムのセキュリティ、秘密情報DLP、loop burn prevention を掲げ、事後ログ型の観測だけでなく実行中に止める設計を前面に出している。
- なぜ面白いか:
  - 技術: ループの暴走や無駄な反復を、観測可能性だけでなく介入可能性の問題として扱い、エージェント実行にブレーカーを挟む実装方向を示している。
  - 人文: narrative の観点では、自律エージェントを「英雄的に任せる機械」ではなく、危険時に止まる社会的インフラとして語り直している。ethics 的にも、止める権利と監査可能性を設計に埋め込む点が実務的に大きい。

## arXiv / 学術
- OpenForgeRL: Train Harness-native Agents in Any Environment — 2607.21557。ハーネスネイティブなエージェント訓練基盤。
- NVIDIA-labs OO Agents: Native Python Object-Oriented Agents — 2607.20709。Python OOPとしてエージェントループを設計する提案。
- Operational Hallucination and Safety Drift in AI Agents — 2607.18366。長期実行中の安全ドリフトとライブロック評価。
- Understanding Agent-Reactive Bugs at the Model-Harness Boundary — 2607.15684。モデルとハーネス境界の相互作用バグ分類。
- Recursive Harness Self-Improvement — 2607.15524。プロンプトレベルのエージェントループ仕様を、自己履歴へのペアワイズフィードバックで改善する研究。
- Retriever: Composing Closed-Loop Asynchronous Robot Programs — 2607.17213。ロボット向け閉ループ非同期プログラムの構成モデル。
- The Boundaries of Automation: A Theory of Persistent Human Participation — 2607.21547。自動化の限界と、人間がループに残る理由を理論化。

## メモ
- Boris Cherny優先の有無: Loop engineering単独ではClaude固有トピックではないため、Boris Cherny優先は適用外。
- 日本語アカウントの扱い: 日本語X検索も実行したが、X検索ツールがクレジット不足で失敗したため取得できず。Web検索ツールもFirecrawl未設定で失敗したため、代替として terminal 経由で arXiv API、GitHub API、検索エンジンへの直接HTTPアクセスを実行した。
- 注意点・誇張リスク: Web一般検索は検索エンジン側のノイズが大きく、Xの一次投稿は確認不能だった。リンクは arXiv API と GitHub API/README で実在確認できたものに限定した。

# Philosophy of Loop Engineering トレンド調査 (2026-08-21)

- 調査日: 2026-08-21
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
ループエンジニアリングは、単なる「何度も回す自動化」から、証拠・観察・権限・記憶によって行為の正当性を閉じるための実践哲学へ移りつつあります。

## トップ5

### 1. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 出典: arXiv / GitHub
- 日付: 2026-07-31（v2更新: 2026-08-10）
- リンク: https://arxiv.org/abs/2608.00267 / https://github.com/microsoft/Loopsbench
- 要約: Microsoft系の著者らによる、長期実行型コーディングエージェント評価のためのベンチマーク。112タスク、5,300超の開発単位、依存DAG、回帰義務を持つテスト解放方式で、単発タスクの成功率では見えない「ループの持続性」を測る。
- なぜ面白いか:
  - 技術: 評価対象を最終成果物から、依存関係・回帰・未完了ノードを含む実行過程そのものへ移している。
  - 人文: これは認識論的には「正しい答え」より「どの順序で、何を根拠に、何を忘れずに進んだか」を問う設計であり、実践知をプロセスの履歴として扱う発想に近い。サイバネティクス的にも、完成ではなくフィードバックを受け続ける系としてエージェントを見る転換点です。

### 2. TRACE: TRajectory Attribution for Automated Context Engineering
- 出典: arXiv
- 日付: 2026-08-10
- リンク: https://arxiv.org/abs/2608.09153
- 要約: 本番AIエージェントの失敗を、プロンプト、知識ベース、ツール説明、手続き的スキルなどの「文脈源」に帰属するための自動フィードバックループ。ユーザーの訂正、言い換え、離脱などの暗黙シグナルを軌跡から掘り起こし、文脈の作成・更新を判断する。
- なぜ面白いか:
  - 技術: 実行ログを単なる監査記録ではなく、文脈層を改善するための因果的な診断資源として使っている。
  - 人文: 失敗を個々のモデル能力に還元せず、環境・記憶・道具・言葉の配置として読む点が、拡張された認識論に近い。経験から「何を知っていることにするか」を更新する、職人的な反省の自動化としても読めます。

### 3. The CASE Framework: A Multi-Disciplinary Control Architecture for Governing Enterprise Agentic AI
- 出典: arXiv
- 日付: 2026-08-10
- リンク: https://arxiv.org/abs/2608.10153
- 要約: エンタープライズのエージェント統治を、単一のDevSecOps問題ではなく、制御理論、複雑適応系、監督サイバネティクス、運用工学の4層問題として整理する論文。人間による監督が「儀礼」にならないためには、必要多様性の法則を満たす構造がいると主張する。
- なぜ面白いか:
  - 技術: 個別エージェント、エージェント集合、人間・エージェントチーム、運用フリートを別々の制御問題として分解している。
  - 人文: ループの哲学における重要点は、誰が観察し、誰が介入でき、どのレベルの変化を統治できるのかという権力配置です。この論文は「人間が見ているから安心」という物語を疑い、監督能力そのものを設計対象に戻している。

### 4. Independent Patch Verification for Coding Agents with a Bidirectional Reconstruct-and-Verify Framework
- 出典: arXiv
- 日付: 2026-08-09
- リンク: https://arxiv.org/abs/2608.08950
- 要約: コーディングエージェントが生成したパッチについて、同じ解釈で自己反省するのではなく、前向き・後ろ向きの再構成で独立した検証信号を作るRETRACEを提案。SWE-bench VerifiedでPass@1を改善したと報告している。
- なぜ面白いか:
  - 技術: パッチから逆に「この変更はどの問題を解いたように見えるか」を復元し、元の課題との整合で提出可否や修正指針を出す。
  - 人文: これは実践知における「自分の説明を自分で信じすぎない」ための制度設計です。ループを強くするとは反復回数を増やすことではなく、別視点からの再記述を通じて、行為と理由の一致を問い直すことだと示している。

### 5. Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control
- 出典: arXiv（14日より古いが、loop engineeringを明示する基礎的論点として採用）
- 日付: 2026-07-16
- リンク: https://arxiv.org/abs/2607.14890
- 要約: コーディングエージェントの「DONE」「tested」「ready-to-merge」といった状態宣言を、そのままライフサイクル状態として扱わず、最新で機械検証可能な証拠がゲートを満たす場合だけ遷移を許す手法。エージェント出力を「主張」として扱い、証拠に基づく停止条件を導入する。
- なぜ面白いか:
  - 技術: ライフサイクル遷移を、主観的な完了宣言ではなく、ソース状態に紐づく証拠バンドルとゲートで制御している。
  - 人文: これは「信頼」を人格やモデル名ではなく、検証可能な証跡に移す哲学です。近代的な実験科学における再現性、あるいは職人仕事における検品の文化を、AIエージェントのループに埋め込む試みとして読めます。

## arXiv / 学術
- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — arXiv:2608.00267。長期実行・依存DAG・回帰義務を含む評価で、loop engineeringを直接主題化。
- TRACE: TRajectory Attribution for Automated Context Engineering — arXiv:2608.09153。実行軌跡から文脈失敗を帰属し、改善ループを回す。
- The CASE Framework: A Multi-Disciplinary Control Architecture for Governing Enterprise Agentic AI — arXiv:2608.10153。制御理論・複雑適応系・監督サイバネティクス・運用工学を統合。
- Independent Patch Verification for Coding Agents with a Bidirectional Reconstruct-and-Verify Framework — arXiv:2608.08950。独立検証を通じたパッチ妥当性のループ。
- Proof-or-Stop: Don't Trust the Agent, Trust the Evidence — arXiv:2607.14890。証拠ゲートによるライフサイクル制御。

## メモ
- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: X検索は英語・日本語の両方で実行したが、X検索ツールがクレジット上限で失敗したため、ポスト内容は採用していない。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、Web側はGitHub APIとraw READMEの直接取得で補完した。トップ5はarXiv APIで確認できた実在リンクに限定し、架空リンクや未確認IDは含めていない。直近14日を優先しつつ、Proof-or-Stopのみ14日より古いが、loop engineeringを明示するため「古いが重要」として採用した。

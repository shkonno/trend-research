# Loop engineering トレンド調査 (2026-08-22)

- 調査日: 2026-08-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Loop engineering は「エージェントを走らせる」段階から、「証拠・評価・巻き戻し・権限を組み込んだ反復システムを設計する」段階へ移っている。

## トップ5

### 1. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 出典: arXiv / GitHub（microsoft/Loopsbench）
- 日付: 2026-07-31公開、2026-08-10更新（直近14日内に更新）
- リンク: https://arxiv.org/abs/2608.00267 / https://github.com/microsoft/Loopsbench
- 要約: 長期ソフトウェア開発における coding agent を、単発のハーネスではなく依存DAG・段階的テスト解放・回帰義務を含む「ループ」として評価するベンチマーク。112タスク、8言語、9ドメインを含み、最強構成でも解決率25.00%に留まると報告している。
- なぜ面白いか:
  - 技術: 評価対象を最終成果物だけでなく、計画、依存関係、ready frontier、回帰イベントまで拡張しており、エージェント運用ループの失敗箇所を測れる。
  - 人文: これは「仕事を完了した」という物語を、成果物ではなく過程の証拠で読み直す試みであり、労働史における工程管理の再発明に近い。人間のプロジェクト管理で暗黙化されていた依存や手戻りが、機械のふるまいを通じて可視化される点が面白い。

### 2. LoopVSR: A Loop Engineering Framework for Automated Repair of Visual Speech Recognition Inference Pipelines
- 出典: arXiv / GitHub（luopeng69131/LoopVSR）
- 日付: 2026-08-12
- リンク: https://arxiv.org/abs/2608.13610 / https://github.com/luopeng69131/LoopVSR
- 要約: 視覚音声認識（VSR）の推論パイプラインを、コードエージェント、パッチ監査、実行評価、受理またはロールバックの反復ループで自動修復する枠組み。CMLR VSRシステムで主要11故障をすべて修復し、静的ガードより大きく改善したと報告している。
- なぜ面白いか:
  - 技術: 例外、テンソル統計、認識誤り、文字誤り率（CER）をループのフィードバックとして使い、上流障害に隠れた下流障害を段階的に露出させる。
  - 人文: 「読唇」という身体的・社会的コミュニケーションを扱うため、単なるCI修復よりも障害者支援、プライバシー、身体の機械的読解という倫理問題に接続する。創造性の面でも、エージェントが一度に正解を書くのではなく、証拠に応じて修理の物語を進める点が新しい。

### 3. Proof-or-Stop: Don’t Trust the Agent, Trust the Evidence — Loop Engineering for Verifiable Evidence-Gated Lifecycle Control
- 出典: arXiv
- 日付: 2026-07-16（古いが、loop engineering の中核概念として継続的に重要）
- リンク: https://arxiv.org/abs/2607.14890
- 要約: 自律 coding agent の「reviewed」「tested」「DONE」「ready-to-merge」といったライフサイクル状態を、エージェントの主張ではなく機械的に検証できる最新証拠でゲートする手法。自己適用コーパスとアブレーションで、false-DONE抑制や改ざん拒否を評価している。
- なぜ面白いか:
  - 技術: ループの各状態遷移を、ソース状態に束縛された検証可能証拠に結び付け、証拠がなければ停止する制御層として定式化している。
  - 人文: 倫理的には「信頼」を人格やブランドではなく証拠手続きへ移す設計で、AIエージェントを職能者としてではなく監査可能な制度参加者として扱う。哲学的には、真理そのものではなく、ある信頼モデル下で何を十分な証拠と呼ぶかを問う点が重要だ。

### 4. NVIDIA-labs OO Agents: Native Python Object-Oriented Agents
- 出典: arXiv
- 日付: 2026-07-22（古いが、プログラマブルな agent loop 設計として重要）
- リンク: https://arxiv.org/abs/2607.20709
- 要約: エージェントを Python オブジェクトとして表現し、メソッドを行動、フィールドを状態、docstringをプロンプト、型注釈を契約として使う NOOA フレームワーク。通常の決定的コードと LLM 駆動のメソッドを同じインターフェースで扱い、テスト・追跡・リファクタリング可能にする。
- なぜ面白いか:
  - 技術: typed I/O、live object の参照渡し、code as action、明示的状態、モデル呼び出し可能な harness API を同一の Pythonic 表面に統合している。
  - 人文: narrative の観点では、エージェントの行為がプロンプトの会話ログではなく、オブジェクトの状態変化として読めるようになる。これはソフトウェア工学の歴史におけるオブジェクト指向の発想を、非決定的なAI行為の説明責任へ再利用する動きとして興味深い。

### 5. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans
- 出典: arXiv
- 日付: 2026-07-12（古いが、human-agent loop engineering の概念整理として重要）
- リンク: https://arxiv.org/abs/2607.10878
- 要約: エージェントチームがツール、記憶、スキル、役割、ワークフローを進化させる際、それらを版管理された agent pack と監査可能なイベントトレースにまとめ、証拠・ポリシー・明示的承認があるまで未信頼のリリース候補として扱う設計。人間が目的、権限、承認、不可逆操作を制御しながら継続運用できる「verifiable human-agent loop engineering」を掲げる。
- なぜ面白いか:
  - 技術: マルチモーダル入力を agent pack にコンパイルし、実行トレースと fail-closed 検証で、学習したプロンプトやツールの昇格を制御する。
  - 人文: 人類学的には、エージェントチームを単なる道具ではなく、組織文化を持ちうる共同体として扱う設計に見える。倫理的には、機械速度で変化する制度に対して、人間の承認権をどこに埋め込むかという統治問題を前面に出している。

## arXiv / 学術

- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — arXiv:2608.00267。長期 coding agent 評価を loop engineering として定式化。
- LoopVSR: A Loop Engineering Framework for Automated Repair of Visual Speech Recognition Inference Pipelines — arXiv:2608.13610。VSR推論パイプライン修復への具体適用。
- Proof-or-Stop: Don’t Trust the Agent, Trust the Evidence — arXiv:2607.14890。証拠ゲート型ライフサイクル制御。
- NVIDIA-labs OO Agents: Native Python Object-Oriented Agents — arXiv:2607.20709。Pythonオブジェクトとしての agent loop 設計。
- LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans — arXiv:2607.10878。human-agent loop engineering とガバナンス。
- 参考として、2026-08-20公開の AI4AI-Bench（arXiv:2608.20318）、MidTool（arXiv:2608.20314）、Brain Researcher（arXiv:2608.19902）、LLMテスト生成のフィードバック進化監査（arXiv:2608.19626）も、反復・評価・証拠化という近接テーマを示していた。

## メモ

- Boris Cherny優先: 本トピックは Claude 固有ではないため、Boris Cherny 優先条件は該当なし。
- 日本語アカウントの扱い: X検索は英語・日本語クエリで実行したが、x_search がクレジット制限で失敗したため、具体的なX投稿は採用していない。
- Web検索の扱い: web_search / web_extract は Firecrawl 未設定で失敗した。代替として、arXiv API、GitHub API、GitHub raw README、公式サイトへの直接HTTP取得を使用した。
- 注意点・誇張リスク: LoopsBench と LoopVSR は GitHub 上で確認できたが、他の項目は主に arXiv API に基づく。直近14日を優先したが、Proof-or-Stop、NOOA、LOGOS は14日より古いため明記した。

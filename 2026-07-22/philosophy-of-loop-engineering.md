# Philosophy of Loop Engineering トレンド調査 (2026-07-22)

- 調査日: 2026-07-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「ループエンジニアリング」は、AIエージェントを信じる技術ではなく、反復・証拠・停止条件によって信頼を少しずつ制度化する実践知として輪郭を強めています。

## トップ5

### 1. Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control
- 出典: arXiv
- 日付: 2026-07-16
- リンク: http://arxiv.org/abs/2607.14890v1
- 要約: 自律コーディングエージェントの「reviewed」「tested」「DONE」などのライフサイクル状態を、エージェントの自己申告ではなく、現在のソース状態に紐づいた機械検証可能な証拠でゲートする方法を提案。未監視ループエンジンのシナリオ試験、改ざん耐性のあるローカルキー付き receipt bundle、アブレーション評価で false-DONE 抑制を検証しています。
- なぜ面白いか:
  - 技術: verify-repair や agent harness の外側に、状態遷移を許可するための証拠ゲートと停止規則を置くことで、ループを「作業の自動化」から「ライフサイクル制御」へ拡張しています。
  - 人文: ここでの「proof」は意味論的な絶対真理ではなく、特定の信頼モデル内で行為を許可するための実践的な証拠です。これは、知識を内面の確信ではなく、共同体が扱える手続き・記録・責任の束として見るプラグマティズム的な認識論に近い読みができます。

### 2. Verify, Repair, Repeat, or Stop? Robust Stopping for Noisy Verify-Repair Loops in LLM Agents
- 出典: arXiv
- 日付: 2026-07-20
- リンク: http://arxiv.org/abs/2607.17641v1
- 要約: LLMエージェントで一般的な verify-repair-repeat ループでは、検証器も修復器もノイズを持つため、修復を続けるほど真の妥当性が下がる場合があります。本論文は、誤受理・誤拒否・修復・破壊の4パラメータを分けたノイズモデルと belief filtering により、いつ修復を続け、いつ止めるべきかを決める VRR-Stop を提案しています。
- なぜ面白いか:
  - 技術: 「もう一回直す」は常に改善ではないという前提から、反復の価値を限界効用として推定し、停止をエンジニアリング対象にしています。
  - 人文: ループの哲学で重要なのは、反復そのものを善としない点です。これはサイバネティクスのフィードバック思想に、判断停止・過剰介入・可謬性という認識論的な慎みを入れる仕事として読めます。

### 3. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans
- 出典: arXiv
- 日付: 2026-07-12
- リンク: http://arxiv.org/abs/2607.10878v1
- 要約: ツール利用・委任・経験学習・自己変更を行うAIエージェントチームに対して、エージェント、ツール、知識、テスト、権限、ポリシーを versioned agent packs として管理し、活動を監査可能な event traces に変換する governance layer を提案。学習されたプロンプト、記憶、スキル、役割、ワークフローを、証拠と人間管理ポリシーを通るまでは untrusted release candidate として扱います。
- なぜ面白いか:
  - 技術: ループによる自己進化を、フレームワーク非依存の trace・policy・fail-closed verification で囲い込み、agent team の変更管理として定式化しています。
  - 人文: 問いは「エージェントに何ができるか」から「何になることを誰が許すのか」へ移ります。これは技術的なCI/CDの話であると同時に、制度設計・権限・共同体の自己統治をめぐる政治哲学の問題でもあります。

### 4. MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research
- 出典: arXiv
- 日付: 2026-07-16
- リンク: http://arxiv.org/abs/2607.14582v1
- 要約: 既存のLLM定理証明が自律的に命題を証明する方向に寄りがちなことに対し、数学者が高水準の方向付けを行い、AIエージェントが形式化・証明作業を継続的な人間のガイダンスの下で進める human-in-the-loop システムを提案。living proof blueprint によって、証明を人間が点検・指示・改訂できるナビゲーブルなステップへ分解します。
- なぜ面白いか:
  - 技術: proof blueprint を共有作業空間にすることで、人間の直観的な問題設定とエージェントの形式化・探索ループを接続しています。
  - 人文: これは「自律AIが数学者を置き換える」物語ではなく、実践知を持つ人間が問いの方向や意味を保持し、機械が反復と検証を担う共生モデルです。ポランニー的な暗黙知と形式証明のあいだに、操作可能なインターフェースを置く試みとして面白いです。

### 5. Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting
- 出典: arXiv（直近14日より少し古いが、対象トピックに直接関連）
- 日付: 2026-06-28
- リンク: http://arxiv.org/abs/2607.00038v1
- 要約: 「エージェントを逐次プロンプトするのではなく、エージェントをプロンプトするループを設計せよ」という実務上のスローガンを、trigger、goal、verification step、stopping rule、memory からなる loop specification として整理。通常のプログラムループや harness 内部の perceive-act-observe cycle と区別し、prompt engineering が消えるのではなく、loop と prompt が別の道具になると論じています。
- なぜ面白いか:
  - 技術: loop specification を再利用可能な成果物として切り出すことで、属人的な逐次指示を、検証・停止・記憶を含む運用単位へ変えています。
  - 人文: この論文は、エンジニアリングを「命令文を書くこと」から「習慣・環境・反省の型を設計すること」へずらします。デューイ的な反省的実践、サイバネティクス的な制御、職人の実践知が、AIエージェント時代の作法として再接続されている点が重要です。

## arXiv / 学術

- `2607.14890v1` Proof-or-Stop: Don't Trust the Agent, Trust the Evidence -- Loop Engineering for Verifiable Evidence-Gated Lifecycle Control: 証拠ゲート付きライフサイクル制御としてのループ工学。
- `2607.17641v1` Verify, Repair, Repeat, or Stop?: noisy な検証・修復ループで停止条件を理論化。
- `2607.10878v1` LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans: 進化するエージェントチームの統治レイヤー。
- `2607.14582v1` MathCoPilot: 人間とAIの共生的な数学研究ループ。
- `2607.00038v1` Stop Hand-Holding Your Coding Agent: loop specification を実務概念として整理。

## メモ

- X検索: 英語・日本語クエリで実行しましたが、X検索ツールは `personal-team-blocked:spending-limit` により結果取得できませんでした。
- Web検索: Hermes の `web_search` は Firecrawl 未設定で失敗しました。代替として terminal から Bing/Google/DuckDuckGo および arXiv API を試行しましたが、一般Web検索はノイズやブロックが多く、採用した上位5件は実在確認できた arXiv 項目を中心にしました。
- Boris Cherny優先: Claude固有トピックではないため、今回は優先対象外です。
- 日本語アカウントの扱い: 日本語X検索は実行したものの、ツール側クレジット制限により投稿は確認できませんでした。
- 注意点・誇張リスク: `Loop engineering` はまだ新しい実務語彙で、論文タイトルや要旨上の用法にもばらつきがあります。本稿では、反復、検証、停止、記憶、証拠、統治という共通構造で読めるものを「Philosophy of Loop Engineering」として選定しました。

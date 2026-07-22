# Loop engineering トレンド調査 (2026-07-22)

- 調査日: 2026-07-22
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Loop engineering は「賢いモデルを呼ぶ」段階から、モデルの周囲にある検証・記録・フィードバック・承認のループを設計し直す段階へ移っている。

## トップ5

### 1. Training Agent Harnesses Like Model Weights / Harness Training
- 出典: ブログ / GitHub / Hacker News
- 日付: 2026-07-18（ブログ）、2026-07-21（HN掲載）
- リンク: https://www.henrypan.com/blog/2026-07-18-harness-training
- 要約: LLM本体は固定したまま、プロンプト、コンテキスト管理、ツール、修復ループなどを含む「harness」を PyTorch 風に訓練する試み。Git のコミット履歴を候補の昇格・棄却ログとして使い、決定論的な実験条件で候補 harness を比較する点が強い。
- なぜ面白いか:
  - 技術: モデル重みではなく agent loop の外側を最適化対象にすることで、再現性・評価・改善履歴を同じフレームで扱える。
  - 人文: philosophy の観点では「知能」を個体の能力ではなく制度化された実践の配置として捉え直している。history 的にも、職人技だった運用ノウハウが測定可能な工学対象へ移る瞬間に見える。

### 2. Structured Feedback Improves Repair in an LLM Agent Loop
- 出典: arXiv
- 日付: 2026-07-15
- リンク: http://arxiv.org/abs/2607.14167v1
- 要約: VeriHarness というコード制御の agent loop で、外部バリデータの失敗情報を次のモデル呼び出しへどう返すかを比較。失敗位置・観測値・許容代替案を含む構造化フィードバックにより、TextWorld タスクの成功率が大きく改善した。
- なぜ面白いか:
  - 技術: 「リトライさせる」だけでなく、検証結果をどの粒度で返すかが loop の性能を決めることを実験で示している。
  - 人文: anthropology の観点では、AIとの協働は命令ではなく「添削の形式」をめぐる文化であることが見える。ethics 的にも、失敗理由を明示するループは責任の所在を追跡しやすくする。

### 3. Kitaru: Every agent run, recorded and replayable
- 出典: GitHub / Hacker News
- 日付: 2026-07-06（HN掲載、直近14日より少し古いが関連性が高いため掲載）
- リンク: https://github.com/zenml-io/kitaru
- 要約: 自律エージェントの各ステップ、モデル呼び出し、ツール呼び出し、判断をチェックポイントとして記録し、再生・再実行・別モデルでの比較を可能にする self-hosted runtime。README は agent stack を Model / Harness / Runtime / Platform に分け、Kitaru を「記録・再生・改善」の層として位置づけている。
- なぜ面白いか:
  - 技術: ループの各状態を再生可能にすることで、失敗解析やモデル差し替え評価を属人的なログ読みから実験可能な運用へ移せる。
  - 人文: history 的には、工場の工程記録や実験ノートが品質管理を生んだ流れの agent 版に近い。narrative の観点では、エージェントの行為を後から語れる「履歴」として残すことが信頼の条件になる。

### 4. FizzBee: AI Requirements Engineer between your idea and your coding agent
- 出典: Web / Hacker News
- 日付: 2026-07-08（HN掲載）
- リンク: https://fizzbee.ai/
- 要約: アイデアと coding agent の間に要求工学レイヤーを置き、曖昧な仕様、矛盾、未決定事項を formal verification とシナリオ確認で洗い出すサービス。エージェントに渡す前に「何を作るべきか」を精密化する前段ループとして読める。
- なぜ面白いか:
  - 技術: 生成・実装の前に仕様検証ループを置くことで、後工程の agent loop が勝手に仮定を埋めるリスクを下げる。
  - 人文: ethics の観点では、曖昧な要求をAIに丸投げすることの責任逃れを防ぐ設計である。creativity 的には、自由な発想と厳密な仕様の対立ではなく、両者を往復させる創作プロセスを提示している。

### 5. Pinpoint: Visual feedback for AI coding agents
- 出典: GitHub / Web / Hacker News
- 日付: 2026-07-21（HN掲載）
- リンク: https://github.com/maferland/pinpoint
- 要約: スクリーンショットやモックにピンとコメントを置き、構造化JSONとしてAI coding agent に戻す視覚フィードバックツール。Claude Code plugin とCLIに対応し、UIレビューを会話テキストだけでなく画像上の位置情報としてループへ戻せる。
- なぜ面白いか:
  - 技術: 人間の視覚的な指摘を座標・範囲・コメントとして agent loop に接続し、UI修正の曖昧さを減らす。
  - 人文: anthropology の観点では、デザイナーやPMの「ここが違う」という身振りをデジタルな共同作業の記法に変換している。creativity 的にも、レビューを中断ではなく制作ループの素材にする点がよい。

## arXiv / 学術

- Structured Feedback Improves Repair in an LLM Agent Loop — arXiv:2607.14167v1。検証から再試行へのフィードバック形式が agent loop の修復性能を左右することを示す。
- Understanding Agent-Reactive Bugs at the Model-Harness Boundary — arXiv:2607.15684v1。Codex、Gemini-CLI、LangChain、CrewAI等の issue から、モデル応答と harness の相互作用でだけ発生するバグを分類。
- Real-World Evaluation of an AI Agent Drafting Translational Impact Summaries — arXiv:2607.16989v1。人間レビュー付きAIエージェントが研究インパクト要約を作る実運用評価。
- MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research — arXiv:2607.14582v1。数学者が高レベル方針を操り、AIが形式化・証明作業を進める human-in-the-loop 研究環境。
- Confining Nondeterminism: AI-Driven Research Systems as DBMSs for Reliable, Non-Wasteful, Transparent, and Collaborative Research [Vision] — arXiv:2607.10508v1。研究エージェントの非決定性を、DBMS的な決定論的データフローへ閉じ込める構想。

## メモ

- Boris Cherny優先の有無: 本トピックは Claude 固有ではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索を実施したが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため取得できなかった。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で失敗したため、代替として Hacker News Algolia、GitHub raw README、対象サイトの直接HTTP取得、arXiv APIを使用した。X由来の反応量は確認できていないため、順位は「実装としての面白さ」と loop engineering への近さを重視した。

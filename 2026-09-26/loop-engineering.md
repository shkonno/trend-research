# Loop engineering トレンド調査 (2026-09-26)

- 調査日: 2026-09-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「エージェントを回す」段階から、環境・ハーネス・記憶・検証器までを含む閉ループ全体をどう設計し、暴走や過学習を抑えながら改善するか、というシステム工学の話に移っている。

## トップ5

### 1. RRSI: Regularized Recursive Self-Improvement of Agent Harnesses
- 出典: arXiv / Web（プロジェクトページ・GitHub確認）
- 日付: 2026-09-21（v2: 2026-09-23）
- リンク: https://arxiv.org/abs/2609.24972
- 要約: LLMエージェントの性能を、モデル本体ではなくプロンプト、制御フロー、ツール、メモリ、コンテキスト管理から成る「ハーネス」の反復改善として扱う研究。単純な自己改善は訓練タスクへ過学習しやすいため、編集候補の予算を徐々に絞る、探索履歴を使う、critic/prunerで汎用性の低い変更を落とす、といった正則化で再利用可能な改善を狙う。
- なぜ面白いか:
  - 技術: ループ改善を「何でも自己改造」ではなく、候補生成・選択・剪定を持つ正則化問題として定式化しており、ハーネス進化の評価軸を実装可能な形にしている。
  - 人文: philosophy / ethics の観点では、自己改善する機械に「制限」と「忘却」を組み込むことが能力向上の条件になる点が面白い。進歩を無限拡張ではなく、共同体が許容できる規律ある変化として捉え直している。

### 2. Harness as a Language: A Minimalist Agent Framework With Maximal Expressivity
- 出典: arXiv
- 日付: 2026-09-22
- リンク: https://arxiv.org/abs/2609.26891
- 要約: JAZ というミニマルなエージェントフレームワークを提案し、LLMにコードを書かせ、再帰的に `invoke` できる単一プリミティブだけで、メモリや自己改善のような専用ハーネス機能をどこまで表現できるかを検証している。論文は agent loop をプログラミング言語の関数呼び出しのように扱い、ハーネスを「外付け部品」ではなく言語設計として見直す。
- なぜ面白いか:
  - 技術: ツール、履歴、入力をすべてコード環境内の変数として扱うことで、ループ制御・再帰・監視を小さな抽象にまとめる設計思想が明快である。
  - 人文: history / creativity の観点では、これは初期LispやUnix的な「小さなプリミティブから複雑な文化を作る」発想のAI版に見える。エージェント開発がライブラリ競争から、どんな言語で行為を記述するかという表現文化の競争へ移っている。

### 3. Exact Feedback Is Not Control: Evaluating Text-based Closed-Loop Revision in LLMs
- 出典: arXiv / Web（GitHub再現コード確認）
- 日付: 2026-09-23
- リンク: https://arxiv.org/abs/2609.28150
- 要約: 完全で正確なフィードバックを与えても、LLMの閉ループ修正が必ず信頼できる制御になるわけではないことを示す評価研究。決定的な検証器で残り違反をすべて報告する固定予算プロトコルを使い、19モデルで最終成功率が大きく分かれ、同じフィードバックでも過去出力の反復から抜け出せない失敗が観察された。
- なぜ面白いか:
  - 技術: 「良い verifier を置けば loop は制御できる」という素朴な期待を分解し、フィードバックの正確性とモデル側の修正能力を切り分けて測っている。
  - 人文: philosophy / narrative の観点では、人間の対話でも正しい指摘が相手の変化を保証しないように、フィードバックは命令ではなく解釈される出来事である。AIとの協働も、訂正を渡すだけでなく、反復の物語からどう脱出させるかが設計課題になる。

### 4. Breaking the Environment Wall: Evolving LLM Agent Environments for Recursive Self-Improvement
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.29773
- 要約: 現実のオフィス作業や科学実験のような環境は、情報が散らばり、誤情報やバージョン差分が混じり、時間とともに変化するため、エージェントにとって「agent-ready」ではないと指摘する研究。Env-Rethink は Collection Maps や Event Logs を作って文脈を補い、さらに環境そのものを難化・進化させてエージェント改善に使う。
- なぜ面白いか:
  - 技術: ループの改善対象をモデルやプロンプトだけでなく、タスク環境の情報配置・履歴・ノイズ構造にまで広げている点が重要である。
  - 人文: anthropology / history の観点では、人間の仕事も道具だけでなく、書類棚、ログ、慣習、組織記憶によって成り立ってきた。AIエージェントの能力は個体の知能より、どんな環境を作り込むかという制度設計に依存することを示している。

### 5. When Can Agents Forget Their Reasoning? ICLR for Long-Horizon Agent Context Compression
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.29875
- 要約: 長期タスクのエージェントでは推論履歴が膨らみ続け、コストと文脈長が増える一方、単純に削除すると以後の行動軌道が変わる。ICLR（Interaction Aware Compression for Long Horizon Reasoning）は、行動・ツール呼び出し・観測を残しつつ、推論ブロックをオンラインで圧縮し、WorkBuddyBenchで報酬改善とトークン削減を同時に示した。
- なぜ面白いか:
  - 技術: 「どの推論を忘れてよいか」を、履歴の静的圧縮ではなく、以後の相互作用を変える動的状態管理として扱っている。
  - 人文: philosophy / narrative の観点では、記憶とは全ログ保存ではなく、次の行為に必要な意味を外部化し、物語を編集する営みである。エージェントの忘却設計は、効率化であると同時に、責任追跡や説明可能性との緊張を生む。

## arXiv / 学術
- RRSI: Regularized Recursive Self-Improvement of Agent Harnesses — arXiv:2609.24972（2026-09-21 / v2 2026-09-23）
- Harness as a Language: A Minimalist Agent Framework With Maximal Expressivity — arXiv:2609.26891（2026-09-22）
- Exact Feedback Is Not Control: Evaluating Text-based Closed-Loop Revision in LLMs — arXiv:2609.28150（2026-09-23）
- Breaking the Environment Wall: Evolving LLM Agent Environments for Recursive Self-Improvement — arXiv:2609.29773（2026-09-24）
- When Can Agents Forget Their Reasoning? ICLR for Long-Horizon Agent Context Compression — arXiv:2609.29875（2026-09-24）
- 関連候補として Qwen-Planner-Agent: A Closed-Loop AI-for-AI Framework for Real-World Mobile Planner Agents — arXiv:2609.29892（2026-09-24）も確認したが、今回のトップ5ではハーネス/環境/フィードバック/記憶圧縮への直接性を優先して除外した。

## メモ
- Boris Cherny優先の有無: 本トピックはClaude固有ではないため優先対象外。
- 日本語アカウントの扱い: X検索は英語・日本語の両方で実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、X由来の投稿は採用していない。
- Web検索の扱い: Hermes の web_search は Firecrawl 未設定で失敗したため、代替として arXiv API、GitHub API、直接HTTP確認を使用した。RRSI の GitHub/プロジェクトページ、Exact Feedback の再現コードURL、各 arXiv URL は HTTP 200 を確認済み。
- 注意点・誇張リスク: 直近14日の arXiv プレプリント中心で、査読済みの確立知見ではない。特に recursive self-improvement 系はベンチマーク依存の可能性が高く、実運用では安全境界、評価データ漏洩、失敗トレースの扱いを別途検証する必要がある。

# Loop engineering トレンド調査 (2026-10-01)

- 調査日: 2026-10-01
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「エージェントを賢くする」話から、「失敗・検証・人間の昇格判断まで含む反復系をどう設計するか」へ重心が移っている。

## トップ5

### 1. Relay – a harness for AI coding agents that recover and verify
- 出典: Hacker News / Relay 公式サイト
- 日付: 2026-09-29
- リンク: https://relayevals.com
- 要約: HN投稿によると、Relay はコーディングエージェントに「試行 → 新しいサンドボックスで検証 → 失敗ログを読んで再試行 → 合格したら通常のGit PRとして出す」というループを持たせるハーネス。単発のチャット補助ではなく、失敗を状態として扱い、同じ誤りを繰り返さないようにする点が Loop engineering 的に重要。
- なぜ面白いか:
  - 技術: エージェント実行を検証可能な反復ループに閉じ込め、チェック通過と人間可読な差分を最終出口にする設計が明確。
  - 人文: ethics の観点では、ブラックボックスな「自律性」を増やすのではなく、失敗の履歴とPRという監査可能な形に戻して責任の所在を保っている。anthropology 的には、AIを同僚ではなく「試行錯誤する見習い」として職場のレビュー儀礼に組み込む設計に見える。

### 2. amux – Open-source control plane for AI coding agents
- 出典: GitHub
- 日付: 2026-10-01 更新（作成は2026-02-18）
- リンク: https://github.com/mixpeek/amux
- 要約: amux は Claude Code、Codex、Gemini など複数のコーディングエージェントを、共有ボード、atomic task、schedule、loop、origin-stamped messaging、self-healing recovery で束ねる Rust 製コントロールプレーン。GitHub API確認時点で 511 stars、複数エージェントの作業を「チーム運用」として扱う方向性が強い。
- なぜ面白いか:
  - 技術: ループ、スケジューリング、メッセージの出所記録、自己回復を単一の実行基盤に載せ、複数モデル運用を観測・制御可能にしている。
  - 人文: history の観点では、工場の工程管理やチケット駆動開発が、今度は人間だけでなくAIワーカーにも拡張されている。narrative 的には「AIに頼む」から「AI部隊を運営する」へ、開発者の物語上の役割が作業者から監督者に変化している。

### 3. Agent Chaos Monkey – fault-injection middleware for AI agents
- 出典: GitHub
- 日付: 2026-09-30 作成・更新
- リンク: https://github.com/Baddevil512/agent-chaos-monkey
- 要約: CrewAI / LLM tools 向けに、API 502、レイテンシ急増、壊れたJSONなどを注入し、無限リトライや夜間のトークン浪費を本番前に発見するための故障注入ミドルウェア。従来の chaos engineering を、エージェントのループ失敗に直接当てる発想が新しい。
- なぜ面白いか:
  - 技術: 成功パスだけでなく、外部ツール障害・遅延・不正形式レスポンスに対する停止条件と回復動作を検査できる。
  - 人文: ethics 的には、エージェントの暴走を「賢さ不足」ではなく、設計者が事前に試験すべき安全工学の問題として扱っている。philosophy 的にも、知能を目的達成能力だけでなく、失敗時に止まれる能力として定義し直している点が興味深い。

### 4. ownframework-loop – durable engineering protocol for AI coding agents
- 出典: GitHub
- 日付: 2026-09-30 更新（作成は2026-08-10）
- リンク: https://github.com/william-london/ownframework-loop
- 要約: human-originated specs、exact-SHA review、bounded repairs、human-controlled promotion を掲げる、AIコーディングエージェント向けの耐久的な開発プロトコル。実装そのものよりも、ループの境界、修復回数、昇格権限をプロトコルとして固定しようとする点が目立つ。
- なぜ面白いか:
  - 技術: 仕様の起点、レビュー対象のSHA、修復の上限、人間による昇格を明示し、エージェントの反復を無限化させないガードレールを置いている。
  - 人文: philosophy の観点では、これは「誰が意図を持ったのか」を保存する設計であり、AI生成物の作者性を曖昧にしすぎない。history 的には、ソフトウェア工学が長く積み上げてきた変更管理・レビュー・リリース承認を、エージェント時代に再翻訳している。

### 5. SimpleEvol – An Agent-Loop Framework for LLM-Driven Automated Heuristic Design with Minimal Human Priors
- 出典: arXiv
- 日付: 2026-09-29
- リンク: http://arxiv.org/abs/2609.37172
- 要約: LLMを進化計算の狭い部品として使うのではなく、ヒューリスティック設計の反復生成・評価・改良ループの中心に置く論文。人間が作り込んだ prior の少なさを測る AHI と、LLM能力を性能に変換する効率 ICE を提案し、より少ない手作りルールのフレームワークほど高い ICE を示すと報告している。
- なぜ面白いか:
  - 技術: Loop engineering を開発ワークフローだけでなく、アルゴリズム設計そのものの自動反復へ拡張し、評価指標まで提案している。
  - 人文: creativity の観点では、人間の創造性を細かな操作設計から、探索空間・評価・制約の設計へ移す動きとして読める。philosophy 的には「人間の prior を減らすこと」が進歩なのか、それとも暗黙の価値判断を見えにくくするのかという問いも残る。

## arXiv / 学術
- 見つかった論文: SimpleEvol: An Agent-Loop Framework for LLM-Driven Automated Heuristic Design with Minimal Human Priors / arXiv:2609.37172 / 2026-09-29。LLM主導の自動ヒューリスティック設計を agent-loop として定式化しており、本日のトップ5に採用。
- 参考候補: Guardrailed Meta-Agent Loops: Stress-Testing Policy Pinning, Budget Bounds, and Crash Recovery / arXiv:2609.12216 / 2026-09-10。検索結果では確認できたが、詳細取得時に arXiv API の 429 rate limit が発生したため、本文では未採用。

## メモ
- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため取得できず。英語X検索も同じ理由で失敗。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で利用できなかったため、代替として Hacker News Algolia API、GitHub API、arXiv API を使用した。GitHub項目は更新日時が新しい一方、成熟度や実利用数は限定的なものを含むため、stars や作成日だけで品質を過大評価しないこと。

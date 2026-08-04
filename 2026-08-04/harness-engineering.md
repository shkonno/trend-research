# Harness engineering トレンド調査 (2026-08-04)

- 調査日: 2026-08-04
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの性能差は「モデル単体」より、フック、権限、評価、記憶、セキュリティをどう束ねるかというハーネス設計に移っている。

## トップ5

### 1. Model or Harness? An Interaction-Centric Taxonomy for Localizing Agent Failures
- 出典: arXiv
- 日付: 2026-07-30
- リンク: https://arxiv.org/abs/2607.28802
- 要約: エージェント失敗を、モデル、ハーネス、ユーザー、ツール、メモリ、環境などの相互作用に分解し、どこを直すべきかを割り当てる分類法を提案している。結果だけを見て「モデルが悪い」と判断するのではなく、ハーネス側の足場、ツール統合、環境、採点器の問題を切り分ける点が、Harness engineeringの中核に近い。
- なぜ面白いか:
  - 技術: 41の失敗モードを相互作用エッジと責任側に割り当て、改善対象をモデル訓練、ハーネス修正、環境再設計、ベンチマーク修正へ具体的に振り分けられる。
  - 人文: AI失敗の責任を「知能の不足」という物語から、制度・道具・環境の設計問題へ移す視点がある。これは、人間組織での事故調査に近く、エージェント時代の責任論をより成熟させる。

### 2. Distributing Security Controls Through Harness Engineering
- 出典: arXiv
- 日付: 2026-07-28
- リンク: https://arxiv.org/abs/2607.25890
- 要約: 商用AIコーディングエージェントに対し、ベンダー固有機能だけに頼らず、カスタム・エージェントハーネスを通じてセキュリティ制御を配布・拡張できるかを検証している。OWASP Top 10 for Agentic Applications由来の23テストで、制御なし、ベースライン、セキュリティ強化ハーネスを比較する設計が実務的。
- なぜ面白いか:
  - 技術: 権限、ツール、入出力、監査をハーネス層で制御することで、複数チームへ安全策を標準配布する設計パターンを示している。
  - 人文: コーディングエージェントの導入障壁は「賢さ」より「誰がどこまで任せてよいか」という信頼の制度設計にある。ハーネスは、個人の注意力ではなく組織的な安全文化をコード化する装置として読める。

### 3. Claude CodeのHooks / Subagents / Status lineが「実務ハーネス」の標準部品化を進める
- 出典: Anthropic公式ドキュメント / Claude Code changelog
- 日付: 2026-08-04確認（Claude Code v2.1.221 changelog確認）
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks / https://docs.anthropic.com/en/docs/claude-code/sub-agents / https://docs.anthropic.com/en/docs/claude-code/statusline / https://github.com/anthropics/claude-code/blob/main/CHANGELOG.md
- 要約: Claude Code公式ドキュメントでは、ライフサイクルイベントに応じてシェル、HTTP、LLMプロンプトを実行するHooks、独立コンテキストで動くSubagents、コスト・文脈・git状態を表示するStatus lineが整備されている。v2.1.221のchangelogでも、サンドボックス認証ファイルのマスク、権限チェック迂回の修正、MCP接続修正など、ハーネス層の安全性・観測性に関わる改善が目立つ。
- なぜ面白いか:
  - 技術: PreToolUse/PostToolUse、PermissionRequest、SubagentStart/Stop、statusLineなどが、loop engineeringを実装可能なイベント面・制御面・観測面として提供されている。
  - 人文: 開発者はAIに「お願いする人」から、作業環境そのものを設計する舞台監督に近づいている。Claude Codeの周辺機能は、エージェントとの協働を一回限りの対話ではなく、儀式・監査・役割分担を持つ作業文化に変える。

### 4. Building a Process-Modeling Tool using Agentic AI: An Experience Report on PM4Py-UCM
- 出典: arXiv
- 日付: 2026-07-30
- リンク: https://arxiv.org/abs/2607.28825
- 要約: Claude Codeを含む18のエージェントセッション、374の人間ターン、10,328のツールアクション、151コミット、20リリースを分析し、プロセスマイニング/モデリングツールPM4Py-UCMをAI支援で構築した経験報告。テスト数が108から691へ増え、修正が機能追加の2.3倍、約18%のターンがエージェント誤りの訂正に使われたという具体的な数字が重要。
- なぜ面白いか:
  - 技術: 「エージェントが動いた記録」そのものを採掘し、オラクルベース検証とテスト成長で「動くと言った」ギャップを閉じるハーネス設計を示している。
  - 人文: AI開発は魔法の自動化ではなく、訂正、撤回、一貫性維持、検証を含む共同制作であることが可視化されている。人間の役割は消えるのではなく、判断のログを残し、意味のある失敗を学習可能にする方向へ変わる。

### 5. SKIMIX: Multi-Agent Harness-Time Scaling with Skill Mixture for Dynamic Harness Engineering
- 出典: arXiv
- 日付: 2026-07-30
- リンク: https://arxiv.org/abs/2607.27994
- 要約: 大規模スキルライブラリを持つAIエージェントで、どのスキルを選び、組み合わせ、更新するかを扱うマルチエージェント・フレームワーク。埋め込みベースのスキル検索、anti-dilution routing、適応的スキル進化を組み合わせ、数学推論では改善がある一方、多肢選択では効果が限定的または逆効果になると報告している。
- なぜ面白いか:
  - 技術: 「モデルを大きくする」以外に、ハーネス実行時にスキルの混合と反復をどう設計するかというスケーリング軸を提示している。
  - 人文: 専門家チームを増やせば必ず賢くなるわけではない、という組織論に似た結果が出ている。エージェントの群れにも、分業、希釈、調停、初回改善の限界という社会的な問題が宿る。

## arXiv / 学術
- Model or Harness? An Interaction-Centric Taxonomy for Localizing Agent Failures — arXiv:2607.28802。失敗原因をモデルかハーネスか環境かに局所化する、今回の最重要論文。
- SKIMIX: Multi-Agent Harness-Time Scaling with Skill Mixture for Dynamic Harness Engineering — arXiv:2607.27994。スキル混合をハーネス実行時スケーリングとして扱う。
- Distributing Security Controls Through Harness Engineering — arXiv:2607.25890。AIコーディングエージェントの安全策をハーネスで配布する実務寄り研究。
- Harness Engineering for LLM-Driven GPU Kernel Generation — arXiv:2607.17979（2026-07-20、直近14日より少し古いが関連性が高い）。GPUカーネル生成で、評価ハーネス、プロファイル、アーティファクト保存、Codex/Claude Codeエージェントを分離する設計。
- Building a Process-Modeling Tool using Agentic AI: An Experience Report on PM4Py-UCM — arXiv:2607.28825。Claude Codeの実作業ログを材料に、テスト・修正・検証のハーネス的意味を示す。

## メモ
- Boris Cherny優先の有無: X検索で `@bcherny` とClaude Code/loop/harnessの直近投稿を優先確認する予定だったが、x_searchはクレジット上限で実行不能だったため、本調査時点でBoris Cherny本人の直近接点は確認できなかった。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で実行不能。代替としてGitHub検索・Anthropic公式ドキュメント・arXiv APIを使用したが、日本語コミュニティの生の反応は十分に取得できていない。
- 注意点・誇張リスク: Web検索ツールもFirecrawl未設定で使用不能だったため、DuckDuckGoの自動検索はブロックされ、公式URLの直接取得、GitHub API、arXiv APIに寄せた。したがってX上の話題量や日本語圏での流行度は過小評価の可能性がある。
- 追加観測: GitHub APIでは、Claude Code hooks/subagents/statusline周辺に `digimon-companion`、`knit-statusline`、`claude-tdd`、`skill-harness`、`harness-eval` など小規模リポジトリが直近更新されており、個人・小チームが自分用の制御盤を作る動きは見えた。ただしスター数や一次情報の厚みを踏まえ、トップ5本体には公式ドキュメントと論文を優先した。

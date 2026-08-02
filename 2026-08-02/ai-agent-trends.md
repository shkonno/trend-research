# AI agent trends トレンド調査 (2026-08-02)

- 調査日: 2026-08-02
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの話題は「もっと賢いデモ」から、「長時間・多人数・MCP接続・監査・本番運用で壊れないか」を測る段階へ移っている。

## トップ5

### 1. Claude Code 2.1.219: Opus 5、ネットワーク制御、MCPエラー可視化、ネストsubagent
- タイトル: Claude Code 2.1.219: Opus 5、ネットワーク制御、MCPエラー可視化、ネストsubagent
- 出典: Anthropic Claude Code changelog / 公式ドキュメント
- 日付: 2026-07-24
- リンク: https://docs.anthropic.com/en/docs/claude-code/changelog
- 要約: Claude Code 2.1.219では、Claude Opus 5がOpusのデフォルトとして追加され、1M contextやfast modeに加えて、`sandbox.network.strictAllowlist`、`mcp_server_errors`、`workflowSizeGuideline`、stream-jsonでのネストsubagent転送など、運用寄りの変更がまとまって入った。単なるモデル更新ではなく、背景agent・MCP・sandbox・workflowを制御する面が強いリリースとして読める。
- なぜ面白いか:
  - 技術: 長時間agentを本番で回すためのネットワークegress制御、MCP接続失敗の観測性、subagent階層のトレース性が同時に強化されている。
  - 人文: 「自律性を上げる」と「行動範囲を絞る」が同じリリースに並ぶ点が象徴的で、AIを同僚化するには自由だけでなく境界線の設計が必要だと示している。Boris Cherny優先確認はX側の制限で直接確認できなかったが、Claude Code周辺の最重要実務変化として採用した。

### 2. MCP is going stateless: What the new spec means for AI agents
- タイトル: MCP is going stateless: What the new spec means for AI agents
- 出典: New Relic Blog
- 日付: 2026-07-28
- リンク: https://newrelic.com/blog/ai/mcp-is-going-stateless
- 要約: New Relicは、MCPがstateless方向へ進むことにより、AI agentのスケーリング、状態管理、OpenTelemetry連携がどう変わるかを解説している。MCP serverを「個々の会話に貼り付くプロセス」ではなく、観測可能で水平展開しやすい運用部品として扱う流れが見える。
- なぜ面白いか:
  - 技術: stateless化は、MCP接続をロードバランス、障害復旧、トレース収集の対象にしやすくし、agent基盤を通常の分散システム運用へ近づける。
  - 人文: agentの身体にあたるtool接続が標準化されるほど、責任の所在は「モデル」だけでなく「道具を配る組織」にも広がる。観測性は単なるSRE機能ではなく、後から説明できる行為者を作るための社会的インフラになる。

### 3. Stop Shipping AI Agents on Faith: Capability Is Not Production Readiness
- タイトル: Stop Shipping AI Agents on Faith: Capability Is Not Production Readiness
- 出典: arXiv
- 日付: 2026-07-30
- リンク: http://arxiv.org/abs/2607.27677v1
- 要約: この論文は、デモや能力ベンチマークだけではAI agentを本番投入してよいか判断できないとして、Evaluation、Context、Compliance、Governanceの4軸からなるProofAgent Indexを提案する。agentが情報取得、tool呼び出し、状態維持、代理行為を行う環境では、「できる」ことと「運用してよい」ことを分けて測るべきだと主張している。
- なぜ面白いか:
  - 技術: PAIは実行結果だけでなく、実行環境・規制適合・監査可能性を含めてagent readinessをスコア化しようとする点が実務的。
  - 人文: これはAI評価を「才能の測定」から「委任の制度設計」へ移す議論であり、人間がどこまで機械に代理権を渡せるかという古典的な統治問題に接続している。agentブームの熱狂に対して、信頼ではなく証拠を求める姿勢が重要だ。

### 4. ORCA-bench: How Ready Are Language Model Agents for Oncall?
- タイトル: ORCA-bench: How Ready Are Language Model Agents for Oncall?
- 出典: arXiv
- 日付: 2026-07-30
- リンク: http://arxiv.org/abs/2607.28545v1
- 要約: ORCA-benchは、OpenTelemetryつきマイクロサービス、Prometheus、Jaeger、OpenSearch/Grafana、ソースコードを組み合わせ、1,079件のオンコールRCAタスクで汎用coding agentを評価するベンチマーク。要旨では、現実的入力に近いMedium難度で最良agentでもRCA Accuracyが25.3%に留まると報告されており、運用現場の曖昧な障害対応はまだ難しいことを示す。
- なぜ面白いか:
  - 技術: ログ・メトリクス・トレース・コードを横断するRCAは、単純なコード修正ベンチより本番agentの限界を露出しやすい。
  - 人文: オンコールは技術作業であると同時に、夜中に誰が責任を引き受けるかという労働文化の問題でもある。agentがSREを助ける未来は魅力的だが、25.3%という数字は「人を置き換える」より先に「人の判断をどう補助するか」を考えよと促している。

### 5. agentacct: coding agentsの作業・コスト・テスト実行をローカルで可視化
- タイトル: agentacct: coding agentsの作業・コスト・テスト実行をローカルで可視化
- 出典: GitHub repository search / mikehasa/agentacct
- 日付: 2026-07-24作成、2026-08-01更新確認
- リンク: https://github.com/mikehasa/agentacct
- 要約: `agentacct`は、Claude Code、Codex、OpenCodeなどのcoding agentが何をしたか、どのtoolを使ったか、どのファイルを変えたか、テストを走らせたか、時間とtoken/costをどれだけ使ったかをローカルファーストに可視化するダッシュボード。GitHub API検索では2026-07-19以降作成のClaude Code agent関連repoの中で目立つ星数を集めていた。
- なぜ面白いか:
  - 技術: agent実行を「会話ログ」ではなく、作業ステップ・副作用・検証・コストの会計情報として扱うことで、チーム運用や予算管理に接続できる。
  - 人文: agentに仕事を任せるほど、人間側には「何が起きたのかを説明してもらう権利」が必要になる。ローカルファースト監査は、便利さとプライバシーの両方を守りながら、AI労働の透明性を高める方向性として面白い。

## arXiv / 学術
- 見つかったもの:
  - `2607.27677v1` — Stop Shipping AI Agents on Faith: Capability Is Not Production Readiness。本番投入判断を能力ではなく評価・文脈・コンプライアンス・ガバナンスで見る提案。
  - `2607.28545v1` — ORCA-bench: How Ready Are Language Model Agents for Oncall? 本番風オンコールRCAでagentを測るベンチマーク。
  - `2607.25297v1` — Hybrid Analysis for Secure MCP Tool Use in LLM Agents。MCP tool useの安全性を静的・動的解析で守るMTGuardを提案。
  - `2607.27294v1` — AgentS4D: Benchmarking Runtime Risks across the Execution Lifecycle of LLM-Based Workspace Agents。workspace agentの実行ライフサイクル全体でのリスク評価。
  - `2607.23933v1` — SpecBox: Speculative Sandbox Scheduling for Efficient LLM Agent Serving。MCP sandboxのcold startと資源利用を両立させるruntime提案。

## メモ
- Boris Cherny優先の有無: X検索でBoris Cherny / `@bcherny`を優先確認したが、x_searchは `personal-team-blocked:spending-limit` で失敗したため、当日のBoris発言は直接確認できなかった。
- 日本語アカウントの扱い: 日本語・英語のX検索を試行したが同じくX側のクレジット制限で失敗。Web検索ツールもFirecrawl未設定だったため、代替としてAnthropic公式docs、New Relic記事、arXiv API、HN Algolia、GitHub API、直接HTTP取得を使った。日本語圏実践は十分に拾い切れていない可能性がある。
- 注意点・誇張リスク: Reuters等の「rogue agent」系ニュースはHN検索で見つかったが、一次確認と技術的詳細の検証が不足するためトップ5から外した。GitHub repoの星数や更新日はAPI検索時点のシグナルであり、品質保証ではない。

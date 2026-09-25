# AI agent trends トレンド調査 (2026-09-25)

- 調査日: 2026-09-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの話題は「賢いモデル」そのものから、権限・監査・コスト・ブラウザ/実行環境をどう統制するかへ重心が移っている。

## トップ5

### 1. Claude Code v2.1.280〜v2.1.282: MCP・auto mode・継続セッションの運用改善
- 出典: GitHub Releases / Anthropic Claude Code
- 日付: 2026-09-22〜2026-09-24
- リンク: https://github.com/anthropics/claude-code/releases/tag/v2.1.282
- 要約: Claude Codeの直近リリースでは、MCP URL-mode elicitation、MCP server checks、MCP description length設定、auto modeのserver-side classifier、継続/再開セッションの履歴・thinking・prompt cacheまわりの修正が続いた。単発機能よりも、長い実作業でエージェントが壊れないための地味な運用品質が目立つ。
- なぜ面白いか:
  - 技術: MCP連携、権限プロンプト、履歴再送、prompt cache、thinking blockの扱いが、コーディングエージェントを「日常的な開発インフラ」にするためのボトルネックとして修正されている。
  - 人文: エージェントが共同作業者になるほど、人間は「何を許可したか」「どの記憶が引き継がれたか」を気にするようになる。これは単なるCLI改善ではなく、信頼できる作業記憶をどう社会的に共有するかという問題でもある。

### 2. 4% of Sessions, 65% of the Bill: Claude Code Telemetryから見るコスト偏在
- 出典: PromptArmor / Hacker News掲載
- 日付: 2026-09-24
- リンク: https://www.promptarmor.com/resources/claude-cost-and-risk-otel-findings
- 要約: Claude CodeのOpenTelemetry観測をもとに、一部の長時間・高負荷セッションがコストの大半を占めるという問題を扱う記事。AIコーディングの生産性議論が、いよいよ「誰がどの操作で予算を消費しているか」というFinOps/統制の話に接続してきた。
- なぜ面白いか:
  - 技術: エージェント運用では成功率だけでなく、セッション単位のトークン、ツール呼び出し、モデル選択、リトライを観測しないと費用爆発を検知できない。
  - 人文: AIの「魔法感」は、請求書によって組織内の政治問題に変わる。少数の探索的作業をどう正当に評価し、同時に共有予算を守るかがチーム文化の論点になる。

### 3. Your Agent Speaks MCP. Give It a Computer.
- 出典: Fly.io Blog / Hacker News掲載
- 日付: 2026-09-24
- リンク: https://fly.io/blog/sprites-mcp/
- 要約: MCPを話せるエージェントに、単なるAPIではなく実行環境・コンピュータを与える方向性を示す記事。MCPが「データやツールへの接続規格」から、クラウド上の作業環境を接続する実践へ広がっている。
- なぜ面白いか:
  - 技術: MCPサーバー、リモート実行環境、ブラウザ/OS操作を組み合わせることで、エージェントはコード補完ではなく継続的な作業プロセスを担える。
  - 人文: 人間が道具を持つように、エージェントにも「作業場」が必要になる。ここで問われるのは知能の高さだけでなく、どんな環境を任せると安全で、どこから先は人間の場に踏み込みすぎるのかという境界線である。

### 4. Control AI agents at the execution layer, not the prompt
- 出典: GitHub / CTRLRun（Hacker News掲載）
- 日付: 2026-09-24頃（リポジトリ更新: 2026-09-23）
- リンク: https://github.com/CTRLRun/ctrlrun
- 要約: CTRLRunは「AI agentsのexecution safety layer」を掲げ、プロンプトで安全性を祈るのではなく、実行レイヤで制御する発想を示している。プロンプトインジェクション対策や権限管理の議論が、OS/ランタイム的なガードレールへ移っていることを象徴する。
- なぜ面白いか:
  - 技術: エージェントの安全性をモデル出力後の実行経路で制限する設計は、MCPやシェル/ブラウザ操作を伴うワークフローで現実的な防御線になる。
  - 人文: 「言い聞かせる安全」から「制度としての安全」への移行は、人間社会の規則設計に近い。信頼とは人格の善良さではなく、逸脱しても被害が限定される構造から生まれる。

### 5. MCP-GRANITE / Zero-Trust Authorizationなど、MCPエージェント評価・認可研究の増加
- 出典: arXiv
- 日付: 2026-09-18〜2026-09-21
- リンク: https://arxiv.org/abs/2609.24161
- 要約: arXivでは「MCP-GRANITE Benchmark: GRANularity Interface TEsting for MCP-Based LLM Agents」（2609.24161）や「Zero-Trust Authorization and Discovery for Enterprise MCP」（2609.22573）が直近で確認された。MCPベースのLLMエージェントについて、粒度の細かいインターフェーステスト、ゼロトラスト認可、ツール幻覚対策が研究対象になっている。
- なぜ面白いか:
  - 技術: MCPが普及すると、単に接続できるかではなく、ツール記述・認可・発見・テナント分離を評価するベンチマークと設計原則が必要になる。
  - 人文: エージェントが組織の内部システムへ入るほど、「誰の代理人なのか」「どの権限をなぜ持つのか」が倫理とガバナンスの中心になる。MCP研究は、AIを社会的制度に埋め込むための身分証・通行証の研究とも読める。

## arXiv / 学術
- MCP-GRANITE Benchmark: GRANularity Interface TEsting for MCP-Based LLM Agents — arXiv:2609.24161（2026-09-21）: MCPベースLLMエージェントのインターフェース粒度を評価するベンチマーク。
- Zero-Trust Authorization and Discovery for Enterprise MCP — arXiv:2609.22573（2026-09-18）: 企業MCPの認可・発見をゼロトラストの観点から扱う。
- A Large-Scale Empirical Study of Quality Assurance Practices and Gaps in AI Agents — arXiv:2609.17698（2026-09-15）: AIエージェントのQA実践とギャップを大規模に調査。
- Authorization Architectures for Tool-Using AI Agents — arXiv:2609.15906（2026-09-14）: ツール利用エージェントの認可アーキテクチャを整理。
- NovaFabric: Tamper-Evident, Replayable Evidence for Autonomous AI Agent Runs — arXiv:2609.12582（2026-09-11）: 自律エージェント実行の改ざん検知可能な証跡・再現性を扱う。

## メモ
- Boris Cherny優先の有無: `from:bcherny Claude Code MCP agents` を含むX検索を実施したが、x_searchが `personal-team-blocked:spending-limit` で失敗したため、本調査時点ではBoris Cherny本人投稿は確認できなかった。
- 日本語アカウントの扱い: 日本語クエリ（AIエージェント / Claude Code / MCP / 運用 / 実践）でX検索を実施したが同じくX側の利用制限で取得できなかった。日本語圏の実践例は今回のトップ5には入れず、確認できたWeb/GitHub/arXiv情報を優先した。
- 注意点・誇張リスク: Web検索ツールも未設定（Firecrawl未設定）だったため、代替としてGitHub API、arXiv API、公式ドキュメント/ニュースページ、HN RSS、直接HTTP取得を使用した。X由来の反応量や日本語圏での拡散度は十分に測れていない。

# sharp LLM usage トレンド調査 (2026-09-26)

- 調査日: 2026-09-26
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
LLM活用の焦点は「賢いプロンプト」から、検証・権限・コスト可視化・人間の承認を含む、壊れにくい作業システム設計へ移っている。

## トップ5

### 1. Screen Before You Serve: Simulation for Production Customer Experience AI Agents at 140M Scale
- 出典: arXiv
- 日付: 2026-09-24
- リンク: http://arxiv.org/abs/2609.30137v1
- 要約: 顧客対応AIエージェントを本番投入する前に、仮説駆動のシミュレーションで大規模にふるいにかける研究。手動E2Eテストだけでは拾えない、意図判定・運用ポリシー遵守・ツール利用の破綻を、本番顧客に触れる前に検出する発想が中心。
- なぜ面白いか:
  - 技術: LLMエージェントの品質保証を「良い回答例」ではなく、本番前シミュレーション、失敗仮説、ツール実行経路の検査として扱っている。
  - 人文: 顧客対応は企業と生活者の信頼関係そのものなので、失敗をユーザーに押しつけず事前に社会実験を閉じる設計が重要になる。AI活用の成熟は、派手な自律性より「誰を実験台にしないか」の倫理に表れている。

### 2. Specifying and Maintaining Agentic Workflows: An Empirical Study of GitHub Agentic Workflows
- 出典: arXiv
- 日付: 2026-09-23
- リンク: http://arxiv.org/abs/2609.27263v1
- 要約: GitHub Agentic Workflows のような、Markdownの自然言語指示と設定から実行可能なワークフローを作る実践を分析した研究。単発プロンプトではなく、繰り返し実行される「保守対象の指示ファイル」としてエージェント運用を見る点が鋭い。
- なぜ面白いか:
  - 技術: プロンプトをチャット欄の一時的な文章ではなく、バージョン管理・設定・実行環境に接続されたソフトウェア成果物として扱う方向性を示している。
  - 人文: 人間の仕事の多くは暗黙知の手順でできているが、エージェント化はそれを文章化し、レビューし、継承可能にする。これは自動化であると同時に、組織の記憶をどう書き残すかという文化の問題でもある。

### 3. Runtime Authorization Consistency Checking for MCP-based Agentic Workflows
- 出典: arXiv
- 日付: 2026-09-20
- リンク: http://arxiv.org/abs/2609.23498v1
- 要約: MCPベースの複数ステップのツール利用で、各ツール呼び出しは個別には許可されていても、連鎖全体ではセッションの権限境界を越える「authorization drift」を扱う研究。LLMに何をさせるかだけでなく、作業列全体として許されるかを実行時に検査する。
- なぜ面白いか:
  - 技術: per-callの権限チェックから、ワークフロー単位の一貫性チェックへ視点を上げており、MCP/ツール利用型LLMの実運用に直結する。
  - 人文: 権限逸脱は単なるセキュリティ事故ではなく、委任の境界が曖昧になることから起きる統治の失敗でもある。人間がAIに仕事を任せるほど、「許可したつもり」の範囲を明文化する必要が増す。

### 4. Master Prompt Agreement: file-backed operating model for AI agents
- 出典: GitHub リポジトリ
- 日付: 2026-09-20 更新（初回作成 2026-03-11）
- リンク: https://github.com/laurenzpavlosmalisianos/master-prompt-agreement
- 要約: AIエージェントに対し、明示的な権限、スコープ付きワークフロー、コンテキストルーティング、ソース規律、検証証跡、プロジェクト状態をファイルとして与える運用モデル。READMEでは、既存ファイルを勝手に上書きしない、計画を提示して承認を得る、トランザクション内で検証する、といった実践が強調されている。
- なぜ面白いか:
  - 技術: 「長いシステムプロンプト」ではなく、永続ファイル、現在状態、受け入れ証跡、専門ガイドの遅延ロードでコンテキストを構造化する実用パターンになっている。
  - 人文: これはAIに命令する技術というより、共同作業の契約書を作る技術に近い。人間とエージェントの関係を、気分で変わる会話から、責任範囲と証跡を持つ作業関係へ移す試みとして読める。

### 5. Ask HN: Multi-agent workflows in production; Where people using 1000s of agents?
- 出典: Hacker News / Algolia API
- 日付: 2026-09-13
- リンク: https://news.ycombinator.com/item?id=49689454
- 要約: 大規模なマルチエージェント構成が本当に必要な場面はどこか、数千エージェントの実運用例はあるのかを問うスレッド。コメントでは、少数の強いLLMで足りるケースが多いこと、規模が増えると最大の痛みはエージェントそのものより観測性・トレーシングになることが指摘されていた。
- なぜ面白いか:
  - 技術: 「エージェント数を増やす」より、いつ分割が必要で、どの粒度でトレースし、失敗時にどこをデバッグできるかを問う実務的な論点が前面に出ている。
  - 人文: AIシステムの魅力はしばしば群れや自律性のイメージで語られるが、現場の知恵はむしろ可観測性と説明責任を求めている。ここには、複雑な組織を作るほど官僚制と監査が必要になるという歴史的な反復がある。

## arXiv / 学術
- Screen Before You Serve: Simulation for Production Customer Experience AI Agents at 140M Scale — arXiv:2609.30137v1。顧客対応エージェントを本番前シミュレーションで検査する実践寄りの研究。
- Specifying and Maintaining Agentic Workflows: An Empirical Study of GitHub Agentic Workflows — arXiv:2609.27263v1。自然言語ワークフローを保守対象として扱う研究。
- Runtime Authorization Consistency Checking for MCP-based Agentic Workflows — arXiv:2609.23498v1。ツール連鎖における権限ドリフトを扱う研究。
- Total Cost of Agency: Exact Attribution of Memory Injection Cost in Multi-Agent LLM Workflows — arXiv:2609.23790v1。マルチエージェントのメモリ注入コストを可視化する研究で、コスト設計の観点から関連が強い。
- Can LLMs in Draft-Verify-Revise Pipelines Resolve Deictic Ambiguity? — arXiv:2609.12162v1。2026-09-10で対象期間よりやや古いが、draft-verify-revise型オーケストレーションの限界を考える上で関連。

## メモ
- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。Claude Code関連のHacker News候補（2026-09-06「Cutting (Claude Code) token spend on dynamic workflows 80%」）も確認したが、直近14日外のためトップ5から外した。
- 日本語アカウントの扱い: X検索は英語・日本語の両方で実行したが、x_search が `spending-limit` で失敗したため、投稿本文の確認はできなかった。日本語Web検索も Firecrawl 未設定により web_search が利用できず、代替として arXiv API、Hacker News Algolia API、GitHub API、直接HTTP取得を使った。
- 注意点・誇張リスク: X/Web検索基盤に制限があり、SNS上の日本語実践例は十分に拾えていない。リンクは実際にAPIまたはHTTPで確認できたもののみ採用し、確認できないX投稿や不確かなブログは含めていない。

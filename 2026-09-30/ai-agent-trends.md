# AI agent trends トレンド調査 (2026-09-30)

- 調査日: 2026-09-30
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの焦点は「賢いデモ」から、長時間実行・MCP接続・権限境界・監査可能性を備えた実運用の基盤へ移っています。

## トップ5

### 1. Claude Sonnet 5.5: agentic coding性能と運用コストの同時改善
- 出典: Anthropic公式ニュース
- 日付: 2026-09-28
- リンク: https://www.anthropic.com/claude-sonnet-5-5
- 要約: AnthropicはClaude Sonnet 5.5を発表し、Sonnet 5より30%以上高速、タスクあたり最大30%低コストと説明しています。Agentic coding評価のTerminal-Bench 4.0で70.6%（Sonnet 5は10.3%）という大幅な改善が示され、日常的なバグ修正・文書作成・設計レビュー向けの高速な協働モデルとして位置づけられています。
- なぜ面白いか:
  - 技術: エージェント性能が単なる推論力ではなく、CLI上の長い作業・画像理解・コスト効率まで含む運用指標で語られ始めています。
  - 人文: 「高性能な相棒」が安く速くなるほど、チームの作業配分は人間の実装量ではなく、問題設定・レビュー・責任分担を中心に再編されます。協働相手としてのAIをどう信頼し、どこで人が判断を戻すかが実務文化の論点になります。

### 2. Claude Code v2.1.285: MCPプラグイン設定、サブエージェント権限、WebFetch制御が細かく更新
- 出典: GitHub / Anthropic Claude Code changelog
- 日付: 2026-09-29
- リンク: https://github.com/anthropics/claude-code/releases/tag/v2.1.285
- 要約: Claude Code v2.1.285では、`CLAUDE_CODE_DISABLE_WEB_FETCH`、`claude plugin configure`、MCPB同梱MCPサーバー設定のインストール時指定、許可プロバイダ制限、フォークサブエージェントの権限モード継承、MCPサーバー切替時のツール残存修正などが入っています。派手な新機能より、企業・チームで安全に回すための細部が多いリリースです。
- なぜ面白いか:
  - 技術: Web取得、MCP、サブエージェント、プロバイダ制限、権限プロンプトといった「エージェント運用の事故点」を個別に潰す方向の改善です。
  - 人文: エージェント導入の成熟は、万能感ではなく「何を禁止し、誰が許可し、ログに何を残すか」という制度設計に現れます。Claude Codeが開発者個人の道具から組織的な作業環境へ移る兆候として読めます。

### 3. Anthropic MCP connector: Messages APIからリモートMCPサーバーへ直接接続
- 出典: Anthropic公式ドキュメント
- 日付: 2026-09-15 beta header確認、調査日 2026-09-30
- リンク: https://docs.anthropic.com/en/docs/agents-and-tools/mcp-connector
- 要約: AnthropicのMCP connectorは、独自MCPクライアントを実装せずにMessages APIからリモートMCPサーバーへ接続し、OAuth、複数サーバー、ツールのallowlist/denylist、個別設定に対応します。`mcp-client-2026-09-15` beta headerではサーバーのツール一覧をピン留めする設定も示されています。
- なぜ面白いか:
  - 技術: MCPがローカル開発者ツールの接続規格から、API経由で管理・制限・監査できるエージェント統合層へ拡張されています。
  - 人文: 「どの道具をAIに渡すか」は、組織の権力と責任の分配そのものです。ツールを列挙し、許可し、固定する仕組みは、エージェントの自由度と人間側の説明責任を折り合わせる社会的インフラになります。

### 4. AI Agent Swarms as Researchers: エージェント群が研究成果を量産し、人間のレビューがボトルネックに
- 出典: arXiv
- 日付: 2026-09-28
- リンク: https://arxiv.org/abs/2609.35719v1
- 要約: 論文は、既製のコーディングエージェント群に文献・計算ツール・継続実行指示を与え、最適化理論や物理科学などで研究ノート、論文草稿、形式証明、実験案を大量生成させたと報告しています。著者らは全てが新規・正確とは主張せず、むしろ生成速度が人間の査読速度を上回る点を中心問題として提示しています。
- なぜ面白いか:
  - 技術: エージェントのボトルネックが「成果を作れるか」から「生成物を検証し、信用し、帰属させられるか」へ移っています。
  - 人文: 研究者の価値が、発想や執筆から、問題の選定、検証、共同体としての信用形成へ移る可能性があります。学習や著者性、研究機関の存在意義まで揺さぶる、AIエージェント時代らしい論点です。

### 5. MCP Error Messages Written for Developers Hurt the Most Capable Agents Most
- 出典: arXiv
- 日付: 2026-09-28
- リンク: https://arxiv.org/abs/2609.35381v1
- 要約: 150の広く使われるMCPサーバーに含まれる3,001件のエラーのうち949件を調べ、人間開発者向けのエラーメッセージが、ツール呼び出ししかできないエージェントにとって実行不能な指示を含む問題を分析しています。特に高性能エージェントほど、こうした「読めるが実行できない」エラーに引っかかりやすいという示唆が重要です。
- なぜ面白いか:
  - 技術: MCPサーバーの品質は正常系のスキーマだけでなく、失敗時にエージェントが回復できる機械可読なエラー設計に依存します。
  - 人文: ソフトウェアのエラーメッセージは長く人間への説明文でしたが、今後はAIという非人間の作業者にも読ませる公共言語になります。人間中心の開発者体験から、人間とエージェントの共同作業体験へ設計対象が広がっています。

## arXiv / 学術
- 見つかったもの:
  - **AI Agent Swarms as Researchers: Progress, Challenges, and Open Questions** / arXiv:2609.35719v1 / 2026-09-28 / https://arxiv.org/abs/2609.35719v1 — エージェント群による研究生産とレビュー不足の問題。
  - **MCP Error Messages Written for Developers Hurt the Most Capable Agents Most** / arXiv:2609.35381v1 / 2026-09-28 / https://arxiv.org/abs/2609.35381v1 — MCPエラー設計とエージェント回復性。
  - **Poster: Towards ProofWeave: A Privacy-Minimised, Integrity-Anchored Evidence Plane for Continuous Agentic Assurance** / arXiv:2609.35234v1 / 2026-09-28 / https://arxiv.org/abs/2609.35234v1 — エージェント行動の監査・証跡基盤。
  - **DGF-Bench: A Benchmark for Simulating and Auditing Deception Against Multi-Agent Governance Boards** / arXiv:2609.34913v1 / 2026-09-28 / https://arxiv.org/abs/2609.34913v1 — マルチエージェント統治委員会に対する欺瞞の監査ベンチマーク。
  - **Progressive Skill Discovery as Access Control for Tool-Using LLM Agents** / arXiv:2609.28693v1 / 2026-09-23 / https://arxiv.org/abs/2609.28693v1 — ロールに応じた能力開示をアクセス制御として扱う提案。

## メモ
- Boris Cherny優先の有無: X検索でBoris Cherny（@bcherny）を優先確認しようとしましたが、x_searchは `personal-team-blocked:spending-limit` で利用できませんでした。x.comの公開HTMLは取得できたものの、投稿本文の信頼できる抽出はできなかったため、Boris由来の項目は採用していません。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で失敗しました。日本語圏の実践例は今回のトップ5には入れず、未確認として扱います。
- Web検索の注意: Hermesのweb_searchはFirecrawl未設定で失敗しました。代替として、公式ページ・GitHub API・arXiv API・HN Algolia・直接HTTP取得を使用しました。Google/DuckDuckGoは自動化ブロックが出たため、検索網羅性には制約があります。
- 誇張リスク: GitHub検索結果にはスター数や更新時刻が異常に大きい・将来日付環境に依存する可能性のある情報が混ざるため、トップ5では公式Anthropic、GitHub公式リリース、arXivの確認可能なリンクを優先しました。

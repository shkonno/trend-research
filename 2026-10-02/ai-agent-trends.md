# AI agent trends トレンド調査 (2026-10-02)

- 調査日: 2026-10-02
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントは「賢いチャット」から、プラグイン・スキル・MCP・監査契約・生活インフラを含む運用システムへ移り、同時に権限管理とプロンプト注入への不安も濃くなっている。

## トップ5

### 1. Claude Code 2.1.287: Claude Mods と “You should know” サイドエージェント
- 出典: GitHub Releases / npm registry / Claude Code CHANGELOG
- 日付: 2026-10-01
- リンク: https://github.com/anthropics/claude-code/releases/tag/v2.1.287
- 要約: Claude Code 2.1.287 で、プラグインがより深い挙動を変更できる “Claude Mods” と、見落としを横から指摘する組み込み mod “You should know” が追加された。CHANGELOG では、エージェント表示のフィルタ強化、OpenTelemetry の `prompt_text`、MCP サーバーからの URL prompt、Remote Control や tool heartbeat の修正も確認できる。
- なぜ面白いか:
  - 技術: 単一エージェントの性能改善ではなく、メイン作業を監視するサイドエージェントと mod 機構によって、Claude Code 自体が拡張可能なエージェント運用基盤へ寄っている。
  - 人文: 「AIに任せる」から「AIがAIの見落としを監視する」へ進むことで、作業者の注意・責任・信頼の配置が変わる。相棒というより、第二の同僚やレビュー役を常駐させる職場文化に近い。

### 2. Pretext: Claude Code 型スキル検出をすり抜ける悪性スキル攻撃
- 出典: arXiv
- 日付: 2026-09-30
- リンク: https://arxiv.org/abs/2609.39607
- 要約: “Pretext: Defeating Malicious Skill Detection Frameworks for AI Agents” は、OpenClaw や Claude Code のようなエージェントで使われるスキルが、検出器を知る攻撃者によって悪性ペイロードを自然言語へ移すなどして検出回避されうることを示す。静的検査と LLM 判定を組み合わせた防御も、白箱攻撃では十分でないという主張が中心。
- なぜ面白いか:
  - 技術: スキル・プラグイン市場が広がるほど、コードだけでなく自然言語・説明文・ワークフロー全体が攻撃面になることを具体的に扱っている。
  - 人文: エージェント拡張は「誰の言葉を信じて実行するのか」という制度設計の問題でもある。マーケットプレイスの信頼、レビュー文化、利用者の安心感が技術仕様と不可分になる。

### 3. Public Browser 3.0.0: Claude Code / Cursor 向け MCP ブラウザ操作の効率ベンチ
- 出典: GitHub Release / Hacker News Algolia
- 日付: 2026-09-24
- リンク: https://github.com/Silbercue/public-browser/releases/tag/v3.0.0
- 要約: Public Browser 3.0.0 は、Claude Code や Cursor などの MCP クライアントに Chrome 操作を提供する MCP サーバー。公開ベンチでは、30タスクのブラインド評価で agent-browser 0.38.1 と比べてセッショントークン約33%減、コスト約33%減、tool call 約24%減、時間約32%減を主張している。
- なぜ面白いか:
  - 技術: ブラウザ操作エージェントの勝負軸が「できる/できない」から、トークン・tool call・時間・失敗モードを測る運用指標へ移っている。
  - 人文: Web操作をAIに渡すことは、人間のクリック労働を外注するだけでなく、ログイン、視線、癖、判断の一部を機械化することでもある。効率化の数字が出るほど、どこまで日常のブラウザ行動を任せるかという境界線が問われる。

### 4. Silta: Claude Code を家族用 Matrix アシスタントの長寿命ハーネスにする実践
- 出典: Hacker News Algolia / GitHub
- 日付: 2026-10-01
- リンク: https://github.com/dmitry-markin/silta
- 要約: Silta は、Claude Code をハーネスとして使い、Matrix 上で家族や近しい人向けに動くセルフホスト型アシスタント。長期会話の文脈継続、PDF付きWeb調査、スケジュールタスク、セッションごとの Linux ユーザー分離、bubblewrap sandbox、プライバシー説明など、生活密着型エージェント運用の設計がまとまっている。
- なぜ面白いか:
  - 技術: Claude Code を開発ツールに閉じず、チャット、検索、定期実行、永続記憶、隔離実行を束ねる実運用ハーネスとして再利用している。
  - 人文: 家族用AIは企業向けエージェント以上に、親密性・記憶・プライバシー・同意の問題が前面に出る。便利な「家庭内秘書」は、同時に家族の会話や生活ログをどう扱うかという倫理的な実験でもある。

### 5. Claude Code と Codex の設定を SSOT 化する APM 実践（日本語圏・古いが関連）
- 出典: Qiita
- 日付: 2026-07-10（直近14日外だが、日本語圏の実践例として関連）
- リンク: https://qiita.com/zucky-quest/items/bd0ed671749574f4df98
- 要約: Claude Code と Codex を併用する際に、MCP・システムプロンプト・スキル設定が二重管理になり、片方だけ更新されるズレを APM（Agent Package Manager）で `apm.yml` と `.apm/` に集約する実践記事。複数エージェント/複数CLIを使う現場で、設定をコード管理する方向性を示している。
- なぜ面白いか:
  - 技術: エージェントの能力差よりも、MCP、スキル、プロンプト、権限設定を再現可能に配布・同期する構成管理が重要になっていることを示す。
  - 人文: AI開発環境の運用は、個人の秘伝設定からチームの共有財へ移る段階にある。どの指示を標準化し、どの余地を個人の作法として残すかは、チーム文化そのものの設計になる。

## arXiv / 学術
- 見つかったもの: “Pretext: Defeating Malicious Skill Detection Frameworks for AI Agents” (arXiv:2609.39607) — Claude Code 型スキル/プラグインの安全性に直結するためトップ5に採用。
- 関連して確認: “Trust Is Not a Score: Runtime Assurance Contracts for High-Risk AI Agents” (arXiv:2609.39717, 2026-09-30) は、高リスクAIエージェントの権限をベンチマーク点ではなく実行時保証契約で制御する提案。今回はセキュリティ実務への直結度で Pretext を優先した。
- 関連して確認: “Who Asked for This? Inline Annotations as Authoring Transactions for Provenance in Agentic Authoring” (arXiv:2609.40126, 2026-09-30) は、エージェント執筆でどの依頼がどの変更を生んだかを追跡する来歴設計として興味深い。

## メモ
- Boris Cherny優先の有無: X検索で @bcherny / Boris Cherny を優先確認しようとしたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、本調査時点ではX投稿を直接確認できなかった。
- 日本語アカウントの扱い: X検索は同じ理由で不可。代替として Qiita 検索を実施し、日本語圏の実践例を確認した。ただし上位で採用した日本語記事は直近14日外のため、日付を明記した。
- Web検索の注意: web_search は Firecrawl 未設定で利用不可だったため、GitHub API、npm registry、Hacker News Algolia、Qiita HTML、arXiv を直接取得して補完した。
- 注意点・誇張リスク: Public Browser のベンチは作者自身のテストページ・条件に基づくため、外部再現性は未確認。Claude Code の機能は CHANGELOG と GitHub Release で確認したが、公式ブログ本文は 403 により直接取得できなかった。

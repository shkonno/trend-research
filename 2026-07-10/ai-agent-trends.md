# AI agent trends トレンド調査 (2026-07-10)

- 調査日: 2026-07-10
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
エージェントの話題は「賢いモデル」から、MCP・設定管理・観測・スキル配布・人間の仕事設計を含む運用基盤へ一段移った。

## トップ5

### 1. Codex as agent provider and agentic enhancements in JetBrains IDEs
- 出典: GitHub Changelog（Web / 公式）
- 日付: 2026-07-07（ページ上の datePublished は 2026-07-07T19:55:53-07:00）
- リンク: https://github.blog/changelog/2026-07-07-codex-as-agent-provider-and-agentic-enhancements-in-jetbrains-ides
- 要約: GitHub が JetBrains IDE 向けに Codex を新しい agent provider としてパブリックプレビュー提供し、Hooks、MCP server 管理、カスタムモデル設定を含むエージェント機能の拡張を告知した。IDE 内エージェントが単なるチャット補助ではなく、複数プロバイダ・MCP・フックで構成される実行環境になっている点が重要。
- なぜ面白いか:
  - 技術: エージェント運用の差別化点がモデル単体ではなく、IDE、MCP、Hooks、モデル選択を統合する制御プレーンへ移っている。
  - 人文: 開発者は「AIを使う人」から「複数の代理実行者を編成する人」へ近づいている。これは職能の中心がタイピング量から、委任・監督・環境設計へ移る変化として読める。

### 2. Claude Code と Codex の設定を1つのSSOTに統一する - APMでAIエージェント設定をコード管理した話
- 出典: Qiita（日本語圏実践）
- 日付: 2026-07-10
- リンク: https://qiita.com/ZuckyQuest/items/bd0ed671749574f4df98
- 要約: Claude Code と Codex を併用する現場で、MCP、システムプロンプト、スキル設定が二重管理になった問題を、Microsoft APM（Agent Package Manager）で `apm.yml` と `.apm/` を SSOT 化して解く実践記事。権限・セキュリティ設定は共有せずツール個別管理にする、という線引きも具体的。
- なぜ面白いか:
  - 技術: エージェント設定を生成物として扱い、CI でドリフト検知する発想は、エージェント運用を Infrastructure as Code / Docs as Code に近づける。
  - 人文: チームがAIに何を許し、何を覚えさせ、どの作法で動かすかは、組織文化そのものの記述になる。SSOT化は効率化であると同時に、暗黙の仕事観をレビュー可能にする試みでもある。

### 3. How Boris Cherny Uses Claude Code
- 出典: Web / Hacker News 経由で確認（Boris Cherny 優先確認）
- 日付: 2026-06-27（HN 掲載日。サイト自体は更新継続の可能性あり）
- リンク: https://howborisusesclaudecode.com
- 要約: Claude Code creator の Boris Cherny が日常ワークフローで使うとされる 118+ tips を集めたページで、`CLAUDE.md`、worktrees、plan mode、hooks、subagents などが中心テーマ。本人の X 検索は今回ツール制限で直接確認できなかったが、サイトの構造化データ上でも Boris / Claude Code / Anthropic への言及を確認した。
- なぜ面白いか:
  - 技術: Claude Code の実践知が、プロンプト単発ではなく、リポジトリ常駐の指示、ブランチ分離、計画モード、フック、サブエージェントという運用パターンに整理されている。
  - 人文: 作者の使い方が共有されると、ツールは機能一覧ではなく「職人芸の型」として伝播する。AI時代の熟練は、コードを書く手つきだけでなく、代理作業者に文脈を渡す儀礼として現れている。

### 4. Anthropic「2026 Agentic Coding Trends Report」を読み解く──エンジニアは「書く人」から「設計して任せる人」へ
- 出典: Qiita（日本語解説）＋ Anthropic 公式レポート（Web / 公式）
- 日付: 2026-06-29（公式レポートのランディングページとPDFも取得確認）
- リンク: https://qiita.com/nogataka/items/46fb464d05e2eb53d09c
- 要約: Anthropic の「2026 Agentic Coding Trends Report」を日本語で読み解き、8つのトレンドを foundation / capability / impact の3カテゴリで整理している。日本の開発現場・個人開発への読み替えを含み、Claude Code などのコーディングエージェント利用者が自分の仕事の変化を言語化する助けになる。
- なぜ面白いか:
  - 技術: Agentic coding の論点を、開発プロセス、エージェント能力、組織インパクトに分けて扱うことで、導入判断が「便利そう」から設計課題へ進む。
  - 人文: 「書く人」から「設計して任せる人」への転換は、エンジニアのアイデンティティに直撃する。日本語圏でこの変化を翻訳・再解釈する記事が出ていること自体、現場文化への浸透を示している。

### 5. SkillCenter: A Large-Scale Source-Grounded Skill Library for Autonomous AI Agents
- 出典: arXiv
- 日付: 2026-07-08
- リンク: https://arxiv.org/abs/2607.07676
- 要約: 自律AIエージェント向けに、216,938件の構造化スキルを24ドメインで提供する大規模スキルライブラリを提案する論文。うち114,565件は査読論文、arXiv、24,000以上の技術ソースに基づき、各主張を出典引用へ対応させる source grounding と SQLite FTS5 によるオフライン検索可能性を特徴とする。
- なぜ面白いか:
  - 技術: エージェントの能力拡張を「都度プロンプト」ではなく、出典付きスキルの検索・配布・品質ゲートとして設計している。
  - 人文: これはAIエージェントにとっての図書館や職業訓練校に近い。便利さの一方で、どの知識をスキルとして制度化するか、誰の実践知が標準になるかという知識政治の問題も生まれる。

## arXiv / 学術
- SkillCenter: A Large-Scale Source-Grounded Skill Library for Autonomous AI Agents（2607.07676）: 出典付きスキルライブラリを大規模化する方向。
- Institutional Red-Teaming: Deployment Rules, Not Just Models, Causally Shape Multi-Agent AI Safety（2607.07695）: マルチエージェントの安全性をモデルだけでなく配置ルールの因果効果として評価。
- Beyond Attack-Success Rate: Action-Graded Severity Scale for Tool-Using AI Agents（2607.07474）: tool-using agent の攻撃評価を成功/失敗の二値ではなく行為の深刻度で採点。
- When Claws Remember but Do Not Tell: Stealthy Memory Injection in Persistent Personal Agents（2607.05189）: 長期記憶を持つ個人エージェントへの stealth memory injection を扱う。
- Agent Delivery Engineering Predictive Reliability Framework（2607.07689）: 長時間稼働するマルチエージェントの信頼性を予測・監視する枠組み。

## メモ
- Boris Cherny優先の有無: 優先確認した。`x_search` は実行したが、xAI 側の `personal-team-blocked:spending-limit` エラーで X 本体の検索結果は取得できなかったため、Hacker News と Web ページ確認で補完した。
- 日本語アカウントの扱い: X検索は同上の理由で取得不可。代替として Qiita API で日本語圏の実践記事を検索し、Claude Code / Codex / MCP / APM の具体運用を優先採用した。
- 注意点・誇張リスク: Qiita の個人実践記事や集計値は再現性・測定条件に依存するため、主張を一般統計として扱わない。GitHub Changelog と arXiv はリンク実在を実ツールで確認した。架空リンク・架空 arXiv ID は含めていない。

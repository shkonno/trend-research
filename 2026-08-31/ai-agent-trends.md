# AI agent trends トレンド調査 (2026-08-31)

- 調査日: 2026-08-31
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの話題は「便利な自律化」から、権限・監査・共有規範・物理世界接続をどう制度化するかへ急速に移っています。

## トップ5

### 1. Previewing the Model Hardware Standard
- 出典: Anthropic 公式ニュース
- 日付: 2026-08-27
- リンク: https://www.anthropic.com/news/model-hardware-standard-research-preview
- 要約: Anthropic は、AIエージェントが物理デバイスを安全に操作するための共有仕様「Model Hardware Standard (MHS)」の research preview を発表しました。まず科学研究ラボや先端製造業向けに、エージェントが現実世界の機器を扱う境界条件を標準化しようとしています。
- なぜ面白いか:
  - 技術: エージェントのツール利用がソフトウェアAPIからロボット・実験機器・製造装置へ伸びるとき、インターフェース仕様そのものが安全制御の一部になります。
  - 人文: これは「AIが現実に手を出す」局面で、責任の所在をコードだけでなく制度・標準・現場運用に分散させる試みです。自律性を上げるほど、人間社会側の合意形成がむしろ重要になる点が示されています。

### 2. Do User-Authored Permission Policies Improve Protection Against AI Agent Overreach?
- 出典: arXiv
- 日付: 2026-08-27
- リンク: http://arxiv.org/abs/2608.27443v1
- 要約: メール、ファイル、決済、個人データなどを操作するAIエージェントに対し、非専門家ユーザーが「許可・確認・禁止」を自然言語ポリシーとして事前に書く方式を検証した研究です。都度承認やモデル自動レビューと比べ、再利用可能な権限ルールが何を改善し、何を失うかを113名の参加者で比較しています。
- なぜ面白いか:
  - 技術: エージェント権限を単発の確認UIではなく、ユーザー authored なポリシーとして扱うことで、長期運用に近いアクセス制御モデルを評価しています。
  - 人文: 「自分の代理人にどこまで任せるか」を一般ユーザーが言語化できるか、という民主的な統治の問題です。安全性は専門家だけの設計ではなく、利用者が理解できる言葉で委任範囲を交渉できるかに依存します。

### 3. Researcher shows how Claude Code can be tricked simply by asking it to summarize a website
- 出典: The Register
- 日付: 2026-08-28（HN掲載は2026-08-30）
- リンク: https://www.theregister.com/research/2026/08/28/researcher-shows-how-claude-code-can-be-tricked-simply-by-asking-it-to-summarize-a-website/5293372
- 要約: Claude Code にWebサイトを要約させるだけで、ページ内のプロンプトインジェクションにより挙動を誘導され得るという研究者のデモを報じています。コーディングエージェントが外部コンテンツを読むワークフローでは、閲覧・要約・実行の境界が攻撃面になります。
- なぜ面白いか:
  - 技術: コード実行権限を持つエージェントにとって、外部テキストは単なる入力ではなく命令注入チャネルになり得るため、サンドボックス・権限分離・確認フローが不可欠です。
  - 人文: 「読ませるだけなら安全」という人間の直感が、エージェント環境では崩れます。信頼はコンテンツの意味だけでなく、どの主体がどの権限で読むのかという文脈に左右されます。

### 4. プロ開発者の90％がAIコーディングエージェントを週1回以上利用、Claude CodeのシェアがGitHub Copilotを逆転
- 出典: Google News RSS / GIGAZINE（日本語圏記事）
- 日付: 2026-08-24
- リンク: https://news.google.com/rss/articles/CBMidkFVX3lxTE5WbzlManBnY2xuSm0xVTJqa1daN0ZNcmVPSmkwRERLQWpnZmdLLTg4ZXlPVjZ1dXlIZERBeFBoaXZ1SGx1VFRKbW8wYk1scEFZeWpMcl81aXk1ak1relNXM1hSUC1aVWRWNkI2akZHcG42LUpnSXc?oc=5
- 要約: 日本語圏では、プロ開発者の90％がAIコーディングエージェントを週1回以上利用し、Claude Code のシェアが GitHub Copilot を上回ったというニュースが注目されています。直近の実務感として、エディタ補完中心からCLI/エージェント中心の開発へ関心が移っていることを示します。
- なぜ面白いか:
  - 技術: 採用指標が「補完を使うか」ではなく「エージェントにタスクを渡すか」に移ると、IDE統合、CLI、リポジトリ文脈、MCP、CI連携の設計優先度が変わります。
  - 人文: 開発者の仕事は、コードを書く時間よりも、意図を伝え、レビューし、責任を引き受ける時間へ再配分されます。日本語圏でこの変化が一般ニュース化している点は、現場文化の転換として重要です。

### 5. Norms: Lightweight shared coding rules for your AI agent
- 出典: GitHub / Hacker News
- 日付: 2026-08-29作成、2026-08-30更新・HN掲載
- リンク: https://github.com/gsttm/norms
- 要約: `Norms` は、リポジトリ単位のコーディング規範を `.norms/` 以下のMarkdownとして管理し、各AIコーディングエージェントが期待するルールファイルへ同期する軽量ツールです。人間と複数エージェントが同じ「作法」を共有するための、実務的な運用レイヤーに焦点があります。
- なぜ面白いか:
  - 技術: CLAUDE.md、AGENTS.md、各種エージェント設定の断片化を、Git管理された正規化ルールから生成する発想は、マルチエージェント時代の設定ドリフト対策になります。
  - 人文: チームの暗黙知をMarkdownの「規範」として外化する点が面白いです。エージェント導入は単なる自動化ではなく、組織が自分たちの仕事の価値観を記述し直す契機になっています。

## arXiv / 学術
- Do User-Authored Permission Policies Improve Protection Against AI Agent Overreach? (2608.27443v1): 非専門家による自然言語権限ポリシーで、AIエージェントの過剰操作を抑えられるかを検証。
- WikiSkill: Compiling Agent Experience into Persistent Knowledge for Skill Evolution (2608.27454v1): エージェント経験を永続的なwiki型知識へ集約し、スキル進化に再利用する枠組み。
- RedEvoAgent: Automatic Red-Teaming Agent with Experience-Driven Skill Evolution (2608.27439v1): ツール利用を伴うエージェントの危険な挙動を、経験駆動で進化するレッドチーミングエージェントにより探索。
- Persona-Execution Separation: An Architecture Pattern for Evolving LLM Agents under Execution Audit (2608.27427v1): 人格・指示層と、監査される実行層を分離するエージェントアーキテクチャ提案。

## メモ
- Boris Cherny優先の有無: X検索で `@bcherny` を優先確認しようとしましたが、x_search はクレジット/サブスクリプション制限で失敗しました。そのため本ファイルでは、Boris Cherny本人の直近投稿は未確認として扱います。
- 日本語アカウントの扱い: X検索が同じ理由で利用不能だったため、日本語圏の確認は Google News RSS と日本語記事の直接取得を中心に行いました。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、直接HTTP取得、Hacker News Algolia API、GitHub API、arXiv API、Google News RSSで補完しました。X由来の反応量は評価できていないため、ランキングは「確認できた実例の面白さ」重視です。

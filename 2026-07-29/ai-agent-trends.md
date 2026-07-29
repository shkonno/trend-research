# AI agent trends トレンド調査 (2026-07-29)

- 調査日: 2026-07-29
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AIエージェントの話題は「もっと自律的に」から、「長い作業をどう検証し、記憶し、権限を閉じ、運用品質として扱うか」へ重心が移っています。

## トップ5

### 1. Claude Code 2.1.x: Sonnet 5、1Mコンテキスト、MCP/バックグラウンド運用修正が継続
- 出典: Anthropic公式ドキュメント / Claude Code release notes
- 日付: 2026-07下旬確認（ページ内バージョン 2.1.197 ほか）
- リンク: https://docs.anthropic.com/en/release-notes/claude-code
- 要約: Claude Code 2.1.197ではClaude Sonnet 5がデフォルトになり、ネイティブ1Mトークン文脈と8月末までのプロモーション価格が示されています。同じリリース列では、MCPサーバーの認証・再接続・タイムアウト・ツール検索・バックグラウンドエージェントなど、実運用で詰まりやすい部分の修正が大量に続いています。
- なぜ面白いか:
  - 技術: 「大きなモデル」そのものより、MCP接続、バックグラウンドジョブ、サブエージェント、ワークスペース信頼、権限確認のような運用面が主要な開発対象になっています。
  - 人文: コーディングエージェントは単発の補助者ではなく、長時間一緒に働く同僚に近づいています。そのため、速さだけでなく、記憶、責任、失敗時の復旧、誰が許可したかという労働環境の設計が前面に出ています。

### 2. Loop Engineering: 「プロンプトを書く」から「エージェントのループを設計する」へ
- 出典: GitHubリポジトリ / cobusgreyling/loop-engineering
- 日付: 2026-07-28 更新確認（作成: 2026-06-09、pushed: 2026-07-28）
- リンク: https://github.com/cobusgreyling/loop-engineering
- 要約: `loop-engineering` は、AI coding agents向けにループ設計、監査、初期化、コスト確認、MCPサーバーなどをまとめた実践パターン集です。説明文で Addy Osmani と Boris Cherny に触れつつ、「Stop prompting. Design the loop. Get a score.」を掲げ、プロンプト単体ではなく反復プロセス全体を対象にしています。
- なぜ面白いか:
  - 技術: エージェント利用を、CLI、監査、コスト、ワークツリー、MCPという実装部品に分解し、反復作業を測定可能な設計対象へ変えています。
  - 人文: これは「天才的な一問一答」から「制度化された作業習慣」への移行です。人間の熟練も、ひらめきよりチェックリスト、レビュー、環境設計で支えられてきたことを思い出させます。

### 3. 日本語圏のClaude Code実践: CLAUDE.md、plan、PR化、記憶の外部化が日常化
- 出典: Qiita記事 / Claude Code毎日使い倒して気づいた実践Tips集【2026年版】
- 日付: 2026-07-29
- リンク: https://qiita.com/sescore/items/88f8ce268734e761bcac
- 要約: 日本語圏では、Claude Codeを「仕事の7割を一緒にやる」道具として使い、`CLAUDE.md` にプロジェクト規約・テスト・触らないファイルを書き、`/plan` で実装前に計画を出させる実践が共有されています。同日周辺には、記憶をメモ帳・日記・本棚に分ける `dejavu` の記事や、blastengine MCPをClaude Code CLIへ導入する記事も出ており、実務導入の粒度が細かくなっています。
- なぜ面白いか:
  - 技術: エージェント精度をモデル変更だけで上げるのではなく、リポジトリ内の規約ファイル、計画モード、MCP、外部記憶で安定化する方向が明確です。
  - 人文: 日本語圏の実践は、派手なデモよりも「毎日使って困ったこと」を丁寧に潰す生活技術として現れています。AI導入は魔法ではなく、職場の暗黙知をどこに書き、どう引き継ぐかという文化の再編です。

### 4. Looping Is Not Reliability: エージェントの生成・テスト・修正ループは信頼性そのものではない
- 出典: arXiv
- 日付: 2026-07-27
- リンク: https://arxiv.org/abs/2607.24604
- 要約: コーディングエージェントで一般的な generate-test-revise ループについて、反復すれば信頼性が上がるとは限らないと実験で示した論文です。HumanEval修復やリポジトリ実験を通じ、いったん正しい修正を見つけても、古いトレースや強制的な再修正によって正しさを失う問題を扱い、状態に束縛された証拠と型付き修正契約を提案しています。
- なぜ面白いか:
  - 技術: 「ループ回数」ではなく、現在の状態、証拠、修正契約、提出条件を管理することがエージェント信頼性の核心だと示しています。
  - 人文: 人間の仕事でも、やり直し続けることは誠実さに見えて、実は成果物を壊すことがあります。AIエージェントにも、努力量ではなく、いつ止めるか・何を証拠とするかという判断倫理が必要です。

### 5. Agentic Permissions Policy Algebra: プロンプトインジェクション時代の「権限と汚染」を数理化する
- 出典: arXiv
- 日付: 2026-07-27
- リンク: https://arxiv.org/abs/2607.24625
- 要約: APPA（Agentic Permissions Policy Algebra）は、LLMエージェントが機密度の異なるデータを扱うときのプロンプトインジェクションや推論ミスを、情報フロー制御の観点から扱う研究です。未検証データを読んだ主文脈を永久に汚染する代わりに、子トラジェクトリを分岐させ、信頼されたサニタイザだけが限定的な派生成果を親へ返す設計を提案しています。
- なぜ面白いか:
  - 技術: エージェントの文脈を一枚岩にせず、権限ラベル、分岐、事前取得チェック、サニタイズ済み派生物として制御する点が実装上重要です。
  - 人文: これはAI版の「誰に何を見せてよいか」「一度見たものを忘れられるか」という制度設計です。自律性が増すほど、信頼は人格的な善意ではなく、境界線と記録の作り方に依存します。

## arXiv / 学術

- 見つかった論文:
  - `2607.24604` Looping Is Not Reliability: State-Bound Evidence and Typed Revision Contracts for Agentic Code Repair — コーディングエージェントの修正ループと信頼性。
  - `2607.24625` Agentic Permissions Policy Algebra for Taint Confinement in LLM Agents — エージェント文脈の権限・汚染制御。
  - `2607.24663` A corrective agentic hybrid RAG and an operations-grounded evaluation for a scientific facility — 科学施設運用におけるMCPツール層付きReAct/RAG。
  - `2607.24006` Agentic Cloud Decoys: A Deception-Driven Framework for Autonomous Intrusion Investigation — クラウド侵入調査をエージェントで要約・調査する枠組み。
  - `2607.24720` The Physics of Multi-Turn Long-Horizon Planning — 長期計画能力の獲得・蒸留・評価。

## メモ

- Boris Cherny優先の有無: X検索で @bcherny を直接確認する予定でしたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、直接のX投稿確認はできませんでした。代替として、Boris Chernyに言及する `loop-engineering` リポジトリとClaude Code公式リリースノートを優先確認しました。
- 日本語アカウントの扱い: X検索は同じ理由で不可。代替としてQiita APIを使い、日本語圏のClaude Code/MCP実践記事を確認しました。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）も未設定で失敗したため、公式ページ・GitHub API・Qiita API・arXiv APIを直接HTTP取得して調査しました。リンクは実取得できたものに限定しています。

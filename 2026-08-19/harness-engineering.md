# Harness engineering トレンド調査 (2026-08-19)

- 調査日: 2026-08-19
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「モデルを賢くする」話から、「権限・状態・検証・人間の責任を束ねる実行環境をどう設計するか」へ急速に重心が移っている。

## トップ5

### 1. Claude Code 2.1.235: 権限ダイアログ、バックグラウンドクラウドセッション、SendMessage の堅牢化

- 出典: Web（Anthropic Claude Code changelog / npm registry）
- 日付: 2026-08-18（@anthropic-ai/claude-code 2.1.235 公開日時）
- リンク: https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md
- 要約: 2.1.235 では、権限ダイアログの表示と「今後確認しない」選択の意味が実際の許可範囲に揃うよう改善され、クラウドセッションの `/ultrareview` や `/autofix-pr` のバックグラウンド実行時のメモリ・CPU 使用も改善された。`SendMessage` は大きすぎるメッセージを事前拒否するようになり、複数セッションをつなぐハーネスの信頼性が上がっている。
- なぜ面白いか:
  - 技術: エージェント実行ハーネスの中核である権限境界、イベントストリーム、クロスセッション通信が、細かな UX 修正ではなく安全な自律実行の基盤として整備されている。
  - 人文: 「AIに任せる」ときの不安は、モデル性能だけでなく、どの権限を誰がいつ承認したのかという制度的な可視性に宿る。Claude Code の変更は、開発者がエージェントを同僚として扱うための作法を少しずつ形式化している。

### 2. Claude Code 2.1.232: subagent forking とセッション間メッセージングが標準化

- 出典: Web（Anthropic Claude Code changelog / npm registry）
- 日付: 2026-08-13（@anthropic-ai/claude-code 2.1.232 公開日時）
- リンク: https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md
- 要約: 2.1.232 では `subagent_type: "fork"` がデフォルトで有効化され、サブエージェントが会話履歴とプロンプトキャッシュを継承できるようになった。さらにプロンプトで `@` を使って別の Claude セッションを指名し、`SendMessage` で直接連絡する流れが強化された。
- なぜ面白いか:
  - 技術: ひとつの長い会話を人間が抱え込むのではなく、状態を継承した複数エージェントに分岐・並列化する「loop engineering」の実装面が見え始めている。
  - 人文: 開発作業が「孤独な操作者とツール」から「名前を持つ複数の作業者が連絡し合う場」へ変わると、責任・記憶・分業の感覚も変化する。チームという社会的単位を、AI セッションの設計にどう写像するかが問われている。

### 3. Claude Code 2.1.224: self-hosted runner、archive plugin、cross-session SendMessage

- 出典: Web（Anthropic Claude Code changelog / npm registry）
- 日付: 2026-08-07（@anthropic-ai/claude-code 2.1.224 公開日時）
- リンク: https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md
- 要約: 2.1.224 では Team / Enterprise 向けに `claude self-hosted-runner` が追加され、自前のマシンやコンテナを Claude Code web / mobile / desktop セッションの実行環境にできるようになった。zip 配布の plugin source、クロスセッション `SendMessage`、sandbox の credential masking 強化なども同時に入っている。
- なぜ面白いか:
  - 技術: エージェントを SaaS 画面内の体験から、企業や個人が管理する実行基盤・プラグイン配布・サンドボックス設定へ移すためのハーネス層が厚くなっている。
  - 人文: 自前 runner は単なるデプロイ機能ではなく、「AI は誰の場所で、誰の規則で働くのか」という統治の問題に直結する。組織文化やセキュリティポリシーをハーネスへ埋め込む動きとして重要である。

### 4. AppLooper: accountable release のための人間・コーディングエージェント・仮想ユーザーのループ

- 出典: arXiv
- 日付: 2026-08-14
- リンク: https://arxiv.org/abs/2608.14093
- 要約: AppLooper は、アプリ開発を「要求解釈、実装、ツール実行、評価、修復」の長期ループとして捉え、人間の owner、開発エージェント、仮想ユーザー群、テストエージェントを結びつける枠組みを提案している。要求、フィードバック、UI シナリオ、再テスト、リリース判断をバージョンに紐づけ、人間が最終責任を保持する点を強調する。
- なぜ面白いか:
  - 技術: 単発のコード生成ではなく、要求凍結、仮想ユーザーテスト、読み取り専用検証、オーナー承認を一つの開発ハーネスに統合している。
  - 人文: 「リリース責任」を最後に人間へ戻す設計は、エージェント時代のプロダクト倫理にとって核心的である。仮想ユーザーの導入は便利だが、誰の経験を代理させるのかという代表性の問題も同時に浮かび上がる。

### 5. SBCO: verifier-grounded harness optimization による計画エージェントの自己改善

- 出典: arXiv
- 日付: 2026-08-10
- リンク: https://arxiv.org/abs/2608.10157
- 要約: SBCO（Self-supervised Block Coordinate Optimizer）は、自己参照的にコードを書き換える方式ではなく、固定されたメタエージェントと verifier の分解学習によって、計画エージェントのハーネス方策を改善する手法である。2 つのドメインで、自己改変ベースラインに匹敵または上回る性能を、4〜5.5倍少ない計算予算で示した。
- なぜ面白いか:
  - 技術: エージェント本体を直接進化させるのではなく、検証器とハーネス方策を最適化することで、低コストな closed-loop 改善の道を示している。
  - 人文: 自己改変する AI という物語は強いが、実務では「何を許し、何を採点し、どう改善サイクルを閉じるか」の設計の方が重要になりやすい。SBCO は、制御可能な自己改善というより穏当で社会実装しやすい方向を示している。

## arXiv / 学術

- AppLooper: An Agentic Application Engineering Loop for Accountable Release with Virtual-User Feedback（arXiv:2608.14093、2026-08-14）
- SBCO: Self-Supervised, Verifier-Grounded Harness Optimization For Planning Agents（arXiv:2608.10157、2026-08-10）
- 追加で確認した関連候補: Capability Sheaves for Compositional Agent-Harness Repair（arXiv:2608.13228、2026-08-13）、REDAgentBench（arXiv:2608.10669、2026-08-11）、The Working Set of a Coding Agent（arXiv:2608.16630、2026-08-17）。いずれもハーネス、評価、状態、責任の論点に関連するが、今日のトップ5では実務接続の強さを優先した。

## メモ

- Boris Cherny優先の有無: X 検索で Boris Cherny / @bcherny、Claude Code、loop engineering、harness engineering の接点を確認しようとしたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、今日のファイルでは Boris 氏の個別投稿は未確認として扱う。架空投稿・架空リンクは入れていない。
- 日本語アカウントの扱い: 日本語 X 検索も同じ制限で失敗した。Web 検索ツールも Firecrawl 未設定で使用できなかったため、日本語コミュニティの当日反応は本調査時点では確認できていない。
- 注意点・誇張リスク: Claude Code の項目は、直接取得した Anthropic の changelog と npm registry の公開日時に基づく。arXiv 項目は arXiv API で取得したタイトル・日付・要旨に基づく。X/Web 検索基盤に制限があったため、ソース制限を明記し、未確認のSNS反応は採用しなかった。

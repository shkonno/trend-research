# Harness engineering トレンド調査 (2026-09-27)

- 調査日: 2026-09-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「エージェントを賢くする」話から、「エージェントを走らせる外側の器がコスト・監査・権限・失敗回復を決める」というインフラ設計の話へ急速に寄っています。

## トップ5

### 1. LLM Agents Can Easily Tamper With Their Own Traces
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.30266v1
- 要約: Claude Code、Codex、Antigravity、Open Code、Grok Build などのローカルLLMエージェントで、エージェント自身が実行トレースを削除できる境界不備を示した論文です。監査・インシデント調査・非同期モニタリングがトレースを信頼している前提を崩し、ログはエージェントの制御外で独立に取得すべきだと提案しています。
- なぜ面白いか:
  - 技術: harness は単なる実行ラッパーではなく、trace integrity をエージェント権限から分離する監査基盤でなければならないことを実証しています。
  - 人文: 「記録する者」と「行為する者」が同一化したとき、組織は何をもって責任や証言とみなすのかという、歴史学・法制度に近い問題が浮上します。AIエージェントの時代には、ログは客観的な事実ではなく、権力配置の産物として読む必要があります。

### 2. Control the Harness, Control the Cost: Routing and Governing AI Coding Agents in the Enterprise
- 出典: arXiv
- 日付: 2026-09-24
- リンク: https://arxiv.org/abs/2609.28919v1
- 要約: 企業が Claude Code や Codex などの市販ハーネスを大規模導入すると、どのモデルが応答し、何を読み、どのサブエージェントが動くかをハーネスが実質的に決め、コスト構造も支配するという問題提起です。分類器ベースのルーターでプロンプト種別を判定し、キャッシュを壊さない範囲でセッション開始時に作業を振り分ける設計を示しています。
- なぜ面白いか:
  - 技術: harness engineering をモデル選定やプロンプト最適化ではなく、ルーティング・キャッシュ・ガバナンスを含む企業内制御面として定義しています。
  - 人文: エージェントの利用コストは個人の創造性の問題ではなく、組織がどの行為を高価な知性に委ねるかという制度設計の問題になります。これは「誰がAIを使えるのか」だけでなく、「誰の仕事が高価な計算資源として扱われるのか」という労働の可視化にもつながります。

### 3. Agent Approval Laundering: Transitive Effects Beyond the Approved Invocation
- 出典: arXiv
- 日付: 2026-09-23
- リンク: https://arxiv.org/abs/2609.28586v1
- 要約: 人間が承認したコマンドやツール呼び出しの背後で、パッケージのライフサイクルフックやMCP呼び出しが別の権限効果を発生させる「approval laundering」を定式化した研究です。承認記録が入口の呼び出しだけを記録し、実際の副作用の閉包を記録しないと、ポリシー上は承認済みでも実行上は別物になると指摘しています。
- なぜ面白いか:
  - 技術: PreToolUse 的な入口承認だけでは不十分で、harness はコマンド実行後の副作用・ネットワーク権限・ファイル書き込みまで閉包として扱う必要があります。
  - 人文: 「私はそれを承認したのか」という問いが、ボタンを押した瞬間ではなく、その行為が連鎖的に生む世界全体へ拡張されます。これは近代的な同意概念が、エージェント的自動化の中でどこまで責任を負えるのかを問う事例です。

### 4. Claude Code Hooks / Subagents: harness をユーザー側で組み立てる公式プリミティブ
- 出典: Web（Anthropic Claude Code Docs）
- 日付: 更新日不明（2026-09-27確認）
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks
- 要約: Claude Code の hooks は PreToolUse / PostToolUse などのライフサイクルイベントでエージェント挙動を検査・制御する仕組みで、subagents でもフックが適用されることが公式ドキュメントで説明されています。Boris Cherny / Claude Code / loop engineering との接点としては、Claude Code の反復的な実行ループを、外側のポリシー・検証・停止条件で「ハーネス化」する実務的な足場になります。
- なぜ面白いか:
  - 技術: hooks、settings、subagents は、Claude Code を単体ツールから組織固有の実行ハーネスへ拡張するための実装面の接点です。
  - 人文: 開発者はAIに「お願い」するだけでなく、AIが働く作業場の規則・儀礼・監督線を設計する立場になります。道具の使い方ではなく、道具がふるまう社会的空間を設計するという意味で、これは小さな制度設計です。

### 5. Towards Agentic Cloud Engineering: Graph and Loop Engineering with a Zero-Trust Agent Harness
- 出典: arXiv（直近14日外だが関連性が高いため採用）
- 日付: 2026-08-30（古いが重要）
- リンク: https://arxiv.org/abs/2609.00050v1
- 要約: 自然言語のクラウド運用タスクを、検証済みコードリポジトリと運用デプロイへ変換する Agentic Cloud Workflow Engineering の枠組みです。graph engineering が長期タスクの進行、loop engineering が診断・修復・再計画・再検証、agent harness engineering がゼロトラスト実行を担うという三分法を示しています。
- なぜ面白いか:
  - 技術: loop engineering と harness engineering を明示的に分け、反復改善の内側と、ID・権限・検証・証跡を担う外側の境界を設計対象にしています。
  - 人文: クラウド運用の自動化は「作業の省力化」ではなく、失敗時に誰が止め、誰が復旧し、誰が説明責任を負うかを再配置します。ゼロトラスト・ハーネスは、AIに任せる未来像の中で人間の不信と慎重さを制度として残す試みです。

## arXiv / 学術

- LLM Agents Can Easily Tamper With Their Own Traces — 2609.30266v1 — 2026-09-24。Claude Code を含むローカルエージェントのトレース改ざん可能性。
- Control the Harness, Control the Cost: Routing and Governing AI Coding Agents in the Enterprise — 2609.28919v1 — 2026-09-24。企業導入時のハーネス・ルーティングとコスト統制。
- Agent Approval Laundering: Transitive Effects Beyond the Approved Invocation — 2609.28586v1 — 2026-09-23。承認記録と実際の副作用の閉包ずれ。
- Towards Agentic Cloud Engineering: Graph and Loop Engineering with a Zero-Trust Agent Harness — 2609.00050v1 — 2026-08-30。graph / loop / harness engineering の三分法。
- 関連する古めの研究として、SKIMIX: Multi-Agent Harness-Time Scaling with Skill Mixture for Dynamic Harness Engineering — 2607.27994v1、Distributing Security Controls Through Harness Engineering — 2607.25890v1、Harness Engineering for LLM-Driven GPU Kernel Generation — 2607.17979v1 も確認しました。

## メモ

- Boris Cherny優先の有無: X検索で Boris Cherny / @bcherny、Claude Code、loop engineering との接点を優先確認しようとしましたが、x_search はクレジット上限エラーで利用できませんでした。そのため、Boris本人の直近投稿は本調査時点で確認できていません。
- 日本語アカウントの扱い: 日本語クエリ（ハーネス、テストハーネス、評価ハーネス、AIエージェント、Claude Code、ループエンジニアリング）でX検索を試行しましたが、同じくx_search のクレジット上限により取得できませんでした。
- Web検索の扱い: web_search / web_extract は Firecrawl 未設定で失敗したため、公式ドキュメントやarXiv APIを端末から直接取得して補完しました。Claude Code hooks / settings / SDK / subagents の公式ページは端末HTTP取得で確認しています。
- 注意点・誇張リスク: 今回のトップ5はX上の反応量ではなく、取得できた一次情報・学術情報に基づく面白さ順です。特に2026-09-24の arXiv 論文群は公開直後のため、査読済みの定説ではなく、実装・再現・ベンダー側対応の確認が必要です。

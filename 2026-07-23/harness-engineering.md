# Harness engineering トレンド調査 (2026-07-23)

- 調査日: 2026-07-23
- 情報源: X / Web（Firecrawl web_search/web_extractは未設定のため、X検索と端末からの公式Docs・arXiv API直接取得で補完） / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Harness engineering は「良いプロンプト」ではなく、エージェントが安全に反復し、検証され、監査できる作業環境そのものを作る技術として、Claude Code / loop engineering の周辺で一気に言語化されている。

## トップ5

### 1. Claude Code 周辺で “Harness → Loop → Graph” が日本語圏にも流入
- 出典: X投稿（@jar2, @AIPlus_Findy, @TAKAKING22, @tuzuminami ほかの日本語圏議論）
- 日付: 2026-07-20〜2026-07-22
- リンク: https://x.com/jar2/status/2079820011552837733 / https://x.com/AIPlus_Findy/status/2079102341283012649 / https://x.com/TAKAKING22/status/2079773714603020741 / https://x.com/tuzuminami/status/2079510894862860338
- 要約: 日本語コミュニティでは、Harness engineering を「AIが信頼性高く働ける環境・制約・ツール・検証ゲートを設計すること」と捉え、そこから Loop engineering、さらに Graph engineering へ進む図式が共有されている。特に Claude Code の実践文脈で、Memory、Skills、Protocols、サブエージェント、Sandbox、自動テスト、静的解析、承認ゲートがハーネスの構成要素として語られている。
- なぜ面白いか:
  - 技術: 単発プロンプトの巧拙ではなく、エージェントの入出力境界、権限、検証、反復条件を設計する「周辺システム」が性能を左右するという認識が広がっている。
  - 人文: 「コードを書く人」から「AIが働く制度を作る人」への職能変化が見える。若手がハーネス設計経験を積めなくなる Apprentice Gap への懸念もあり、教育・徒弟制・専門性の継承という社会的テーマを含んでいる。

### 2. Boris Cherny の `/checkup` はハーネス保守をプロダクト機能にしたサイン
- 出典: X投稿（Boris Cherny / @bcherny）
- 日付: 2026-07-08（直近14日より少し古いが、Claude Code / Boris 優先のため関連重要項目として採用）
- リンク: https://x.com/bcherny/status/2074997570317779038
- 要約: Boris Cherny は Claude Code の新機能 `/checkup` を告知し、未使用の skills/MCP/plugins の整理、CLAUDE.md の重複解消、root CLAUDE.md の分割、遅い hooks の無効化、最新版への更新、auto mode や読み取りコマンド事前承認などを挙げている。これは「生成させる」機能ではなく、Claude Code が働くローカル環境の健康診断・整備を支援する機能である。
- なぜ面白いか:
  - 技術: skills、MCP、plugins、hooks、CLAUDE.md、権限設定を対象にした保守は、Claude Code 利用環境そのものをハーネスとして扱う実装例になっている。
  - 人文: エージェントの賢さだけでなく、道具の整理・文脈の清掃・権限の手入れが成果を決めるという点で、AI時代の「工房管理」の感覚が出ている。Boris/Claude Code 接点としても、loop engineering の前提になる足場整備がプロダクト内に入ったことが重要。

### 3. Claude Code 公式Docsの `/loop`・Subagents・Hooks がハーネスの標準部品になっている
- 出典: Anthropic Claude Code Docs（端末で直接取得）
- 日付: 2026-07-23取得（ページ更新日は取得結果からは未確認）
- リンク: https://docs.anthropic.com/en/docs/claude-code/common-workflows / https://docs.anthropic.com/en/docs/claude-code/sub-agents / https://docs.anthropic.com/en/docs/claude-code/hooks
- 要約: 公式Docsでは、`/loop` が現在のCLIセッションで短いポーリング型タスクを回す手段として説明され、サブエージェントは独自ツール・プロンプト・権限を持つカスタムエージェントとして定義されている。Hooks reference では、PreToolUse / PostToolUse が「agentic loop の各ツール呼び出し」で発火し、ブロックや意思決定制御に使えると説明されている。
- なぜ面白いか:
  - 技術: `/loop`、subagents、hooks は、反復・分業・実行前後検証をCLI内部に組み込むためのハーネス部品として読める。
  - 人文: これはAIを「話し相手」から「手順・役割・儀礼を持つ作業組織」へ変える設計である。人間が直接すべてを見張るのではなく、どの場面で止め、誰に任せ、何を記録するかを文化として設計する段階に入っている。

### 4. arXiv: Harness Engineering for LLM-Driven GPU Kernel Generation
- 出典: arXiv
- 日付: 2026-07-20
- リンク: http://arxiv.org/abs/2607.17979v1
- 要約: LLMによるGPUカーネル生成で、評価ハーネスとプロファイルに基づく最適化コントローラを分離し、コンパイル、正しさ、公式指標に沿った計測、成果物アーカイブをハーネス側で担わせる研究。Codex と Claude Code エージェントが制約内で候補カーネルを生成し、人間が書いた skills が制約・参照実装・プロファイリング手順・昇格ルールを保持する。
- なぜ面白いか:
  - 技術: LLMの生成能力を直接信じず、コンパイル・正当性・計測・昇格ルールで囲い込むことで、最適化タスクを再現可能な探索問題に変えている。
  - 人文: 「創造的なコード生成」と「競技・計測・監査」のあいだに制度設計を置く発想が鮮明で、AIの才能をどう公正に評価し、どこまで人間がルールを与えるべきかという問いを投げている。

### 5. arXiv: From Prompts to Contracts と DataFlow-Harness が示す監査・DAG化の方向
- 出典: arXiv
- 日付: 2026-07-09 / 2026-07-18
- リンク: http://arxiv.org/abs/2607.08028v1 / http://arxiv.org/abs/2607.16617v1
- 要約: “From Prompts to Contracts” は、企業LLMエージェントをプロンプト中心の試作から、ソース境界、エンティティルーティング、回答契約、再現可能トレースを持つ監査可能アーキテクチャへ作り替える harness-engineering アプローチを提示する。“DataFlow-Harness” は、自然言語から自由形式スクリプトを出すのではなく、型付きの増分変更でプラットフォームネイティブなDAGを構築させ、12タスクのデータエンジニアリングベンチマークで93.3%の観測end-to-end pass rateを報告している。
- なぜ面白いか:
  - 技術: 契約・スキーマ・検証成果物・MCP・ライブ状態・DAGエディタを通じて、LLM出力を監査可能で編集可能な構造物へ変換している。
  - 人文: 企業やデータ基盤では、AIの「答え」より、誰が何を根拠にどの境界内で操作したかの記録が重要になる。Harness engineering は、AIを組織に受け入れるための説明責任と共同編集の作法として機能し始めている。

## arXiv / 学術

- Harness Engineering for LLM-Driven GPU Kernel Generation — arXiv:2607.17979v1 — 2026-07-20。GPUカーネル生成を、評価ハーネス・プロファイル・昇格ルールで制御する研究。
- DataFlow-Harness: A Grounded Code-Agent Platform for Constructing Editable LLM Data Pipelines — arXiv:2607.16617v1 — 2026-07-18。LLMエージェントをDAG編集プラットフォームに接続する研究。
- From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents — arXiv:2607.08028v1 — 2026-07-09。企業LLMエージェントを契約・トレース・検証で監査可能にする研究。
- Agent Hacks Agent: Autoresearch for Production-Agent Red-Teaming — arXiv:2607.11698v1 — 2026-07-13。サンドボックスハーネス上で本番エージェントの脆弱性発見ループを回す関連研究。
- When Does Restricting a Coding Agent to execute_code Help? — arXiv:2607.10569v1 — 2026-07-12。Claude Code / Codex CLI を含む比較で、ツール面・ハーネス・プロンプトを固定したエージェント設計アブレーションを行う関連研究。

## メモ

- Boris Cherny優先: 実施。@bcherny の直近投稿では、直接 “harness” や “loop” を前面に出す投稿よりも、Claude Code の `/checkup` やプロダクト改善投稿が目立ったため、ハーネス保守の具体例として採用した。
- 日本語アカウントの扱い: 実施。@jar2、@AIPlus_Findy、@TAKAKING22、@tuzuminami、@junkmemo、@itsuki_dev、@stepney141 などの日本語圏X議論を優先確認した。
- Web検索の注意点: Hermes の Firecrawl web_search/web_extract が未設定で失敗したため、端末から Anthropic 公式Docsと arXiv API を直接取得して補完した。一般Web記事の網羅性は限定的。
- 誇張リスク: “Harness/Loop/Graph engineering” はバズワード化しており、概念の境界はまだ流動的。既存のテスト、CI、権限管理、ワークフロー設計をAIエージェント向けに再命名・再編している面もあるため、用語そのものより実装された検証ゲートと運用ループを重視すべき。

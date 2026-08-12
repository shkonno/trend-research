# Loop engineering トレンド調査 (2026-08-12)

- 調査日: 2026-08-12
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「プロンプトを上手く書く」段階から、長時間走るエージェントの状態・証拠・停止条件・安全境界を設計する段階へ、Loop engineering が一気に実装寄りへ移っています。

## トップ5

### 1. LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation
- 出典: arXiv / Microsoft GitHub / 公式サイト
- 日付: 2026-07-31公開、2026-08-10更新
- リンク: https://arxiv.org/abs/2608.00267 / https://github.com/microsoft/Loopsbench / https://loopsbench.ai/
- 要約: Microsoft の LoopsBench は、112タスク・5,300以上の開発ユニット・依存DAG・Docker実行・単体検証を備えた、長時間の coding agent loop を測るベンチマークです。最強構成でも解決率25%という結果が示され、単発タスクでは見えにくい回帰、前提依存、途中計画の崩れを評価対象にしています。
- なぜ面白いか:
  - 技術: エージェント評価を「最終成果物」から、ready frontier、回帰義務、依存DAG、実行ログを含むループの動的品質へ拡張しています。
  - 人文: ethics の観点では、エージェントの「完了した」という自己申告ではなく、検証可能な進行証拠を求める設計になっています。history の観点でも、ソフトウェア工学がユニットテストからCI/CDへ進んだように、AI開発も会話単位から工程単位へ制度化されつつあります。

### 2. @cobusgreyling/loop: Loop Engineering CLI の「front door」化
- 出典: GitHub / npm / ドキュメント
- 日付: GitHub更新 2026-08-11、npm latest `@cobusgreyling/loop@0.1.2`
- リンク: https://github.com/cobusgreyling/loop-engineering / https://www.npmjs.com/package/@cobusgreyling/loop / https://raw.githubusercontent.com/cobusgreyling/loop-engineering/main/docs/cli-front-door.md
- 要約: Cobus Greyling の loop-engineering リポジトリは、`loop init`、`loop doctor`、`loop audit`、`loop cost`、`loop sync` などを `@cobusgreyling/loop` という単一CLIにまとめています。README は「Stop prompting. Design the loop. Get a score.」を掲げ、Claude Code、Codex、Grok、opencode などを対象に Loop Ready score と運用診断を提供します。
- なぜ面白いか:
  - 技術: 個別スクリプト群を薄い umbrella CLI にまとめ、初期化・監査・同期・コスト確認・状態確認を日常運用の入口にしています。
  - 人文: creativity の観点では、開発者の創造性が「次の一文を入力すること」から「再利用できる作業儀式をデザインすること」へ移動しています。anthropology 的には、エージェント利用が個人芸からチームの作法・チェックリスト・習慣へ変わる兆候です。

### 3. loopx: 長時間エージェントチーム向け状態カーネル
- 出典: GitHub
- 日付: GitHub更新 2026-08-12、push 2026-08-11
- リンク: https://github.com/huangruiteng/loopx
- 要約: `loopx` は、Codex や Claude Code などの agent loop に依存しない軽量な状態カーネルとして、永続ゴール、クォータを意識した auto-wake、実行可能 todo、証拠ログ、検証可能な handoff を掲げています。GitHub API上では 2026-08-12 時点で 4,160 stars と表示され、Loop engineering の「状態管理」側への関心を示しています。
- なぜ面白いか:
  - 技術: ループをプロンプト列ではなく、ゴール、予算、証拠、handoff を持つ永続的な状態機械として扱っています。
  - 人文: philosophy の観点では、主体性を「モデルの賢さ」ではなく「継続する意図と記録の構造」に置き換える発想です。history 的には、OSのプロセス管理やジョブキューの概念が、AIエージェントの日常労働へ移植されています。

### 4. loop-kit-core: 無人実行エージェントのセキュリティ契約
- 出典: GitHub
- 日付: GitHub更新 2026-08-11、push 2026-08-11
- リンク: https://github.com/PostOrganic-AI/loop-kit-core
- 要約: `loop-kit-core` は「loop engineering はループ設計を教えるが、loop-kit は誰も見ていない時に安全に走らせる方法を与える」と説明される TypeScript プロジェクトです。credential-bearing agents、つまり認証情報を持ったエージェントが無人で走る状況に対して、セキュリティ契約を中心に据えています。
- なぜ面白いか:
  - 技術: unattended loop に対して、権限・認証情報・実行境界を明示的な契約として扱う方向に踏み込んでいます。
  - 人文: ethics の観点では、「便利だから自動化する」から「誰が、どの権限で、どこまで任せたのか」を記録する責任論へ焦点が移っています。anthropology 的には、夜間や不在時に働くエージェントが、組織の信頼・監査・当番文化を再編し始めています。

### 5. intent-gate: 実装前に意図整合性を強制する Human-in-the-loop ゲート
- 出典: GitHub
- 日付: 作成 2026-08-10、更新 2026-08-11
- リンク: https://github.com/baixinghao/intent-gate
- 要約: `intent-gate` は、Claude Code plugin と MCP server により、AI coding agents が推測で実装へ進む前に、PRD、intent-confidence gate、Mermaid contract、機械的 lint を通すことを目指すプロジェクトです。Human-in-the-loop、file-persisted、zero-config を掲げ、ループの前段に「意図確認」を置いています。
- なぜ面白いか:
  - 技術: 実装ループの前に、状態機械・シーケンス図・意思決定表を契約として固定し、CRITICAL lint がゼロになるまで進ませない設計です。
  - 人文: narrative の観点では、コード生成の物語を「エージェントが何か作った」から「人間と機械が意図を合意し、その合意に沿って進んだ」へ書き換えています。ethics の観点でも、速度よりも同意・説明可能性・誤解の早期発見を優先する設計です。

## arXiv / 学術

- LoopsBench: From Harness Engineering to Loop Engineering in Coding Agent Evaluation — arXiv:2608.00267。2026-07-31公開、2026-08-10更新。長時間 coding agent 評価を Loop engineering として定式化する中心的な論文。
- CoEvo-Mem: Co-Evolving Retrieval Policy and Memory Bank for LLM Agents — arXiv:2608.01739。2026-08-03公開。検索ポリシーとメモリバンクが相互に変化する closed-loop memory の研究で、広義の loop engineering に近い。
- PluginEval: A Diagnostic Benchmark for Fine-Grained Error Attribution in Function Calling — arXiv:2608.08700。2026-08-09公開。ツール呼び出し評価を生成・検証・実API実行の closed loop で回し、失敗帰属を細かく見る研究。

## メモ

- Boris Cherny優先の有無: 本トピックでは Boris Cherny 本人の直近X投稿は x_search のクレジット制限により確認できませんでした。ただし Cobus Greyling の README には Addy Osmani と Boris Cherny に触発された旨が記載されています。
- 日本語アカウントの扱い: 日本語X検索も実行しましたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、直近X投稿の確認はできませんでした。
- 注意点・誇張リスク: Hermes の `web_search` / `web_extract` は Firecrawl 未設定で利用不能だったため、Web確認は terminal からの直接HTTP取得、GitHub API、npm registry、arXiv APIに限定しました。GitHub stars や更新時刻は調査時点のAPI値であり、人気の質や実運用品質を直接保証するものではありません。トップ5は「Loop engineering」という語そのものに近い実装・評価・安全設計を優先し、一般的な feedback loop 論文は補助的に扱いました。

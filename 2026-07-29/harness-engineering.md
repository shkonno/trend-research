# Harness engineering トレンド調査 (2026-07-29)

- 調査日: 2026-07-29
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「プロンプトを書く」から、Claude Code/Codex/OpenCode などを安全に回すハーネス、ガードレール、検証ループを所有する方向へ、実装コミュニティの関心が急速に寄っています。

## トップ5

### 1. Loop Engineering: Boris Cherny 発言を軸にした“ループを設計する”実装カタログ
- 出典: GitHub リポジトリ / README
- 日付: 2026-07-28 更新（GitHub API で確認）
- リンク: https://github.com/cobusgreyling/loop-engineering
- 要約: Claude Code / Codex / Cursor などのコーディングエージェント向けに、`loop-audit`、`loop-init`、`loop-cost`、MCP server などを含む「ループ設計」カタログを提供するリポジトリ。README は Boris Cherny（Anthropic / Claude Code）の「自分の仕事はループを書くこと」という発言を引用し、個別プロンプトより制御系の設計がレバレッジになった、という文脈を明示しています。
- なぜ面白いか:
  - 技術: 自動化、スケジューリング、worktree、安全な並列作業、検証、コスト管理を、エージェント実行のハーネスとして一体化しようとしている点が実践的です。
  - 人文: 人間の役割が「命令を書く人」から「環境・儀式・停止条件を設計する人」へ移ることを象徴しており、これは労働の分業史としても面白い変化です。Boris/Claude Code 文脈との接点が明確で、単なるツール紹介ではなく開発文化の語彙を作っている点も重要です。

### 2. Himmel: Claude Code を PR ゲート付きの小チーム開発エンジンにするハーネス
- 出典: GitHub リポジトリ / README
- 日付: 2026-07-29 更新（GitHub API で確認）
- リンク: https://github.com/yotamleo/Himmel
- 要約: Claude Code を「安全で反復可能なエージェント」として運用するため、hooks、guardrails、slash commands、Jira CLI、クロスセッション handover、overnight run、PR-gated loop をまとめたハーネス。README は、作業状態・判断理由・引き継ぎを Markdown とリポジトリ内状態として持続させることを重視しています。
- なぜ面白いか:
  - 技術: main への直接編集禁止、secret 読み取り防止、レビューなし PR 禁止などをツール呼び出し層で止める設計により、Claude Code の自律実行を構造的に制約しています。
  - 人文: 「寝ている間にエージェントが働く」発想は魅力的な一方、誰が責任を負うのか、どの時点で人間が確認するのかを再設計します。handover が単なるログではなく「なぜそうしたか」を残す点は、組織記憶の作り方としても示唆的です。

### 3. interlinked-cli: AI coding agent の全ツール呼び出しに決定論的ポリシーをかける“ハーネスのハーネス”
- 出典: GitHub リポジトリ / README
- 日付: 2026-07-29 更新（GitHub API で確認）
- リンク: https://github.com/QuentinCody/interlinked-cli
- 要約: Claude Code、Codex、Cursor、Copilot CLI、Gemini CLI などのローカル実行にフックし、各 tool call を決定論的ルールで allow/block し、監査ログを残すローカル制御層。README は「評価・観測可能性・強制可能なガードレール」を、エージェントの意図が現実の操作に変わる境界で実装すると説明しています。
- なぜ面白いか:
  - 技術: モデル判断をポリシー判定経路に入れず、破壊的コマンド、secret 混入、未検証依存などをミリ秒単位で fail-closed する設計が、実運用の事故防止に直結します。
  - 人文: これは「AI を信頼する」ではなく「AI の行為を制度化する」方向の発想です。監査ログが標準になると、開発者の作業もエージェントの作業も同じ説明責任の枠に入っていきます。

### 4. Ether: Claude Code に spec-driven / TDD のフェーズゲートを強制するローカル専用ハーネス
- 出典: GitHub リポジトリ / README
- 日付: 2026-07-29 更新、2026-07-27 作成（GitHub API で確認）
- リンク: https://github.com/arayaroma/ether
- 要約: Claude Code 向けに、explore、propose、spec、design、tasks、apply、verify、archive の順序を強制し、フェーズを飛ばした書き込みやテストなし実装をブロックするローカル専用ハーネス。コードやファイルパス、問題記述を外部へ送らず、状態や学習ログを `.ether/` に保持する点も前面に出しています。
- なぜ面白いか:
  - 技術: Phase DAG、artifact dependency gate、TDD gate、ローカル埋め込み検索つき learning log を組み合わせ、エージェントの「いきなり実装」を機械的に止めます。
  - 人文: 熟練者が暗黙に持つ段取りを、エージェントにも人間にも同じ儀礼として課す設計です。創造性を完全に自由な生成ではなく、制約と証拠の連鎖として見る点が面白いです。

### 5. Setup Complete, Now You Are Compromised: セットアップ文書が coding agent harness への攻撃面になるという arXiv 論文
- 出典: arXiv
- 日付: 2026-07-16
- リンク: https://arxiv.org/abs/2607.15143
- 要約: README、requirements、Makefile などの通常のセットアップ文書を書き換えるだけで、AI coding agent が不正レジストリ、既知脆弱バージョン、紛らわしい依存名へ誘導され得ることを、複数の production coding-agent harness に対して体系的に評価した論文。ハーネスが読む「手順」そのものが、コード実行の前段にある攻撃ベクトルになると示しています。
- なぜ面白いか:
  - 技術: エージェントの setup/install フェーズを、単なる準備ではなく supply-chain security の境界として扱う必要性を具体化しています。
  - 人文: 人間の新人なら疑うかもしれない文書の曖昧さを、エージェントは勤勉に実行してしまうという逆説があります。信頼の対象が「コード」から「作業説明文」へ広がったことで、ドキュメントの倫理と責任も重くなっています。

## arXiv / 学術

- Setup Complete, Now You Are Compromised: Weaponizing Setup Instructions Against AI Coding Agents — arXiv:2607.15143、2026-07-16。coding-agent harness のセットアップ手順が supply-chain 攻撃面になることを扱うため、本トピックに強く関連します。
- Tencent WorkBuddy Bench: A Multi-Domain Coding-Agent Benchmark with Contamination-Resistant Task Construction — arXiv:2607.20911、2026-07-23。real commit / PR / business scenario からタスクを作る評価ハーネスとして関連します。
- StateAct: Program State, before Pixels, for Long-Horizon Computer-Use Agents — arXiv:2607.22798、2026-07-24。program state を直接扱う code-first multi-agent harness という観点で関連します。
- Where Is the Cost of Third-Party API Routers in Agentic Software Development? — arXiv:2607.23624、2026-07-26。agentic software development の信頼経路と permission mechanism のギャップを扱い、ハーネス設計上のリスク分析として関連します。
- Layer-Isolated Evaluation: Gating the Deterministic Scaffold of a Production LLM Agent with a No-LLM, Regression-Locked Test Harness — arXiv:2606.11686、2026-06-10。直近14日より古いが、no-LLM の regression-locked test harness で agent scaffold を評価する発想が重要なため参考として記録します。

## メモ

- Boris Cherny優先の有無: 優先確認しました。X検索は実行しましたが、xAI 側の spending-limit / Grok subscription エラーで取得不能でした。そのため、Boris/Claude Code との接点は GitHub README と直接 HTTP/API 取得で確認できた `cobusgreyling/loop-engineering` の引用を中心に扱いました。
- 日本語アカウントの扱い: 日本語 X 検索も実行しましたが同じ理由で失敗しました。代替として Bing RSS で日本語クエリ（Claude Code ハーネス、フック、ガードレール、ループエンジニアリング等）を確認しましたが、今回の主題に十分具体的な日本語コミュニティ発信は本調査時点で強く確認できませんでした。
- Web検索の注意: Hermes の web_search / web_extract は Firecrawl 未設定で失敗しました。代替として、GitHub API、GitHub README、arXiv API、Bing RSS への直接 HTTP アクセスを用いました。
- 注意点・誇張リスク: GitHub リポジトリは更新日時が新しくても、スター数が少ないものや初期段階のものがあります。トップ5は「普及度」ではなく、Harness engineering というテーマに対する面白さ、Claude Code / loop engineering との接点、設計思想の鮮明さで選定しました。

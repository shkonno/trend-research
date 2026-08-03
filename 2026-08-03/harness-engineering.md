# Harness engineering トレンド調査 (2026-08-03)

- 調査日: 2026-08-03
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Claude Code 周辺では「LLMに頑張らせる」より、フック、記録、権限、評価、監査を外側から組むハーネス設計が主役になっています。

## トップ5

### 1. keka v0.3.0 — Claude Code 用ハーネスに prompt coach / secrets guard / conventions を追加

- 出典: GitHub リポジトリ / Release
- 日付: 2026-08-03
- リンク: https://github.com/MohammedMoataz/keka/releases/tag/v0.3.0
- 要約: `keka` は “A harness for Claude Code” を掲げる新しい OSS で、v0.3.0 では曖昧なプロンプトに一行助言する prompt coach、ツール実行前の secrets guard、チーム規約を残す conventions を追加した。リリース本文では、実クレデンシャルをブロックし、`.env` や秘密鍵ファイルの読み取りを確認制にし、ガード自体は fail-open でログする、という実務寄りの設計が説明されている。
- なぜ面白いか:
  - 技術: Claude Code の内部推論ではなく PreToolUse 的な外部ガード、プロンプト品質検査、チーム規約メモリを組み合わせ、エージェント実行を「制御可能な工程」に変えている。
  - 人文: これは開発者の注意力や倫理観だけに安全を委ねない設計であり、AI時代の職人技を「習慣」から「作業環境の制度」へ移す動きに見える。ハーネスは単なる自動化ではなく、チームが何を危険とみなし、何を良い依頼とみなすかを刻む文化的装置になっている。

### 2. Claude Code Hooks 公式ドキュメント — deterministic control をハーネスの中核に置く

- 出典: Anthropic / Claude Code 公式ドキュメント
- 日付: 2026-08-03 取得（公式ページに個別更新日は確認できず）
- リンク: https://code.claude.com/docs/en/hooks-guide
- 要約: 公式の Hooks ガイドは、Claude Code の特定ライフサイクルでシェルコマンドを自動実行し、フォーマット、通知、コマンド検証、プロジェクトルール強制を行う仕組みとして説明している。参照ページでは `SessionStart` / `UserPromptSubmit` / `PreToolUse` / `PostToolUse` / `Stop` などのイベント、JSON 入出力、HTTP hooks、MCP tool hooks まで扱う。
- なぜ面白いか:
  - 技術: LLM が自発的に守るルールではなく、ツール呼び出しの前後に決定的な処理を挟むため、テスト、監査、サンドボックス、通知を再現可能な制御点として設計できる。
  - 人文: 「賢いモデル」への信頼を、「止める・記録する・確認する」仕組みへの信頼へ分散する点が重要。これは自律エージェントとの付き合い方を、個人の勘から組織的な作法へ移す小さな制度設計である。

### 3. Claude Code と Codex の作業履歴を SQLite に貯め、hook 遅延を 268ms から p95 17ms へ落とした日本語実践例

- 出典: Qiita / 日本語コミュニティ記事
- 日付: 2026-08-02
- リンク: https://qiita.com/heboHebo-san/items/0edf082cd00ae5a3be2e
- 要約: Claude Code / Codex の hook で作業履歴を自動収集する `agent-history` を作ったところ、同期 SQLite 書き込みが Claude Code の体感速度を悪化させたため、hook は spool ファイルを置くだけにし、常駐 worker がバッチ投入する二段構成へ変えたという実測記事。HDD 環境では hook 1回 268ms、プロセス起動 11.8ms など、ハーネスの性能コストが具体的に示されている。
- なぜ面白いか:
  - 技術: エージェントの観測可能性を高めるハーネスは、同期 I/O をクリティカルパスに置くと UX を壊すため、非同期化、spool、バッチ書き込みが設計上の必須論点になる。
  - 人文: AI開発では「結論のコード」だけでなく「考えた過程」が失われがちで、履歴ハーネスは記憶の外部化として働く。一方で、その記憶装置が遅すぎると人間の集中を削るため、記録する倫理と作業リズムの尊重を両立させる必要がある。

### 4. Stop Shipping AI Agents on Faith — ProofAgent Harness と PAI による本番準備度評価

- 出典: arXiv
- 日付: 2026-07-30
- リンク: https://arxiv.org/abs/2607.27677
- 要約: “Capability is not production readiness” を掲げ、AIエージェントを能力デモだけで出荷せず、Evaluation / Context / Compliance / Governance の4次元で本番準備度を測る ProofAgent Index を提案する論文。PAI は ProofAgent Harness というオープンソースの監査可能な評価・ガバナンス基盤内に実装されたとされ、医療・金融ドメインで検証している。
- なぜ面白いか:
  - 技術: 単発ベンチマークではなく、実行環境、規制遵守、運用承認、監査可能性まで含めたハーネスを評価対象にしている。
  - 人文: エージェントの「できる」は、社会的に「任せてよい」と同義ではない。この論文は、AI導入判断を性能競争から説明責任と統治の問題へ引き戻す点で、かなり実務倫理に近い。

### 5. AgentS4D — Claude Code / Hermes / Codex などを含むワークスペースエージェントの実行時リスク評価ベンチマーク

- 出典: arXiv
- 日付: 2026-07-29
- リンク: https://arxiv.org/abs/2607.27294
- 要約: AgentS4D は、LLMベースのワークスペースエージェントについて、外部ツール、永続状態、副作用をまたぐライフサイクル全体で安全性を評価するサンドボックス型ベンチマーク。要旨では Hermes、OpenClaw、Claude Code、Codex の4ハーネスと5種類の LLM バックエンドを組み合わせた 6,560 run を評価し、事前定義された unsafe signal が多数発生したと報告している。
- なぜ面白いか:
  - 技術: プロンプト単体の安全性ではなく、ツール呼び出し、状態変化、実行後証拠という複数チェックポイントでリスクを測るため、ハーネス設計そのものの比較が可能になる。
  - 人文: エージェントの危険は「悪い返答」だけでなく、ファイル変更、権限、ログ、後始末といった時間的な連鎖に宿る。これはAIを一回の対話相手ではなく、職場に滞在する行為者として扱う発想であり、責任の所在を考えるうえで重要である。

## arXiv / 学術

- 確認された関連論文:
  - `2607.27677` — “Stop Shipping AI Agents on Faith: Capability Is Not Production Readiness” (2026-07-30): ProofAgent Harness / PAI による本番準備度評価。
  - `2607.27294` — “AgentS4D: Benchmarking Runtime Risks across the Execution Lifecycle of LLM-Based Workspace Agents” (2026-07-29): Claude Code など複数ハーネスを含む実行時安全性ベンチマーク。
  - `2607.28591` — “Change2Task: From Repository Changes to Executable Coding Agent Tasks and Environments” (2026-07-30): PR履歴から実行可能な coding agent タスク環境を作る評価データ生成。
  - `2607.26777` — “CodeSpec: Dual Executable Specifications for Agentic Long-Horizon Feature Development” (2026-07-29): 長期機能開発で仕様を実行可能な検証器に変える手法。
  - `2607.27994` — “SKIMIX: Multi-Agent Harness-Time Scaling with Skill Mixture for Dynamic Harness Engineering” (2026-07-30): skill mixture と multi-agent refinement による harness-time scaling。
  - `2607.28272` — “MemHarness: Memory Is Reconstructed, Not Replayed” (2026-07-30): 過去経験をそのまま再生せず、現在文脈に合わせて再構成するエージェント記憶ハーネス。

## メモ

- Boris Cherny優先の有無: X検索で Boris Cherny / @bcherny / Claude Code / harness / loop engineering の接点を優先確認しようとしたが、今回の cron 実行では x_search が `personal-team-blocked:spending-limit` で失敗した。代替として GitHub API と Claude Code 公式ドキュメント、Qiita API、arXiv API を確認した範囲では、Boris Cherny との直接接点は確認できなかった。
- 日本語アカウントの扱い: X検索は同じ理由で実行不能だったため、日本語コミュニティ確認は Qiita API に切り替えた。Claude Code hooks、settings、サンドボックス、履歴収集、ハーネス有無の検証記事が 2026-08-02〜08-03 に複数見つかった。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定で、通常の web_search / web_extract は利用できなかった。公式 Markdown への直接 HTTP 取得、GitHub API、Qiita API、arXiv API で補完したが、X上の反応量・拡散度は未確認である。GitHub の `keka` は作成直後で star 数は 0 のため、流行度よりも設計上の面白さを優先して採用した。

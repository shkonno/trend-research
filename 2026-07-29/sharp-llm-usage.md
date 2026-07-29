# sharp LLM usage トレンド調査 (2026-07-29)

- 調査日: 2026-07-29
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
LLM活用の鋭さは「よいプロンプト」単体から、状態・権限・検証・人間の判断点を設計するワークフローへ移っている。

## トップ5

### 1. Tines 3B – safe workflow automation for when everyone builds software
- 出典: Hacker News / Tines
- 日付: 2026-07-28
- リンク: https://news.ycombinator.com/item?id=49084371
- 要約: Tines 3Bは、社内の非エンジニアや各部門がClaude CodeやCodexで作ったダッシュボード、エージェント、業務自動化を、個人PCや個人アカウントではなく、IT・セキュリティが見える実行環境で動かすという提案。LLMが書いたコードを隔離実行し、資格情報はコードへ埋め込まずプロキシ経由で扱う点が実践的です。
- なぜ面白いか:
  - 技術: 「LLMに作らせる」だけでなく、実行環境、credential handling、可観測性、権限境界をワークフロー側に寄せている。
  - 人文: これはシャドーITを禁止する発想ではなく、人々がすでに作っている小さなソフトウェアを組織の公共圏へ移す設計です。AI時代の統治は、創造性を止める門番ではなく、安心して作れる舞台装置に近づいています。

### 2. Dn – plan collaboratively, let agents execute
- 出典: Hacker News / GitHub README
- 日付: 2026-07-28
- リンク: https://github.com/chesapeakedev/dn
- 要約: `dn`は、GitHub issueやローカル仕様をMarkdownの永続的なplanに変換し、OpenCode、Cursor、Claude Code、Codex CLIなど任意のエージェントに実装させるCLI。`kickstart`でissueから実装、`meld`で複数コンテキストを計画へ統合、`loop`で中断作業を再開し、`land`や`fixup`でPR化・レビュー修正まで接続します。
- なぜ面白いか:
  - 技術: 会話履歴ではなくリポジトリ内の`plans/`をコンテキストの正本にし、受け入れ基準・ブランチ・PR・CIをエージェント実行の外骨格にしている。
  - 人文: 「小チームに必要なのは別のダッシュボードではなく、人間の判断と機械の実行の境界」という思想が明確です。LLM活用を個人芸からチームの記憶へ変換する試みとして読めます。

### 3. Hanesu – An experimental workflow layer for AI coding agents
- 出典: Hacker News / GitHub README
- 日付: 2026-07-23
- リンク: https://github.com/jezmn/hanesu
- 要約: Hanesuは、AI coding agentに対して、長い一発プロンプトではなく、task files、phase、role handoff、quality gates、progress artifactsを与えるリポジトリ内ワークフロー層。READMEは「Context before code」「Artifacts over memory」「Verification before completion」「Smoke test in verify」など、LLMが文脈を失う失敗に対する具体的な運用原則を列挙しています。
- なぜ面白いか:
  - 技術: `CLAUDE.md`のような静的指示では保存できない実行状態を`.hanesu/feature.json`や`current.json`で持ち、search→spec/diagnose→implement→diff review→verifyのような段階に分ける。
  - 人文: エージェントを万能な同僚として扱うのではなく、忘れやすく迷いやすい存在として道具立てを整える姿勢が誠実です。人間の熟練とは、機械に任せる勇気だけでなく、任せられる環境を作る忍耐でもあります。

### 4. Why I prefer Opus 5 to Fable 5
- 出典: Hacker News
- 日付: 2026-07-28
- リンク: https://news.ycombinator.com/item?id=49081970
- 要約: 投稿者は、Fableを「briefを渡すと9時間走る agency 的ブラックボックス」とし、事前に設計判断を固める「Gold in, gold out」が必須だと述べています。一方でOpus 5は自然なphase gateで報告し、ユーザーを開発リズムに巻き込み続けるため、強力さよりも透明性と共同作業性を評価しています。
- なぜ面白いか:
  - 技術: 長時間自律エージェントの性能比較が、単なるベンチマークではなく、phase gate、進捗報告、自己検証、コスト消費、ユーザー介入点という運用指標で語られている。
  - 人文: 「速く終わる黒箱」と「遅くても関与できる相棒」の対比は、AIを代理人として使うか、共作者として使うかの分岐です。人間の満足感や責任感をどこに残すかが、LLM活用の品質そのものになっています。

### 5. A corrective agentic hybrid RAG and an operations-grounded evaluation for a scientific facility
- 出典: arXiv
- 日付: 2026-07-27
- リンク: https://arxiv.org/abs/2607.24663
- 要約: Advanced Photon Sourceの運用知識に対するAPS-RAGは、電子ログブック、技術文書、wiki、チャット、保守記録、制御システムデータを対象に、dense/sparse/KG検索、query-type-adaptive fusion、corrective agentic loop、MCPツール層を組み合わせた実運用RAG。APS-Benchという監査可能な50問の評価セットと6層評価ハーネスを用い、cross-encoder rerankerを外すとstrict vital recallが32.8%落ちるなど、実装上の勘所が数字で示されています。
- なぜ面白いか:
  - 技術: RAGを「答えが合っていそう」ではなく、gold answer、vital-nugget recall、reranker ablation、operations-grounded evaluationで検証する実践例になっている。
  - 人文: 施設運用の知識は、文書だけでなく、現場のログ、会話、保守の記憶に分散しています。LLM活用がうまくいくかは、組織の暗黙知をどう尊重し、監査可能な形で引き出すかにかかっています。

## arXiv / 学術
- `2607.24663` A corrective agentic hybrid RAG and an operations-grounded evaluation for a scientific facility: 実運用RAGに対し、監査可能なベンチ、reranker ablation、corrective loop、MCP tool layerを組み合わせた事例。
- `2607.24625` Agentic Permissions Policy Algebra for Taint Confinement in LLM Agents: unvetted dataを読む子trajectoryとsanitizerを使い、親コンテキストを汚染せず権限・taintを管理する提案。プロンプトインジェクション対策と実用性の両立が焦点。
- `2607.24348` DeepFaith: Evidence-Grounded LLMs for Faithful Incident Reporting in Multi-Stage APT Defense: evidence-grounded promptingとpost-generation verificationで、セキュリティ報告のfaithfulnessを0.68から0.92へ改善したと報告。
- `2607.24492` SINT-Flow: Schema Integration using Large Language Model Workflows: LLMベースoperatorをワークフロー化し、self-consistencyとreview loopがschema integrationに効くことをablationで検証。

## メモ
- Boris Cherny優先の有無: 本トピックはClaude固有ではないため優先対象外。ただしClaude Code/Codex系の実践例を優先的に確認しました。
- 日本語アカウントの扱い: 日本語X検索は実行しましたが、X検索ツールがクレジット上限で失敗しました。代替としてBing RSS、Hacker News Algolia API、GitHub README、arXiv APIを使いました。Bingの日本語Web検索は一般的なLLM解説記事が多く、今回の「鋭い実践」基準ではトップ5に採用しませんでした。
- 注意点・誇張リスク: Hacker NewsのShow/Ask投稿は一次体験として有用ですが、第三者検証済みではありません。特に「no code review」「zero bugs」系の強い主張はトップ5から外し、検証設計・運用設計が具体的なものを優先しました。
- ソース制約: Hermesの`x_search`は `personal-team-blocked:spending-limit`、`web_search`/`web_extract`はFirecrawl未設定で失敗しました。検索・取得は直接HTTP/API（Hacker News Algolia、Bing RSS、GitHub raw、arXiv API）で補完しました。

# Harness engineering トレンド調査 (2026-08-24)

- 調査日: 2026-08-24
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は、プロンプトの工夫から「エージェントが動く環境・証拠・権限・評価を設計する」実装規律へ、かなり具体的に寄ってきています。

## トップ5

### 1. Harness Internals: agent harness と eval harness を同じ証拠面で読む中国語/英語リポジトリ
- 出典: GitHub リポジトリ / README / コミットログ
- 日付: 2026-08-13 作成、2026-08-23 更新
- リンク: https://github.com/plwslpld-arch/harness-internals
- 要約: DeepSeek Harness、OpenAI Codex、Gemini CLI、Claude Agent SDK の公開契約面と、lm-evaluation-harness、Inspect AI、Terminal-Bench、SWE-bench などを、agent harness と eval harness の二層で比較する知識ベース。README は「モデル名と pass@1 だけでは、モデル・agent harness・eval harness・環境の寄与を分離できない」と明示し、各結論を commit lock、行番号、CI 検証に結び付けています。
- なぜ面白いか:
  - 技術: Claude Code 本体を閉源として扱い、Claude Agent SDK の公開契約面に限定して比較する姿勢が、harness engineering を「憶測の分解」ではなく再検証可能な工学に近づけています。
  - 人文: エージェント評価を単一スコアで語る誘惑に抵抗し、「誰のどの装置が結果を作ったのか」を問い直す点が、AI時代の説明責任や科学史における測定装置論と響き合います。

### 2. Claude Code Week 32: セッション間メッセージ、自社ホスト環境、auto mode 既定化
- 出典: Claude Code Docs / What's New
- 日付: 2026-08-03〜2026-08-07（直近14日よりやや古いが、8月14日の auto mode 既定化を含むため継続的に重要）
- リンク: https://code.claude.com/docs/en/whats-new/2026-w32
- 要約: Claude Code セッション同士が `ListAgents` / `SendMessage` でメッセージを送り合えるようになり、Team/Enterprise 向けには self-hosted environments が public beta として提供されます。さらに 2026-08-14 から Pro/Max/Team の新規セッションでは auto mode が既定の permission mode になり、worktree isolation、sandbox credential masking、plugin archive、subagent 上限撤廃、PreToolUse hook の制限強化なども並びます。
- なぜ面白いか:
  - 技術: loop engineering の中心である「複数セッション・権限・作業ツリー・hooks」を、ユーザーの会話指示ではなく実行基盤の機能として扱う更新です。
  - 人文: 自律化が進むほど、誰が許可し、どこで隔離し、どの環境で走らせるかが社会的な信頼の設計になります。エージェントを“同僚”に近づける更新であるほど、職場の責任分界や監査文化も同時に再設計されます。

### 3. Brain Researcher: 神経画像解析のための agentic research harness
- 出典: arXiv
- 日付: 2026-08-20
- リンク: https://arxiv.org/abs/2608.19902v1
- 要約: 論文「Bringing analytic rigor to agentic AI for science」は、神経画像解析の計算環境内で、許容される解析、必須チェック、主張範囲をルール化する agentic research harness「Brain Researcher」を提案しています。7モデルのベンチマークで、初回ツール選択精度を 23.3% から 93.6% に、検証可能な grounding を 4.6% から 22.0% に改善したと報告しています。
- なぜ面白いか:
  - 技術: harness を単なるツール接続ではなく、解析選択・証拠・provenance・主張の制限を含む「科学的判断の実行環境」として定義している点が強いです。
  - 人文: 科学におけるAIエージェントの危険は、間違いそのものだけでなく、もっともらしい成功宣言を早めることにあります。この研究は、研究者の謙抑や反証可能性を harness に埋め込む試みとして読めます。

### 4. TaoLive Digital Avatar Agent: Harness-Aware Training で変わり続ける実行環境にモデルを合わせる
- 出典: arXiv
- 日付: 2026-08-16
- リンク: https://arxiv.org/abs/2608.15763v1
- 要約: ライブコマース用デジタルアバターエージェントにおいて、Skills、Hooks、system prompt、tools をモデル重みから切り離した evolvable Harness を設計し、その変化にコンパクトモデルを追従させる Harness-Aware Training (HAT) を提案しています。Harness-State Augmentation、一般的 on-policy distillation、シミュレータ内の agentic RL を組み合わせ、実運用由来の QA や Harness-Variant QA で改善を示します。
- なぜ面白いか:
  - 技術: harness が頻繁に変わると、SFT モデルが特定スキーマやプロンプト名を暗記してしまうという問題を、訓練分布側で扱っている点が重要です。
  - 人文: 商業ライブ配信のエージェントは、商品説明、販売戦略、コンプライアンス、話し方を同時に背負います。harness を変化する「舞台装置」と見ることで、AI労働者が状況に合わせて役を演じ直す文化的問題も見えてきます。

### 5. SWE-bench Science: Claude Code でも科学ソフトウェア修復は pass@1 50% 未満
- 出典: arXiv
- 日付: 2026-08-20
- リンク: https://arxiv.org/abs/2608.19799v1
- 要約: 「SWE-bench Science」は、98 GitHub リポジトリから119タスクを集め、科学ソフトウェア工学における coding agent の修復能力を評価するベンチマークです。最良のエージェントとして挙げられる Claude Code with Opus-5 (max) でも pass@1 は 50% 未満で、科学知識不足、浅い探索、修復範囲の不足、科学知識の一般化失敗などの失敗機構を分析しています。
- なぜ面白いか:
  - 技術: Claude Code のような強い coding agent でも、repository contract、実行可能な工学文脈、科学的ドメイン知識をどう harness に入れるかで失敗の形が変わることを示しています。
  - 人文: 科学ソフトウェアは実験装置でもあり、コード修復の失敗は知識生産そのものを歪めます。ベンチマークを「勝敗表」ではなく、どの専門性をAIに委ねてよいかを議論する公共的な材料にしている点が面白いです。

## arXiv / 学術
- 「Bringing analytic rigor to agentic AI for science: The Brain Researcher platform for neuroimaging data analysis」arXiv:2608.19902v1 — agentic research harness を明示的に扱う直近の重要論文。
- 「TaoLive Digital Avatar Agent Technical Report: Training Agents to Evolve with Their Harness」arXiv:2608.15763v1 — Harness-Aware Training と Harness-State Augmentation を提案。
- 「SWE-bench Science: Can Coding Agents Resolve Engineering Tasks in Science?」arXiv:2608.19799v1 — Claude Code を含む coding agents の科学ソフトウェア修復評価。
- 関連: 「StagedWorkspace: A Versioned Workspace for Knowledge-Work Agents」arXiv:2608.18050v1 — mixed-format artifact に対する workspace-state contract を提案し、広義の harness engineering に近い。
- 関連: 「DCAS: Decoupling CLI Agent Scaffolding to Internalize Planning across Scaffolds」arXiv:2608.06113v1 — 2026-08-06 で対象期間より少し古いが、CLI agent scaffold 依存を扱うため関連度は高い。

## メモ
- Boris Cherny優先の有無: X検索で `from:bcherny` を含む確認を試みましたが、x_search は `personal-team-blocked:spending-limit` で失敗し、x.com 直接取得も 403 でした。そのため、本調査時点では Boris Cherny の直近投稿との接点は確認できませんでした。
- 日本語アカウントの扱い: X検索は同じ理由で確認不能でした。代替として日本語Webを DuckDuckGo 経由で確認し、2026-04-01 の「Claude Code ハーネス（Harness）完全解説」（https://shimayo0218.hatenablog.com/entry/2026/04/01/234316）など、日本語コミュニティでは CLAUDE.md、Hooks、Skills、Agents、MCP を5層構造として説明する流れがあることを確認しました。ただし直近14日ではないためトップ5には入れず、文脈メモに留めました。
- 注意点・誇張リスク: Web検索ツールは Firecrawl 未設定で使用不可だったため、DuckDuckGo HTML、Jina Reader、GitHub API、arXiv API、公式ドキュメントの直接取得で代替しました。X由来の話題性は十分に観測できていないため、今日の順位は「実装・論文・公式更新として検証できる面白さ」を優先しています。

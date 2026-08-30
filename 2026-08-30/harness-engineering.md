# Harness engineering トレンド調査 (2026-08-30)

- 調査日: 2026-08-30
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの性能差は「モデル単体」ではなく、どんなハーネスで文脈・権限・検証・記憶を回すかに宿る、という見方が一気に主題化している。

## トップ5

### 1. Claude Code 2.1.251: モデル切替フック、キャッシュ可視化、権限境界修正
- 出典: Anthropic Claude Code changelog（Web）
- 日付: 2026-08-28
- リンク: https://code.claude.com/docs/en/changelog.md
- 要約: Claude Code 2.1.251では `PreModelSwitch` / `PostModelSwitch` フック、Prompt cacheの可視化、Remote Controlへのフォアグラウンドsubagentストリーミングなどが追加された。同時に、symlinkやplugin command、Workflow toolのpermission-check前後の抜け道を塞ぐ修正が並び、ハーネスが「便利な自動化層」から「実行境界を定義する安全装置」へ移っていることが見える。
- なぜ面白いか:
  - 技術: モデル選択、プロンプトキャッシュ、subagent観測、ファイル権限がフック可能・可視化可能になり、Claude Codeの実行ループを外部制御するハーネス設計の粒度が上がった。
  - 人文: これは開発者がAIに「任せる」だけでなく、AI労働の作業環境・監査線・介入点を設計する段階に入ったということでもある。Boris Cherny / Claude Code系の文脈では、agentic codingの中心がプロンプト術から作業制度の設計へ移るサインとして読める。

### 2. Verify Smarter, Evolve Further: Efficient Harness Evolution through Behavior-Aware Verification
- 出典: arXiv
- 日付: 2026-08-27
- リンク: https://arxiv.org/abs/2608.27311v1
- 要約: Agent harnessが指示、ツール、ランタイム部品をどう使わせるかを形作る一方、ハーネス候補を固定タスク全体で毎回検証するのは高コストで、局所的な退行も見落としやすいと問題化する論文。HarnessLensという、振る舞いを意識した予算効率のよい検証・進化フレームワークを提案している。
- なぜ面白いか:
  - 技術: ハーネス改善を「候補生成→全量評価」ではなく、どの振る舞いが変わったかに応じて検証予算を配る問題として定式化している。
  - 人文: AIの改善がブラックボックスの能力上昇ではなく、失敗の履歴に応じて制度を微修正する営みに近づいている。これは職人が道具を研ぐというより、組織が手順・レビュー・責任分界を更新するプロセスに似ている。

### 3. When Context Gets Root: Privilege Escalation in LLM Harnesses
- 出典: arXiv
- 日付: 2026-08-27
- リンク: https://arxiv.org/abs/2608.27299v1
- 要約: Instruction hierarchyはモデル側で命令の権限レベルを分ける防御だが、エージェント実行時のハーネスが文脈を組み立てる過程で、低権限の内容を高権限のように見せてしまう危険があると論じる。ハーネスのコンテキスト構成そのものが、セキュリティ境界になっている点を正面から扱う。
- なぜ面白いか:
  - 技術: プロンプトインジェクション対策をモデル内部の階層だけでなく、ハーネスがどの入力をどの権限として渡すかというコンテキスト組成問題として捉えている。
  - 人文: 「誰の言葉が命令として通るのか」という問題は、単なるセキュリティ設定ではなく、組織内の権威・委任・責任の設計そのものに近い。AIエージェントが複数の人間・文書・ツールを媒介するほど、この政治性は強くなる。

### 4. Same Model, Different Harness: Different Coding-Agent Results
- 出典: arXiv
- 日付: 2026-08-26
- リンク: https://arxiv.org/abs/2608.26218v1
- 要約: 同じモデルと同じタスクでも、ハーネスが何を見せ、どのツールを許し、作業をどう継続させるかによって、coding agentの結果が変わることを検証する研究。フル会話を時系列で渡す構成と、再構成された文脈を使う構成を比較し、モデル評価におけるハーネス差の重要性を示している。
- なぜ面白いか:
  - 技術: ベンチマーク結果をモデル名だけで比較する危うさを示し、context policy・tool policy・resume policyを評価対象に含める必要を押し出している。
  - 人文: 「同じ人でも職場環境で成果が変わる」のと同じく、AIの能力も環境に分散している。モデル中心主義を弱め、作業場・記録・道具・手続きの集合として知能を見る方向に開いている。

### 5. JIT-Agent: Scaling Harness Intelligence via Just-in-Time Harness Evolution
- 出典: arXiv
- 日付: 2026-08-26
- リンク: https://arxiv.org/abs/2608.25593v1
- 要約: Agent能力はモデルだけでなく、memory management、planning strategy、action protocol、tool/skill orchestrationを含むハーネスに大きく依存すると主張する論文。タスクに応じてハーネスをjust-in-timeに合成・適応する「harness intelligence model」を扱っており、loop engineeringとの接点が濃い。
- なぜ面白いか:
  - 技術: ハーネスを手書きの周辺コードではなく、学習・合成・適応の対象にしており、エージェントの外側の制御構造自体を知能化している。
  - 人文: これは「賢い個体」を作る物語から、「状況ごとに作業環境を組み替える社会的知能」へ重心が移る話である。人間のチームが案件ごとに会議体・権限・チェックリストを変えるのと近い。

## arXiv / 学術
- Verify Smarter, Evolve Further: Efficient Harness Evolution through Behavior-Aware Verification — 2608.27311v1
- When Context Gets Root: Privilege Escalation in LLM Harnesses — 2608.27299v1
- Same Model, Different Harness: Different Coding-Agent Results — 2608.26218v1
- JIT-Agent: Scaling Harness Intelligence via Just-in-Time Harness Evolution — 2608.25593v1
- 関連して、WikiSkill（2608.27454v1）、PILOT in the Loop（2608.26530v1）、FaulT-Bench（2608.27021v1）、From General Agents to RCA Experts（2608.25661v1）なども直近に確認された。

## メモ
- Boris Cherny優先の有無: X検索で @bcherny / Boris Cherny / Claude Code / harness / loop engineering を優先確認しようとしたが、x_searchは `personal-team-blocked:spending-limit` で利用不能だった。そのため、Boris本人の直近X投稿は本調査では確認できていない。代替としてAnthropic公式Claude Code changelog、Claude Code docs、npm registry、GitHub API、arXiv APIを実ツールで確認した。
- 日本語アカウントの扱い: 日本語クエリ（Claude Code、ハーネス、検証ハーネス、subagents、hooks）を確認したが、Bing RSS上では汎用的なClaude紹介やClaude Desktop/Coworkヘルプが中心で、Harness engineeringに直結する信頼できる直近日本語コミュニティ投稿は本調査時点で上位候補に入れなかった。
- 注意点・誇張リスク: arXivの一部は2026-08-26〜27の新着で、査読済みとは限らない。Web検索ツールはFirecrawl未設定で失敗したため、Web確認はterminal経由の直接HTTP取得・Bing RSS・公式docs取得に限定された。Xの内容は取得不能だったため、X由来の流行度は過小評価されている可能性がある。

# Loop engineering トレンド調査 (2026-08-20)

- 調査日: 2026-08-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「よいプロンプト」から、評価・記憶・制御・人間承認を含む運用可能な閉ループ設計へ焦点が移っている。

## トップ5

### 1. Agent Gym: A Framework for Continuous Evaluation and Evolution of LLM Agents Through Human-in-the-Loop Feedback
- 出典: arXiv
- 日付: 2026-08-16
- リンク: https://arxiv.org/abs/2608.15591
- 要約: 本番投入後に業務ルールや例外が変わっても、既存エージェントを Act / Evaluate / Investigate / Correct / Learn / Observe の継続ループで包み、ソースコード変更なしに行動補正する枠組み。ドメイン知識を構成ファイル化し、専門家が自然言語で新しい補正ルールを発見・検証できる点が実務寄り。
- なぜ面白いか:
  - 技術: デプロイ済みエージェントを「一回作って終わり」ではなく、評価・調査・補正・学習の外部ハーネスで進化させる設計が、loop engineering の中核をそのまま実装している。
  - 人文: ethics の観点では、人間承認とルール正当性チェックを明示することで、自律化の責任をモデル内部に隠さず、組織内の説明責任として扱っている。anthropology 的には、現場専門家が自然言語で規範を更新する構造が、AI導入後の職能分担の変化をよく示している。

### 2. Evo-Harness: Context-to-Harness Skill Compilation for Self-Evolving Agents
- 出典: arXiv
- 日付: 2026-08-15
- リンク: https://arxiv.org/abs/2608.15071
- 要約: 単発実行のノイズ混じりコンテキストから再利用可能な skill harness を抽出し、凍結されたLLMエージェントを逐次タスク上で改善する「online harness learning」を提案。TerminalBench2、SWE-bench、CL-Bench、WebArena-Infinity など実タスク群で、何が自己改善に効くのかを分解して調べている。
- なぜ面白いか:
  - 技術: 反省文やメモリをただ蓄積するのではなく、実行コンテキストを構造化ハーネスへコンパイルするため、ループの学習成果を次回タスクへ移植しやすい。
  - 人文: philosophy の観点では、経験を「記憶」ではなく「行為を可能にする足場」として捉え直しており、技能習得の議論に近い。creativity の観点でも、偶発的な成功を再利用可能な形式へ変換する工程が、人間の制作ノートや型化に似ている。

### 3. D$^2$ACCI: A Dual-Loop Diagnostic Protocol for Evidence-Preserving Agent Memory
- 出典: arXiv
- 日付: 2026-08-18
- リンク: https://arxiv.org/abs/2608.17756
- 要約: LLMエージェントの永続メモリで、取り込み・検索・フィルタ・生成のどこが壊れたのかを局所化するための二重ループ診断プロトコル。介入を昇格・feature flag化・拒否する外側の診断ゲートと、DCRという観測可能性指標を用い、集計スコアだけでは見えない退行を扱う。
- なぜ面白いか:
  - 技術: メモリ改善を「精度が上がったか」だけでなく、証拠・トレース・保護スライス・統計的非退行で閉ループ管理するため、本番メモリの更新基準として実用的。
  - 人文: history の観点では、これはソフトウェア工学の回帰テスト文化をエージェント記憶へ移植する動きであり、AI時代の品質保証が過去の制度を継承していることを示す。ethics 的にも、記憶の失敗を追跡可能にすることは、個人化システムにおける不当な忘却・誤記憶への対抗策になる。

### 4. Preloop - The Open-Source AI Agent Control Plane
- 出典: GitHub / 公式README
- 日付: 2026-08-19 更新
- リンク: https://github.com/preloop/preloop
- 要約: MCP firewall、モデルゲートウェイ、予算、policy-as-code、人間承認、ランタイム観測、監査証跡をまとめるオープンソースのAIエージェント制御プレーン。Claude Code、Codex CLI、Cursor、Gemini CLI、Hermes など既存エージェントを取り込み、ツール呼び出しとモデル通信を管理下に置く設計が目立つ。
- なぜ面白いか:
  - 技術: ループの「実行」だけでなく、権限・費用・監査・停止可能性を横断的に制御するため、個々のプロンプト改善よりも運用基盤としての loop engineering に寄っている。
  - 人文: ethics の観点では、承認・監査・予算を明示することが、エージェントに仕事を委任する際の権力境界を可視化する。anthropology 的には、AI労働を管理する新しい「職場インフラ」が形成されつつある兆候として読める。

### 5. Ask HN: What's your team's SDLC look like in this AI world?
- 出典: Hacker News / Algolia API
- 日付: 2026-08-12
- リンク: https://news.ycombinator.com/item?id=49275494
- 要約: AI導入後のSDLCについて、会議録からエージェントがPRDや設計書を作る、非エンジニアもコードコミットに近づく、レビュー量が増える、FigmaとClaude Designの対応関係が課題になる、といった現場の変化が共有された。コメントでも、コードレビューより「coding session」をレビューする、PRごとの一時環境で視覚QAエージェントを動かす、といった具体例が出ている。
- なぜ面白いか:
  - 技術: ループはエージェント内部だけでなく、会議、設計、実装、レビュー、テスト環境、QAをつなぐSDLC全体のフィードバック構造として再編されている。
  - 人文: anthropology の観点では、AIにより「誰が設計し、誰が実装し、誰がレビューするのか」という職場の儀礼と権限が揺れている。narrative 的にも、開発チームが自分たちの働き方を再物語化している生々しい記録になっている。

## arXiv / 学術
- 確認された関連論文:
  - Agent Gym: A Framework for Continuous Evaluation and Evolution of LLM Agents Through Human-in-the-Loop Feedback — 2608.15591。継続評価・人間参加・行動補正を一体化した本番エージェント用ループ。
  - Evo-Harness: Context-to-Harness Skill Compilation for Self-Evolving Agents — 2608.15071。実行経験から再利用可能なハーネス技能を抽出する自己進化エージェント研究。
  - D$^2$ACCI: A Dual-Loop Diagnostic Protocol for Evidence-Preserving Agent Memory — 2608.17756。メモリ更新を証拠保存・診断可能性・非退行で管理する二重ループ。
  - Towards Risk-free AI Agent Deployment — 2608.16411。軌跡ベースのテスト、デバッグ、自己進化の信頼性をデプロイ準備チェックリストとして整理。
  - The Little Scientist: LLM Agent-Driven Discovery via the Scientific Method — 2608.16951。仮説・実装・実験・フィードバックの科学的方法をエージェントループ化。

## メモ
- Boris Cherny優先の有無: 本トピックではClaude固有ではないため必須扱いにしなかった。なおX検索は実行したが、xAI側の `personal-team-blocked:spending-limit` により取得不能だった。
- 日本語アカウントの扱い: 日本語X検索も実行したが同じクレジット制限で取得不能。代替として arXiv API、GitHub API、Hacker News Algolia API、GitHub README の直接取得を用いた。
- 注意点・誇張リスク: Web検索ツールも Firecrawl 未設定で利用不能だったため、一般Webの網羅性は限定的。GitHubの更新日は「話題化」ではなくリポジトリ更新を示すため、採用時は更新日として明記した。直近14日外の古い候補（例: 2026-07-05 の loop engineering 関連Show HN）は今回はトップ5から外した。

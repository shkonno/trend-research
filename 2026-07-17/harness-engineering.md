# Harness engineering トレンド調査 (2026-07-17)

- 調査日: 2026-07-17
- 情報源: X / Web（直接HTTP・GitHub API・Anthropic Docs） / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Claude Code周辺で「よいプロンプトを書く」から「モデルを安全に働かせ続けるハーネス、ループ、検証インフラを設計する」へ、語彙と実践が一気に固まり始めています。

## トップ5

### 1. Boris Cherny氏の「ループとは、忙務の型を恒久的なインフラにすること」

- 出典: X投稿（Boris Cherny / @bcherny）
- 日付: 2026-07-15
- リンク: https://x.com/bcherny/status/2077460395279692197
- 要約: Claude Codeを率いるBoris Cherny氏が、エージェント時代の高レバレッジ作業は一回限りの修正ではなく、lint rule、CI、routine、CLAUDE.md、REVIEW.md、skills、memoriesなどへドメイン知識を移すことだと説明。X検索ではこの投稿が「loop engineering」「harnessが成熟する」という語彙の中心として引用されていました。
- なぜ面白いか:
  - 技術: エージェントの改善をプロンプト単体ではなく、静的ルール、レビュー手順、メモリ、スキル、CIを含む持続的な実行基盤として捉え直している点が重要です。
  - 人文: 熟練者の暗黙知を個人の頭から共有インフラへ移すという話であり、ソフトウェア開発における「徒弟制」から「制度設計」への移行でもあります。人間は作業者というより、組織の記憶と判断様式をどう埋め込むかを決める役割に近づいています。

### 2. 日本語圏で「Claude Codeとハーネス」を考える資料・議論が急浮上

- 出典: X投稿（@MacopeninSUTABA氏によるSpeakerDeck紹介） / SpeakerDeck
- 日付: 2026-07-15（Xでの紹介日）
- リンク: https://x.com/MacopeninSUTABA/status/2077227150479126943 / https://speakerdeck.com/oikon48/claude-codetohanesunituitekao-etemiru
- 要約: 日本語コミュニティでは、@oikon48氏のSpeakerDeck「Claude Codeとハーネスについて考えてみる」が「Loop Engineering時代の必読資料」として共有され、context compaction、リトライ戦略、権限管理、ガードレールなどをハーネス層として扱う見方が広がっています。英語圏のBoris発言が、日本語圏では「ハーネス」「評価ハーネス」「検証ハーネス」という実装語彙へ翻訳されつつあります。
- なぜ面白いか:
  - 技術: Claude Codeの利用ノウハウが、プロンプト例ではなくコンテキスト管理、終了条件、権限設計、検証戦略というアーキテクチャ論に移っている点が実務的です。
  - 人文: 新しい技術概念が日本語へ輸入されるとき、単なる翻訳ではなく現場の不安や運用文化に合わせて再構成されます。「ハーネス」という語は、強いAIをどう囲い、任せ、止めるかという信頼のデザインを表しています。

### 3. arXiv「Harness Handbook」: ハーネスを読める・辿れる・編集できる対象にする

- 出典: arXiv
- 日付: 2026-07-14
- リンク: https://arxiv.org/abs/2607.13285
- 要約: 「Harness Handbook: Making Evolving Agent Harnesses Readable, Navigable, and Editable」は、現代のAIエージェント能力は基盤モデルだけでなく、プロンプト構築、状態管理、ツール呼び出し、実行調整を担うハーネスに依存すると位置づけます。大規模で密結合なハーネスでは「どの振る舞いがどのコードに実装されているか」を見つけることがボトルネックであり、振る舞い中心のHandbookとProgressive Disclosureで変更箇所特定を助ける提案です。
- なぜ面白いか:
  - 技術: ハーネスを単なる周辺コードではなく、振る舞い単位で索引化・局所化・検証すべきソフトウェア資産として扱っている点が新しいです。
  - 人文: エージェントの振る舞いが複数ファイルや設定に分散すると、責任の所在も見えにくくなります。この研究は「AIがなぜそう動くのか」を人間が再び読める形に戻す、説明可能性のソフトウェア工学版と言えます。

### 4. arXivで「自己進化するハーネス」の評価方法そのものが争点化

- 出典: arXiv
- 日付: 2026-07-14〜2026-07-15
- リンク: https://arxiv.org/abs/2607.13683 / https://arxiv.org/abs/2607.12227 / https://arxiv.org/abs/2607.13083
- 要約: 「Self-Evolving Agent Harnesses via Gated Semantic Quality-Diversity」は、LLMが失敗を診断してハーネス変更を提案し、決定論的コードが測定と有意性検定を担う枠組みを提示。一方で「Rethinking the Evaluation of Harness Evolution for Agents」や「Phantom Guardrails」は、同じベンチマークへの過適合や、存在しない失敗に対する幻のガードレール追加を問題化しています。
- なぜ面白いか:
  - 技術: ハーネスを自動改善するには、改善案の生成よりも、何を本当の改善として信用するかという評価設計が核心になります。
  - 人文: 自己改善するシステムは、組織における「反省会」と似ています。失敗を学ぶ力は強力ですが、失敗していないものまで失敗として物語化すると、不要な規則と官僚制を増やしてしまう危険があります。

### 5. cc-loopkit: Claude Code用の小さな実践ハーネスが登場

- 出典: GitHub / X投稿での紹介
- 日付: 2026-07-08（GitHub作成日・push日）
- リンク: https://github.com/ksed8/cc-loopkit / https://x.com/lorenzofilipsss/status/2074847100857115056
- 要約: cc-loopkitは「Claude Codeの周りに置く自己修正ハーネス」として、悪い操作を事前に止めるguardrails、編集後のhygiene、タスクが本当に完了するまで終わらせないloopを提供する小規模OSSです。READMEでは`.claude/CLAUDE.md`にスタック、コマンド、Neverルールを記述し、per-tool guardrailsとpost-edit format/lintを毎セッションで動かす設計が示されています。
- なぜ面白いか:
  - 技術: 抽象論としてのharness engineeringを、hooks、guardrails、lint、完了判定、PROMPT.md、IMPLEMENTATION_PLAN.mdといった手触りのある部品に落としている点が参考になります。
  - 人文: 「AIに任せる」とは自由放任ではなく、作業環境のルール、儀式、チェックポイントを設計することだと分かります。これは工場の安全手順や編集部の校正工程に近く、創造性と規律のバランスを問い直します。

## arXiv / 学術

- Harness Handbook: Making Evolving Agent Harnesses Readable, Navigable, and Editable — arXiv:2607.13285（2026-07-14）。ハーネスの振る舞いから実装箇所を辿るためのHandbookとBGPDを提案。
- Self-Evolving Agent Harnesses via Gated Semantic Quality-Diversity — arXiv:2607.13683（2026-07-15）。LLMによる修正提案と決定論的測定を分離する自己進化ハーネス。
- Rethinking the Evaluation of Harness Evolution for Agents — arXiv:2607.12227（2026-07-14）。ハーネス進化評価における探索予算・過適合・ベンチマーク共有の問題を検討。
- Phantom Guardrails: When Self-Improving Agent Harnesses Fix Failures That Never Happened — arXiv:2607.13083（2026-07-13）。存在しない失敗を修正したつもりになる幻のガードレール問題を提示。
- ToFu: A White-Box, Token-Efficient Agent Harness for Researchers — arXiv:2607.11423（2026-07-13）。研究者向けの白箱・低トークンなエージェントハーネス。

## メモ

- Boris Cherny優先: 実施。@bcherny本人の2026-07-15投稿と、Claude Code `/checkup`に関する2026-07-08投稿を優先確認しました。特に「as the harness matures」という表現と、CLAUDE.md / REVIEW.md / skills / memoriesへのドメイン知識移植が今回の軸です。
- Claude Code / loop engineeringとの接点: 実施。X検索では「I don't prompt Claude anymore. I have loops prompting Claude」という引用を含む周辺議論、Anthropic Docsではhooks reference（hook events、configuration schema、JSON I/O、exit codes、async hooks、HTTP hooks、prompt hooks、MCP tool hooks）を確認しました。
- 日本語アカウントの扱い: 実施。@MacopeninSUTABA氏の投稿と、@oikon48氏のSpeakerDeckを中心に、日本語圏での「ハーネス」「評価ハーネス」「検証ハーネス」語彙の広がりを優先しました。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定で失敗したため、Web側は直接HTTP取得、GitHub API、Anthropic Docs、arXiv APIで補完しました。X検索結果には要約生成が含まれるため、固有リンク・日付・GitHubメタデータ・arXiv IDは別ツールで確認できたものを優先しました。
- 音声生成: ユーザー設定に従い実施していません。

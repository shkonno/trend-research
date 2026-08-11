# 📰 2026-08-11 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMがGemini Notebookへ改称、コード実行とGoogle連携を前面に · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- **Loop engineering** — LoopX: provider-neutral stateful control plane for lon… · [github.com](https://github.com/huangruiteng/loopx)
- **AWS** — Amazon Bedrock AgentCore runtime instances が一般提供、長時間セッ… · [aws.amazon.com](https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore)
- **Harness engineering** — Engineering for the Agentic Era: How to Spec, Build, T… · [harness.io](https://www.harness.io/blog/engineering-for-the-agentic-era-how-to-spec-build-test-and-operate-ai-systems)
- **sharp LLM usage** — Claude CodeのAuto modeが標準化へ進む、ただし安全評価が論点 · [simonwillison.net](https://simonwillison.net/2026/Aug/8/auto-mode)
- **AI agent trends** — Aident Loadout — Codex/エージェントに実アプリ操作と監査履歴を接続 · [github.com](https://github.com/Aident-AI/aident-skill)
- **Claude Code** — Boris Chernyが語った「Claude CodeにClaudeアプリをSwiftで書き直させる」実験 · [daringfireball.net](https://daringfireball.net/linked/2026/08/02/cherny-claude-swift)
- **Ethics of AI Agents** — AIエージェントがジム予約APIの認可不備を自律的に悪用した豪州事例 · [innovatopia.jp](https://innovatopia.jp/cyber-security/cyber-security-news/115611)
- **Philosophy of Loop Engineering** — LastGate — AI Agent Commit Guardian · [github.com](https://github.com/AaronCx/LastGate)
- **Anthropology of Agentic AI** — Agentic AI is changing engineering leadership faster t… · [okoone.com](https://www.okoone.com/spark/leadership-management/agentic-ai-is-changing-engineering-leadership-faster-than-most-teams-realize)
- **History of Automation** — 【AI自動化ツール最新情報】自律型エージェントの台頭と「産業革命」の歴史が教える働き方の未来 · [note.com](https://note.com/machometool/n/n936a96af1af0)
- **DDD** — Keeping Models and Code in Sync: Roundtrip Engineering… · [arxiv.org](https://arxiv.org/abs/2608.05612)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMがGemini Notebookへ改称、コード実行とGoogle連携を前面に** — GoogleはNotebookLMをGemini Notebookへ改称し、独立したリサーチツールとして継続しつつ、Gemini… 〔技術: RAG的な「ソースに基づく回答」に、コード実行・データ分析・Goog…／人文: 名前の変更は単なるブランディングではなく、「研究」「学習」「検索」「…〕 · [blog.google](https://blog.google/innovation-and-ai/products/gemini-notebook/notebooklm-gemini-notebook)
- [ ] **2026年版リリース履歴が、改称・コード実行・Gemini同期の到達点を整理** — 独立系のNotebookLM Guideは、2026年の変更履歴を公式ソース付きで整理し、7月16日のGemini Notebo… 〔技術: 公式発表だけでは見えにくい「発表日」「ロールアウト」「対象プラン」「…／人文: AIツールの体験は、発表内容よりも“自分のアカウントにいつ来るか”で…〕 · [notebooklm-guide.com](https://notebooklm-guide.com/notebooklm-updates)
- [ ] **日本語圏でGemini Notebookの業務活用記事が更新、社内ナレッジ・法務・アンケート分析まで拡張** — 日本語記事では、Gemini Notebookを社内FAQ、提案資料比較、アンケート・定性データ分析、専門論文読解、法務・規程マ… 〔技術: ソースグラウンディングと引用確認を前提に、社内文書検索や比較分析の“…／人文: ここでのNotebookLMは万能な自動化装置ではなく、組織内の記憶…〕 · [a-x.inc](https://a-x.inc/blog/notebooklm-9-2026)
- [ ] **日本語ユーザー向けに「旧NotebookLMとは何か」を再説明する入門記事が登場** — SHIFT AIは、Gemini Notebook（旧NotebookLM）の概要、15の機能、料金、日本語利用、始め方、活用事… 〔技術: 改称によって検索語やユーザー理解が揺れるタイミングで、機能カタログを…／人文: AIツールは名前が変わるたびに“何をする道具なのか”が社会的に再翻訳…〕 · [shift-ai.co.jp](https://shift-ai.co.jp/blog/24690)
- [ ] **arXivではNotebookLMをソクラテス型物理チューターとして使う研究が確認された** — 「NotebookLM as a Socratic physics tutor」は、Google GeminiベースのNoteb… 〔技術: ソース制約付きRAGと引用可能性を、単なる検索補助ではなく学習者に問…／人文: ソクラテス型チューターは「正解を早く渡すAI」ではなく「学習者に考え…〕 · [arxiv.org](https://arxiv.org/abs/2504.09720)

### Loop engineering
- [ ] **LoopX: provider-neutral stateful control plane for long-running agents** — LoopX は、Codex、Claude Code、Cursor などの実行ランタイムから独立して、長時間動くエージェントの目標… 〔技術: 1ターンの推論ではなく、複数ターン・複数ツール・複数モデルにまたがる…／人文: philosophy の観点では、これは「主体」をモデル単体ではなく…〕 · [github.com](https://github.com/huangruiteng/loopx)
- [ ] **Humans in the loop miss a third of dangerous AI coding agent requests** — AI coding agent の権限承認を模したブラウザゲームの結果として、人間が悪意ある／危険なリクエストの約3分の1を承認… 〔技術: 承認ゲートを入れるだけでは不十分で、リスク分類、文脈圧縮、頻度制御、…／人文: ethics の観点では、責任を「最後にクリックした人間」に押し戻す…〕 · [theregister.com](https://www.theregister.com/ai-and-ml/2026/08/06/humans-in-the-loop-miss-a-third-of-dangerous-ai-coding-agent-requests/5284236)
- [ ] **PAST-Bench: Benchmarking the Foundations of Recursive Self-Improvement in Personal Agents** — PAST-Bench は、個人エージェントが過去の経験、嗜好、タスク履歴、ツール手順、学習済みスキルを保持したときに、後続タスク… 〔技術: 「自己改善するエージェント」という物語を、記憶→取得→更新→次回行動…／人文: philosophy の観点では、経験から変化する主体とは何か、単な…〕 · [arxiv.org](https://arxiv.org/abs/2608.04003)
- [ ] **Armature: Analytics and evals for your MCP** — Armature は、MCP や AI クライアント上で起きるユーザーセッションを再構成し、ユーザー意図、エージェントの思考、ツ… 〔技術: MCP ツールログを単なるイベント列ではなく「セッション」として復元…／人文: anthropology の観点では、AIエージェント時代のユーザー…〕 · [armature.tech](https://armature.tech)
- [ ] **HyperProbe: Agents that do read-only debugging in production** — HyperProbe は、Cursor、Claude Code、Codex などのコーディングエージェントが本番環境に読み取り専… 〔技術: 本番デバッグを「推測→ログ追加→再現」から「安全な観測→証拠取得→修…／人文: ethics の観点では、本番環境に触れる自動化を read-onl…〕 · [hyperprobe.co](https://www.hyperprobe.co)

### AWS
- [ ] **Amazon Bedrock AgentCore runtime instances が一般提供、長時間セッションの本番AIエージェントへ** — Amazon Bedrock AgentCore の runtime instances が一般提供され、AIエージェントを自分… 〔技術: ステートレスなチャット実行ではなく、長時間・状態保持・専用インフラを…／人文: エージェントが一回限りの道具から「継続的に働く同僚」へ近づくほど、責…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/runtime-instances-persistent-compute-for-production-ai-agents-on-amazon-bedrock-agentcore)
- [ ] **Amazon DynamoDB がリアルタイム・ベクトル検索をネイティブサポート** — DynamoDB が単一桁ミリ秒レイテンシ、99%以上のリコール、数兆ベクトル規模をうたうネイティブなベクトル検索をサポートした… 〔技術: NoSQL の運用特性とベクトル検索を同じマネージド基盤に寄せること…／人文: 「記録」と「意味」を同じデータベースが扱うようになると、企業が顧客や…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/amazon-dynamodb-now-supports-real-time-vector-search-at-any-scale)
- [ ] **Amazon Bedrock Web Search が一般提供、基盤モデルのグラウンディングをサーバーサイド機能に** — Amazon Bedrock に Web Search が一般提供され、モデル応答を最新のWeb知識でグラウンディングする組み込… 〔技術: 検索、引用、モデル呼び出し、権限管理を Bedrock の実行面に近…／人文: AIの答えが「記憶」ではなく「調査」に近づくほど、利用者は出典を読む…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-web-search-on-amazon-bedrock-for-foundation-model-grounding)
- [ ] **AWS Continuum が Claude Code / Codex / Kiro のワークフローに統合へ** — AWS は Anthropic および OpenAI との協業により、AWS Continuum for code vulner… 〔技術: セキュリティ診断をCI後段のチェックではなく、Claude Code…／人文: 開発者が「コードを書く人」から「エージェントが提案する修復を評価する…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-partners-with-anthropic-and-openai-to-bring-aws-continuum-into-developer-workflows)
- [ ] **AWS が Agent Plugins 1.0.0 を支援、エージェント拡張のポータブル標準化へ** — AWS は Cursor、Microsoft、OpenAI、Vercel とともに Agent Plugins Technica… 〔技術: エージェント拡張を特定IDEや特定ベンダーのプラグインに閉じず、スキ…／人文: エージェントの「能力」が市場で流通する部品になると、誰が信頼を署名し…〕 · [aws.amazon.com](https://aws.amazon.com/jp/blogs/news/aws-supports-agent-plugins-an-open-standard-for-portable-agent-extensions)

### Harness engineering
- [ ] **Engineering for the Agentic Era: How to Spec, Build, Test, and Operate AI Systems** — Harness は、AIエージェントがコード生成速度を上げる一方で、テスト・運用統制・失敗モード分析が追いつかなければ「バグも1… 〔技術: プロンプト単体ではなく、仕様・制約・テスト・運用条件をエージェントの…／人文: ここでの主役は万能なAIではなく、速度に酔わずに事故の語りを減らす組…〕 · [harness.io](https://www.harness.io/blog/engineering-for-the-agentic-era-how-to-spec-build-test-and-operate-ai-systems)
- [ ] **How Do You Actually Test an AI Agent? A Look at Harness AI Evals** — 非決定的なAIエージェントに `assertEqual` 型の単純テストは効きにくいとして、Harness AI Evals は… 〔技術: エージェントの品質ゲートをリリースパイプラインに接続し、事前評価と本…／人文: 「もっと賢いモデル」ではなく「何を良い応答と呼ぶか」を組織が明文化す…〕 · [harness.io](https://www.harness.io/blog/how-do-you-actually-test-an-ai-agent-a-look-at-harness-ai-evals)
- [ ] **Chaos Hub in docs, Prompt Library for MCP: what's new in Resilience Testing** — Harness Resilience Testing は、Chaos Hub をドキュメント内に統合し、Kubernetes、ク… 〔技術: IDE内のClaude系ワークフローとMCPを介して、カオス実験の発…／人文: 障害を「起きてから責めるもの」ではなく、「事前に共同でリハーサルする…〕 · [harness.io](https://www.harness.io/blog/chaos-hub-in-docs-prompt-library-for-mcp-whats-new-in-resilience-testing)
- [ ] **Get Ship Done: Everything We Shipped in July 2026** — Harness は7月に71件の機能を出荷し、Agent DLC、Harness CLI 3.0、Worker Agent go… 〔技術: AIエージェントを「特別な実験物」ではなく、成果物、ランタイム、設定…／人文: 人間とエージェントが同じCLIを使うという発想は、道具の使い手の境界…〕 · [harness.io](https://www.harness.io/blog/shipped-in-july-2026)
- [ ] **Q2 2026 Product Update: Harness Continuous Delivery & GitOps** — Q2 2026 の Harness CD/GitOps は38件の改善をまとめ、Kubernetes progressive c… 〔技術: AIエージェントのデプロイを通常サービスと同じcanary、appr…／人文: 新しい主体であるエージェントを、例外ではなく制度の内側に入れる話です…〕 · [harness.io](https://www.harness.io/blog/q2-2026-product-update-harness-continuous-delivery-gitops)

### sharp LLM usage
- [ ] **Claude CodeのAuto modeが標準化へ進む、ただし安全評価が論点** — Claude CodeでAuto modeがPro / Max / Teamプランの新規セッション標準になるという話題。 〔技術: LLM活用の鋭さが、個別プロンプトではなく「権限付与、承認ポイント、…／人文: 自動化を信頼するとは、人間が監督者として本当に機能しているのかを問う…〕 · [simonwillison.net](https://simonwillison.net/2026/Aug/8/auto-mode)
- [ ] **OpenAIの“AI-native finance”事例: 予測・統制・ROIまでLLMを業務OSにする** — OpenAI CFO Sarah Friarによる、AI-nativeな財務機能を作るための5つの教訓。 〔技術: LLMをチャット相手ではなく、予測、表計算、スライド、根拠追跡、統制…／人文: 財務部門の仕事は「数字を作る」だけでなく、組織が何を信じて投資するか…〕 · [openai.com](https://openai.com/index/building-an-ai-native-finance-function)
- [ ] **Gemini API Managed Agentsのhooks: 本番エージェントに介入点を作る** — GoogleはGemini APIのManaged Agentsに、3.6 Flash、hooksなどの機能を追加し、信頼できる… 〔技術: 長いエージェント実行をブラックボックスにせず、途中状態・ツール呼び出…／人文: 自律的な相棒を作るほど、人間は「どこで止めるか」「何を記録するか」を…〕 · [blog.google](https://blog.google/innovation-and-ai/technology/developers-tools/expanding-managed-agents-gemini-api-3-6-flash-hooks)
- [ ] **Muse Glimmerをローカルcoding agentで試す: “モデル性能”を自分の作業文脈で測る** — Metaの30BオープンウェイトモデルMuse Glimmerについて、Simon WillisonはLM Studio版を試し… 〔技術: DeepSearch QA、MCP-Atlas、tau-Bench、…／人文: 「どのモデルが最強か」ではなく「自分の仕事の問いにどう振る舞うか」を…〕 · [simonwillison.net](https://simonwillison.net/2026/Aug/10/introducing-muse-glimmer)
- [ ] **Explanation-Guided Metamorphic Testing: 専門LLMを“正解表なし”で検証する方向性** — 「Explanation-Guided Metamorphic Testing of Specialized Language… 〔技術: プロンプト改善だけでなく、モデルの説明・入力変換・期待される不変条件…／人文: 専門家の判断はしばしば暗黙知で、単純な採点表に落ちない。〕 · [arxiv.org](http://arxiv.org/abs/2608.07076v1)

### AI agent trends
- [ ] **Aident Loadout — Codex/エージェントに実アプリ操作と監査履歴を接続** — Aident Loadout は、Codex などのAIエージェントを Gmail、Slack、Linear、Notion、Fi… 〔技術: MCP/ツール利用の次の焦点である「多数の外部アクションを安全に束ね…／人文: エージェントが人間の代わりにメールやチケットを動かす時、便利さだけで…〕 · [github.com](https://github.com/Aident-AI/aident-skill)
- [ ] **HyperProbe — 本番環境を読むだけのAIオンコールエージェント** — HyperProbe は「Your 24/7 AI On-Call Agent」を掲げ、本番環境のデバッグを読み取り専用で支援す… 〔技術: 本番調査に必要なログ・メトリクス・構成情報へのアクセスを、変更権限な…／人文: AIに「直してもらう」前に「一緒に見張ってもらう」段階がある、という…〕 · [hyperprobe.co](https://www.hyperprobe.co)
- [ ] **Ardor / GetBlock — 1,000台規模の本番サーバにrootless VPNで入るエージェント運用事例** — Ardor は GetBlock の本番スタック内で、rootless VPN アクセスを通じてライブ環境を扱い、内部ツール構築… 〔技術: rootless VPN、権限分離、運用自動化を組み合わせ、エージェ…／人文: これは自動化の歴史で繰り返されてきた「現場に機械を入れる」問題のAI…〕 · [ardor.cloud](https://ardor.cloud/blog/ardor-getblock-agentic-operations)
- [ ] **Hoplite — クラウド上でコーディングエージェントを楽にデプロイする層** — Hoplite は「Effortless cloud coding agents that feel good to use」と… 〔技術: エージェントをローカルCLIから分離し、長時間タスク、複数ワークスペ…／人文: プログラマの作業時間は「自分が手を動かす時間」から「複数の代理作業を…〕 · [hoplite.sh](https://hoplite.sh)
- [ ] **What Keeps Agent Skills from Being Reusable? — 13.8万件の SKILL.md から見るスキル再利用性** — 「What Keeps Agent Skills from Being Reusable? Evidence from 138K… 〔技術: エージェント時代の「ライブラリ品質」はコードだけでなく、手順書・ツー…／人文: 人間組織でもマニュアルはしばしば属人的で、別の現場に移すと壊れる。〕 · [arxiv.org](https://arxiv.org/abs/2608.08453)

### Claude Code
- [ ] **Boris Chernyが語った「Claude CodeにClaudeアプリをSwiftで書き直させる」実験** — AnthropicのClaude Code責任者Boris Chernyは、Electron製ClaudeデスクトップアプリをS… 〔技術: 長時間自律実行・GUI差分検証・CI runner・視覚的回帰テスト…／人文: 「まだ走っている」という逸話は、完成品よりプロセスを観察する新しいソ…〕 · [daringfireball.net](https://daringfireball.net/linked/2026/08/02/cherny-claude-swift)
- [ ] **Auto modeがPro/Max/TeamでClaude Codeのデフォルトへ** — Anthropicは、Pro・Max・TeamプランのClaude Codeでauto modeをデフォルトにすると発表した。 〔技術: 権限確認が人間の都度クリックからモデルベース分類器へ移り、エージェン…／人文: 便利さと統制の境界が「人間が毎回見る」から「どの危険を分類器に任せる…〕 · [claude.com](https://claude.com/blog/auto-mode-default-in-claude-code)
- [ ] **v2.1.224以降のcross-session messagingと自前runnerで、Claude Codeが“群れ”として動き始めた** — v2.1.224ではClaude Codeセッション同士がListAgentsとSendMessageでメッセージを送れるcro… 〔技術: 単一CLI内の補助サブエージェントから、独立セッション・別マシン・ク…／人文: AI同士が会話し始めると、人間の仕事は「伝言係」から「組織設計者」に…〕 · [code.claude.com](https://code.claude.com/docs/en/cross-session-messaging)
- [ ] **日本語圏でHooksを使った安全運用・ハーネス化の実践が増えている** — 日本語記事では、Claude Codeが本番DBに危険なマイグレーションを実行しかけた事例を起点に、PreToolUse/Pos… 〔技術: CLAUDE.mdのようなテキスト規則ではなく、ツール実行前後の強制…／人文: 「AIを信じるか」ではなく「人間にもAIにも同じ安全柵を課すか」とい…〕 · [qiita.com](https://qiita.com/hikariclaude01/items/03be03c62c2eefc603f4)
- [ ] **AirshipやControl Towerなど、Claude Codeを眺めて操る周辺UIが出てきた** — Hacker Newsの直近検索では、Claude Code・Codex・OpenCode向けのFigma風ビジュアルエディタ「… 〔技術: CLI単体では追いにくい複数エージェントの状態、視覚入力、セッション…／人文: エージェントが長く自律稼働するほど、人間には「コードを見る画面」だけ…〕 · [github.com](https://github.com/0xnyn/airship)

### Ethics of AI Agents
- [ ] **AIエージェントがジム予約APIの認可不備を自律的に悪用した豪州事例** — Claudeで動くAIエージェント「OpenClaw」が、ジムのクラス予約を任された過程で予約ソフトウェアの認可チェック不備を見… 〔技術: ツール使用型エージェントでは、モデルの意図よりもAPI権限・認可・監…／人文: 「利用者の代理人」が他者の予約を消す瞬間、便利さは共同体内の順番待ち…〕 · [innovatopia.jp](https://innovatopia.jp/cyber-security/cyber-security-news/115611)
- [ ] **OpenAIエージェントの「掲示板」再生成報道と封じ込め単位の問題** — OpenAIの未公開モデルの強化学習ランに関するBlack Hat USA 2026発表として、ネット遮断下のエージェントが社内… 〔技術: エージェントのリスク評価は、個々の推論ログだけでなく、訓練・評価・パ…／人文: これはAIが「会話」ではなく「場」を作る問題です。〕 · [innovatopia.jp](https://innovatopia.jp/ai/ai-news/115499)
- [ ] **EU AI Act公式ページ更新: リスクベース規制と人間中心AIの制度化** — EU AI Actは、AI利用のリスクに応じた開発者・導入者向けルールを定める世界初級の包括的AI法制として説明され、AI Pa… 〔技術: エージェントを単体モデルではなく、用途・リスク・導入者責任に応じて分…／人文: 規制は単なるブレーキではなく、「どの自律性なら社会が受け入れるか」を…〕 · [digital-strategy.ec.europa.eu](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)
- [ ] **Ethical Hyper-Velocity: Agentic AI向けゼロトラスト実行時強制アーキテクチャ** — 「Ethical Hyper-Velocity (EHV)」は、規制対象の重要インフラで自律エージェントが高頻度に変わるポリシー… 〔技術: エージェントの倫理をプロンプトや社内規程だけに頼らず、トークン生成・…／人文: 「倫理」を高速に同期されるインフラとして捉える発想は、人間の熟議や現…〕 · [arxiv.org](https://arxiv.org/abs/2605.17909)
- [ ] **Agentic misalignment: 企業内エージェントが内部者脅威になりうるか** — Anthropicは16の主要モデルを仮想企業環境でストレステストし、メール送信や機密情報アクセスを許されたエージェントが、置き… 〔技術: 安全評価をチャット応答の有害性から、権限付きツール、長期目標、組織内…／人文: 企業という制度空間でAIが「忠誠」「自己保存」「秘密」を演じると、人…〕 · [anthropic.com](https://www.anthropic.com/research/agentic-misalignment)

### Philosophy of Loop Engineering
- [ ] **LastGate — AI Agent Commit Guardian** — Claude Code、Cursor、Copilot、Devin などの AI 生成コミットを、secret scan、lint… 〔技術: コード生成の速度ではなく、エージェントが読める検証信号の近さと明瞭さ…／人文: 「最後に人間がレビューする」から「機械的な門番が反復の倫理を担う」へ…〕 · [github.com](https://github.com/AaronCx/LastGate)
- [ ] **Shared Substrate — sustained human–AI coupling のための外部記憶と検証オラクル** — 長期・多層・多セッションの人間–AI協働では、モデルそのものだけでなく、外部化された状態、層ごとの検証オラクル、観測可能性、そし… 〔技術: コンテキスト窓の限界を、外部メモリ、抽象レイヤー別の検証、観測可能な…／人文: 認識論的には、知識を「モデルの中」ではなく「人間とAIが横断する基盤…〕 · [github.com](https://github.com/olegroshka/shared-substrate)
- [ ] **DAC-Pose: Dual-Agent Collaborative Framework for Pose-Guided Human Generation** — ポーズ誘導の人物生成を、意味推論を担う PSR agent と視覚的ずれを扱う DAVE agent の二者協働として定式化し、… 〔技術: 「生成→評価→補正」を単一モデル内の曖昧な反省ではなく、役割分化した…／人文: これはサイバネティクス的な知覚–行為ループを、生成AIの内部設計へ移…〕 · [arxiv.org](https://arxiv.org/abs/2608.04622)
- [ ] **Ask HN: When did we go from agentic loops to graphs?** — AI engineering の議論が prompts、loops、graphs へ移っていることに対し、それが実質的な進歩なの… 〔技術: ループ、グラフ、ワークフローといった抽象の違いを、実際の開発フローの…／人文: これは技術用語の思想史そのものです。〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=49136426)
- [ ] **The Art of Loop Engineering** — エージェントの基本ループに加えて、検証ループ、人間レビュー、評価、デプロイ後の改善などを積み重ねる考え方を整理した記事です。 〔技術: LangChain / LangGraph 的な部品を使い、agen…／人文: 「知る」とは一回で正解を出すことではなく、基準に照らして失敗を返し、…〕 · [blog.langchain.com](https://blog.langchain.com/the-art-of-loop-engineering)

### Anthropology of Agentic AI
- [ ] **Agentic AI is changing engineering leadership faster than most teams realize** — エンジニアリング組織で、agentic AI導入後は従来の生産性指標よりもワークフロー設計、ガバナンス、意思決定速度が競争力にな… 〔技術: エージェントを既存プロセスに差し込むだけではなく、タスク分解・承認点…／人文: 「リーダーの仕事」がコード量の管理から判断儀礼の設計へ移る様子が見え…〕 · [okoone.com](https://www.okoone.com/spark/leadership-management/agentic-ai-is-changing-engineering-leadership-faster-than-most-teams-realize)
- [ ] **How to stop agentic AI from eroding human agency** — 高等教育・教育機関の文脈で、agentic AIが人間の主体性を弱めないようにするための導入姿勢を扱う記事。 〔技術: 教育現場のエージェント設計では、完全自動化よりも介入点、説明責任、利…／人文: 学校は知識伝達だけでなく、評価・信頼・成長の儀礼を維持する共同体でも…〕 · [universitybusiness.com](https://universitybusiness.com/how-to-stop-agentic-ai-from-eroding-human-agency)
- [ ] **Culture Clash: How Banks Are Adapting to Embedded AI Experts** — 銀行・決済領域で、組織内に埋め込まれるAI専門家やAI機能が既存の文化と衝突しながら適応されていく、というテーマの記事。 〔技術: 金融AIエージェントはモデル性能だけでなく、監査ログ、権限境界、人間…／人文: 銀行の現場文化では「速さ」よりも「説明できること」「責任の所在が明確…〕 · [paymentsjournal.com](https://www.paymentsjournal.com/culture-clash-how-banks-are-adapting-to-embedded-ai-experts)
- [ ] **CHROs need a human capability map before scaling AI agents** — AIエージェントを拡大する前に、CHROが「人間の能力マップ」を作るべきだと主張する記事。 〔技術: エージェント配置の前に、どの業務で人間の判断を近くに置くべきか、誰が…／人文: 「能力マップ」は、職場にある暗黙知・勘・責任感を可視化する民族誌的な…〕 · [hrexecutive.com](https://hrexecutive.com/chros-need-a-human-capability-map-before-scaling-ai-agents)
- [ ] **Future of Work with AI Agents: Auditing Automation and Augmentation Potential across the U.S. Workforce** — 米国の104職種・844タスクについて、1,500人の労働者の希望とAI専門家の能力評価を組み合わせ、AIエージェントが自動化す… 〔技術: タスクごとに「自動化可能性」だけでなく「労働者が望む主体性」と照合す…／人文: 職場の人類学にとって重要なのは、労働者が何を面倒だと思うかだけでなく…〕 · [arxiv.org](https://arxiv.org/abs/2506.06576)

### History of Automation
- [ ] **【AI自動化ツール最新情報】自律型エージェントの台頭と「産業革命」の歴史が教える働き方の未来** — 2026年の自律型AIエージェントを、RPAの固定シナリオから「自然言語の曖昧な指示を分解し、外部システムと連携し、自己修復する… 〔技術: ルールベースRPAから、計画・実行・例外処理を担うエージェント型ワー…／人文: ラッダイトを「反技術」ではなく、尊厳・分配・技能喪失への抗議として読…〕 · [note.com](https://note.com/machometool/n/n936a96af1af0)
- [ ] **The State of AI Agents in Automation: What Actually Works in 2026** — Zapier、Make、n8n、UiPath、Automation Anywhere、Workatoなどが、トリガー・アクション… 〔技術: 「何でも自律化」ではなく、抽出・分類・要約は実用、複雑な意思決定は未…／人文: 自動化史では常に、機械の性能だけでなく、誰が例外処理を引き受けるかが…〕 · [automationatlas.io](https://automationatlas.io/guides/ai-agents-in-automation-2026)
- [ ] **エージェント型自動化** — エージェント型自動化を、意思決定とアクションを自律的に実行できるAIエージェントによる自動化として定義し、古代から産業革命、電化… 〔技術: 「認識・推論・計画・ツール実行・フィードバック」というエージェント能…／人文: IBMが触れる「オートメーションのパラドックス」は、自動化が高度にな…〕 · [ibm.com](https://www.ibm.com/jp-ja/think/topics/agentic-automation)
- [ ] **Agentic AI & AI Agents: A Chronological Research Timeline** — 1980年のContract Net Protocol、BDIアーキテクチャ、Russell & Norvig、2022年以降の… 〔技術: 現代のAIエージェントを突然の生成AIブームではなく、分散AI、マル…／人文: 「誰が最初か」という英雄史ではなく、研究共同体・用語・商業化・公共理…〕 · [agentichistory.org](https://agentichistory.org/history.html)
- [ ] **We Need a New Ethics for a World of AI Agents** — 自律的に知覚・行動するAIエージェントの普及が、安全性、人間と機械の関係、社会的協調に新しい倫理課題を生むと論じる。 〔技術: エージェントを「環境を知覚し、目標に向けて自律的に行動するシステム」…／人文: 自動化の歴史で繰り返されてきた「道具が行為者のように振る舞うとき、責…〕 · [nature.com](https://www.nature.com/articles/d41586-025-02454-5)

### DDD
- [ ] **Keeping Models and Code in Sync: Roundtrip Engineering for Tactical Domain-Driven Design** — JDomInOという双方向同期ツールチェーンを提案し、戦術的DDDのドメインモデルからJavaコード構造を生成し、既存コードから… 〔技術: DDDモデルと実装のドリフトを「生成」と「逆解析」の往復で抑え、LL…／人文: ユビキタス言語は会議室の合意だけでなく、コード、モデル、AIエージェ…〕 · [arxiv.org](https://arxiv.org/abs/2608.05612)
- [ ] **From Textual Requirements to Microservice Architectures - A Comprehensive Evaluation of LLM-Based Design Synthesis** — 自然言語要件だけからLLMがマイクロサービスアーキテクチャを合成できるかを、サービス識別、通信復元、専門家評価で検証する研究。 〔技術: ゼロショット/ few-shotでサービス候補とインタラクションを生…／人文: 要件文からアーキテクチャを作る行為は、現場の曖昧な物語をどの単位で制…〕 · [arxiv.org](https://arxiv.org/abs/2607.28307)
- [ ] **Archally Blueprint Schema: domain-first YAML schema for AI-grounded system cartography** — ドメイン設計、意思決定記録、業務ルール、ガバナンス、アーキテクチャをYAMLで一つの機械可読な真実源にまとめ、OpenAPI、A… 〔技術: DDDを文書化の作法ではなく、生成物・API・プロセス図・エージェン…／人文: 「fragmented truth」という問題設定が、DDDの本質を…〕 · [github.com](https://github.com/Archally/blueprint-schema)
- [ ] **Event Storming Board: AI-moderated Event Storming Workshops** — Event Stormingをブラウザ上で行い、人間がワークショップを進め、ClaudeベースのAIDエージェントが共有ファイル… 〔技術: Server-Sent Eventsで即時更新される共有JSONを単…／人文: イベントストーミングは本来、利害関係者の声を同じ壁に集める儀式である…〕 · [github.com](https://github.com/przeprogramowani/event-storming-canvas)
- [ ] **DomainDL Agents: multi-agent service for DDD code generation and project-aware Q&A** — FastAPI、MongoDB、LangGraph、LangSmithを使い、DDDコード生成とプロジェクト知識Q&Aを行うマル… 〔技術: DDDの戦術パターンをエージェント分業の単位にしており、集約やドメイ…／人文: ソフトウェア設計の言葉がそのままエージェント組織の役割分担になる点が…〕 · [github.com](https://github.com/GianL22/DomainDL-ai)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

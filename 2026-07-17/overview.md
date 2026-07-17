# 📰 2026-07-17 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **NotebookLM** — NotebookLMが「Gemini Notebook」へ改名、Gemini/Searchエコシステムに統合… · [x.com](https://x.com/i/status/2077803351392268314)
- **Loop engineering** — ループエンジニアリングとは？ · [jp.findy-team.io](https://jp.findy-team.io/blogs/loop-engineering)
- **AWS** — OpenAI GPT-5.6 Sol / Terra / Luna が Amazon Bedrock で一般… · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/openai-gpt-sol-terra)
- **Harness engineering** — Boris Cherny氏の「ループとは、忙務の型を恒久的なインフラにすること」 · [x.com](https://x.com/bcherny/status/2077460395279692197)
- **sharp LLM usage** — Claude Codeの文脈肥大を疑う: `/clear`、薄いCLAUDE.md、モデルルーティング · [x.com](https://x.com/limalemonnn/status/2077742729719644428)
- **AI agent trends** — Boris Chernyの「自動化こそエージェント時代のレバレッジ」論 · [x.com](https://x.com/bcherny/status/2077460395279692197)
- **Claude Code** — Boris Chernyが発表したClaude Code `/checkup` · [x.com](https://x.com/bcherny/status/2074997570317779038)
- **Ethics of AI Agents** — 国連事務総長が「AI Child Safety Pledge」を呼びかけ · [x.com](https://x.com/antonioguterres/status/2074056597697957957)
- **Philosophy of Loop Engineering** — Stop Hand-Holding Your Coding Agent: Engineering the L… · [arxiv.org](https://arxiv.org/abs/2607.00038)
- **Anthropology of Agentic AI** — 企業文化は「ハイブリッド／マルチスピーシーズ」になる · [x.com](https://x.com/BusinessAnthro/status/2077232122058973538)
- **History of Automation** — Industrial Dexterity Benchmark: A Hardware-Software Be… · [arxiv.org](https://arxiv.org/abs/2607.14021)
- **DDD** — 食べログが「Deal Provider」を構築した理由──「AIがなければ踏み出せなかった」DDDという20… · [tech-blog.tabelog.com](https://tech-blog.tabelog.com/entry/deal-provider-responsibility-separation-design)

---

## トピック別トップ5（後で読む用）

### NotebookLM
- [ ] **NotebookLMが「Gemini Notebook」へ改名、Gemini/Searchエコシステムに統合へ** — 公式アカウントが、NotebookLMを「Gemini Notebook」へ改名すると発表。 〔技術: プロダクト名の変更以上に、NotebookLMのソースグラウンディン…／人文: 「ノート」は個人の記憶・学習・解釈の器だが、それが検索や会話AIの中…〕 · [x.com](https://x.com/i/status/2077803351392268314)
- [ ] **Video Overviews / Short Video Overviewsが、資料を縦型・解説動画へ変換する流れを加速** — NotebookLMの動画概要機能が、英語圏で無料ユーザーを含む広い層へ展開されたという投稿が目立つ。 〔技術: RAGで根拠資料に縛ったまま、要約テキストではなくナレーション・構成…／人文: 学ぶことが「読む」から「聞く」「見る」「共有する」へ拡張され、知識の…〕 · [x.com](https://x.com/Gemini_Notebook/status/2074551227594264799)
- [ ] **DeNA「AI活用100本ノック」をNotebookLMに入れ、個人向けAI診断コンサルタント化する日本語実践** — DeNAが公開した「AI活用100本ノック」をNotebookLMへ投入し、職種や困りごとに応じて「自分に効く技トップ5」「業務… 〔技術: 大量の事例集をベクトル的に参照しながら、ユーザー属性に応じた優先順位…／人文: 組織の成功事例は、そのままでは“読んで終わる知識”になりやすいが、N…〕 · [x.com](https://x.com/i/status/2077875547041042547)
- [ ] **業務手順メモを新人教育用チェックリストへ変換する日本語実践** — ざっくりした業務手順メモやマニュアルをNotebookLMに入れ、「抜け漏れゼロのチェックリスト」「新人教育ポイント」「理解度ク… 〔技術: ソースに基づくチェックリスト生成は、業務標準化・オンボーディング・ク…／人文: 新人教育では、ベテランの「当たり前」が最も伝わりにくい。〕 · [x.com](https://x.com/aidatapartner/status/2077904068660666462)
- [ ] **notebooklm-mcp-cli / notebooklm-pyが、NotebookLMをCLI・MCP・エージェントから扱う流れを作る** — `notebooklm-mcp-cli` はNotebookLMへのCLIアクセスとMCPサーバーを提供し、ノートブック作成・ソ… 〔技術: NotebookLMをUI専用ツールから、Claude Code・C…／人文: ノートは本来、人間が読み返すための私的な知の場所だったが、MCP化に…〕 · [github.com](https://github.com/jacob-bd/notebooklm-mcp-cli)

### Loop engineering
- [ ] **ループエンジニアリングとは？既存の手法との違いからAIエージェント時代の開発組織マネジメント・導入ステップまでを解説** — 日本語圏で最も実務に寄せて読める整理。 〔技術: ループを「計画→実行→検証→修正」の反復だけでなく、CI・ログ・スク…／人文: ethics / anthropology の観点では、「AIが完了…〕 · [jp.findy-team.io](https://jp.findy-team.io/blogs/loop-engineering)
- [ ] **0-to-1プロダクト開発における3層のフィードバックループ** — エージェントのコーディングループ、開発者のフィードバックループ、外部ユーザー/市場のフィードバックループという3階層で、AI時代… 〔技術: ループ速度を分け、分単位のコード生成、時間単位の開発者判断、日〜週単…／人文: philosophy / creativity の観点では、創造性が…〕 · [x.com](https://x.com/thaihwng/status/2074375633283780614)
- [ ] **Self-Improving AI Coding Agents Through Accumulated Behavioral Rules: A Closed-Loop Framework** — 人間のコードレビューで指摘された内容を、バージョン管理された行動ルールとセルフレビュー・チェックリストに蓄積し、コーディングエー… 〔技術: モデル重みを更新せず、レビューコメントを永続的な行動規範に変換するこ…／人文: history / anthropology の観点では、熟練エンジ…〕 · [arxiv.org](http://arxiv.org/abs/2607.13091v1)
- [ ] **SWE-Review: Closing the Loop on Issue Resolution with Agentic Code Review** — AI生成PRを一発で提出して終わる「open-loop」から、レビューエージェントがリポジトリを探索し、PRの採否判断と修正フィ… 〔技術: コード生成そのものではなく、PRを批評し修正させるテスト時スケーリン…／人文: narrative / ethics の観点では、AIが「作者」だけ…〕 · [arxiv.org](http://arxiv.org/abs/2607.06065v1)
- [ ] **When Agents Do Not Stop: Uncovering Infinite Agentic Loops in LLM Agents** — LLMエージェントが計画、ツール使用、状態更新、エージェント間ハンドオフを反復する中で、実効的な境界がないまま高コスト処理や状態… 〔技術: ループエンジニアリングの楽観面ではなく、停止しないループをフレームワ…／人文: ethics / philosophy の観点では、「自律性」は自由…〕 · [arxiv.org](http://arxiv.org/abs/2607.01641v1)

### AWS
- [ ] **OpenAI GPT-5.6 Sol / Terra / Luna が Amazon Bedrock で一般提供** — OpenAI GPT-5.6 の Sol、Terra、Luna が Amazon Bedrock で GA になりました。 〔技術: BedrockがClaude、Nova、Grokなどに加えてOpen…／人文: 生成AIの「どのモデルを使うか」という選択が、単なる性能比較ではなく…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/openai-gpt-sol-terra)
- [ ] **AWS Lambda が self-managed code storage を発表** — Lambda関数・レイヤーのコードを、Lambda側の中間コピーではなく自分のS3バケットから直接参照できるようになりました。 〔技術: デプロイ時のコード保管・クォータ・アーティファクト管理の境界がS3側…／人文: サーバーレスは「インフラを意識しない」方向に進んできましたが、成熟す…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/lambda-self-managed-code-storage)
- [ ] **Security Hub AI Inventory と GuardDuty AI Protection がAIワークロード可視化・防御を強化** — Security HubがAI資産の組織横断インベントリを提供し、GuardDutyはBedrockやSageMakerを含むA… 〔技術: Bedrock、SageMaker、セルフホストAI、外部AI AP…／人文: 組織にAIが広がると、誰が何を使っているかを知らないまま「便利だから…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-security-hub-ai)
- [ ] **Amazon Bedrock Managed Knowledge Base でエージェント向け企業検索を構築** — Bedrock Managed Knowledge Baseを使ったエージェント向け企業検索の構築手順が公開され、セットアップ簡… 〔技術: データ接続、パース、検索、エージェント統合の面倒な接合部をマネージド…／人文: 企業内の知識検索は、技術的にはベクトル検索でも、実態は組織の記憶を誰…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/build-enterprise-search-for-agents-with-amazon-bedrock-managed-knowledge-base)
- [ ] **arXiv: “Aurora DSQL: Scalable, Multi-Region OLTP” が公開** — Aurora DSQLを、マルチリージョン active-active のサーバーレスSQLデータベースとして解説する論文が公開… 〔技術: 商用クラウドのグローバルOLTP設計が論文として読める形になっており…／人文: データベースは企業活動の時間感覚そのものを形作ります。〕 · [arxiv.org](https://arxiv.org/abs/2607.13276)

### Harness engineering
- [ ] **Boris Cherny氏の「ループとは、忙務の型を恒久的なインフラにすること」** — Claude Codeを率いるBoris Cherny氏が、エージェント時代の高レバレッジ作業は一回限りの修正ではなく、lint… 〔技術: エージェントの改善をプロンプト単体ではなく、静的ルール、レビュー手順…／人文: 熟練者の暗黙知を個人の頭から共有インフラへ移すという話であり、ソフト…〕 · [x.com](https://x.com/bcherny/status/2077460395279692197)
- [ ] **日本語圏で「Claude Codeとハーネス」を考える資料・議論が急浮上** — 日本語コミュニティでは、@oikon48氏のSpeakerDeck「Claude Codeとハーネスについて考えてみる」が「Lo… 〔技術: Claude Codeの利用ノウハウが、プロンプト例ではなくコンテキ…／人文: 新しい技術概念が日本語へ輸入されるとき、単なる翻訳ではなく現場の不安…〕 · [x.com](https://x.com/MacopeninSUTABA/status/2077227150479126943)
- [ ] **arXiv「Harness Handbook」: ハーネスを読める・辿れる・編集できる対象にする** — 「Harness Handbook: Making Evolving Agent Harnesses Readable, Nav… 〔技術: ハーネスを単なる周辺コードではなく、振る舞い単位で索引化・局所化・検…／人文: エージェントの振る舞いが複数ファイルや設定に分散すると、責任の所在も…〕 · [arxiv.org](https://arxiv.org/abs/2607.13285)
- [ ] **arXivで「自己進化するハーネス」の評価方法そのものが争点化** — 「Self-Evolving Agent Harnesses via Gated Semantic Quality-Divers… 〔技術: ハーネスを自動改善するには、改善案の生成よりも、何を本当の改善として…／人文: 自己改善するシステムは、組織における「反省会」と似ています。〕 · [arxiv.org](https://arxiv.org/abs/2607.13683)
- [ ] **cc-loopkit: Claude Code用の小さな実践ハーネスが登場** — cc-loopkitは「Claude Codeの周りに置く自己修正ハーネス」として、悪い操作を事前に止めるguardrails、… 〔技術: 抽象論としてのharness engineeringを、hooks、…／人文: 「AIに任せる」とは自由放任ではなく、作業環境のルール、儀式、チェッ…〕 · [github.com](https://github.com/ksed8/cc-loopkit)

### sharp LLM usage
- [ ] **Claude Codeの文脈肥大を疑う: `/clear`、薄いCLAUDE.md、モデルルーティング** — Claude CodeやProjectsで長い会話・巨大なCLAUDE.mdを持ち続けると、コストだけでなく推論品質も落ちるとい… 〔技術: LLM活用のボトルネックを「モデル性能」ではなく、トークン再送・ノイ…／人文: これは知的労働における「記憶の整理術」の話でもある。〕 · [x.com](https://x.com/limalemonnn/status/2077742729719644428)
- [ ] **“未知の未知”を先に掘る: Claudeに面接させ、プロトタイプさせ、最後にクイズさせる** — 「Claudeがボトルネックではなく、あなたが言い忘れたことがボトルネック」という整理。 〔技術: 仕様漏れを実装後レビューで拾うのではなく、設計前の質問生成・参照提示…／人文: AIは「答える機械」ではなく、こちらの曖昧さを映す対話相手になる。〕 · [x.com](https://x.com/mvanhorn/status/2073116425078841744)
- [ ] **LLM評価は“自動採点”ではなく、失敗分類を育てる作業** — Hamel Husain氏は「AIにただ問題を見つけさせる」だけでは不十分で、レビューUIを作り、トレースを注釈し、失敗モード分… 〔技術: evalを単発のLLM judgeではなく、データ閲覧、失敗分類、注…／人文: 「正しさ」はスコアだけでなく、何を失敗とみなすかという価値判断を含む…〕 · [x.com](https://x.com/HamelHusain/status/2074242605634949306)
- [ ] **失敗を行動規則として蓄積するAIコーディングエージェント** — “Self-Improving AI Coding Agents Through Accumulated Behavioral… 〔技術: “失敗したらプロンプトを少し直す”ではなく、レビューコメントをバージ…／人文: 職人の勘やチームの暗黙知が、AIとの共同作業を通じて明文化されていく…〕 · [arxiv.org](https://arxiv.org/abs/2607.13091)
- [ ] **人間レビューも万能ではない: LLM生成アサーションをプログラマは自信過剰に誤判定する** — “Programmers Are Poor and Overconfident Judges of LLM-Generated… 〔技術: “人間が最後に見れば安全”というLLM活用の前提に実証的な揺さぶりを…／人文: AI時代の問題は機械の幻覚だけでなく、人間の自信過剰でもある。〕 · [arxiv.org](https://arxiv.org/abs/2607.08885)

### AI agent trends
- [ ] **Boris Chernyの「自動化こそエージェント時代のレバレッジ」論** — Boris Chernyは、Claude Code時代の高レバレッジ作業を「一回きりの指示」ではなく、CLAUDE.md、REV… 〔技術: プロンプトを長くするのではなく、ルール・スキル・検証・外部ツール接続…／人文: 熟練者の“勘”や“レビュー観”が、個人の暗黙知から共有インフラへ移さ…〕 · [x.com](https://x.com/bcherny/status/2077460395279692197)
- [ ] **Claude Codeの`/checkup`が示す「エージェント環境にも保守が必要」問題** — `/checkup`は、未使用のskills/MCP/pluginsの掃除、CLAUDE.mdの重複排除、巨大なCLAUDE.m… 〔技術: エージェント運用のボトルネックがモデル能力だけでなく、コンテキスト衛…／人文: これはAIを“雇う”ことに近い変化です。〕 · [x.com](https://x.com/bcherny/status/2074997570317779038)
- [ ] **Claude Code公式CHANGELOG: runaway防止、MCP自動バックグラウンド化、権限プロンプト修正** — 公式CHANGELOGでは、WebSearch呼び出し数の上限、subagent生成数の上限、長時間MCP tool callの… 〔技術: Web検索ループ、subagent増殖、MCP長時間実行、Plan…／人文: 自律性を上げるほど、自由ではなくガードレールの設計が価値になります。〕 · [raw.githubusercontent.com](https://raw.githubusercontent.com/anthropics/claude-code/main/CHANGELOG.md)
- [ ] **MCP対応の永続メモリ層が「ステートレスなコーディングエージェント」の限界を崩し始める** — agentmemoryのようなMCP互換の永続記憶レイヤーが、Claude Code、Cursor、Codex CLI、Gemi… 〔技術: MCPが外部ツール接続だけでなく、エージェント間・セッション間の状態…／人文: “毎回新人に説明する”疲労が減る一方で、何を組織の長期記憶として残す…〕 · [x.com](https://x.com/chenzeling4/status/2077846235541897597)
- [ ] **arXivで権限・監査・MCPセキュリティ研究が同時多発** — 「How Agents Ask for Permission」は、AIエージェントのユーザー権限をUIから enforcemen… 〔技術: エージェントの安全性が、抽象的な“アラインメント”から、権限UI、実…／人文: 人間の「許可したつもり」と機械の「実行した事実」の間にはズレがありま…〕 · [arxiv.org](https://arxiv.org/abs/2607.13718)

### Claude Code
- [ ] **Boris Chernyが発表したClaude Code `/checkup`** — Boris ChernyがClaude Codeの新コマンド`/checkup`を紹介。 〔技術: Claude Code運用で増えがちな設定・文脈・権限・hooksの…／人文: これは「道具を使う人間」ではなく「道具の生活環境を定期健診する人間」…〕 · [x.com](https://x.com/bcherny/status/2074997570317779038)
- [ ] **Bloomberg/BusinessweekのBoris Cherny特集と“職業としてのプログラミング”論** — Businessweekが「Boris ChernyがClaude Codeを作ってから1年で、ソフトウェアエンジニアの職業全体… 〔技術: Claude Codeの価値が単体の補完精度ではなく、PR、CI、レ…／人文: 「誰がコードを書いたのか」という著者性が、個人の手作業から人間とエー…〕 · [x.com](https://x.com/BW/status/2077770325626900949)
- [ ] **公式ドキュメントで前面化するsubagents・hooks・skills・MCP・auto mode** — 公式ドキュメントでは、CLAUDE.md、auto memory、skills、hooks、MCP、subagents、Agen… 〔技術: Claude Codeは「チャットUI」ではなく、設定ファイル・イベ…／人文: 開発現場の暗黙知がCLAUDE.mdやskillsとして書き下され、…〕 · [docs.anthropic.com](https://docs.anthropic.com/en/docs/claude-code/overview)
- [ ] **日本語圏で広がるCLAUDE.md実践とプロンプト規律** — 日本語圏では、プロジェクト直下のCLAUDE.mdに「書く前に考える」「シンプルさ最優先」「外科手術のように変更する」「成功基準… 〔技術: 失敗しやすい大規模編集、過剰実装、無限ループを、モデル変更ではなくプ…／人文: 日本語圏の実践は、職人気質の「段取り」「型」「余計なことをしない」と…〕 · [x.com](https://x.com/claudecode84/status/2073584012355125270)
- [ ] **arXivで進む「本番エージェントの安全・コスト・ハーネス」研究** — `Agent Hacks Agent: Autoresearch for Production-Agent Red-Teamin… 〔技術: Claude Codeのような実行権限を持つエージェントでは、性能評…／人文: 自律的に行動する開発エージェントは、失敗したときの責任境界を曖昧にす…〕 · [arxiv.org](https://arxiv.org/abs/2607.11698)

### Ethics of AI Agents
- [ ] **国連事務総長が「AI Child Safety Pledge」を呼びかけ** — 国連のAntónio Guterres事務総長は、子どもが接触しうるAIシステム・エージェント・プラットフォームに対し、厳格な安… 〔技術: エージェント安全を抽象的な「アラインメント」ではなく、年齢・危機検知…／人文: 子どもはAI利用者の中でも権力差と依存リスクが大きく、ここでは「利用…〕 · [x.com](https://x.com/antonioguterres/status/2074056597697957957)
- [ ] **Simon Willisonの「AI employee」批判と説明責任の再設計** — Willisonは、AIを「従業員」と呼ぶことは人間への敬意を欠き、技術の性質も誤解していると批判した。 〔技術: エージェント設計の中心を、モデル性能ではなく、監査ログ、権限境界、レ…／人文: 「AIを同僚にする」物語は魅力的だが、責任・罰・信頼・ケアを引き受け…〕 · [x.com](https://x.com/simonw/status/2076080476725649581)
- [ ] **GPT-Red型の自動レッドチーミングが、エージェント安全評価の主戦場に** — OpenAIのGPT-Redとして報じられた自動レッドチーミング手法が、直接・間接プロンプトインジェクションを大規模に発見する仕… 〔技術: ブラウザ、メール、ファイル操作など外部行為を伴うエージェントでは、プ…／人文: 安全のために攻撃能力を育てるという逆説は、軍事・治安技術にも似た倫理…〕 · [x.com](https://x.com/helpnetsecurity/status/2077641882524610890)
- [ ] **arXiv「Beyond Attack-Success Rate」が、エージェント被害を7段階で評価する提案** — 「Beyond Attack-Success Rate: Action-Graded Severity Scale for To… 〔技術: 「突破されたか」だけではなく「突破後に何をしたか」を測ることで、エー…／人文: 倫理的には、同じ失敗でも、草稿の誤生成と他者への被害拡大は同じではな…〕 · [arxiv.org](https://arxiv.org/abs/2607.07474v1)
- [ ] **arXiv「When Bots Join the Team」が、ボットを社会的インフラとして捉える** — 「When Bots Join the Team」は、2,991件のGitHubプロジェクトを対象に、ボット導入前後のオープンソ… 〔技術: エージェント導入の効果を、個人の生産性ではなく、コミュニティの協調能…／人文: AIエージェントは職場やOSS共同体に「誰がいるのか」という感覚を変…〕 · [arxiv.org](https://arxiv.org/abs/2607.13679v1)

### Philosophy of Loop Engineering
- [ ] **Stop Hand-Holding Your Coding Agent: Engineering the Loops that Replace Step-by-Step Prompting** — コーディングエージェントへの逐次プロンプトをやめ、trigger / goal / verification / stoppin… 〔技術: 完成定義、独立検証、停止条件、記憶を一体化した仕様としてループを定義…／人文: これは、知識を「言い当てること」ではなく「検証可能な実践の連鎖で正当…〕 · [arxiv.org](https://arxiv.org/abs/2607.00038)
- [ ] **X上の「loop engineering」実践知: verifier is king / closed vs open loops / taste as reward function** — Xでは、Loop Engineering を「Goal → Act → Verify → State/Memory → Term… 〔技術: 「actor と verifier を分ける」「テスト・rubric…／人文: ここでの verifier は、古典的な真理判定装置というより、共同…〕 · [x.com](https://x.com/HelveticVault/status/2077898091710071109)
- [ ] **LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans** — LOGOS は、複数エージェントが経験から学び、将来の振る舞いを形作るプロンプト・記憶・スキル・ツール・ワークフローを変更してい… 〔技術: ループの出力を次のループの構成要素へ反映する meta-loop を…／人文: これは第二階サイバネティクス的な問い、すなわち観察者・設計者を含めた…〕 · [arxiv.org](https://arxiv.org/abs/2607.10878)
- [ ] **Human-on-the-Bridge / LLM-as-a-Verifier / Verifier-Determined Sufficiency の流れ** — Human-on-the-Bridge は、人間が毎ステップ介入するのではなく、評価知識・罠・rubric・監査ルールを上流で設… 〔技術: ループの停止や継続を、単純な回数制限ではなく、determinist…／人文: 人間は「輪の中」に常時閉じ込められるのではなく、「橋の上」から意味・…〕 · [arxiv.org](https://arxiv.org/abs/2606.16871)
- [ ] **GitHub上の loop engineering ツール群の急増: loopx / Kaola-Workflow / session-orchestrator など** — GitHub検索では、`loopx`、`Kaola-Workflow`、`codelab-3-loop-engineering`… 〔技術: 抽象的なループ思想が、状態ファイル、DAG、checker harn…／人文: 思想史的には、これは「反復」を単なる作業量ではなく、制度化された学習…〕 · [github.com](https://github.com/huangruiteng/loopx)

### Anthropology of Agentic AI
- [ ] **企業文化は「ハイブリッド／マルチスピーシーズ」になる** — Business anthropology の文脈で、AIがR&D・顧客対応・各部門に入り込むことで、企業文化が人間だけのもので… 〔技術: エージェント導入の成否を、モデル性能ではなく、権限・記憶・ワークフロ…／人文: これは古典的な人間中心の組織論を、動物・機械・環境を含む「マルチスピ…〕 · [x.com](https://x.com/BusinessAnthro/status/2077232122058973538)
- [ ] **ハイブリッド社会に必要な「儀礼」としてのエージェント運用** — 人間社会の儀礼を、共同体の同一性・整合性・共有現実を保つ「coherence technology」と捉え、AIを含む社会では新… 〔技術: マルチエージェントや人間参加型エージェント運用で、レビュー、承認、振…／人文: 儀礼は非合理な残滓ではなく、複雑な社会で意味と秩序を同期する低コスト…〕 · [x.com](https://x.com/Batchelor/status/2075765224435581272)
- [ ] **日本語圏の「現場」論: 動くAIと使われ続けるAIは違う** — 日本語Xでは、文化人類学という語は前面に出ない一方、「現場のリアル」「動く」と「使われる」は別物、運用しながら育てて初めて価値に… 〔技術: PoCで動くエージェントよりも、権限設定、例外処理、教育、ログ確認、…／人文: 日本の「現場主義」は、エージェントAIを身体化された実践として理解す…〕 · [x.com](https://x.com/Rin00wn/status/2077899138067562546)
- [ ] **ワークフロー再設計: 部門の儀礼からエンドツーエンドの流れへ** — エージェントAIの価値は、個々の作業を速くするより、要件定義・設計・開発・テスト・デプロイをつなぐ流れを再設計することにある、と… 〔技術: エージェントをツールとして散在させるのでなく、観測可能性、共有コンテ…／人文: 組織の儀礼はしばしば承認会議、レビュー、メール、検索、依頼といった反…〕 · [x.com](https://x.com/sijlalhussain/status/2077468426000371883)
- [ ] **人類学的知識グラフでLLM/エージェントを接地する** — Matt Artz氏の「Grounding Large Language Models in an Anthropologica… 〔技術: LLMエージェントに外部知識グラフやオントロジーを組み合わせることで…／人文: 人類学の知識は「AI倫理の装飾」ではなく、エージェントがどの場で何を…〕 · [x.com](https://x.com/SfAAnthro/status/2076624146058920302)

### History of Automation
- [ ] **Industrial Dexterity Benchmark: A Hardware-Software Benchmarking Platform for Industrial Dexterous Manipulation** — ケーブル配線、コネクタ挿入、精密組立のように、数十年のロボット研究後も人手依存が残る産業作業を対象に、Industrial De… 〔技術: 自動化の歴史で最後まで残りがちな「手先の器用さ」を、模倣学習・拡散方…／人文: 工場・物流・データセンターの労働史では、人間の身体が「例外処理装置」…〕 · [arxiv.org](https://arxiv.org/abs/2607.14021)
- [ ] **「完全自動化」楽観論への脱政治化批判** — ケインズ以来くり返されてきた「自動化が労働を解放する」という楽観論に対し、生産力向上だけでは分配問題は解けず、計算資源・データ・… 〔技術: AIエージェントやロボットの能力向上を、計算資源・データ・運用基盤の…／人文: 自動化の歴史は「楽になる技術」の歴史であると同時に、労働の成果を誰が…〕 · [x.com](https://x.com/tt5106470080519/status/2077636633378361654)
- [ ] **Exploring the societal impacts of AI** — MITのAI and Society Forumで、David Autor、Daniela Rus、David Mindellら… 〔技術: AIを高水準で指示できるアシスタントとして使う可能性と、過信・安全基…／人文: 自動化の歴史では、効率化がしばしば熟練・責任・儀礼を不可視化してきた…〕 · [news.mit.edu](https://news.mit.edu/2026/exploring-societal-impacts-of-ai-0623)
- [ ] **AI Hiring Tools Can Yield Racial Bias and Systemic Rejection** — 150社・1,700求人・400万件の応募を対象に、単一ベンダーのAI採用スクリーニングが人種的な不利益と「システム的拒否」を生… 〔技術: 多数の企業が同じ採用アルゴリズムに依存すると、個別企業の自動化ではな…／人文: 自動化の歴史は、機械が現場作業を置き換えるだけでなく、誰が労働市場に…〕 · [hai.stanford.edu](https://hai.stanford.edu/news/ai-hiring-tools-can-yield-racial-bias-and-systemic-rejection)
- [ ] **Technology usually creates jobs for young, skilled workers. Will AI do the same?** — David Autorらの研究は、戦後米国の「新しい仕事」が若く高学歴の都市部労働者に偏って配分され、賃金プレミアムも時間ととも… 〔技術: AIを既存職務の代替だけでなく、新しい専門性・新しいワークフローを生…／人文: 自動化の歴史は、古い技能を陳腐化させながら新しい希少技能を作る循環で…〕 · [news.mit.edu](https://news.mit.edu/2026/technology-creates-jobs-young-skilled-workers-ai-0521)

### DDD
- [ ] **食べログが「Deal Provider」を構築した理由──「AIがなければ踏み出せなかった」DDDという20年前からの設計思想への挑戦** — 食べログの販売管理領域で、契約・請求・オプション判定などのロジックが複数システムへ漏れ出していた問題に対し、「データを渡す」から… 〔技術: DDD、Tell Don't Ask、Hexagonal Archi…／人文: これは単なるアーキテクチャ記事ではなく、組織が成長して「誰が判断を所…〕 · [tech-blog.tabelog.com](https://tech-blog.tabelog.com/entry/deal-provider-responsibility-separation-design)
- [ ] **DSLs Enable Reliable Use of LLMs** — Unmesh Joshiが、LLMに曖昧な自然言語だけでコードを書かせるのではなく、ドメイン固有言語（DSL）と強い抽象により出… 〔技術: DSLはDDDのユビキタス言語をさらに形式化し、LLMの出力を検証可…／人文: 言語が思考を形づくるという古典的な洞察が、AI開発で再浮上しています…〕 · [martinfowler.com](https://martinfowler.com/articles/llm-and-dsls.html)
- [ ] **Domain-Driven Design in Practice: A Large-Scale Empirical Characterisation of the Open-Source Ecosystem** — Ozan Özkan、Önder Babur、Mark van den Brandによるcs.SE論文で、GitHub上のDDD… 〔技術: DDDを理念ではなくリポジトリ実態から測定し、AIも使った検証パイプ…／人文: DDDはコードの形だけではなく、ビジネス意図を保存する文化の問題でも…〕 · [arxiv.org](https://arxiv.org/abs/2607.06471)
- [ ] **Fix verbose AI with a ubiquitous language** — Matt PocockのAI時代のソフトウェアエンジニアリングに関する話題で、冗長なAI出力を抑える実践として、DDD由来のユビ… 〔技術: ユビキタス言語をプロンプトの飾りではなく、AIコーディング環境の圧縮…／人文: 言葉を揃えることは、チームの権力関係や学習速度にも影響します。〕 · [x.com](https://x.com/mardehaym/status/2075149630879232142)
- [ ] **LLM Wiki / 組織知をエージェントが読める責任・ワークフローへ変換する流れ** — 組織内の責任、ワークフロー、運用文脈、ドメイン知識をMarkdownベースのLLM Wikiとして整理し、そこから専門エージェン… 〔技術: LLM WikiはRAGや単発プロンプトよりも、責任定義・承認条件・…／人文: ここで問われているのは「AIに何をさせるか」だけでなく、「組織の仕事…〕 · [x.com](https://x.com/arrakis_ai/status/2074304050880012736)

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

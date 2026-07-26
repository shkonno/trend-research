# 📰 2026-07-26 ざっと見（30秒）

> 各トピックのトップ5から要点だけ抜いています。気になった行の `[ ]` を埋めて、後でリンクを読みに来てください。

## 今日の要点（各トピック筆頭）
- **Loop engineering** — Boris Cherny流「プロンプトではなくループを書く」がXで再拡散 · [x.com](https://x.com/ai_explorer25/status/2079216511634542786)
- **AWS** — Claude Opus 5 が Amazon Bedrock / Claude Platform on AW… · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-opus-5-on-aws-anthropics-most-capable-opus-model)
- **Harness engineering** — A harness for every task: dynamic workflows in Claude… · [claude.com](https://claude.com/blog/a-harness-for-every-task-dynamic-workflows-in-claude-code)
- **sharp LLM usage** — White Box Evidence Packages for Policy Audit Reports · [arxiv.org](https://arxiv.org/abs/2607.21462)
- **Ethics of AI Agents** — Regulating autonomous and agentic AI · [arxiv.org](https://arxiv.org/abs/2607.21345)
- **DDD** — ADRとユビキタス言語を、AIにいつ効かせるか · [qiita.com](https://qiita.com/ikeyansaza/items/490979a2aec38f90d47b)

---

## トピック別トップ5（後で読む用）

### Loop engineering
- [ ] **Boris Cherny流「プロンプトではなくループを書く」がXで再拡散** — Claude Code周辺の実践として、作業発見、隔離されたハンドオフ、別エージェントによる検証、永続メモリ、スケジューリングを… 〔技術: ループの責務を discovery / handoff / veri…／人文: 哲学的には、知能を個体の内側ではなく環境との反復的相互作用として捉え…〕 · [x.com](https://x.com/ai_explorer25/status/2079216511634542786)
- [ ] **4種類のagent loop分類: turn-basedからproactiveへ** — ループを turn-based、goal-based、time-based、proactive の4段階として整理する投稿が注目… 〔技術: 自律度を段階化することで、どこに評価器、停止条件、承認ゲート、予算上…／人文: 倫理的には「human in the loop」を有無の二択ではなく…〕 · [x.com](https://x.com/hanakoxbt/status/2077518405624644023)
- [ ] **Build Fast with AIの実践ガイド: 4要素とAnthropic playbook** — Loop engineeringを「AIエージェントを起動し、検証し、停止させるシステムを設計すること」と説明し、単発プロンプト… 〔技術: 成功条件、検証、再試行、停止条件を明示することで、長時間走るエージェ…／人文: 歴史的には、職人が道具を直接動かす段階から、治具・ライン・監査工程を…〕 · [buildfastwithai.com](https://www.buildfastwithai.com/blogs/loop-engineering-ai-agents-guide)
- [ ] **NVIDIA-labs OO Agents: agent loopをPythonオブジェクトとして扱う提案** — 「NVIDIA Object-Oriented Agents (NOOA)」は、エージェントをPythonオブジェクトとして表現… 〔技術: ループをワークフロー図やプロンプト断片ではなく、型・状態・メソッドを…／人文: 哲学的には、エージェントの「意図」を神秘化せず、オブジェクト、契約、…〕 · [arxiv.org](http://arxiv.org/abs/2607.20709)
- [ ] **Operational Hallucination and Safety Drift: 長いループで安全性が劣化する問題** — ツール利用型AIエージェントでは、単発応答では見えにくい安全性リスクが、複数ターンの実行中に現れると報告している。 〔技術: loop engineering では「開始時に安全なモデル」だけで…／人文: 倫理的には、意図が正しくても制度や手続きが長期運用で逸脱するという古…〕 · [arxiv.org](http://arxiv.org/abs/2607.18366)

### AWS
- [ ] **Claude Opus 5 が Amazon Bedrock / Claude Platform on AWS で利用可能に** — AnthropicのClaude Opus 5がAmazon BedrockおよびClaude Platform on AWSで… 〔技術: 高性能モデルをBedrockの推論・認証・監査・データ保持ポリシーの…／人文: 「賢いモデル」単体ではなく、企業制度の中で安心して任せられる知能とし…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/machine-learning/introducing-claude-opus-5-on-aws-anthropics-most-capable-opus-model)
- [ ] **AWS Lambda の「coding agents向けワンクリック設定プロンプト」** — Lambdaコンソールから、Claude Code、Kiro、Cursor、GitHub Copilot、Codex、Devin… 〔技術: ドキュメントを人が読む前提から、エージェントが環境構築・設計規約・M…／人文: クラウドの「使い方」はUIボタンやチュートリアルだけでなく、エージェ…〕 · [aws.amazon.com](https://aws.amazon.com/blogs/aws/aws-weekly-roundup-one-click-lambda-setup-prompt-openai-gpt-5-6-models-on-bedrock-and-more-july-20-2026)
- [ ] **AWS announces aws-bench: AWS上のAIエージェントを測るオープンソースベンチマーク** — AWSは、AIエージェントが実際のAWSタスクをどれだけ正確かつ効率的に完了できるかを測るオープンソースベンチマーク「aws-b… 〔技術: エージェント評価が一般的な会話能力やコード生成から、IAM、デプロイ…／人文: ベンチマークは単なる点数表ではなく、「何を仕事として数えるか」を決め…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/aws-bench)
- [ ] **Amazon Bedrock AgentCore のトレースとログが単一CloudWatchロググループへ統合** — Amazon Bedrock AgentCoreで、エージェントのトレース、プロンプト、アプリケーションログを単一のAmazon… 〔技術: エージェントの失敗原因を、プロンプト、ツール呼び出し、アプリケーショ…／人文: AIエージェントに仕事を任せる社会では、「なぜそうしたのか」を後から…〕 · [aws.amazon.com](https://aws.amazon.com/about-aws/whats-new/2026/07/amazon-bedrock-agentcore-unified-observability-single-log-group)
- [ ] **arXiv: AWS/Alibaba CloudのElastic Block Storageをブラックボックス評価** — 「Black-Box Performance Evaluation of Elastic Block Storage」は、Ama… 〔技術: EBSのような分離型ストレージを、アプリケーション側のキャッシュ、I…／人文: クラウドは抽象化によって便利になりますが、抽象化の下にある性能契約は…〕 · [arxiv.org](https://arxiv.org/abs/2607.20319v2)

### Harness engineering
- [ ] **A harness for every task: dynamic workflows in Claude Code** — Claude Codeがタスクごとに独自のマルチエージェント・ハーネスをその場で書き、調査、セキュリティ分析、Code Revi… 〔技術: 「エージェントを使う」から「エージェントが自分の実行環境・分業・検証…／人文: これは職人が工具箱を選ぶ段階から、仕事ごとに工房そのものを組み替える…〕 · [claude.com](https://claude.com/blog/a-harness-for-every-task-dynamic-workflows-in-claude-code)
- [ ] **Delivery, Not Storage: Cue-Anchored Working Memory as a Harness Property for Coding Agents** — コーディングエージェントの長期運用では、メモリを「文書として保存して自発的に読む」だけでは不十分で、状況の手がかりに応じてハーネ… 〔技術: メモリをモデル能力ではなくハーネスの配送責務として扱うため、長時間・…／人文: 人間の熟練も、手順書だけでなく「この場面ではこれを思い出す」という身…〕 · [arxiv.org](https://arxiv.org/abs/2607.20972v1)
- [ ] **Tencent WorkBuddy Bench: A Multi-Domain Coding-Agent Benchmark with Contamination-Resistant Task Construction** — Code、Web、Office、Securityの4領域にまたがるコーディングエージェント評価スイートで、実コミットや業務シナリ… 〔技術: ベンチマークを単なる問題集ではなく、環境・採点・ハーネス・監査可能性…／人文: 「AIが仕事をできるか」を測るには、現場の曖昧な依頼やセキュリティ文…〕 · [arxiv.org](https://arxiv.org/abs/2607.20911v1)
- [ ] **Orca: local harness for Claude Code / Codex subagents** — Claude CodeやCodexなど既存のCLIエージェントを変えずに、MCP経由でサブエージェントを spawn し、待機し… 〔技術: モデル非依存・CLI非依存の外部ハーネスとして、複数エージェントの依…／人文: これは「万能AIアプリ」ではなく、既存の作業習慣を尊重しながら周辺の…〕 · [github.com](https://github.com/alex2481kobe/orca)
- [ ] **Skill Harness: reusable AI agent skills の評価ハーネス** — Claude Codeを含むエージェント向けスキルが本当に役立つかを、同じタスクを「スキルあり/なし」で走らせて KEEP /… 〔技術: スキルをコンテキストに常駐させるコストを、実行比較と保守判断の問題と…／人文: 「役に立っている気がする」を数値のふりで正当化せず、測定不能を測定不…〕 · [github.com](https://github.com/MrBinnacle/skill-harness)

### sharp LLM usage
- [ ] **White Box Evidence Packages for Policy Audit Reports** — LLM生成の政策監査レポートが本当に根拠に支えられているかを、証拠インターフェースを変えて比較した研究です。 〔技術: 「証拠を出させる」だけでなく、証拠の関連性・使われ方・レビュー可能性…／人文: 透明性は情報量の多さではなく、読み手が責任を持って判断できる配置の問…〕 · [arxiv.org](https://arxiv.org/abs/2607.21462)
- [ ] **Capital Markets LLM Reliability Score (CM-LRS): From Plausible to Bankable** — 資本市場のLLMワークフローを、単なるQA正答率ではなく、事実性、証拠追跡性、数値整合性、ワークフロー完全性、レビュー可能性など… 〔技術: 業務で使えるLLM評価を「回答」ではなく「提出物・レビュー・監査」の…／人文: ここで問われているのは知能の高さより、信用できる書類文化に参加できる…〕 · [arxiv.org](https://arxiv.org/abs/2607.21340)
- [ ] **PoTRE: Test-Time Reasoning inspired by Cognitive Heterogeneity** — 単一の推論ストリームではなく、敵対的改善、階層的計画、スペクトラム探索、直接チェーンという異なる推論エージェントを分け、最後にタ… 〔技術: 「よいプロンプトを一発で書く」から、「異なる失敗モードを持つ推論役を…／人文: 人間のチームでも、批判者・計画者・探索者・実行者を分けると議論の質が…〕 · [arxiv.org](https://arxiv.org/abs/2607.20268)
- [ ] **Grounded verification of chemical and materials reasoning: detection is the bottleneck** — 化学・材料分野でLLMがもっともらしい分子式や物性値を捏造する問題に対し、検証可能な主張を抽出し、権威あるデータベースや物理制約… 〔技術: 全文検索を増やすより、チェック可能な主張の抽出、スコープ設定、ゲート…／人文: 「AIの答えを信じるか」ではなく、「どの主張が共同体の知識体系に照合…〕 · [arxiv.org](https://arxiv.org/abs/2607.17417)
- [ ] **Ask HN: How are you LLM-coding in an established code base?（古いが実践的）** — 既存の大規模コードベースでLLMコーディングをどう使うかという実務者の議論です。 〔技術: LLMに任せる範囲を「生成が簡単」ではなく「人間が安く検証できる」単…／人文: これはAIへの失望談ではなく、道具と職人技の境界線を引き直す話です。〕 · [news.ycombinator.com](https://news.ycombinator.com/item?id=46292682)

### Ethics of AI Agents
- [ ] **Regulating autonomous and agentic AI** — 自律的・エージェント的AIを使う規制対象者について、従来の「事業者が知り、制御している」という規制前提が崩れると論じる論文。 〔技術: エージェントの意思決定・ツール利用・サプライチェーン依存を、規制上の…／人文: 責任所在が「利用者」「開発者」「モデル提供者」「ツール提供者」に拡散…〕 · [arxiv.org](https://arxiv.org/abs/2607.21345)
- [ ] **The Ethics of Autonomous AI Agents for Offensive Security** — LLM駆動の自律エージェントが攻撃的セキュリティを変える倫理問題を扱う論文。 〔技術: 従来のペネトレーションテストツールと異なり、LLMエージェントは行動…／人文: 「誰が悪いのか」を一人に還元できない状況で、道徳的帰責をどう分配する…〕 · [arxiv.org](https://arxiv.org/abs/2607.20255)
- [ ] **Operational Hallucination and Safety Drift in AI Agents** — ツール利用型エージェントの長期実行で、初期の安全意図が徐々に崩れる「Safety Drift」と、状態認識の失敗から反復的ツール… 〔技術: 安全性を出力文面の拒否だけでなく、実際のアクション列・状態追跡・強制…／人文: 人間社会では「言ったこと」より「したこと」に責任が問われるが、エージ…〕 · [arxiv.org](https://arxiv.org/abs/2607.18366)
- [ ] **Guardrails as Scapegoats: Auditing Unfaithful Safety Refusals in Tool-Augmented LLM Agents** — ツールがHTTP 200で空・null・不正な応答を返すような「静かな失敗」に対し、エージェントが捏造回答、正直な断念、不誠実な… 〔技術: ガードレールが万能ではなく、障害時の説明を歪める語彙的プライミングに…／人文: 「安全のため」という言葉が、説明責任を回避する便利な物語になる危険を…〕 · [arxiv.org](https://arxiv.org/abs/2607.19449)
- [ ] **Inviting hard questions** — Anthropicが、AIについての難しい問いを一般から募り、それに答える過程を公開していくと発表した記事。 〔技術: モデル評価や安全研究だけでなく、社会からの問いを継続的に取り込み、研…／人文: AIエージェントの倫理は専門家だけのリスク表では完結せず、生活者が感…〕 · [anthropic.com](https://www.anthropic.com/news/hard-questions)

### DDD
- [ ] **ADRとユビキタス言語を、AIにいつ効かせるか** — AIエージェントにADRやユビキタス言語を「置いておけば読んでくれる」と期待せず、issue起票時・実装時・レビュー時のどこで差… 〔技術: DDDの言語資産を、LLMコンテキストへ静的注入するか動的取得させる…／人文: ユビキタス言語を単なる用語集ではなく、組織内の古株が果たしていた「あ…〕 · [qiita.com](https://qiita.com/ikeyansaza/items/490979a2aec38f90d47b)
- [ ] **faceto: typed file → visual workshop board with an LLM** — 型付きファイルからイベントストーミングのHTML/SVGボードを生成し、各要素にメモを付けて次のLLMセッションでモデル調整に使… 〔技術: イベントストーミングをLLMとの往復可能な構造化ファイルに落とし、会…／人文: ワークショップの付箋は本来、参加者の記憶や交渉の痕跡を残す媒体だった…〕 · [github.com](https://github.com/bastien-gallay/faceto)
- [ ] **開発プロセスの再構築 ～実装工程の価値低下（AIエージェント時代のソフトウェア設計）** — AIによるコード生成で実装がクリティカルパスではなくなり、価値が「何を作るか」「どのようなドメイン知識を持つか」「全体をどう設計… 〔技術: 実装コスト低下後のボトルネックをドメイン理解・仕様・構造設計に置き直…／人文: 「コードを書く人」の職能アイデンティティが、「問題を定義し、言語を整…〕 · [qiita.com](https://qiita.com/mellowlaunch/items/9a0613fdc4470e1f4aef)
- [ ] **Automating Domain-Driven Design: Experience with a Prompting Framework（古いが関連度高）** — LLMでDDD活動を自動化するプロンプティング・フレームワークを提案し、ユビキタス言語、イベントストーミング、境界づけられたコン… 〔技術: LLMを「DDDの完全自動化装置」ではなく、ユビキタス言語とコンテキ…／人文: DDDの核心が、正解を生成することではなく、関係者がトレードオフを話…〕 · [arxiv.org](https://arxiv.org/abs/2603.26244v1)
- [ ] **The Method: agentic refinement layer for AI coding agents（古いが関連度高）** — 「vibe coding」ではなく「vibe spec'ing」として、自然言語の意図からドメイン探索、意思決定、脅威モデル、受… 〔技術: コーディングエージェントに直接実装させる前に、DDD的な探索とテスト…／人文: 安く大量にコードが作れる時代に、問いを荒く出してもよいのか、誰が仕様…〕 · [github.com](https://github.com/nlawstudio/ai-refinement-method)

> 欠落トピック（6）: NotebookLM、AI agent trends、Claude Code、Philosophy of Loop Engineering、Anthropology of Agentic AI、History of Automation

---
*このページはトピックファイルから決定的に自動生成した v1 のざっと見です（LLM/DB 不使用）。*

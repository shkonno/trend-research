# Loop engineering トレンド調査 (2026-08-07)

- 調査日: 2026-08-07
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「賢いモデルを呼ぶ」段階から、失敗検知・修復・記憶・評価・人間承認を含む実行ループ全体を設計する段階へ移っている。

## トップ5

### 1. Deep Agents vs LangChain vs LangGraph
- 出典: LangChain Blog
- 日付: 2026-08-06
- リンク: https://www.langchain.com/blog/deep-agents-vs-langchain-vs-langgraph
- 要約: LangChain が、Deep Agents / LangChain / LangGraph の使い分けを整理した記事。単純なチェーン、状態を持つグラフ、長期実行の深いエージェントをどう選ぶかが、loop engineering の設計判断として読める。
- なぜ面白いか:
  - 技術: エージェントのループを「抽象度」「状態管理」「制御可能性」で分け、いつ LangGraph の明示的な状態遷移に降りるべきかを示している。
  - 人文: narrative の観点では、AI開発の物語が「万能エージェント」から「仕事に合った作法を選ぶ職人性」へ変わっている。anthropology 的にも、チームがどのフレームワークを選ぶかは、その組織が不確実性・失敗・責任分担をどう文化化するかの表れになっている。

### 2. How we built an autonomous SRE agent for Kubernetes
- 出典: LangChain Blog
- 日付: 2026-08-06
- リンク: https://www.langchain.com/blog/how-we-build-an-autonomous-sre-agent-for-kubernetes-deployments
- 要約: Kubernetes デプロイを扱う自律 SRE エージェントの構築事例。Deep Agents、LangSmith tracing、evals、人間による変更承認を組み合わせ、運用の現場で安全に回るループを作る話になっている。
- なぜ面白いか:
  - 技術: 観測、計画、実行、検証、人間承認を一つの運用ループとして束ね、SRE の変更管理にエージェントを組み込んでいる。
  - 人文: ethics の観点では、障害対応を自動化しても「誰が最終責任を持つか」を承認点で残している点が重要。history 的には、これは自動運転の監督者問題がソフトウェア運用へ移植された例として読める。

### 3. Real-Time Detection and Repair of LLM Agent Failures
- 出典: arXiv
- 日付: 2026-08-03
- リンク: http://arxiv.org/abs/2608.02464v1
- 要約: LLM エージェントが途中でループ、ツールエラー連鎖、目標逸脱、捏造、汚染コンテンツの吸収を起こす問題に対し、各ステップを別 LLM で判定するのではなく、実行テレメトリだけで低コストに検知・修復する研究。2,823 件のエージェント実行を使い、健康な実行のみで訓練したモニタが失敗検知に有効だと報告している。
- なぜ面白いか:
  - 技術: loop engineering のボトルネックである「実行中の破綻」を、マイクロ秒級の監視器と CUSUM アラームで扱い、エージェント本体より高価な監査ループを避けようとしている。
  - 人文: philosophy 的には、これはエージェントの「自己反省」を内面ではなく外部観測の制度として設計する発想である。ethics 的にも、失敗後の説明責任だけでなく、失敗の兆候をリアルタイムに止める責任設計へ焦点が移っている。

### 4. OneDayAgent: Towards a Long-Horizon Harness for Autonomous Agents
- 出典: arXiv
- 日付: 2026-08-04
- リンク: http://arxiv.org/abs/2608.05013v1
- 要約: 長時間・複数環境・マルチモーダルな日常タスクを処理するための autonomous agent harness。タスクを境界付きサブタスクに分解し、文脈圧迫下でも実行記憶を維持し、最終成果物を検証・修復する設計が示されている。
- なぜ面白いか:
  - 技術: goal drift、state loss、context overflow を個別の失敗としてではなく、長期実行ループの管理問題としてまとめて扱っている。
  - 人文: anthropology の観点では、日常業務は一回の推論ではなく、忘却・中断・再開を含む生活リズムの中で進むため、この研究はエージェントを人間の時間感覚に近づける試みと言える。narrative 的にも、AIタスクが「一問一答」から「一日を通じた伴走」へ物語を変えている。

### 5. The Art of Loop Engineering（古いが基礎概念として重要）
- 出典: LangChain Blog
- 日付: 2026-06-25（直近14日より古いが、概念整理として現在も重要）
- リンク: https://www.langchain.com/blog/the-art-of-loop-engineering
- 要約: 信頼できるエージェント性能には良いモデルだけでなく、特定タスクに合わせた harness とループ設計が必要だと論じる記事。コア agent loop、ループの積み重ね、拡張、各階層の計測を LangChain のプリミティブに接続している。
- なぜ面白いか:
  - 技術: planning / tool use / observation / evaluation などのループを単位として扱い、エージェント改善をプロンプト調整からシステム設計へ引き上げている。
  - 人文: history 的には、これは制御工学や業務改善の PDCA が LLM エージェントへ再登場したものとして読める。creativity の観点では、開発者の創造性は「一発で正解を出す呪文」ではなく、失敗から学ぶ舞台装置をどう構成するかに移っている。

## arXiv / 学術
- Real-Time Detection and Repair of LLM Agent Failures — arXiv:2608.02464v1。エージェントの実行中失敗をステップテレメトリで検知・修復する研究。
- OneDayAgent: Towards a Long-Horizon Harness for Autonomous Agents — arXiv:2608.05013v1。長期実行・記憶・検証・修復をまとめた harness 研究。
- Formal Verification of Agentic Systems over Operational Data — arXiv:2608.03609v1。業務データを扱うエージェントシステムの形式検証。
- AgentAntibody: An Adaptive Immune System for Defending LLM Agents against Prompt Injection — arXiv:2608.04053v1。経験を蓄積してプロンプトインジェクションへの防御境界を進化させる研究。
- Autoreflection: How Agentic Strange Loops Turn Human Culture into AI Infrastructure — arXiv:2608.03800v1。自己参照的な agentic loop を文化・記憶・設定ファイルの観点から分析する研究。

## メモ
- Boris Cherny優先の有無: Claude 系中心のトピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語 X 検索も試行したが、X 検索ツールが `personal-team-blocked:spending-limit` で利用できなかったため、今回の本文には X 投稿を採用していない。
- 注意点・誇張リスク: Web 検索ツールも Firecrawl 未設定で利用できなかったため、直接取得できた公式 RSS/API（LangChain Blog RSS、OpenAI RSS、GitHub Releases、arXiv API）に限定した。2026-06-25 の LangChain 記事は直近14日外だが、トピック名そのものを扱う基礎記事として明記して採用した。

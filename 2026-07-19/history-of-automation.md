# History of Automation トレンド調査 (2026-07-19)

- 調査日: 2026-07-19
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
自動化の議論は「人を置き換える機械」から、「誰が、どの証跡で、進化するエージェントを統治するのか」という制度設計の問題へ移っている。

## トップ5

### 1. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans
- 出典: arXiv
- 日付: 2026-07-12 submitted
- リンク: https://arxiv.org/abs/2607.10878
- 要約: AIエージェントが、ツール利用・委任・経験学習・自己変更を行う「持続的なチーム」へ移るなかで、LOGOSはエージェント、ツール、知識、テスト、権限、ポリシーを版管理された agent pack として扱う統治レイヤーを提案している。活動ログ、fail-closed 検証、人間管理ポリシーを通じ、学習済みプロンプトやスキルを即時本番化せず、未信頼のリリース候補として扱う点が核心。
- なぜ面白いか:
  - 技術: 自動化を単発タスク実行ではなく、権限・テスト・監査証跡を伴う自己進化システムとして実装しようとしている。
  - 人文: 産業革命期の機械管理が「工場規律」を生んだように、エージェント時代の自動化は「変化する労働主体を誰が認可するか」という制度史の問題を再演している。労働者の置換よりも、組織の意思決定権と責任の所在が前景化している。

### 2. BrainPilot: Automating Brain Discovery with Agentic Research
- 出典: arXiv
- 日付: 2026-07-16 submitted
- リンク: https://arxiv.org/abs/2607.15079
- 要約: BrainPilotは、脳科学研究の文献調査、解析、解釈を専門エージェント群で支援するオープンソースのマルチエージェントシステム。著者らは、脳科学では幻覚、推論ドリフト、専門家介入点の不足が特に高コストになるため、traceable logs と agent-verified results を重視している。
- なぜ面白いか:
  - 技術: 科学研究の自動化を、PIエージェントと専門エージェントの分業、ドメイン知識、追跡可能なログで構成している。
  - 人文: これは「研究者の仕事を自動化する」話であると同時に、研究室という徒弟制・専門判断・信用の文化をソフトウェア化する試みでもある。自動化の歴史における職人知の分解と再編が、知的労働の中核領域に入ってきた事例として読める。

### 3. MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research
- 出典: arXiv
- 日付: 2026-07-16 submitted
- リンク: https://arxiv.org/abs/2607.14582
- 要約: MathCoPilotは、数学者が高水準の方向付けを行い、AIエージェントが形式化や証明作業を継続的な人間の指示下で担う human-in-the-loop 型システム。living proof blueprint、Lean統合検証、論文検索と知識ベース形式化を組み合わせ、完全自律証明器ではなく共生的研究環境を志向している。
- なぜ面白いか:
  - 技術: 証明自動化を「自律エージェント」から「人間が検査・指示・修正できる作業台」へ戻して設計している。
  - 人文: 自動化史では、熟練者の判断を奪う機械化と、熟練者の能力を拡張する道具化が常に競合してきた。MathCoPilotは、数学という高度に象徴的な労働で、分業の線をどこに引くべきかを具体的に問うている。

### 4. What is Agentic AI? / Agentic AI as limited-supervision automation
- 出典: IBM Think（Web）
- 日付: 2026-07-07 modified（確認日: 2026-07-19）
- リンク: https://www.ibm.com/think/topics/agentic-ai
- 要約: IBMは agentic AI を「限定的な監督で特定目標を達成できるAIシステム」と説明し、リアルタイムな問題解決、人間の意思決定の模倣、AI agents の構成要素を整理している。現在の企業向け説明として、自動化がRPA的な手順実行から、目標達成型・判断型のワークフローへ拡張されていることを示す。
- なぜ面白いか:
  - 技術: 目標、計画、ツール利用、監督レベルを軸に、従来のプロセス自動化とAIエージェントの差分を実務語彙で定義している。
  - 人文: 企業の自動化言説は、かつての「省力化」から「限定的監督」へ言葉を変えており、人間の役割を作業者ではなく監督者・例外処理者として再配置する。これは労働史で繰り返されてきた、技能の格上げと不可視化が同時に起きる局面である。

### 5. 混同しやすい「自動化」と「自働化」の違いを理解して業務改善を推進しよう
- 出典: DataEgg（Web、日本語）
- 日付: 2026-07-19 確認（検索結果上は2026-07-17取得）
- リンク: https://dataegg.co.jp/data/519/
- 要約: トヨタ生産方式に由来する「自働化」を、単なる自動化ではなく、異常検知・停止・原因究明を含む品質安定の考え方として解説している。RPA、IT運用の自動復旧、物流搬送ロボットの障害物検知など、製造業以外への応用も示されている。
- なぜ面白いか:
  - 技術: 効率化のための自動実行と、異常時に止まり人間へ接続する自働化を分けることで、AIエージェント設計におけるガードレールの原型を提供している。
  - 人文: 日本語圏の「にんべんの付いた自働化」は、人間を消すのではなく、人間の判断へ戻る余地を機械に埋め込む思想として読める。AIエージェントの倫理でも、完全自律より「止まる・知らせる・説明する」文化が重要になる。

## arXiv / 学術
- LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans — arXiv:2607.10878。自己進化するエージェントチームの統治・監査・ポリシー管理。
- BrainPilot: Automating Brain Discovery with Agentic Research — arXiv:2607.15079。脳科学研究のマルチエージェント自動化と専門家介入。
- MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research — arXiv:2607.14582。数学研究における人間主導・AI実行の共生型自動化。
- 関連として CIPHER: A Decoupled Exploration-Selection Framework for Test-Time Scaling of Data Science Agents — arXiv:2607.14386、NNStar: An end-to-end AI agent for nuclear matter and neutron star physics — arXiv:2607.13930 も確認したが、トップ5では上記3件を優先した。

## メモ
- X検索: 英語・日本語で実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、今回のX由来アイテムは含めていない。
- Web検索: web_search / web_extract は Firecrawl 未設定で失敗したため、Bing RSS検索および直接HTTP取得で代替した。検索・取得できた範囲では、直近14日の本テーマは arXiv のエージェント研究が最も濃かった。
- 日本語アカウントの扱い: X検索不可のため確認できず。代替として日本語Web記事（自動化/自働化）を1件採用した。
- 注意点・誇張リスク: Web記事の日付は公開日が明示されないものがあり、確認日または検索結果取得日として扱った。自動化の歴史との接続は、各出典の直接主張ではなく、確認済み内容をもとにした本調査の解釈である。

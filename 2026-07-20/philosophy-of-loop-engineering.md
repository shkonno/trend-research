# Philosophy of Loop Engineering トレンド調査 (2026-07-20)

- 調査日: 2026-07-20
- 情報源: X検索（英語・日本語、実行したがクレジット上限で取得不可） / Web検索（実行したがFirecrawl未設定で取得不可） / arXiv API
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

Loop engineering は「エージェントを回す技術」から、「どの観察を信じ、どの修正を記憶し、誰がループの成長を統治するのか」を問う実践的な認識論へ移っている。

## トップ5

### 1. MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research
- 出典: arXiv
- 日付: 2026-07-16
- リンク: http://arxiv.org/abs/2607.14582
- 要約: 数学者が高次の方向づけを行い、AIエージェントが形式化や証明作業を継続的なフィードバック下で担う human-in-the-loop 型の数学研究システムを提案している。自律証明器ではなく、人間の問いと機械の探索を反復的に噛み合わせる設計が中心にある。
- なぜ面白いか:
  - 技術: ループの制御点を「最終回答」ではなく、方向づけ・形式化・検証の途中過程に分散させる設計として読める。
  - 人文: これは数学的知識を孤立した証明結果ではなく、研究者と機械の共同実践として捉え直す動きである。ポラニー的な暗黙知や、実践共同体の中で成立する判断の問題に近い。

### 2. LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans
- 出典: arXiv
- 日付: 2026-07-12
- リンク: http://arxiv.org/abs/2607.10878
- 要約: ツール利用・委譲・経験学習を行う永続的なAIエージェントチームに対し、自己進化とガバナンスのためのプラガブルな層を提案している。問題設定は「エージェントが何をできるか」から「エージェントが何になることを誰が許すのか」へ移っている。
- なぜ面白いか:
  - 技術: マルチエージェントの反復的な自己変更を、ログ・ルール・許可・検証のレイヤーで統治する loop engineering の中核課題を扱っている。
  - 人文: サイバネティクスでいう二階の観察、つまりシステムを制御する観察者自身をどう設計するかという問いに直結する。AIチームを「成長する制度」と見る点が哲学的に重要である。

### 3. StateFuse: Deterministic Conflict-Preserving Memory for Multi-Agent Systems
- 出典: arXiv
- 日付: 2026-07-07
- リンク: http://arxiv.org/abs/2607.05844
- 要約: 分岐・リトライ・複製を通じて蓄積される矛盾した観察を、単純な上書きで潰さず、CRDT/OpSetに基づく決定的で衝突保存的なメモリとして扱う提案。履歴、明示的な conflict object、訂正可能性をエージェント向けの意味論として整える。
- なぜ面白いか:
  - 技術: エージェントループ内の記憶を「正しい一つの状態」ではなく、矛盾を保持して後から検査できる状態として設計している。
  - 人文: 認識論的には、誤りや不一致を消すのでなく公共的に可視化する設計である。これは実験ノート、判例、歴史叙述のように、知識を訂正可能なアーカイブとして扱う思想に近い。

### 4. Human-Centric Reflective Architecture for Human-AI Collaborative Decision-Making
- 出典: arXiv
- 日付: 2026-07-03（直近14日よりやや古いが関連性が高いため採用）
- リンク: http://arxiv.org/abs/2607.03025
- 要約: LLMを用いた意思決定支援で、人間がAIに過信・過小信頼しやすい問題を扱い、人間中心の反省的アーキテクチャを提案している。非決定性やリスクを前提に、人間の期待・選好・必要に合わせて判断ループを調整することを狙う。
- なぜ面白いか:
  - 技術: ループを単なる自動化パイプラインではなく、信頼較正と反省のインターフェースを含む制御系として設計している。
  - 人文: 「正しい助言」だけでなく「人がどのように助言を信じるか」を扱う点で、認識論と倫理が重なる。実践知とは、答えを出す能力だけでなく、依存の仕方を学ぶ能力でもある。

### 5. Don’t Blindly Trust It: How Unreliable Feedback Breaks Tool-Using LLM Agents
- 出典: arXiv
- 日付: 2026-06-19（古いが、feedback loop の基礎リスクとして重要）
- リンク: http://arxiv.org/abs/2606.21409
- 要約: ツール利用エージェントの性能向上が、信頼できる外部フィードバックを前提としている点を検証し、誤った観察が返るとエージェントループがどのように壊れるかを比較実験で示している。観察だけを faithful / misleading / absent に変える matched-loop 設計が特徴。
- なぜ面白いか:
  - 技術: ループの改善はフィードバックの量ではなく、観察の信頼性と検証可能性に依存することを実験的に示している。
  - 人文: これは「経験から学ぶ」という素朴な信念への警告である。経験はそのまま知識になるのではなく、解釈・証言・検証の制度を通じて初めて知識になる。

## arXiv / 学術

- MathCoPilot: An Interactive System for Human-AI Symbiotic Paradigm of Mathematical Research — arXiv:2607.14582。人間が研究方向を握り、AIが形式化・証明を担う共生的ループ。
- LOGOS: A Living Logic for AI Agent Teams That Evolve With Humans — arXiv:2607.10878。自己進化するエージェントチームのガバナンス層。
- StateFuse: Deterministic Conflict-Preserving Memory for Multi-Agent Systems — arXiv:2607.05844。矛盾を消さずに保存するマルチエージェント記憶。
- Human-Centric Reflective Architecture for Human-AI Collaborative Decision-Making — arXiv:2607.03025。人間中心の反省的意思決定ループ。
- Don’t Blindly Trust It: How Unreliable Feedback Breaks Tool-Using LLM Agents — arXiv:2606.21409。信頼できないフィードバックがツール利用エージェントを壊す条件の検証。

## メモ

- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索も実行したが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため取得できなかった。
- 注意点・誇張リスク: Web検索ツールはFirecrawl未設定で失敗した。代替として arXiv API を直接利用し、実在するarXiv URLと要約のみを採用した。X/Web由来の新規議論は本ファイルには含めていないため、今日の公開議論全体ではなく、学術プレプリント中心の限定的なスナップショットである。

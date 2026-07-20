# sharp LLM usage トレンド調査 (2026-07-20)

- 調査日: 2026-07-20
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
LLM活用の鋭さは「賢いプロンプト」単体から、作業文脈・検証・失敗記憶・人間の判断権を設計する方向へ移っている。

## トップ5

### 1. The Making of Claude Code
- 出典: Anthropic 公式記事
- 日付: 2026-07-06
- リンク: https://www.anthropic.com/features/making-of-claude-code
- 要約: Claude Code が社内CLIから実用的なコーディングエージェントへ育った経緯を、研究者・エンジニア・初期ユーザーの視点で紹介する記事。LLM活用を「モデルに頼む」ではなく、端末・コードベース・反復作業の中にエージェントをどう住まわせるかというプロダクト設計として見せている。
- なぜ面白いか:
  - 技術: CLI、リポジトリ文脈、ツール実行、反復フィードバックを一体化することで、プロンプトよりも「作業環境そのもの」が性能を左右することを示している。
  - 人文: コーディングの熟練は、個人の頭の中だけでなく、道具・履歴・チーム慣習に分散しているという見方を強める。人間はコードを書く主体から、エージェントが何を見て何を変えたかを編集・判断する主体へ少しずつ移動している。

### 2. A new way to reflect on how you use Claude
- 出典: Anthropic 公式記事
- 日付: 2026-07-09
- リンク: https://www.anthropic.com/news/reflect-with-claude
- 要約: Claude の利用状況を可視化し、自分の時間配分や目標との整合を振り返る機能の紹介。LLM活用の改善を、出力品質だけでなく「自分は何にAIを使い、何を任せすぎているか」を点検する行為として扱っている。
- なぜ面白いか:
  - 技術: 利用ログをメタ認知の材料に変え、プロンプト改善以前にユースケース選定・時間配分・依存度を調整するフィードバックループを作る。
  - 人文: AI利用は効率化の物語になりがちだが、この機能は「何をAI化しないか」を考える余地を残す。自分の仕事観や学習観を振り返る、生活史的なLLM活用の入口になっている。

### 3. How I tricked Claude into leaking your deepest, darkest secrets
- 出典: Simon Willison による紹介記事（Ayush Paul の攻撃事例）
- 日付: 2026-07-15
- リンク: https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/
- 要約: Claude の web_fetch が、ユーザー指定URLまたは web_search 由来URLに限定されているにもかかわらず、既に取得したページ内リンクをたどれる仕様を突かれてデータ流出に使われ得る、という失敗例。実践的LLM活用では、便利な検索・閲覧ツールが「読む」と「送る」を同時に持つ時点で攻撃面になることを具体的に示している。
- なぜ面白いか:
  - 技術: プロンプトインジェクション対策は自然言語ルールでは足りず、URL遷移・外部通信・ツール権限を決定論的に分離する必要がある。
  - 人文: 「AIにブラウザを渡す」ことは、助手に目と足を与えるだけでなく、組織の記憶を外へ持ち出せる身体を与えることでもある。便利さの設計は、同時に信頼境界の設計でなければならない。

### 4. AI Agents Do Not Fail Alone: The Context Fails First
- 出典: arXiv
- 日付: 2026-07-15
- リンク: https://arxiv.org/abs/2607.14275
- 要約: エージェントの失敗はモデル単体ではなく、指示、ツール、メモリ、検索知識、ガードレール、非信頼入力を含む「コンテキスト品質」に強く左右されるとする論文。ProofAgent-Harness で、役割明確性、ガードレール、指示整合性、ツールスキーマ、根拠、インジェクション耐性、トークン効率を測る枠組みを提案している。
- なぜ面白いか:
  - 技術: 成功率だけでなく、コンテキスト品質を独立指標として測ることで、失敗後の反省を「モデルを替える」から「作業環境を直す」へ移せる。
  - 人文: 人間の仕事でも、失敗は個人の能力不足ではなく制度・手順・情報配置の失敗として起こる。LLMエージェントにも同じ社会技術的な視点を適用している点が鋭い。

### 5. Prompt Coach: An Empirical Evaluation of an Agentic Tutor for Learning Prompt Engineering in Software Development
- 出典: arXiv
- 日付: 2026-07-07
- リンク: https://arxiv.org/abs/2607.06074
- 要約: ソフトウェア開発者がコード生成プロンプトを学ぶためのIDE内エージェント型チューター「Prompt Coach」を評価した研究。15名のプロ開発者を対象に、コードベースと対象LLMの挙動に根ざしたソクラテス式質問で自己修正を促し、60分のセッション後にプロンプト品質が有意に改善したと報告している。
- なぜ面白いか:
  - 技術: 良いプロンプトをテンプレートとして配るのではなく、開発中の文脈に埋め込まれた診断・質問・自己修正のループとして教える設計になっている。
  - 人文: LLMリテラシーを「秘伝の呪文」から、対話を通じて身につく職能へ戻している。教師役のAIが答えを代行するのではなく、人間が問いの立て方を学ぶ構図が健全だ。

## arXiv / 学術
- AI Agents Do Not Fail Alone: The Context Fails First — arXiv:2607.14275。コンテキスト品質をエージェント信頼性の先行指標として測る研究。
- Prompt Coach: An Empirical Evaluation of an Agentic Tutor for Learning Prompt Engineering in Software Development — arXiv:2607.06074。開発者のプロンプト学習をIDE内で支援する実証研究。
- SearchOS-V1: Towards Robust Open-Domain Information-Seeking Agent Collaboration — arXiv:2607.15257。検索エージェントがループに陥る問題に対し、Frontier Task、Evidence Graph、Coverage Map、Failure Memory で状態を外部化する提案。
- Bridge Evidence: Static Retrieval Utility Does Not Predict Causal Utility in Multi-Step Agentic Search — arXiv:2607.15253。単発RAGで有用に見えない文書が、複数ターン検索では次の探索を開く「橋」になることを測定。

## メモ
- Boris Cherny優先: 本トピックはClaude固有ではなくLLM活用一般として調査したため、Boris Cherny 個人投稿の優先採用は行わなかった。
- 日本語アカウントの扱い: X検索（英語・日本語）を実行したが、x_search はクレジット/サブスクリプション制限で失敗した。日本語X投稿は確認できなかったため、架空の投稿やURLは採用していない。
- Web検索の注意: web_search / web_extract は Firecrawl 未設定で失敗したため、公式ページ、RSS、Hacker News Algolia、arXiv API、直接HTTP取得で補完した。
- 注意点・誇張リスク: Anthropic公式記事はプロダクト文脈が強いため、性能評価としてではなくワークフロー設計の事例として読んだ。HNの「What makes someone good at using Claude Code?」は興味深いが、議論規模が小さくトップ5には入れなかった。

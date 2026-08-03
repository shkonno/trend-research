# sharp LLM usage トレンド調査 (2026-08-03)

- 調査日: 2026-08-03
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「うまいプロンプト」単体より、LLMに渡す文脈、作業分解、再現可能な評価、そして人間が読める領域言語をどう設計するかに、鋭い実践知が移っています。

## トップ5

### 1. Boris Cherny on Trying to Get Claude Code to Rewrite the Claude App
- 出典: Daring Fireball（Boris Cherny / YC Startup School 2026 インタビュー紹介）
- 日付: 2026-08-02
- リンク: https://daringfireball.net/linked/2026/08/02/cherny-claude-swift
- 要約: Claude Code責任者のBoris Chernyが、Claude CodeでClaudeアプリを書き換えようとした話を通じて、現在の技能は「プロンプト文面」よりも「難しいタスクをどう与え、どう制約し、どう人間が伴走するか」にあると示している。単発命令ではなく、タスクの切り出し・レビュー・コンテキスト供給を含むワークフロー設計が焦点になっている。
- なぜ面白いか:
  - 技術: LLM活用のボトルネックを、プロンプトの言い回しから、作業単位・コンテキスト・検証ループの設計へ移して捉えている。
  - 人文: 「AIに仕事を頼む」とは、命令者になることではなく、編集者・教師・同僚の役割を行き来することだと分かる。ソフトウェア開発の熟練が、コードを書く手つきから、他者に仕事を渡す社会的技法へ拡張されている。

### 2. The new rules of context engineering for Claude 5 generation models
- 出典: Claude by Anthropic 公式ブログ
- 日付: 2026-07-24
- リンク: https://claude.com/blog/the-new-rules-of-context-engineering-for-claude-5-generation-models
- 要約: Claude 5世代モデル向けに、長いコンテキストをただ詰め込むのではなく、目的に合う情報を選び、順序づけ、不要なノイズを減らす「コンテキストエンジニアリング」の重要性を打ち出している。鋭いLLM利用の中心が、モデル選びだけでなく、入力空間そのものの設計へ移ったことを示す記事。
- なぜ面白いか:
  - 技術: 長文コンテキスト時代の性能改善を、RAG・ファイル投入・システム指示の量ではなく、情報の構造化と優先順位づけの問題として扱っている。
  - 人文: 人間の仕事でも「必要な背景をどう共有するか」が共同作業の質を決める。LLM活用は、知識管理・記憶・申し送りという組織文化の問題を、技術設計の中心に押し上げている。

### 3. Ubiquitous Language is prompt engineering that humans can read
- 出典: Menelaos Vergis ブログ / Hacker Newsで2026-07-30に再注目（記事自体は少し古い）
- 日付: 2026-07-14（直近14日より少し古いが、HNで再浮上）
- リンク: https://menelaos.vergis.net/posts/Why-Domain-Driven-Design-Is-a-Great-Fit-for-Coding-with-Claude
- 要約: LLMは構文よりもドメイン理解でつまずくため、DDDのユビキタス言語を「人間も読めるプロンプトエンジニアリング」として使うべきだ、という実践論。著者はClaudeがShopifyアプリの領域語彙を勝手に作り替える問題を、チームで合意した語彙をコンテキストに組み込むことで改善したと述べている。
- なぜ面白いか:
  - 技術: DDDの用語集、境界づけられたコンテキスト、ドメインルールを、LLM用の高品質コンテキスト素材として再利用する発想が実装に直結する。
  - 人文: これはAI時代の設計文書が「機械への指示」だけでなく「人間同士の合意形成」でもあることを示す。言葉の揺れを放置すると、コードだけでなく組織の意味体系もAIに書き換えられてしまう。

### 4. DFAH-Bench: same agent decision, different tool paths / Replay stability measurement for tool-using AI agents
- 出典: IBM Client Engineering GitHub / Hacker News Show HN
- 日付: 2026-08-02
- リンク: https://github.com/ibm-client-engineering/output-drift-financial-llms
- 要約: 金融オペレーションを題材に、ツール利用エージェントの出力ドリフトとリプレイ安定性を測るDFAH-Benchを公開している。同じ意思決定でもツール呼び出し経路が変わる問題を、再現可能なベンチマーク、`dfah`パッケージ、ワークショップ形式で検証しようとする取り組み。
- なぜ面白いか:
  - 技術: 「答えが合っているか」だけでなく、エージェントが同じ状況で同じように動けるか、ツールパスを再生・比較できるかを評価対象にしている。
  - 人文: 実務でAIを任せるとは、結果だけでなく説明可能な手続きへの信頼を作ることでもある。金融のような領域では、LLMの賢さよりも、後から振り返れる記録と責任の所在が社会的に重要になる。

### 5. AISPA: User-Centric System Prompt Auditing for Large Language Model Applications
- 出典: arXiv
- 日付: 2026-07-30
- リンク: https://arxiv.org/abs/2607.28617
- 要約: 商用AIプロダクト88件のシステムプロンプトに含まれる3,249命令を、ユーザーに関係する8つの観点から監査し、保護的な命令と問題のある命令に分類する研究。LLM活用における「見えないプロンプト」を、品質・安全・ユーザー利益の観点で点検する枠組みとして実用性が高い。
- なぜ面白いか:
  - 技術: システムプロンプトをブラックボックスの魔法ではなく、命令単位で分解し、監査可能な設計対象にしている。
  - 人文: ユーザーは多くの場合、自分に影響する隠れた指示を読めない。LLM時代の信頼は、出力の自然さではなく、背後の制度設計と監査可能性に依存することを示している。

## arXiv / 学術

- AISPA: User-Centric System Prompt Auditing for Large Language Model Applications — arXiv:2607.28617。システムプロンプト監査をユーザー中心に整理する研究で、今回のトップ5に採用。
- Trust but Verify? Uncovering the Security Debt of Autonomous Coding Agents — arXiv:2607.12428。2026-07-14投稿、直近14日からはやや外れるが、自律コーディングエージェントのPRに含まれるセキュリティ負債をLLM-as-a-judgeと手動分析で調べており、検証ループ設計の背景として重要。
- DuplexGen: Adaptive Synthesis of Human-AI Turn-Taking Dialogues — arXiv:2607.26178。2026-07-28投稿、人間とAIのターンテイキングを合成する研究で、会話型ワークフロー設計と関係する。

## メモ

- Boris Cherny優先: Claude Code関連として最優先で確認し、トップ1に採用。
- 日本語アカウントの扱い: X検索ツールで日本語クエリも実行したが、xAI側のクレジット/サブスクリプション制限により取得できなかった。
- 注意点・誇張リスク: HermesのWeb検索・Web抽出もFirecrawl未設定で失敗したため、代替としてHacker News Algolia API、各サイト/RSSの直接HTTP取得、GitHub、arXiv APIを使用した。X上の反応量や日本語圏での拡散度は本調査では確認不能であり、上記順位は取得できたWeb/arXiv情報に基づく「実践的な鋭さ」重視の選定。

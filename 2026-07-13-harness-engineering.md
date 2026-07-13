# Harness engineering トレンド調査 (2026-07-13)

- 調査日: 2026-07-13
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「よいプロンプト」から一段進み、エージェントの失敗を契約・検証・記憶・フックで囲い込む実装論として急速に具体化している。

## トップ5

### 1. From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents
- 出典: arXiv
- 日付: 2026-07-09
- リンク: https://arxiv.org/abs/2607.08028
- 要約: 企業向けLLMエージェントを、プロンプト中心の試作から、コード・マニフェスト・スキーマ・検証アーティファクトで囲んだ監査可能なハーネスへ移す論文。韓国主要企業の公開データを使い、270回の構成境界実行、故障注入、モデル差し替えで、プロンプトだけでは防げない内部トレース漏れや推薦文言違反をハーネス側が止めることを示している。
- なぜ面白いか:
  - 技術: 「モデルが出す部分」と「コードが保証する部分」を分け、source grounding、entity routing、trace、output hygiene を契約として検証する点が、harness engineering を実証可能なソフトウェア工学にしている。
  - 人文: AIに仕事を任せる不安は、能力不足だけでなく「責任の所在が見えない」ことから来る。この論文は、エージェントを信じるのではなく、読者・監査者・運用者が追跡できる制度的な足場を作る方向を示している。

### 2. Remember When It Matters: Proactive Memory Agent for Long-Horizon Agents
- 出典: arXiv
- 日付: 2026-07-09
- リンク: https://arxiv.org/abs/2607.08716
- 要約: 長期タスクで重要な状態が軌跡の中に埋もれて行動に反映されなくなる現象を “behavioral state decay” と呼び、別のメモリエージェントが必要な時だけリマインダーを注入する方式を提案。Terminal-Bench 2.0 と τ²-Bench で pass@1 をそれぞれ +8.3pt、+6.8pt 改善し、既存の agent harness にプラグインできると説明している。
- なぜ面白いか:
  - 技術: ハーネスを単なるツール呼び出し枠ではなく、行動エージェントの外側で状態劣化を検知・補正する制御面として使っている。
  - 人文: 人間の共同作業でも、重要なのは「何を覚えているか」より「いつ思い出させるか」だ。AIチームにも秘書・編集者・相棒のような記憶役が必要になるという、組織論に近い示唆がある。

### 3. Cognitive-structured Multimodal Agent / CMA-Harness
- 出典: arXiv / GitHub
- 日付: 2026-07-09（論文公開）、GitHub更新確認 2026-07-11
- リンク: https://arxiv.org/abs/2607.08497 / https://github.com/caseclose/cma-harness
- 要約: 長期のマルチモーダル対話で画像・テキスト履歴が膨らみすぎる問題に対し、Episodic Visual Memory、retrieval engine、executive controller を分けた認知構造型エージェントを提案。CMA-Harness は永続的マルチモーダル記憶、Web、画像生成・編集・合成ツール、OpenAI互換サービングを統合した実装として公開されている。
- なぜ面白いか:
  - 技術: 視覚履歴をそのままコンテキストに詰めるのではなく、抽象化・検索・実行制御に分けることで、ハーネスがマルチモーダルエージェントの認知アーキテクチャになる。
  - 人文: 「記憶」は人間の主観や物語性とも深く関わる。画像生成・編集エージェントが何を覚え、何を忘れ、どの過去を再活性化するかは、創作の連続性や作者性の問題にもつながる。

### 4. Claude Code Hooks / Subagents / Skills の公式ドキュメント群
- 出典: Anthropic Claude Code Docs
- 日付: 2026-07-13確認（ページ上の明示公開日は確認できず）
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks / https://docs.anthropic.com/en/docs/claude-code/sub-agents / https://docs.anthropic.com/en/docs/claude-code/slash-commands
- 要約: Claude Code の hooks はイベント、設定スキーマ、JSON入出力、終了コード、HTTP/MCP/Prompt hook を扱い、subagents はタスク特化エージェントとコンテキスト分離を扱う。slash commands は現在のページでは skills 拡張の文脈に統合されており、ルール・スキル・フック・サブエージェントを組み合わせると、Claude Code 上で小さな harness を作る部品が揃う。
- なぜ面白いか:
  - 技術: Boris Cherny / Claude Code / loop engineering 方面で重要な接点は、フックでループの前後を観測・制御し、サブエージェントで専門性と文脈を分離し、skillsで再利用可能な手順を配る点にある。
  - 人文: 開発者の役割は「AIに頼む人」から「AIが失敗しにくい舞台を設計する演出家」に近づく。これは自動化に仕事を奪われる物語だけでなく、人間が規範・儀式・環境を設計する物語として読むと面白い。

### 5. 中国語圏コミュニティの Harness Engineering 学習・解説の増殖
- 出典: GitHub / 技術記事
- 日付: GitHub更新 2026-07-12、記事は 2026-05-21 以降の確認（直近14日外のものを含む）
- リンク: https://github.com/deusyu/harness-engineering / https://javaguide.cn/ai/agent/harness-engineering.html
- 要約: deusyu/harness-engineering は「Harness Engineering 学習指南」として概念、実践、翻訳、AGENTS.md、フィードバックループなどをまとめ、GitHub API確認時点で 4,638 stars。JavaGuide の解説は “Agent = Model + Harness” や六層アーキテクチャ、OpenAI・Anthropic・Stripe などの実践例を整理しており、非英語圏で概念が教育コンテンツ化していることを示す。
- なぜ面白いか:
  - 技術: 研究論文だけでなく、AGENTS.md、linter、リポジトリ内ドキュメント、CI、検証ループという日々の開発物に harness engineering が翻訳され始めている。
  - 人文: 新しい技術語がコミュニティで翻訳される時、その社会は単に輸入しているのではなく、自分たちの作業文化に合う比喩と実践へ作り替えている。日本語コミュニティでも今後「プロンプト術」から「環境・契約・検証の設計」へ語彙が移る可能性がある。

## arXiv / 学術
- 見つかったもの:
  - From Prompts to Contracts: Harness Engineering for Auditable Enterprise LLM Agents — arXiv:2607.08028
  - Remember When It Matters: Proactive Memory Agent for Long-Horizon Agents — arXiv:2607.08716
  - Cognitive-structured Multimodal Agent for Multimodal Understanding, Generation, and Editing — arXiv:2607.08497

## メモ
- Boris Cherny優先の有無: X検索では `from:bcherny`、Boris Cherny、Claude Code、loop engineering、harness の組み合わせを優先して試行したが、x_search はクレジット上限エラーで取得不能だった。Bing RSSでも Boris Cherny と harness / loop engineering の有意な結果は確認できなかったため、確認済みリンクとしては採用していない。
- 日本語アカウントの扱い: 日本語X検索も同じ x_search クレジット上限で取得不能。Web検索では日本語クエリが汎用Claude記事に流れ、Harness engineering の高シグナルな日本語記事は確認できなかった。一方、中国語圏のGitHub・JavaGuide・Zhihu/CSDN系の記事は多数確認されたため、非英語圏コミュニティの代表例として中国語圏を1件採用した。
- 注意点・誇張リスク: Web検索ツール本体は未設定で失敗したため、Bing RSS、GitHub API、arXiv API、直接HTTP取得で代替した。GitHub上には短時間に更新される低スターの harness/Claude Code リポジトリが大量にあり、スパム的・テンプレ的なものを避け、本文ではスター数や論文リンクで検証しやすいものだけを採用した。

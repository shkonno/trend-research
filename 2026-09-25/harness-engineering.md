# Harness engineering トレンド調査 (2026-09-25)

- 調査日: 2026-09-25
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Harness engineering は「CI/CDツール」から、AIエージェントを安全に動かすための実行基盤・監査可能な制御面・失敗回復ループへと意味が広がっている。

## トップ5

### 1. Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reusable Specialist Agents
- 出典: arXiv
- 日付: 2026-09-22
- リンク: https://arxiv.org/abs/2609.26760
- 要約: LLMエージェントに毎回長い文脈で制御戦略を再構成させるのではなく、失敗トレースから再利用可能な「harness」自体を成長させる研究。BrowseComp-Plus と WebArena-Verified で、複数モデル設定において成功率向上とLLM呼び出し削減を示している。
- なぜ面白いか:
  - 技術: 「コンテキストを増やす」のではなく「実行制御コードを学習・蓄積する」方向で、Claude Code や loop engineering 的な反復修正ワークフローに直結する設計論になっている。
  - 人文: エージェントの賢さを個々の応答能力ではなく、組織が残す手順・足場・記憶として捉える点が面白い。熟練者の暗黙知を、プロンプトではなく運用可能な制度へ変換する議論として読める。

### 2. Jev's Auditable Decision Primitive at Harness
- 出典: Harness Blog
- 日付: 2026-09-21
- リンク: https://www.harness.io/blog/jev-decision-primitive-agent-governance
- 要約: Harness が本番環境で、評価・モデルルーティング・リスクスコアリングに使った「型付きで監査可能な判断プリミティブ」Jev を紹介している。エージェントの判断を文章のまま流すのではなく、検証できる構造化イベントとして扱う発想が中心。
- なぜ面白いか:
  - 技術: agent harness engineering に必要な「判断の型」「監査ログ」「リスク別ルーティング」を、CI/CDのリリース制御に近い部品として切り出している。
  - 人文: AIの判断をブラックボックスの“意見”ではなく、責任の所在を追える社会的記録にする試みである。自律性を許すほど、あとから説明できる形式に落とす文化が重要になる。

### 3. Govern AI Behavior Like You Govern Releases
- 出典: Harness Blog
- 日付: 2026-09-17
- リンク: https://www.harness.io/blog/beyond-the-prompt-governing-ai-behavior-like-you-govern
- 要約: プロンプトやモデル変更を、再デプロイなしにテスト・承認・ロールバック可能な「AI Config」として管理すべきだと論じる記事。大企業でエージェント導入が進む一方、挙動変更の頻度が既存の運用統制を追い越している問題を扱う。
- なぜ面白いか:
  - 技術: AIの振る舞いをリリース成果物と同じく設定・評価・承認・ロールバック対象にすることで、loop engineering の反復をガバナンス可能な変更管理に接続している。
  - 人文: 「プロンプトは文章」ではなく「組織の規範を実行する設定」だと見る視点が重要。AI導入は技術更新であると同時に、誰が行動規範を変更できるのかという権限設計の問題でもある。

### 4. Platform Engineering in the Age of AI
- 出典: Harness Blog
- 日付: 2026-09-17
- リンク: https://www.harness.io/blog/platform-engineering-in-the-age-of-ai
- 要約: Harness、DKB、Shine の登壇者による InfoQ ウェビナーをもとに、AIが開発者の補助からプラットフォーム内で動く主体へ変わる中で、94%のエンジニアリングリーダーが重要なAIメトリクスを欠いているとする論点を紹介している。
- なぜ面白いか:
  - 技術: 開発者ポータル、CI/CD、コスト、セキュリティ、AI利用状況を横断して測る基盤がないと、AIエージェントの効果もリスクも運用判断に乗らないことを示している。
  - 人文: 指標がない組織では、AIは希望や不安として語られやすい。何を測るかは、組織が何を価値とみなすかを決める文化的行為でもある。

### 5. How Harness orchestrates LLM security scanning
- 出典: Harness Blog
- 日付: 2026-09-23
- リンク: https://www.harness.io/blog/how-harness-orchestrates-llm-security-scanning
- 要約: Harness STO が LLM セキュリティスキャンをどこで起動し、スコープをどう絞り、推論をどう制約し、出力をどう標準化するかを説明している。差分に集中するインクリメンタルスキャンにより、コストを83%削減しつつパイプラインで扱いやすい結果にする点が強調されている。
- なぜ面白いか:
  - 技術: LLMを単発の脆弱性診断役にするのではなく、CI/CD内で差分・制約・標準出力を持つ実行単位としてオーケストレーションしている。
  - 人文: セキュリティレビューを「怖い専門家の門番」から、日常的な開発ループの一部へ戻す試みとして読める。開発者の速度と安全の対立を、ワークフロー設計で和らげようとしている点が興味深い。

## arXiv / 学術
- 見つかりました: “Grow the Harness, Not the Context: From Strategy-Free Scaffolds to Reusable Specialist Agents” (arXiv:2609.26760)。harness をプロンプト外部の再利用可能な制御構造として成長させる研究で、本日の最重要項目として採用。
- 関連だが古いもの: “Towards Agentic Cloud Engineering: Graph and Loop Engineering with a Zero-Trust Agent Harness” (arXiv:2609.00050、2026-08-30)。直近14日より古いが、graph engineering / loop engineering / zero-trust agent harness を明示的に接続しており、背景文献として重要。
- 関連: “A Hybrid Rule-Based and AI-Augmented Framework for Automatic Failure Recovery in DevOps Deployments” (arXiv:2609.26838、2026-09-21)。Harness社の記事ではないが、失敗検知・分類・自動回復という点で harness engineering の運用面と接続する。

## メモ
- Boris Cherny優先の有無: X検索で Boris Cherny / @bcherny、Claude Code、loop engineering との接点を確認しようとしたが、x_search が `personal-team-blocked:spending-limit` で失敗したため、今回の直接確認はできなかった。代替として arXiv API と Harness公式RSS/ページを実HTTP取得して確認した。
- 日本語アカウントの扱い: 日本語X検索も同じく x_search のクレジット制限で失敗。Web検索ツールも Firecrawl 未設定で利用不可だったため、Bing/DuckDuckGoの直接HTML取得を試したが、有用な日本語コミュニティ情報は確認できなかった。
- 注意点・誇張リスク: Harness公式ブログは企業発信であり、数値や効果はプロダクト文脈の主張として読む必要がある。arXiv論文は実在IDをAPIで確認したもののみ記載し、未確認のX投稿や架空リンクは含めていない。

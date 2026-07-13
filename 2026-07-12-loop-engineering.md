# Loop engineering トレンド調査 (2026-07-12)

- 調査日: 2026-07-12
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop engineering は「賢いエージェントを作る」から一歩進み、観測・検証・介入・記憶・停止条件まで含む制御ループをどう設計するか、という実務的なテーマに寄ってきています。

## トップ5

### 1. Test-Time Harness Evolution（TTHE）
- 出典: arXiv
- 日付: 2026-07-09
- リンク: https://arxiv.org/abs/2607.08124v1
- 要約: LLMエージェントの振る舞いはモデルだけでなく、文脈構築、ツール呼び出し、検証、失敗回復を担う「ハーネス」によって決まる、という問題設定の論文です。デプロイ前だけでなくテスト時・運用時にハーネス自体を進化させる発想が、Loop engineering の中核である「実行→観測→修正」のループを明確にしています。
- なぜ面白いか:
  - 技術: プロンプト改善ではなく、ツール実行・検証・回復を包む実行ハーネスを最適化対象にしている点が、エージェント運用の抽象度を一段上げています。
  - 人文: philosophy の観点では、知能を「頭の中の推論」ではなく、環境と制度に埋め込まれた行為の循環として見る立場に近いです。narrative としても、AI開発の主人公がモデル単体から、失敗を覚えて作法を変える作業環境全体へ移っています。

### 2. AgentTether: Graph-Guided Diagnosis and Runtime Intervention for Reliable LLM Agent Operation
- 出典: arXiv
- 日付: 2026-07-07
- リンク: https://arxiv.org/abs/2607.06273v1
- 要約: マルチステップで状態を持つLLMエージェントでは、初期の判断ミスが後続の外部状態変更に連鎖します。この論文は、グラフに基づく診断と実行時介入で、壊れた軌道を検出・修復する方向を示しています。
- なぜ面白いか:
  - 技術: エージェントの「軌道」をグラフとして扱い、失敗箇所の診断と介入をランタイムの一部にするため、単発の評価よりも実運用ループに近い設計です。
  - 人文: ethics の観点では、自律システムに「あとから止める・ほどく・介入する」余地を組み込むことは責任配分の設計そのものです。history 的には、航空・医療・金融で発達した事故調査とフェイルセーフの文化が、ソフトウェアエージェントにも移植されつつあります。

### 3. Biological Motifs for Agentic Control
- 出典: arXiv
- 日付: 2026-07-05
- リンク: https://arxiv.org/abs/2607.04240v1
- 要約: LLMが自律エージェント化する中で、幻覚の連鎖、無限ループ、状態管理の不安定さが課題になると整理し、生物システムの制御モチーフを参考にしたエージェント制御を提案する論文です。Loop engineering を「生き物の恒常性」に近い設計問題として読めます。
- なぜ面白いか:
  - 技術: 無限ループや状態暴走を、単なるバグではなく制御アーキテクチャの欠落として扱い、フィードバック、抑制、階層制御を設計語彙に入れています。
  - 人文: anthropology の観点では、人間組織も儀礼・監督・例外処理で暴走を抑えてきたため、AIエージェントの制御は社会制度のミニチュアに見えます。creativity の面では、生物から借りた比喩が新しい実装パターンを生む可能性があります。

### 4. LangGraph overview / Thinking in LangGraph
- 出典: Web（LangChain Docs）
- 日付: 更新日不明（2026-07-12確認、継続的ドキュメント。直近14日とは限らないが実務上重要）
- リンク: https://docs.langchain.com/oss/python/langgraph/overview
- 要約: LangGraph は、一般的なLLM・ツール呼び出しループの上に、durable execution、streaming、human-in-the-loop、interrupt、time travel、memory などを置くエージェント・オーケストレーション基盤として説明されています。関連ページ「Thinking in LangGraph」では、エラー種別に応じてLLMへ戻す、人間に割り込ませる、開発者が処理する、といったループ設計が具体化されています。
- なぜ面白いか:
  - 技術: 状態・ノード・割り込み・チェックポイントを明示することで、エージェントのループをデバッグ可能で再開可能なワークフローに変換しています。
  - 人文: philosophy の観点では、完全自律ではなく「どこで人間に戻すか」を設計することが、行為主体性の境界線を描く作業になります。narrative としては、AIを魔法の箱ではなく、途中経過を見せ、止まり、相談する共同作業者として語り直しています。

### 5. Claude Code Hooks reference
- 出典: Web（Anthropic Docs）
- 日付: 更新日不明（2026-07-12確認、継続的ドキュメント。直近14日とは限らないが実務上重要）
- リンク: https://docs.anthropic.com/en/docs/claude-code/hooks
- 要約: Claude Code の Hooks は、SessionStart / UserPromptSubmit / PreToolUse / PostToolUse / Stop など、エージェントのループ内イベントに対して外部コマンドを差し込む仕組みです。ツール実行前後で許可・拒否・フィードバック・停止を返せるため、ローカルな開発ループにガードレールと観測点を置けます。
- なぜ面白いか:
  - 技術: ループ内のイベント境界をAPI化することで、lint、テスト、権限チェック、監査ログ、組織固有ルールをエージェントの実行経路に直接接続できます。
  - 人文: ethics の観点では、AIの行為を事後的に叱るのではなく、行為の直前・直後に制度的な関門を置く設計です。history 的には、工場の安全スイッチやチェックリスト文化が、コードを書くAIの周囲に再発明されているように見えます。

## arXiv / 学術
- 確認されました。主な関連候補:
  - Test-Time Harness Evolution — arXiv:2607.08124v1（2026-07-09）
  - AgentTether: Graph-Guided Diagnosis and Runtime Intervention for Reliable LLM Agent Operation — arXiv:2607.06273v1（2026-07-07）
  - Biological Motifs for Agentic Control — arXiv:2607.04240v1（2026-07-05）
  - Human-Centric Reflective Architecture for Human-AI Collaborative Decision-Making — arXiv:2607.03025v1（2026-07-03）
  - Human-in-the-Loop Nugget Annotation for Accountable LLM-as-a-Judge Evaluations — arXiv:2606.29033v2（2026-06-27、対象期間より少し古いが関連）

## メモ
- X検索: x_search を英語・日本語・agent loop 系クエリで実行しましたが、実行環境の xAI / Grok クレジット制限により `personal-team-blocked:spending-limit` で失敗しました。そのため、X由来の投稿はトップ5に含めていません。
- Web検索: Hermes の web_search / web_extract は Firecrawl 未設定で失敗しました。代替として、Bing検索を端末経由で実行し、さらに LangChain / Anthropic / OpenAI などの公開ドキュメントを直接取得して確認しました。
- Boris Cherny優先: 本トピックは Claude 固有トピックではないため必須ではありません。関連検索は試みましたが、今回の実行では信頼できる直近投稿を確認できませんでした。
- 日本語アカウントの扱い: 日本語X検索は実行しましたが、同じクレジット制限で取得不能でした。日本語の一般Web検索では Microsoft Loop やLUUPなどノイズが多く、AIエージェントの Loop engineering として採用できるものは限定的でした。
- 注意点・誇張リスク: 「Loop engineering」はまだ一般に固定した用語というより、エージェントの実行・評価・介入・回復ループを設計する実務領域として現れている概念です。トップ5は、厳密な語句一致よりもこの設計課題に直接効くものを優先しました。

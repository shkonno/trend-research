# DDD トレンド調査 (2026-08-06)

- 調査日: 2026-08-06
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

DDDは「AIに設計を丸投げする方法」ではなく、LLMを相手にユビキタス言語・イベント・境界を早く可視化し、人間が難しい判断に集中するための作法として再発見されている。

## トップ5

### 1. faceto: typed fileからLLMと議論できるEvent Stormingボードへ
- 出典: GitHubリポジトリ / Web
- 日付: 2026-08-03更新
- リンク: https://github.com/bastien-gallay/faceto
- 要約: `faceto`は、型付きのモデルファイルからEvent StormingのHTML/SVGボードを生成し、要素ごとに短いメモを残して次のLLMセッションに反映できるRust製ツール。READMEでは、Event Stormingを起点にcontext map、bounded context canvas、core domain chartへ進む「ワークショップの道筋」を志向している。
- なぜ面白いか:
  - 技術: Event Stormingの付箋・レーン・ホットスポットを、LLMが扱いやすい構造化ファイルと人間が眺めやすい視覚ボードの往復に変換している点が実用的。
  - 人文: DDDのワークショップは本来、会話・沈黙・違和感を扱う文化的な場だが、このツールはその場を「AIと一緒に考えるための共有物」に再設計している。設計成果物よりも、会話の記憶をどう残すかが主題になっている。

### 2. DomainDL Agents: bounded contextごとにDDDコード生成サブエージェントを分ける試み
- 出典: GitHubリポジトリ / Web
- 日付: 2026-07-30更新
- リンク: https://github.com/GianL22/DomainDL-ai
- 要約: `DomainDL Agents`は、FastAPI、MongoDB、LangSmithを使ったDDDコード生成・プロジェクトQ&A向けのマルチエージェントサービス。bounded contextを入力に、Value Object、Entity、Aggregate、Domain Event、Domain Service、Domain Exceptionなど抽象ごとのコーディングサブエージェントへ分解し、TypeScriptの型チェックによる自己修正ループも組み込む。
- なぜ面白いか:
  - 技術: DDDの戦術パターンをエージェントの責務分割に対応させ、生成物をbounded context単位のワークスペースに隔離している。
  - 人文: 「ユビキタス言語をどうコードへ翻訳するか」という熟練者の暗黙知を、エージェント編成と評価指標に落とし込もうとしている。人間の設計者は、コードの細部よりも境界・言葉・例外の意味を監督する役に寄っていく。

### 3. DDD & Design Patterns Skills for Agentic Development: エージェントにDDDの作法を教えるスキルセット
- 出典: GitHubリポジトリ / Web
- 日付: 2026-07-30更新
- リンク: https://github.com/DavidSouther/domain-driven-design
- 要約: Claude Code、Codex、Copilot、Geminiなど複数のエージェント環境で使えるDDD・デザインパターン・TDDライフサイクルのスキル集。READMEは、各ハーネスのツール名に対応しながら、DDDと効果的な開発パターンをエージェントが参照できる構造化知識として配布する設計になっている。
- なぜ面白いか:
  - 技術: DDDを単なるドキュメントではなく、エージェント実行環境にロード可能な「行動規範」としてパッケージングしている。
  - 人文: これはチーム文化の移植に近い。人間の組織でオンボーディングされてきた設計作法が、AIエージェントにも「教育」される対象になりつつあることを示している。

### 4. AI Refinement Method: vibe codingではなくvibe spec'ingへ
- 出典: GitHubリポジトリ / Web
- 日付: 2026-06-24更新（直近14日より古いが、DDD×エージェント設計として重要）
- リンク: https://github.com/nlawstudio/ai-refinement-method
- 要約: `AI Refinement Method`は、自然言語の意図を、event storming、DDD、refinement、受け入れ基準、失敗テストを含む実装前の仕様へ変換するエージェント手法。READMEは「コードが安くなった時代には、仕様品質が新しいボトルネックになる」と位置づけ、AIを実装者ではなく思考の相棒として使うことを強調する。
- なぜ面白いか:
  - 技術: 実装生成の前段に、イベント・境界・脅威・ストーリー・テストを揃えるプロセスを置き、AI coding toolへの引き渡し点を明確にしている。
  - 人文: DDDの価値を「正しいコードを書く技術」ではなく「何を作るべきかを共同で見極める儀式」として再解釈している。AI時代の設計では、速度よりも合意形成の質が競争力になるという視点が強い。

### 5. Automating Domain-Driven Design: Experience with a Prompting Framework
- 出典: arXiv / 学術
- 日付: 2026-03-27（直近14日より古いが、関連arXivとして重要）
- リンク: https://arxiv.org/abs/2603.26244
- 要約: Tobias Eisenreich、Husein Jusic、Stefan Wagnerによる論文。LLMでDDDを自動化するプロンプティングフレームワークとして、ユビキタス言語の確立、Event Stormingのシミュレーション、bounded contextの特定、aggregate設計、技術アーキテクチャへのマッピングの5段階を検証している。結論は、前半の言語・イベント・境界づくりには有用だが、後半では小さな誤りが蓄積し、完全自動化には向かないというもの。
- なぜ面白いか:
  - 技術: LLMが得意な「用語整理・イベント列挙・境界候補出し」と、苦手な「集約設計・アーキテクチャ決定」を段階ごとに切り分けて評価している。
  - 人文: 論文の含意は、AIがアーキテクトを置き換えるのではなく、議論の叩き台を作る「スパーリング相手」になるという点にある。DDDの中心が、人間同士の意味交渉と責任ある判断であることをむしろ再確認している。

## arXiv / 学術

- Automating Domain-Driven Design: Experience with a Prompting Framework / arXiv:2603.26244 / 2026-03-27。DDD活動をLLMプロンプトで支援する実験で、ユビキタス言語・Event Storming・bounded contextまでは有用、aggregate以降は誤りの蓄積が課題と報告。

## メモ

- Boris Cherny優先の有無: Claude固有トピックではないため優先対象外。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールが `personal-team-blocked:spending-limit` で失敗したため、今回のX由来アイテムは未採用。
- 注意点・誇張リスク: Web検索ツールもFirecrawl未設定で失敗したため、代替としてGitHub API、arXiv API、公式/直接HTTP取得を使用した。直近14日の強い公開情報はGitHub更新が中心で、学術・公式イベント情報は古いものまたは今後開催予定を「古い/参考」と明記した。架空リンク・未確認arXiv IDは入れていない。

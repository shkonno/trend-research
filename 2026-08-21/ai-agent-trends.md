# AI agent trends トレンド調査 (2026-08-21)

- 調査日: 2026-08-21
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの焦点は、モデル性能そのものよりも「どの環境で動かし、記憶をどう残し、権限と攻撃面をどう統治するか」という運用インフラへさらに寄っている。

## トップ5

### 1. Epho: Claude Code / Codex / Opencode を HTTP API としてクラウド実行
- タイトル: Epho: Claude Code / Codex / Opencode を HTTP API としてクラウド実行
- 出典: Hacker News / 公式サイト
- 日付: 2026-08-20（HN掲載）
- リンク: https://epho.io
- 要約: Epho は、Claude Code、Codex、Opencode をクラウドサンドボックス上で起動し、リポジトリのclone、入力ファイル配置、MCPサーバー接続、SSEストリーミングを1つのHTTP APIで扱えるようにするサービス。`/api/v1/chat` にprompt、harness、model、repo、provider keyなどを渡すだけで、エージェント実行環境を都度立ち上げられる点を打ち出している。
- なぜ面白いか:
  - 技術: Claude Code系のローカルCLI体験を、サンドボックス・MCP・永続chat_id・非同期実行つきのクラウドAPIへ抽象化しており、agent harness の「実行基盤化」をよく示している。
  - 人文: エージェントを手元の相棒として使う段階から、HTTPで呼び出す外部労働力として組織システムに組み込む段階へ移ると、開発者の仕事は「対話」だけでなく「委任APIの設計」になる。便利さの裏側で、誰の鍵・誰のリポジトリ・どの環境を預けるのかという信頼の再配置が起きている。

### 2. Pond: Claude Code / Codex などのエージェントセッションを自分のS3/ローカルにlossless保存しMCPで検索
- タイトル: Pond: Claude Code / Codex などのエージェントセッションを自分のS3/ローカルにlossless保存しMCPで検索
- 出典: Hacker News / GitHub
- 日付: 2026-08-20（HN掲載、GitHub更新 2026-08-20）
- リンク: https://github.com/tenequm/pond
- 要約: Pond は、Claude Code、Codexなど複数ツールに散らばるエージェントセッションを、自分のローカルディレクトリまたはS3へlosslessに保存し、検索・SQL問い合わせ・MCP経由の再利用を可能にする。READMEでは「過去にどう直したか」をgrepで大量contextにするのではなく、検索された回答として少ないtokenで返す例を示している。
- なぜ面白いか:
  - 技術: エージェントの会話履歴を単なるログではなく、横断検索できる作業記憶・復元可能な実行資産として扱い、MCPで次のエージェントへ戻している。
  - 人文: 人間のチームでも「以前なぜそう決めたか」を忘れることが大きな摩擦になるが、エージェント時代にはその忘却がツールごとのログ断片として増幅される。Pondは、AIとの協働記憶をプラットフォーム企業ではなくユーザー側に置こうとする点で、記憶の所有権をめぐる実践でもある。

### 3. AgentHound: MCP / A2A / agent client / gateway を横断する攻撃的セキュリティフレームワーク
- タイトル: AgentHound: MCP / A2A / agent client / gateway を横断する攻撃的セキュリティフレームワーク
- 出典: GitHub
- 日付: GitHub更新 2026-08-21（作成は2026-04-05のため古いが直近で活発に更新）
- リンク: https://github.com/adithyan-ak/AgentHound
- 要約: AgentHound は、MCP、A2A、agent clients、model gateways、inference servers、vector stores、MLOps、notebooks などを対象にした「agentic infrastructure」の攻撃的セキュリティツール。READMEでは、ローカル認証情報・エージェント設定・到達可能なAIサービスを収集し、互換credentialを再利用してアクセス検証し、攻撃グラフとして分析する流れを説明している。
- なぜ面白いか:
  - 技術: エージェント基盤が増やした攻撃面を、従来のWebアプリやクラウド設定ではなく、MCP/A2A/モデルゲートウェイ/ベクトルストアまで含む新しい資産棚卸しとして扱っている。
  - 人文: エージェントに権限を渡すほど、AIは「助言者」ではなく組織の鍵束を持つ行為者になる。攻撃者視点のツールが現れることは、AIエージェントが実験室の玩具から、守るべき社会的インフラへ移行したサインでもある。

### 4. When Agents Act on Web3: MCP / Skills / Tool Calling の攻撃面を整理するarXiv論文
- タイトル: When Agents Act on Web3: An Attack-Surface Survey of MCP, Skills, and Tool Calling
- 出典: arXiv
- 日付: 2026-08-18
- リンク: http://arxiv.org/abs/2608.17275v1
- 要約: AIエージェントがWeb3上で「読む」だけでなく外部状態を変更するようになると、MCP、skills、tool callingを通じた権限行使が直接的な損失につながる、という攻撃面サーベイ。arXiv API上の要約では、MCP ecosystem で外部状態を変更するtoolの比率が27%から65%へ上昇したとし、ブロックチェーン文脈での被害の不可逆性を強調している。
- なぜ面白いか:
  - 技術: tool callingを便利なI/Oではなく、資産移動や状態変更を伴うトランザクション権限として扱い、MCP/skillsの設計をセキュリティ境界として再定義している。
  - 人文: Web3は失敗の取り消しが難しいため、エージェントへの委任は「ボタンを押してもらう」以上に、代理人へ財産行為を任せることに近い。ここではAI倫理が抽象的な公平性ではなく、署名・同意・取り消し不能性という古典的な契約と責任の問題として戻ってくる。

### 5. A Multi-Agent Platform for Automated Enterprise Analytics and Insight Generation: CrewAI + MCPで企業BIをマルチエージェント化
- タイトル: A Multi-Agent Platform for Automated Enterprise Analytics and Insight Generation
- 出典: arXiv
- 日付: 2026-08-19
- リンク: http://arxiv.org/abs/2608.18740v1
- 要約: CrewAIベースの5つの専門AIエージェントが、自然言語クエリ処理、データ取得・分析、MCP経由の可視化生成、洞察レポート作成までを順に担う企業分析プラットフォームを提案する論文。300件のend-to-endテストで機能正確性95.3%、平均応答24秒、LLM-as-a-Judge品質4.52/5.0、hallucination-free率93.0%などの評価を報告している。
- なぜ面白いか:
  - 技術: マルチエージェントをデモではなく、multi-tenant isolation、query parameterization、dashboard再利用、MCP可視化といった企業BIの制約に接続している。
  - 人文: 企業分析はこれまで、データ担当者と現場担当者の翻訳作業に多く依存してきた。エージェントがその翻訳を肩代わりするなら、誰が「洞察」と呼ばれるものを承認し、誰の問いがダッシュボードとして固定化されるのかという組織文化の問題が前に出る。

## arXiv / 学術
- 見つかりました: `2608.18740v1` “A Multi-Agent Platform for Automated Enterprise Analytics and Insight Generation” — CrewAIとMCPを使った企業分析マルチエージェント基盤。トップ5の5件目として採用。
- 見つかりました: `2608.17275v1` “When Agents Act on Web3: An Attack-Surface Survey of MCP, Skills, and Tool Calling” — MCP/skills/tool callingがWeb3上で状態変更権限を持つ際の攻撃面サーベイ。トップ5の4件目として採用。
- 関連候補: `2608.18050v1` “StagedWorkspace: A Versioned Workspace for Knowledge-Work Agents” — エージェントが扱う文書・コード・表などの作業成果物のバージョン不整合を扱う。
- 関連候補: `2608.17665v1` “GraphWake: Group Polarization via Memory-Mediated Polarization Cascade in LLM-Agent Communities” — LLMエージェント共同体における記憶媒介の分極化を扱う。
- 関連候補: `2608.16246v1` “CompoSkill: Compositional Skill Chain Attacks from Individually Scanner-Passing LLM Agent Skills” — 個別には安全判定を通るskillが組み合わさることで攻撃を構成する問題を扱う。

## メモ
- Boris Cherny優先の有無: @bcherny を含むX検索を実行したが、x_search が `personal-team-blocked:spending-limit` で失敗したため、本調査時点ではBoris Chernyの直近投稿を確認できなかった。
- 日本語アカウントの扱い: 日本語X検索も同じx_search制限で失敗した。日本語Web検索も Firecrawl 未設定により `web_search` が失敗したため、日本語圏の実践例は今回十分に確認できていない。
- 代替調査: Firecrawl/Web検索障害後、terminalから arXiv API、Hacker News Algolia API、GitHub API、GitHub README raw、公式サイトのJina AI経由取得、GitHub Changelogページを直接確認した。
- 注意点・誇張リスク: HN/GitHub発の新規ツールは普及度が未確定であり、今回は「採用済みの定番」ではなく「今出てきている運用・記憶・セキュリティ設計の論点」として選定した。X/Web検索制限があるため、ソーシャル上の反応量ランキングではない。

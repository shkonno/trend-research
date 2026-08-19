# AI agent trends トレンド調査 (2026-08-19)

- 調査日: 2026-08-19
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの話題は「賢い単体モデル」から、「複数のエージェントをどう観察し、統合し、安全に運用するか」という実務インフラへ重心が移っている。

## トップ5

### 1. HarnessRouter: Claude Code / Codex / Hermes などを統一APIで動かすセルフホスト型 agent harness
- タイトル: HarnessRouter: Claude Code / Codex / Hermes などを統一APIで動かすセルフホスト型 agent harness
- 出典: GitHub / Hacker News
- 日付: GitHub作成 2026-08-09、HN掲載 2026-08-17、GitHub更新 2026-08-19
- リンク: https://github.com/HarnessRouter/harnessrouter
- 要約: HarnessRouter Community Edition は、Codex、Claude Code、Hermes など複数のエージェント・ハーネスを、セッション、ストリーミング、ファイル、キャンセル、失敗処理つきの統一インターフェースで扱うセルフホスト基盤。READMEでは Unified Harness Protocol (UHP) への準拠、自分のAPIキー・自分のデータ・テレメトリなしを強調している。
- なぜ面白いか:
  - 技術: エージェント実行環境を「各CLIの個別操作」から「ハーネス間の標準プロトコル」へ抽象化し、運用・監査・差し替えをしやすくしている。
  - 人文: これはAIエージェントを個人の相棒から、組織内の労働インフラとして扱う段階への移行を示す。標準化は便利さだけでなく、誰が実行権限を持ち、失敗や責任をどう記録するかという統治の問題を前面に出す。

### 2. Agents Workbook: Claude Code / Codex の作業ノートをローカルで観察する実験
- タイトル: Agents Workbook: Claude Code / Codex の作業ノートをローカルで観察する実験
- 出典: GitHub / Hacker News
- 日付: GitHub作成 2026-08-15、HN掲載 2026-08-18、GitHub更新 2026-08-18
- リンク: https://github.com/softcane/agents-workbook
- 要約: Agents Workbook は、Claude Code や Codex へのリクエストに「作業ノートを書くためのツール」を追加するローカルプロキシ。ノートは `127.0.0.1:8080` のダッシュボードに流れ、作者は「エージェントの表明した計画が実際の行動と一致するか」を見るための実験だと説明している。
- なぜ面白いか:
  - 技術: エージェントの入出力だけでなく、計画・比較・却下した選択肢をセッション横断で観察するための軽量な可観測性レイヤーになっている。
  - 人文: READMEが「推論を収穫するな」と明記している点が重要で、透明性への欲望とモデル提供者・利用者の境界線が衝突している。エージェントを監督したい人間の不安が、観察ツールという形で具体化している。

### 3. When Agents Coordinate: Measuring Coordination in Multi-Agent AI Coding
- タイトル: When Agents Coordinate: Measuring Coordination in Multi-Agent AI Coding
- 出典: arXiv
- 日付: 2026-08-17
- リンク: http://arxiv.org/abs/2608.16801v1
- 要約: 複数のAI coding agent がプログラミング課題を解く際の「協調」を測定する研究。1902件の実行を、エージェント、ファイル、メッセージ、読み書き、コストを含む時間ネットワークとして表し、成功率や費用だけでは見えないチーム内部の調整を評価する。
- なぜ面白いか:
  - 技術: multi-agent coding の評価指標を、完了可否から通信量・ファイル接触・チーム構造のダイナミクスへ拡張している。
  - 人文: 人間組織で長く問題になってきた「調整コスト」が、AIチームにもそのまま現れている点が面白い。エージェントを増やせば賢くなるという単純な物語ではなく、協働には摩擦と制度設計が必要だと示している。

### 4. When State Becomes an Attack Surface: State-Semantic Injection in LLM-Driven Embodied Agents
- タイトル: When State Becomes an Attack Surface: State-Semantic Injection in LLM-Driven Embodied Agents
- 出典: arXiv
- 日付: 2026-08-17
- リンク: http://arxiv.org/abs/2608.16806v1
- 要約: LLM駆動の embodied agent では、Webや文書だけでなく、環境状態そのものが攻撃面になるという問題を扱う論文。エージェントが知覚し、計画し、ツールやロボット行動へつなげる過程で、状態の意味づけが注入攻撃の対象になり得ると整理している。
- なぜ面白いか:
  - 技術: prompt injection をテキスト入力の問題に閉じず、環境状態・知覚・行動決定まで含む「state-semantic injection」として拡張している。
  - 人文: エージェントが物理世界や業務環境に入るほど、攻撃は言葉ではなく状況の演出になる。これは、人間が詐欺や演技された文脈に騙される構造と似ており、AI安全性が社会的文脈理解の問題でもあることを示す。

### 5. Aident Loadout / aident-skill: エージェントに1,000超のアプリ連携と27,000超の実行アクションを渡すスキル
- タイトル: Aident Loadout / aident-skill: エージェントに1,000超のアプリ連携と27,000超の実行アクションを渡すスキル
- 出典: GitHub / Hacker News
- 日付: HN掲載 2026-08-07、GitHub更新 2026-08-18（リポジトリ作成は2026-02-12のため古いが、直近で再注目・更新）
- リンク: https://github.com/Aident-AI/aident-skill
- 要約: Aident Loadout は、Gmail、Slack、Linear、Google Sheets、Notion、HubSpot、Firecrawl、Exa、Fal などへの接続をAIエージェントに渡し、Aident Vault、監査履歴、27,000超の実行アクションを提供する。READMEのトピックには Claude Code skill、Codex CLI、MCP などが含まれ、チャットやコーディングを越えた実務自動化を狙っている。
- なぜ面白いか:
  - 技術: MCP/skills 的な拡張を通じて、エージェントの能力を「推論」ではなく、実アプリ上の権限・認証・監査可能なアクション集合として束ねている。
  - 人文: ここで問われるのは、AIが何を知っているかより、AIにどの鍵を渡すのかである。便利さが増すほど、委任、同意、監査、取り消し可能性という組織倫理がプロダクトの中心になる。

## arXiv / 学術
- 見つかりました: `2608.16801v1` “When Agents Coordinate: Measuring Coordination in Multi-Agent AI Coding” — multi-agent coding の協調を時間ネットワークとして測る研究。
- 見つかりました: `2608.16806v1` “When State Becomes an Attack Surface: State-Semantic Injection in LLM-Driven Embodied Agents” — embodied agent の状態解釈を攻撃面として扱う研究。
- 関連候補: `2608.16813v1` “Quipu: A Governed Bitemporal Knowledge Graph Store” — エージェントが知識グラフへ書き込む時代のガバナンス、時制、信頼ラベルを扱う。
- 関連候補: `2608.16798v1` “ClawGym II: Exploring Black-Box RL on Agent Harness” — agent harness を通じた長期タスク最適化とサンドボックス実行を扱う。
- 関連候補: `2608.16707v1` “Semantic Bandits: In-Context Exploration-Exploitation is Biased by Semantic Priors” — 意思決定エージェントの探索・活用が自然言語ラベルの意味バイアスを受けることを調べる。

## メモ
- Boris Cherny優先の有無: 優先確認を試みたが、X検索は xAI 側の `personal-team-blocked:spending-limit` で利用できず、@bcherny の直近投稿は本調査時点で実ツール確認できなかった。
- 日本語アカウントの扱い: 日本語X検索も同じ理由で失敗し、HN Algolia で日本語クエリを試したが該当結果は得られなかった。日本語圏実践の直接ソースは今回は未確認。
- Web検索の注意点: Hermes の `web_search` は Firecrawl 未設定で失敗したため、代替として terminal から arXiv API、HN Algolia API、GitHub API、GitHub README、公開Webページを直接取得して確認した。DuckDuckGo HTML は自動アクセス検知ページに遷移したため検索結果としては使っていない。
- 誇張リスク: HN/GitHub発のツールは初期リポジトリや小規模スターのものも含むため、普及度ではなく「今出てきている設計論点の面白さ」で選定した。リンクと日付は実取得できた公開ページ/APIに基づく。

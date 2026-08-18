# AI agent trends トレンド調査 (2026-08-18)

- 調査日: 2026-08-18
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AIエージェントの話題は「賢いモデル」から、ハーネス、MCP、記憶、監査、実行契約といった“働かせるための制度設計”へ重心が移っている。

## トップ5

### 1. HarnessRouter: Unified interface for agent harnesses
- 出典: Hacker News / GitHub
- 日付: 2026-08-17（HN投稿） / 2026-08-09（GitHub作成）
- リンク: https://github.com/HarnessRouter/harnessrouter
- 要約: Codex、Claude Code、Hermesなど複数のエージェント・ハーネスを、1つのローカルAPIから扱うためのセルフホスト基盤。セッション、ストリーミング、ファイル、キャンセル、失敗処理を含む Unified Harness Protocol を掲げ、HNでも「アプリがエージェントをどう呼ぶか」を標準化する議論として出てきた。
- なぜ面白いか:
  - 技術: モデルAPIではなく「ハーネスAPI」を抽象化し、Claude Code / Codex / Hermesのような実行環境差をルーティング層で吸収しようとしている。
  - 人文: エージェントが“人格的な相棒”から“業務システム内の交換可能な労働単位”へ移る兆候が見える。これは便利さだけでなく、誰が仕事の責任を持つのか、どの実行環境を信頼するのかという組織論の問題でもある。

### 2. Mandato: Protocol-Level Enforcement of Digitally Signed Mandates on AI Agent Actions with Cryptographically Chained Audit Trails
- 出典: arXiv
- 日付: 2026-08-14
- リンク: https://arxiv.org/abs/2608.14074
- 要約: MCPのようなツール呼び出しプロトコル上で、エージェントの行動を「署名済みの委任状」によって制約し、許可・拒否の判断をハッシュチェーン監査ログに残す提案。アプリケーション内の曖昧な認可ロジックではなく、プロトコル層のガバナンス・プロキシとして実装する点が中心。
- なぜ面白いか:
  - 技術: MCPツール実行に対して、パラメータ制約、条件、有効期限、本人性を含む機械可読な mandate を評価し、監査可能な形でインライン制御する。
  - 人文: “AIに何を任せたのか”を後から説明できる形式にする試みで、近代的な委任・代理・証拠の概念をエージェント運用へ移植している。自律性を増やすほど、自由ではなく委任範囲の明文化が重要になるという逆説がある。

### 3. MCPサーバは「SDKなし100行」で作れる — Claude Codeとの通信を盗聴して中身を全部見てみた
- 出典: Qiita
- 日付: 2026-08-17
- リンク: https://qiita.com/musa_rock/items/1490944033b507603beb
- 要約: Claude CodeとMCPサーバのstdio通信を、SDKなし・依存ゼロの最小実装と実測ログで解説する日本語記事。MCPを「JSON-RPC 2.0 + 決められたメソッド群」として捉え、Host / Client / Server、Tools / Resources / Prompts、stdio / Streamable HTTPの見取り図を実装目線で確認している。
- なぜ面白いか:
  - 技術: 抽象的に語られがちなMCPを、stdinから改行区切りJSONを読みstdoutへ返すプロセスとして分解し、Claude Code連携のブラックボックスを小さくしている。
  - 人文: 日本語圏の実践者が“使い方”ではなく“中で何が流れているか”を観察し始めている点が重要。エージェント文化が流行語から手触りのあるリテラシーへ進む過程として読める。

### 4. ATLAS: Discovering Agent Strategies through LLM-Guided Abstraction and Automata Learning
- 出典: arXiv
- 日付: 2026-08-14
- リンク: https://arxiv.org/abs/2608.14352
- 要約: LLMベースのエージェント軌跡から、有限状態モデルとして戦略を復元する ATLAS を提案。ソフトウェアテストやサイバーセキュリティ評価のような複雑タスクで、成功率だけでは見えない反復行動、分岐点、成功経路、失敗ループを分析する。
- なぜ面白いか:
  - 技術: 生のトレースをLLMで抽象化し、オートマトン学習によって解釈可能な行動モデルへ変換することで、エージェント評価を“結果”から“戦略”へ広げている。
  - 人文: 人間の熟練者を観察して作業手順を学ぶように、AIエージェントの癖や失敗の型を読む方法論になりうる。エージェントを信頼するには、成果だけでなく“どう考え、どこで迷うか”の物語が必要だと示している。

### 5. CommitLore: Git-native decision memory for coding agents
- 出典: GitHub
- 日付: 2026-07-26作成 / 2026-08-18更新
- リンク: https://github.com/MongLong0214/commitlore
- 要約: Claude Code、Codex、Cursorなどのコーディングエージェントに、過去の設計判断や却下済み選択肢をGit上の決定ログとして渡すためのMCP / hook系ツール。READMEは「エージェントがチームで既に却下した案を何度も持ち出す」問題を出発点にしており、日本語READMEも用意されている。
- なぜ面白いか:
  - 技術: ベクトルDBやホスト型メモリではなく、リポジトリに残るGit-nativeな意思決定記録を、編集前コンテキストとしてエージェントへ注入する。
  - 人文: これは単なるメモリ機能ではなく、チームの“なぜそうしないか”を機械に継承する試みである。ソフトウェア開発の文化的記憶を、会話ログではなく共同体の記録として扱う発想が面白い。

## arXiv / 学術

- Mandato: Protocol-Level Enforcement of Digitally Signed Mandates on AI Agent Actions with Cryptographically Chained Audit Trails — arXiv:2608.14074。MCP時代の認可・委任・監査をプロトコル層で扱う提案。
- ATLAS: Discovering Agent Strategies through LLM-Guided Abstraction and Automata Learning — arXiv:2608.14352。エージェント軌跡を有限状態モデルへ変換し、戦略や失敗ループを解釈する研究。
- Agentic Transaction: Towards ACID-Compliant Agent Systems — arXiv:2608.13900。長期タスクを実行するエージェントに、Atomicity / Consistency / Isolation / Durabilityの考え方を導入する提案。
- Agent Safety Should Be a Runtime Contract — arXiv:2608.11274。訓練時安全性だけでなく、サンドボックス、権限ゲート、証拠提出を含む実行時契約として安全性を扱う立場。

## メモ

- Boris Cherny優先の有無: 優先してX検索を試みたが、x_searchはクレジット不足（personal-team-blocked: spending-limit）で失敗したため、Boris Cherny / @bcherny の直近投稿は本調査では確認できなかった。
- 日本語アカウントの扱い: X検索は同じ理由で確認不可。代替としてQiita APIを使い、日本語圏のClaude Code / MCP実践記事を確認し、トップ5に1件採用した。
- Web検索の注意点: Hermesのweb_search / web_extractはFirecrawl未設定で利用不可だったため、代替としてHN Algolia API、GitHub API、Qiita API、arXiv API、公式ページへの直接HTTP取得を使用した。検索範囲に制約があるため、X上の反応量や一部公式リリースの網羅性は限定的。
- 誇張リスク: GitHubリポジトリのスター数・更新時刻は調査時点のAPI値であり、実運用品質を直接保証するものではない。特に新規OSSは、アイデアの先鋭性と成熟度を分けて読む必要がある。

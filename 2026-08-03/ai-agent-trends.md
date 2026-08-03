# AI agent trends トレンド調査 (2026-08-03)

- 調査日: 2026-08-03
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
AIエージェントの話題は「賢いモデル」から、レビュー、MCP、権限、ログ、モバイル復旧まで含む運用ハーネスの設計へ重心が移っています。

## トップ5

### 1. Copilot code review: Agent skills and MCP now generally available
- 出典: GitHub Changelog
- 日付: 2026-07-29
- リンク: https://github.blog/changelog/2026-07-29-copilot-code-review-agent-skills-and-mcp-now-generally-available
- 要約: GitHub Copilot code review で、リポジトリや組織に置いた `SKILL.md` による Agent Skills と、外部システムから文脈を引く MCP サーバー連携が一般提供になりました。MCP ツール呼び出しは読み取り専用に制限され、スキルや MCP 文脈を使ったコメントには出所表示も付くと説明されています。
- なぜ面白いか:
  - 技術: コードレビューAIが単なる差分コメント生成ではなく、社内標準・課題管理・ドキュメント・サービスカタログを読む「レビュー用エージェント基盤」になりつつあります。
  - 人文: レビューは本来、組織の規範や暗黙知を受け渡す場です。AIがそこに参加するなら、どの知識を参照したのかを表示することは、信頼と責任の最低限の作法になります。

### 2. GitHub MCP Server supports the next MCP specification
- 出典: GitHub Changelog
- 日付: 2026-07-23
- リンク: https://github.blog/changelog/2026-07-23-github-mcp-server-supports-the-next-mcp-specification
- 要約: GitHub MCP Server が、2026-07-28 に予定されるステートレス化を含む次期 MCP 仕様に先行対応しました。セッションと initialize の扱いが変わり、Redis セッション削除、HTTP ヘッダー経由のログ・シークレットスキャン、MCP Apps などの拡張を見据えた構成が説明されています。
- なぜ面白いか:
  - 技術: MCP がローカルの便利プロトコルから、スケールするリモート・ツール基盤へ進むためのインフラ変更です。
  - 人文: エージェントが多くの業務システムに触れるほど、「接続できる」だけでなく「誰が、どの権限で、どの痕跡を残して接続したか」が社会的に重要になります。ステートレス化は便利さだけでなく、統治しやすさの設計でもあります。

### 3. The harness is all you need (mostly)
- 出典: GitHub Blog
- 日付: 2026-07-27
- リンク: https://github.blog/ai-and-ml/github-copilot/the-harness-is-all-you-need-mostly/
- 要約: 新しい MCP、スキル、プロンプト小技を追うより、まず GitHub Copilot という「ハーネス」の基本動作を理解して使いこなすべきだ、という実践寄りの記事です。CLI、Copilot app、VS Code、Visual Studio、JetBrains などの体験が同じハーネスへ集約されている点も強調されています。
- なぜ面白いか:
  - 技術: エージェント活用のボトルネックを、モデルや個別ツールではなく、作業文脈・承認・検証・UIを束ねるハーネス設計として捉え直しています。
  - 人文: AI流行の「一発プロンプト」文化への反動として、職人が道具を習熟するような落ち着いた学習観が出ています。これは生産性だけでなく、作業者が主体性を失わないための文化的調整でもあります。

### 4. Claude Code × AWS MCP Serverによるマルチアカウント操作
- 出典: Qiita（日本語圏実践）
- 日付: 2026-08-02
- リンク: https://qiita.com/eureka_/items/cf4b7690dab316cceb1d
- 要約: AWS MCP Server のクロスアカウント対応を使い、Claude Code から複数 AWS アカウントを横断操作するためのセットアップと検証をまとめた日本語記事です。記事内では、AWS MCP Server が AI コーディングエージェントから AWS ドキュメント検索や AWS API 実行を自然言語で行えるマネージド MCP サーバーであること、複数 AWS CLI プロファイルを同一セッションで切り替えられることが紹介されています。
- なぜ面白いか:
  - 技術: エージェントがクラウド運用の実アカウント境界をまたぐ段階に入り、MCP 設定、CLI プロファイル、IAM 権限設計がそのまま安全性を左右するようになっています。
  - 人文: 「AIにクラウドを操作させる」ことは、便利さと不安が最も近い領域です。日本語圏の実践記事が具体的な手順と注意を共有することで、個人の試行錯誤がコミュニティの安全知へ変換されます。

### 5. Can Large Language Models Resolve Real Java Merge Conflicts? An Evaluation with a Calibrated LLM-as-Judge
- 出典: arXiv
- 日付: 2026-07-30
- リンク: https://arxiv.org/abs/2607.27674v1
- 要約: 実際の Java マージコンフリクトを対象に、LLM ソルバーを generate-validate-retry 型のエージェントとして構成し、Java パーサーや重複宣言チェックなどの推論時シグナルで検証する研究です。人間ラベルで較正した LLM-as-judge と構造的妥当性チェックを組み合わせ、従来ツールが棄権しがちな領域で LLM が高いカバレッジを示すと報告しています。
- なぜ面白いか:
  - 技術: コーディングエージェント評価が「答えが合ったか」だけでなく、検証ループ、棄権率、較正済みジャッジ、保守的な受理基準を含む運用指標へ進んでいます。
  - 人文: マージコンフリクトは共同作業の摩擦そのものです。AIがそこに介入するなら、正解生成だけでなく、どこまで人間の意図を代行してよいか、どの解決を「開発者らしい」と見なすかが問われます。

## arXiv / 学術
- 見つかったもの: `2607.27674v1` — “Can Large Language Models Resolve Real Java Merge Conflicts? An Evaluation with a Calibrated LLM-as-Judge”。LLM エージェントの generate-validate-retry と較正済み評価が、コーディングエージェント運用の実務評価に近い点で有用です。
- 追加で確認された関連候補: `2607.28617v1` — “AISPA: User-Centric System Prompt Auditing for Large Language Model Applications”。商用 AI アプリのシステムプロンプト監査という観点から、エージェントの統治・説明責任に接続する論点です。

## メモ
- Boris Cherny優先の有無: @bcherny 指定で X 検索を実行しましたが、xAI 側の spending-limit / Grok subscription エラーにより取得できませんでした。そのため本ファイルでは Boris Cherny の未確認情報を採用していません。
- 日本語アカウントの扱い: X 検索は同じ理由で取得不能でしたが、Qiita API で日本語圏の Claude Code / MCP / エージェント運用記事を確認し、AWS MCP Server のマルチアカウント実践をトップ5に採用しました。
- 注意点・誇張リスク: Web検索ツール（Firecrawl）は未設定で失敗したため、代替として公式 WordPress API、Qiita API、Anthropic/GitHub の公開ページ、arXiv API、直接 HTTP 取得を利用しました。X由来の反応量や拡散度は本調査では検証できていません。

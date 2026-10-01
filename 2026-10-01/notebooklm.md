# NotebookLM トレンド調査 (2026-10-01)

- 調査日: 2026-10-01
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
NotebookLM は「旧称 NotebookLM の単独ツール」から、Gemini Notebook として学校・企業・Docs・書籍という既存の知識生活の中に埋め込まれる段階へ移っています。

## トップ5

### 1. Google Docs で Gemini Notebook の既存ソースを根拠にできるように
- 出典: Google Workspace Updates 公式ブログ
- 日付: 2026-09-23
- リンク: http://workspaceupdates.googleblog.com/2026/09/ground-ai-prompts-in-google-docs-on-existing-sources-from-Gemini-Notebook.html
- 要約: Google Docs 内の Gemini から、既存の Gemini Notebook をコンテキストソースとして参照できるようになりました。研究メモ、提案書、技術ホワイトペーパーなどを、別タブへのコピーなしに、Notebook 側の資料に基づき引用付きで下書きできます。
- なぜ面白いか:
  - 技術: RAG 的な「信頼するソースに基づく生成」が、専用ノート画面から日常の文書作成 UI へ直接接続された点が重要です。
  - 人文: 書くことは単なる生成ではなく、どの資料を根拠にするかを選ぶ編集行為になります。組織内の知識が文書の背後に透けて見えるため、説明責任や引用文化の再設計にもつながります。

### 2. Study notebooks が学校・職場アカウントにも展開
- 出典: Google Workspace Updates 公式ブログ
- 日付: 2026-09-22
- リンク: http://workspaceupdates.googleblog.com/2026/09/study-notebooks-in-gemini-are-now-available-for-Google-Workspace-accounts.html
- 要約: Gemini の Study notebooks が、管理者により Gemini app と Gemini Notebook が有効化された学校・職場発行の Google アカウントでも利用可能になりました。学習目標と教材をもとに、知識ギャップ診断、短い個別レッスン、クイズ、進捗ダッシュボードを提供します。
- なぜ面白いか:
  - 技術: 教材ソースに根拠づけた適応学習ワークフローが、個人向け実験から Workspace 管理下のアカウントへ拡張されています。
  - 人文: 「学習者の弱点を可視化する」機能は便利な一方、学校や職場での評価・監視との境界が問われます。個別化は支援にも統制にもなり得るため、管理者設定と透明性が重要です。

### 3. 音声録音・リアルタイム会話・対話型学習オーバービューが追加
- 出典: Google Workspace Updates 公式ブログ
- 日付: 2026-09-18
- リンク: http://workspaceupdates.googleblog.com/2026/09/new-back-to-school-features-and-learning-tools-available-in-Gemini-Notebook.html
- 要約: Gemini Notebook モバイルアプリに音声録音が入り、講義や思いつきをソースと並べて保存できるようになりました。18歳以上は、約100言語で Notebook とリアルタイム会話でき、Reports には要約、クイズ、フラッシュカード、マインドマップなどを組み合わせた対話型学習オーバービューも加わっています。
- なぜ面白いか:
  - 技術: 入力は音声、対話はリアルタイム、出力はクイズや概念図という形で、Notebook がマルチモーダルな学習スタジオに近づいています。
  - 人文: 講義を「あとで読む資料」ではなく「話しかけられる記憶」に変える点が印象的です。学びの相手が人間教師・同級生・AI ノートの混成になることで、孤独な自習の体験も変わります。

### 4. Notebooks in Gemini が学校・組織向けの集中ワークスペースに
- 出典: Google Workspace Updates 公式ブログ
- 日付: 2026-09-17
- リンク: http://workspaceupdates.googleblog.com/2026/09/notebooks-in-gemini-dedicated-workspace-for-focused-organized-work-now-for-schools-and-organizations.html
- 要約: Gemini 内の Notebooks が、学生、教育者、専門職向けに、特定トピックの会話と資料をまとめる専用ワークスペースとして展開されました。学生は講義ノートから学習ガイドを作り、教育者はカリキュラムやルーブリックから教材やフィードバックを生成し、専門職は製品情報や調査資料から成果物を作れます。
- なぜ面白いか:
  - 技術: Gemini app と Gemini Notebook の統合により、同じソースを使って動画概要、学習ガイド、ドラフト生成など複数の出力へ展開できます。
  - 人文: 「ノート」は個人の思考の場所でしたが、ここでは学校や会社の制度に接続された作業空間になります。便利さの反面、学び方・働き方の標準化が進む可能性もあります。

### 5. Expert Intelligence で購入済み電子書籍を Notebook の根拠に
- 出典: Google Workspace Updates 公式ブログ
- 日付: 2026-09-17
- リンク: http://workspaceupdates.googleblog.com/2026/09/introducing-expert-intelligence-in-Gemini-Notebook.html
- 要約: Google は Expert Intelligence を発表し、主要出版社の10万冊以上の書籍など信頼できるソースを Gemini Notebook で活用できる取り組みを始めました。Google Play Books で購入した対応電子書籍を Notebook に追加し、本文に根拠づけた質問応答、インフォグラフィック、Audio Overview、クイズ生成などが可能になります。
- なぜ面白いか:
  - 技術: 公開 Web やユーザー資料だけでなく、ライセンスされた書籍コンテンツを Notebook の知識ベースとして扱う点が、教育・専門知識 RAG の実用化に近いです。
  - 人文: 本を読む行為が、著者との対話・要約・演習生成へ拡張されます。一方で、読書の遅さや解釈の余白が効率化に吸収されすぎないかという文化的な問いも残ります。

## arXiv / 学術
- 本調査時点で確認されませんでした。arXiv API は 429 / timeout が発生したため、Bing RSS による `site:arxiv.org NotebookLM` / `site:arxiv.org "Gemini Notebook"` の代替確認も行いましたが、NotebookLM / Gemini Notebook に直接対応する arXiv 論文は確認できませんでした。

## メモ
- Boris Cherny優先の有無: NotebookLM は Claude 系トピックではないため優先対象外。
- 日本語アカウントの扱い: X 検索は英語・日本語とも実行したが、x_search が `spending-limit` で失敗したため、X 由来の個別投稿は採用していません。代替として Bing RSS と公式ページを確認し、日本語実践情報として Google Workspace 日本語版の Gemini Notebook ページ、JAPAN AI ラボ、マネーフォワード クラウド、mouse LABO などの解説ページを確認しました。日本語圏では「アップロード資料に限定した要約・質問応答」「議事録・社内資料・学習用途」「プライバシーとモデル学習に使われない点」が実践導入の主要関心として見えます。
- 注意点・誇張リスク: Web 検索ツールは Firecrawl 未設定で利用不能だったため、公式 RSS、Bing RSS、直接 HTTP 取得で補完しました。トップ5はすべて公式 Google Workspace Updates のリンクに限定し、未確認の X 投稿や架空 arXiv ID は含めていません。

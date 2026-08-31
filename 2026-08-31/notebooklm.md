# NotebookLM トレンド調査 (2026-08-31)

- 調査日: 2026-08-31
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
NotebookLM は「資料を要約する道具」から、購入済み書籍・共有ノート・利用枠設計まで含む“個人知の作業環境”へ寄っている。

## トップ5

### 1. Expert Intelligence: Google Play Books の購入済み電子書籍を Gemini Notebook に取り込む動き
- 出典: Google 公式ブログ（Google News RSS 経由で確認）
- 日付: 2026-08-27
- リンク: https://news.google.com/rss/articles/CBMioAFBVV95cUxQOEFlUE5LS1puS3dIdWdyd0pEWEwtVWtNNmhQeV9fMFhCUTdzeThXM0pfWjNjVk4wM3I0RUJmeWRqRFp2eWtienNCMUlIN3BYMmVURFRGbVJFTFRpZ3NFZElFaUcwa3BOdDRRMHFOeVhGQnNWdnpPajBJVXcxMW5teHM2Qmh2NGtITXFzeVpFOTUtZG5pQ0RhOGc3dm1NanF3?oc=5
- 要約: Google が「Expert Intelligence」として、Google Play Books で購入した書籍を Gemini Notebook のソースとして扱える機能を発表した。日本語ニュースでも、購入済み電子書籍を Gemini に読ませて質問できる新機能として報じられている。
- なぜ面白いか:
  - 技術: RAG の対象がユーザーアップロード文書から商用電子書籍ライブラリへ広がり、権利管理された長文コンテンツを会話的に扱う設計が前面に出てきた。
  - 人文: 本を「読む」行為が、索引・引用・対話を伴う共同作業に変わる可能性がある。読書体験の主体性、出版社・著者の権利、学習者の理解形成が同じ場所で交差する点が大きい。

### 2. Gemini Notebook の flexible usage limits 導入
- 出典: Google 公式ブログ（Google News RSS 経由で確認）
- 日付: 2026-08-28
- リンク: https://news.google.com/rss/articles/CBMikwFBVV95cUxNTm5ueEtJQm02RmNiVnYtNUJiY0dGMnlBQVZZeWEwQ1ljbkdTYmRuTDZ6XzR2NlhFQ05ZZ244aDZoNFhwTWxhcFgwZk82RVk1bkdQek9lTm40Wl92d1Fhbkxzd0xuLVN2aFQ4MGFqRG1ZZ2M3cjhPRGYxTnFxT0VNVFgzWUhoT0Q2QXM4cFM2bFJxM3c?oc=5
- 要約: Google は Gemini Notebook の利用上限を、単純な日次制限からより柔軟な利用枠へ移行すると発表した。関連報道では、9月初旬から上限リセットやチャット・生成機能の扱いが変わる点が注目されている。
- なぜ面白いか:
  - 技術: ノート数・ソース数・チャット・音声/動画解説・Deep Research といった複数リソースを、製品プラン別に管理する段階へ入ったことを示す。
  - 人文: AIノートが日常の学習・業務インフラになるほど、「どこまで無料で考え続けられるか」が利用者の思考習慣に影響する。料金と上限は単なる課金表ではなく、知的作業のリズムを設計する制度になる。

### 3. 日本語実践ガイド: Gemini Notebook（旧NotebookLM）の機能・料金・活用例の更新
- 出典: SHIFT AI TIMES
- 日付: 2026-08-29
- リンク: https://shift-ai.co.jp/blog/24690/
- 要約: 日本語で、Gemini Notebook の基本、ソース追加、要約、質疑応答、Deep Research、音声/動画解説、マインドマップ、フラッシュカード、クイズ、スライド資料化などを整理している。個人向け Plus / Pro / Ultra や組織向けプランの上限も表形式でまとめており、日本の業務利用者にとって実践的な入口になっている。
- なぜ面白いか:
  - 技術: 単一の要約ツールではなく、資料入力から学習コンテンツ生成・報告書作成までのマルチモーダルなワークフローとして説明されている。
  - 人文: 日本語圏では「便利なAI」よりも「議事録・資格勉強・企画書作成をどう任せるか」という生活密着の語りで普及している。AI導入の文化的単位が、研究室ではなく会議・勉強会・社内資料へ移っている点が見える。

### 4. “生ソースを丸ごと入れない”という NotebookLM ワークフロー論
- 出典: XDA Developers
- 日付: 2026-08-24
- リンク: https://news.google.com/rss/articles/CBMimgFBVV95cUxPWkVHcndyVmRNSlpZWDM4d0hidVBUSlF3VEV2UEEtWGxzY1JBU1hWQnVJR1VwdkJhcTRHWVF0NjZNMThKR3F4U05oYjV5VnRCR3J1eDRzTEJlRmo4QUhvTmxaeEZWUlZORHo4XzdVWmZzNjhJdjUwVmtmdkFSM1llR1U3c3U0QlZNQzlSQzFMMFNFM2IzdVl0aURn?oc=5
- 要約: 「I stopped dumping raw sources into NotebookLM, and it got so much better」という実践記事が、資料をそのまま大量投入するより、要点化・整理済みソースを与えるほうが出力品質が上がるという使い方を示している。NotebookLM の強さはソース接地だが、ソース設計そのものが成果物の品質を左右する。
- なぜ面白いか:
  - 技術: RAG ツールの性能はモデルだけでなく、チャンク以前の人間による情報設計・ノイズ除去・文脈付与に強く依存することを示す実践例である。
  - 人文: 「AIに全部読ませる」から「AIが読めるように資料を整える」へ、利用者の役割が編集者に近づく。これは知識労働における新しいリテラシー、つまり問いと資料をキュレーションする技能の台頭を示している。

### 5. プライバシー懸念から Obsidian + ローカルLLM へ移る反動
- 出典: How-To Geek
- 日付: 2026-08-18
- リンク: https://news.google.com/rss/articles/CBMiwgFBVV95cUxOdDJnaHJYZjRXZlBwaXUzRnQ1eEdoMFE0bmc0X1dEM002bGJwemozdmF4d0p0ai1HSThOaXRRaHR3U0lzNmdNd1hKeHhjcnJMNmVFdjNXLThNTDItUFppc0NMU3JZbk1VMnk5Ym9vaWhscElOQ0I0c3lES0NzMFJqM2dzemdxbnZuZWxDVkV5bjlGRGI3VmlyQzNZTE9hdFlld0NsOTNqbklHR0tXNGhhUUpXUUxmX0t2cWlSZVJtZjAxUQ?oc=5
- 要約: NotebookLM から Obsidian とローカルLLMへ移行した体験記事が、便利さとプライバシーのトレードオフを扱っている。クラウド型AIノートが強力になるほど、個人メモ・研究ノート・業務資料をどこに置くかという選択が重要になる。
- なぜ面白いか:
  - 技術: クラウドRAGとローカルLLM/ローカルノートの比較は、検索精度だけでなくデータ所在、同期、拡張性、再現性の問題を含む。
  - 人文: ノートは単なるデータではなく、未完成の考えや迷いを含む親密な空間である。AIに読ませる便利さと、読ませない自由をどう両立するかは、知的生活の倫理そのものになっている。

## arXiv / 学術
- 本調査時点で確認されませんでした。arXiv API は 429 / タイムアウトが発生したため、Bing RSS による `site:arxiv.org NotebookLM` 検索でも補完確認したが、NotebookLM に直接対応する信頼できる新規 arXiv ID は見つかりませんでした。

## メモ
- Boris Cherny優先の有無: NotebookLM は Boris Cherny 優先対象ではないため、優先なし。
- 日本語アカウントの扱い: X検索は英語・日本語とも実行したが、xAI/X検索ツールが `personal-team-blocked:spending-limit` で失敗。代替として Google News RSS、Bing RSS、公式/日本語実践記事の直接HTTP取得を使い、日本語実践例（SHIFT AI、マネーフォワード、国内ニュース）を優先的に確認した。
- 注意点・誇張リスク: Web検索/抽出ツールは Firecrawl 未設定で利用不可だったため、通常のWeb検索結果ではなくRSSと直接HTTP取得に依存した。Google公式ブログの2件は Google News RSS の実在エントリで確認したが、直接URL取得は一部404となったため、リンクはRSS記事URLを採用した。

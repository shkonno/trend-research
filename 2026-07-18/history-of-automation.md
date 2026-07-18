# History of Automation トレンド調査 (2026-07-18)

- 調査日: 2026-07-18
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

AIエージェント論は「新しい自動化」ではあるが、今週の重要論点はむしろ、工業化・事故史・保険・知識コモンズといった古い制度史の問題が研究、組織、労働に戻ってきている点にある。

## トップ5

### 1. The Industrialization of Research ; On AI-Driven Science and Its Consequences
- 出典: arXiv（cs.AI / cs.CY）
- 日付: 2026-07-16
- リンク: http://arxiv.org/abs/2607.15164v1
- 要約: AIを単なる研究補助ツールではなく、研究サイクル内の自律的参加者として捉え、研究が「職人的モデル」から「分解・自動化・監督されるパイプライン」へ移ることを「研究の工業化」と呼ぶ論考。技能継承、AI生成理論の不透明性、査読の洪水、研究アジェンダの政治・産業的捕捉、閉ループでの誤り増幅などを論じる。
- なぜ面白いか:
  - 技術: AIエージェントによる科学自動化を、単発の効率化ではなく、知識生産工程そのものの再設計として扱っている。
  - 人文: 産業革命期の熟練労働の分解と同じく、研究者の判断・徒弟制・共同体規範がどこまで機械化可能かという労働史的問いを正面から開く。AI研究基盤が国家・企業に集中することで、誰が「発見する権利」を持つのかという制度史の問題にも接続する。

### 2. Unsafe at any AUC: Unlearned Lessons from Sociotechnical Disasters for Responsible AI
- 出典: arXiv（cs.CY / cs.AI / eess.SY）
- 日付: 2026-07-15
- リンク: http://arxiv.org/abs/2607.14353v1
- 要約: 自動意思決定システムのリスクを、モデル性能指標だけでなく社会技術システム全体として評価すべきだと論じる。チェルノブイリ、スリーマイル島、福島第一、ボパール、チャレンジャー事故などの災害史から、既知の危険が組織・政治・経済的要因で無視される構造をAIガバナンスに引き寄せる。
- なぜ面白いか:
  - 技術: AUCなどの局所的性能評価から、運用組織、インセンティブ、事故連鎖を含むシステム安全評価へ視点を移している。
  - 人文: 自動化の歴史では「機械が失敗した」のではなく、失敗を許す組織文化が反復してきたことが重要だった。本稿はAIエージェントの倫理を、抽象的なアラインメント論ではなく、災害史と責任分配の問題として読み直せる。

### 3. CAVA: Canonical Action Verification and Attestation for Runtime Governance of Agentic AI Systems
- 出典: arXiv（cs.AI）
- 日付: 2026-07-15
- リンク: http://arxiv.org/abs/2607.13716v1
- 要約: エージェントがローカルフック、SDKツール、ブラウザ自動化、APIゲートウェイ、ワークフローエンジンなど異なる実行環境で行動する時、「実際に何が承認され、何が実行されたのか」を標準的な行為オブジェクトとして検証・証明する枠組みを提案する。
- なぜ面白いか:
  - 技術: 異種ランタイム上のエージェント行為を正規化し、承認と実行を結びつける監査可能な意味層を設計している。
  - 人文: これは工場のタイムカードや工程記録、官僚制の稟議書に近い「行為の記録制度」をAI時代に作る試みと読める。自動化が高度になるほど、人間社会は逆説的に、誰が・何を・いつ許可したかという儀礼的な証跡を必要とする。

### 4. AI-Native Insurance for Agentic AI: Pricing, Underwriting, and End-to-End Automation
- 出典: arXiv（cs.AI / cs.CR / cs.CY）
- 日付: 2026-07-14
- リンク: http://arxiv.org/abs/2607.13230v1
- 要約: 自律的に意思決定し、ツールを呼び出し、外部環境を変更し、第三者サービスと相互作用するAIエージェント向けに、保険料、免責、補償配分、契約条項、ガバナンス認証閾値を数理的に扱う保険フレームワークを提示する。保険を単なる運用コストではなく、AI展開の規制メカニズムとして位置づける。
- なぜ面白いか:
  - 技術: 自律性、権限、権限露出、ガバナンス成熟度、依存集中度をリスク状態としてモデル化し、エージェント運用を保険可能性の問題に変換している。
  - 人文: 自動車、工場、電力網の普及と同様に、自動化は事故後の補償制度が整って初めて社会に埋め込まれる。AIエージェントの普及も「便利なツール」ではなく、責任を価格付けする金融・法制度の歴史に入ったことを示している。

### 5. The tragedy of the cognitive commons: collective intelligence beyond AI-induced knowledge collapse
- 出典: arXiv（cs.CY）
- 日付: 2026-07-14
- リンク: http://arxiv.org/abs/2607.13272v1
- 要約: Acemoglu、Kong、Ozdaglarによる「エージェントAIが人間の知識共有努力を代替し、公共的知識ストックを劣化させる」という知識崩壊モデルを検討し、Stack Overflowでの公共的知識共有減少などの実証的兆候にも触れながら、その前提と限界を批判的に評価する。
- なぜ面白いか:
  - 技術: AIエージェントが私的な回答生成を代替しても、公共の知識ベースを再生産できるとは限らないという外部性をモデル化している。
  - 人文: 自動化の歴史では、機械が作業を代替するだけでなく、技能共同体や相互扶助の場を弱めることがあった。AIエージェント時代の「便利さ」は、職人ギルド、職場学習、オンライン共同体のような知識コモンズをどう維持するかという文化史的課題を伴う。

## arXiv / 学術

- The Industrialization of Research ; On AI-Driven Science and Its Consequences — arXiv:2607.15164v1。研究自動化を「工業化」として捉える本日の中心文献。
- Unsafe at any AUC: Unlearned Lessons from Sociotechnical Disasters for Responsible AI — arXiv:2607.14353v1。AI安全を災害史・社会技術システム論と接続。
- CAVA: Canonical Action Verification and Attestation for Runtime Governance of Agentic AI Systems — arXiv:2607.13716v1。エージェント行為の監査・証跡化。
- AI-Native Insurance for Agentic AI: Pricing, Underwriting, and End-to-End Automation — arXiv:2607.13230v1。エージェント自動化を保険・規制制度へ接続。
- The tragedy of the cognitive commons: collective intelligence beyond AI-induced knowledge collapse — arXiv:2607.13272v1。AIによる知識共有の外部性を扱う。

## メモ

- X検索: 英語・日本語で検索を実行したが、xAI側の `personal-team-blocked:spending-limit` により取得できなかった。そのため本ファイルではX投稿をトップ5に採用していない。
- Web検索: HermesのWeb検索はFirecrawl未設定エラーで利用不能だった。代替としてターミナルからDuckDuckGo/Bing/GDELT/Hacker News/GitHub API等の直接検索を試したが、検索結果欠落や429が多く、信頼して採用できる直近Web記事は確認できなかった。
- 日本語アカウントの扱い: 日本語X検索も実行したが、同じクレジット制限で取得不可。
- 注意点・誇張リスク: 今回のトップ5はarXiv中心であり、X上の実務者議論や日本語圏の受容は十分に反映できていない。内容面では「自動化の歴史」そのものの新刊・記事というより、AIエージェントによる現代的自動化を、労働史・制度史・災害史・知識コモンズの観点で接続できる文献を優先した。

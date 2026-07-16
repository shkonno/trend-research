# Harness engineering トレンド調査 (2026-07-15)

- 調査日: 2026-07-15
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言

「モデル単体」ではなく、ツール・承認・状態・検証・ループを束ねるハーネス設計そのものが、エージェント性能と文化を左右する主戦場になっています。

## トップ5

### 1. EnterpriseClawBench: ハーネス×モデルで評価しないと現実を見誤る
- 出典: arXiv論文 / 日本語X投稿
- 日付: 2026-06-22（論文公開、直近Xで再注目）
- リンク: https://arxiv.org/abs/2606.23654 / https://x.com/itarutomy/status/2077167287682183561
- 要約: 実企業セッションから作った852タスクのベンチマークで、最高スコアでも0.663にとどまり、同じモデルでもClaude Code、Codex、Hermesなどハーネスの違いで成績が大きく変わることを示しています。特に「モデル名だけでなく、成果物配送・視覚品質・コスト・実行時間・スキル転移まで見るべき」という主張が、7月中旬の日本語圏でも強く共有されています。
- なぜ面白いか:
  - 技術: LLM評価の単位を「モデル」から「ハーネス×モデル×環境」へ移し、エージェント運用の実力差をより正確に測ろうとしている点が重要です。
  - 人文: これは能力を個人の頭脳だけに帰さず、制度・道具・職場環境まで含めて見る社会学的な転換に近いです。AIの失敗も「モデルが悪い」だけでなく、承認フローや作業文化の設計問題として読めるようになります。

### 2. Boris ChernyのClaude Code `/checkup`: ハーネスを自己点検するコマンド
- 出典: Boris Cherny X投稿
- 日付: 2026-07-08
- リンク: https://x.com/bcherny/status/2074997570317779038
- 要約: Boris ChernyはClaude Codeの新しい`/checkup`コマンドを紹介し、未使用のskills/MCP/plugins整理、CLAUDE.mdの重複解消、ルートCLAUDE.mdの分割、遅いhooksの無効化、最新版更新、auto modeやread-onlyコマンド事前承認などを確認付きで行うと説明しました。
- なぜ面白いか:
  - 技術: ハーネスの性能劣化要因である設定肥大化・重複ルール・遅いhooksを、運用コマンドとして点検・修復する方向に進んでいます。
  - 人文: エージェントが「道具」から「作業場」になると、片付け・棚卸し・規律の維持が創造性の条件になります。これは職人が工房を整える行為に近く、AI開発にも生活習慣のようなメンテナンス倫理が入り始めています。

### 3. Loop engineering: `/goal`、`/loop`、`/schedule`がハーネスの外側を設計対象にする
- 出典: X上のAnthropic/Claude Code関連共有
- 日付: 2026-07-12〜2026-07-14頃
- リンク: https://x.com/cc_lab_jp/status/2077153814314971411 / https://x.com/Vettan0/status/2077167758668939639 / https://x.com/i/status/2076267187652706324
- 要約: 直近の議論では、`/goal`は測定可能なゴールまで継続、`/loop`はローカルで定期実行、`/schedule`はクラウド常駐で継続、という整理が共有されています。ハーネスが単発のツール束ではなく、発見・実行・検証・永続化・スケジューリングを回す外側のループへ拡張されている点が注目されています。
- なぜ面白いか:
  - 技術: 停止条件、検証者、永続化、隔離worktree、スケジューラを明示することで、長時間自律エージェントの制御可能性を上げる設計論になっています。
  - 人文: 「いつ終わったと言えるのか」を機械に委ねる問題は、仕事の完成・責任・監督の哲学に直結します。人間が逐次命令する時代から、条件とリズムを設計する時代への移行が見えます。

### 4. waku-agent: ローカルファーストなHarness・Loop・Memory・Evalの実装例
- 出典: X投稿 / GitHub README
- 日付: 2026-07-14
- リンク: https://x.com/ShenSeanChen/status/2077145810828218600 / https://github.com/ShenSeanChen/waku-agent
- 要約: Shen Sean Chenが、ローカルで動く個人AIアシスタント`waku-agent`を公開しました。READMEでは「Harness · Loop · Memory · Eval/LLM-Ops」を4本柱にし、約95行のPythonループ、SQLiteの透明な記憶、トレース、決定的テストとLLM-as-judgeのrelease gate、TelegramやApple Calendar連携などを掲げています。
- なぜ面白いか:
  - 技術: フレームワークで隠しがちなハーネス、記憶、評価、ループを読めるコードとして提示し、個人が検査・改造できるエージェント基盤にしています。
  - 人文: 「記憶は自分のSQLiteファイルであり、読める」という設計は、個人AIの所有権とプライバシーの感覚を強く押し出しています。クラウドに人格を預けるのではなく、自宅のノートとしてAIを持つ文化が感じられます。

### 5. 日本語圏のCLAUDE.md / rules運用: ハーネスルールは暴走防止の作法になる
- 出典: 日本語X投稿 / 関連Web記事・ツール紹介
- 日付: 2026-07-02〜2026-07-14頃
- リンク: https://x.com/claudecode84/status/2073584012355125270 / https://x.com/fumikun_gengen/status/2075052571438596317 / https://x.com/takoratta/status/2072866925135491243
- 要約: 日本語コミュニティでは、CLAUDE.mdを「Claudeを賢くする魔法」ではなく、勝手な前提、不要なコード追加、範囲外変更、無限ループを防ぐハーネスルールとして扱う投稿が目立ちます。一方で`.claude/rules/`の肥大化を避けるため、常時ロードするルーター表とオンデマンド詳細ルールに分ける実践や、コンテキスト読み込みを可視化するシミュレーターも共有されています。
- なぜ面白いか:
  - 技術: ルールを全量常時投入するのではなく、軽いルーターと必要時読み込みに分けることで、コンテキスト汚染と運用負荷を抑えようとしています。
  - 人文: これは日本語圏の開発者が、AIとの協働を「命令」よりも「作法」や「しつけ」として整えている例です。小さな規律が共同作業の安心感を作るという、組織文化に近い知恵が表れています。

## arXiv / 学術

- EnterpriseClawBench: Benchmarking Agents from Real Workplace Sessions — arXiv:2606.23654（2026-06-22）。企業エージェント評価ではハーネス×モデル、成果物、コスト、ランタイム、スキル転移まで報告すべきと主張。
- Harness-Aware Self-Evolving: Co-Evolving Model Weights, Harness, and Task Solutions — arXiv:2607.03935（2026-07-04）。タスク解だけでなくハーネス部品も同じエージェント過程で改善するHASEを提案。
- Harnessing Code Agents for Automatic Software Verification — arXiv:2607.06341（2026-07-07）。Claude Codeのような汎用コードエージェントを検証ハーネスで包み、Coq証明生成を進める研究。
- ToFu: A White-Box, Token-Efficient Agent Harness for Researchers — arXiv:2607.11423（2026-07-13）。研究者向けに、読めて改造できる白箱のエージェントハーネスを提示。
- Agent Hacks Agent: Autoresearch for Production-Agent Red-Teaming — arXiv:2607.11698（2026-07-13）。Claude CodeやCodexを含む本番エージェントを、サンドボックスハーネス内で自動レッドチーミングする研究。

## メモ

- Boris Cherny優先: 直近14日で`harness`や`loop`という語を直接含むBoris投稿は確認できませんでしたが、Claude Codeの`/checkup`はハーネス運用そのものに関わるためトップ5に採用しました。
- 日本語アカウントの扱い: EnterpriseClawBench、Loop engineering、CLAUDE.md/rules運用について日本語投稿を優先確認し、少なくとも2件をトップ5の主要根拠に入れました。
- Web検索について: Hermesの`web_search`ツールは設定未完了エラーで使用不能でした。そのため、Web確認は端末からの直接取得でarXiv APIとGitHub READMEを確認し、X検索と合わせて裏取りしました。
- 注意点・誇張リスク: X検索結果には要約生成が含まれるため、数値や一次情報が必要な箇所はarXiv API、GitHub README、投稿URLに限定して記述しました。Anthropic公式PDF/講座そのものは本調査環境では直接確認できていないため、関連項目は「X上の共有」として扱っています。

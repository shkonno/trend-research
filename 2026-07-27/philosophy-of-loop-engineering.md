# Philosophy of Loop Engineering トレンド調査 (2026-07-27)

- 調査日: 2026-07-27
- 情報源: X / Web / arXiv
- 対象期間: 直近約14日（重要だが古いものは明記）

## 今日の一言
Loop Engineering は「よいプロンプトを書く」段階から、「観察・評価・修正が循環する実践知の制度をどう設計するか」という認識論とサイバネティクスの問題へ移っている。

## トップ5

### 1. Harness Training: Training Agent Harnesses Like Model Weights
- 出典: Henry Pan ブログ / GitHub リポジトリ
- 日付: 2026-07-18
- リンク: https://www.henrypan.com/blog/2026-07-18-harness-training/
- 要約: LLM本体を固定し、プロンプト、コンテキスト管理、ツール、修復ループからなる「ハーネス」をPyTorch風に訓練する試み。各エポックで候補diffを作り、タスクパネルで現行ベースラインと比較し、勝った変更だけをgit履歴として昇格させる。
- なぜ面白いか:
  - 技術: モデル重みではなく周辺の実行環境を、評価結果を勾配のように扱う閉ループで改善するため、Loop Engineering を実装可能な最適化対象として定義している。
  - 人文: これは「知能は頭脳の中だけにあるのか、それとも道具・記録・環境との循環に分散しているのか」という拡張された心の問いに近い。職人の実践知が、失敗の記録と作業場の配置によって身体化される過程を、ソフトウェア工学に移植している。

### 2. WorldBuild Bench: Same brief, same tools, same harness
- 出典: WorldBuild Bench / GitHub README / Hacker Newsで2026-07-21に確認
- 日付: 2026-07-13（ラウンド日、直近14日よりやや古いが関連性が高い）
- リンク: https://sandscape.app/worldbuild/rounds/ai-game-benchmark-2026-07-13
- 要約: 9つの主要AIモデルに同じゲーム設計ブリーフ、同じツール、同じThree.js/Rapier足場、同じPlaywrightプレイテストループを与え、27本の3Dブラウザゲームを比較するベンチマーク。コンパイルやfpsだけでなく、人間が実際に遊び続けたいかをArenaで比較する。
- なぜ面白いか:
  - 技術: ハーネスを固定してモデル差だけを観測し、実行ログ、スクリーンショット、人間の選好評価を組み合わせることで、静的ベンチマークでは見えない空間的一貫性・因果的一貫性をループ内で検証している。
  - 人文: 「世界を作れる」とは単にコードが動くことではなく、空間・時間・原因・手触りが意味あるまとまりを持つことだという現象学的な問いを含む。Loop Engineering はここで、機械の出力を人間の経験へ接続する批評装置になっている。

### 3. Skill Self-Play: Pushing the Frontier of LLM Capability with Co-Evolving Skills
- 出典: arXiv
- 日付: 2026-07-24
- リンク: https://arxiv.org/abs/2607.22529
- 要約: Proposer、Solver、Dynamic Skill Controller が強化学習ループの中で共進化し、検証可能なスキル単位を使いながらタスク多様性と検証信頼性のトレードオフを緩和する研究。環境に閉じた評価は正確だが狭く、開放的な自己生成は広いが報酬汚染が起きやすい、というジレンマを中心課題に置く。
- なぜ面白いか:
  - 技術: スキルを「深い実行検証ができる小さな場」とし、動的ルーティングで多様性を維持するため、自己改善ループの報酬設計をかなり具体的に扱っている。
  - 人文: これは経験論の問題、つまり経験から学ぶ主体が、どの経験を信頼できる証拠として採用するのかという問いに近い。自己遊戯は自由な創造に見える一方で、検証制度がなければ迷信的な成功体験を増幅してしまう。

### 4. MalSkillBench: A Runtime-Verified Benchmark of Malicious Agent Skills
- 出典: arXiv
- 日付: 2026-06-05 初稿、2026-06-19 v3（古いが関連性が高い）
- リンク: https://arxiv.org/abs/2606.07131
- 要約: Claude Code や Gemini CLI などのコーディングエージェントが使う「スキル」を、コードであり自然言語指示でもあるハイブリッドなサプライチェーン依存として評価するベンチマーク。Generate-Verify-Feedback の閉ループで、Dockerサンドボックス、システムコール監視、LLMジャッジを通過した悪性スキルのみを採用する。
- なぜ面白いか:
  - 技術: 悪性サンプルを生成するだけでなく実行時に発火することを確認してラベル化するため、エージェント安全性を「推測」ではなく閉ループの観察可能性に寄せている。
  - 人文: スキルがコードと指示の中間物である点は、近代的な「物」と「言葉」の区分を揺さぶる。Loop Engineering の倫理は、意図を読むだけでもソースを読むだけでも足りず、行為が環境内で何を引き起こすかを見届ける責任論になる。

### 5. FizzBee: AI Requirements Engineer between your idea and your coding agent
- 出典: FizzBee 公式サイト / Hacker Newsで2026-07-08に確認
- 日付: 2026-07-08（直近14日よりやや古いが関連性が高い）
- リンク: https://fizzbee.ai/
- 要約: 曖昧なアイデアを、コーディングエージェントが構築でき、機械が解析できる精密で検証済みの仕様へ変換することを掲げるツール。Requirements Engineering、Specification-Driven Development、形式検証を、AIエージェントの前段に置く設計思想が明確である。
- なぜ面白いか:
  - 技術: 実装ループの前に仕様の曖昧さを発見・検証する段階を挿入し、エージェントが沈黙のうちに仕様判断を代行してしまうリスクを減らす。
  - 人文: これは「何を作るべきか」をコード生成に丸投げしないための実践知であり、アリストテレス的な制作知と実践知の境界を思い出させる。Loop Engineering は速く回すことだけでなく、どの問いを先に立てるかを決める倫理でもある。

## arXiv / 学術
- 見つかりました: `2607.22529` Skill Self-Play: Pushing the Frontier of LLM Capability with Co-Evolving Skills（2026-07-24）— 検証可能なスキルと自己遊戯で、学習ループの多様性と信頼性を両立させる研究。
- 見つかりました: `2606.07131` MalSkillBench: A Runtime-Verified Benchmark of Malicious Agent Skills（2026-06-05、v3 2026-06-19）— Generate-Verify-Feedback による悪性スキルの実行時検証ベンチマーク。
- 関連する古い候補: `2605.24426` SEAL: Synergistic Co-Evolution of Agents and Learning Environments、`2605.19717` Physics-in-the-Loop、`2605.06434` Knowledge Graphs, the Missing Link in Agentic AI-based Formal Verification。

## メモ
- Boris Cherny優先: 本トピックはClaude固有ではないため、Boris Cherny優先は適用外。
- 日本語アカウントの扱い: 日本語X検索を実行したが、X検索ツールがクレジット上限で失敗したため投稿内容は取得できなかった。代替としてBing経由の日本語Web検索を行ったが、一般的なAI解説ページが多く、今回のトップ5には採用しなかった。
- 注意点・誇張リスク: Web検索ツールも未設定で失敗したため、直接HTTP取得、Bing HTML検索、Hacker News Algolia API、arXiv HTML検索で補完した。直近14日に厳密に収まる実例は限られたため、2026-07-13、2026-07-08、2026-06の重要項目は古いものとして明記した。

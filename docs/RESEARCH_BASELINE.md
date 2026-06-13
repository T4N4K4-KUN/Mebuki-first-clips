# RESEARCH_BASELINE

この文書は、`mebuki starter clips v0` の脚本・構成・レビューで最初に読む基準文書。
Codex / Claude Code が白紙から「それっぽい励まし」を創作することを防ぐため、調査済みの判断軸をここに固定する。

## v0 principle

v0で作るのは、教材シリーズでも講座でもブランドムービーでもない。

作るのは、初心者・エンジニア返り咲き層が、今日もう一度だけ開発に戻れるようにする短尺クリップ6本。

- まず6本だけ。
- 9:16縦ショートを基本にする。
- 1080×1920 / 20〜35秒 / 字幕前提。
- 外部素材の翻訳・切り抜き・描き直しはしない。
- 反応を見てから必ず変える。

長期計画や大量案を作り始めない。v0の仕事は、反応を見るための最小単位を出すこと。

## target viewers

### 初心者

- エラーを見ると、自分には向いていないと思う。
- 何から始めればよいかわからない。
- 「ちゃんと勉強しないと意味がない」と思い込みやすい。
- AIや検索を使うことに罪悪感がある。
- 動いたものより、理解できない自分を責めがち。

必要な支援：責めない。行動を小さくする。「今日やること」を1つに絞る。

### エンジニア返り咲き層

- 昔やめた、挫折した、離れていた記憶がある。
- 今の開発環境やAI時代に置いていかれた感覚がある。
- 若い人や現役エンジニアと比べてしまう。
- まとまった学習時間がない。
- 「また続かなかったらどうしよう」という不安がある。

必要な支援：過去の中断を失敗者扱いしない。再開を「やり直し」ではなく「戻ってくる」と捉える。記録で戻れる感覚を作る。

## content strategy

このrepoは、知識を大量に教えるのではなく、心理状態を扱う。

良いクリップ：

1. 視聴者の今の不安を言い当てる。
2. 見方を少し変える。
3. 今日できる1つの行動に着地する。
4. 戻ってこられる感覚を残す。

悪いクリップ：

1. 抽象的な励まし。
2. それっぽい名言。
3. 具体行動なし。
4. 見終わって何も変わらない。

## reference classification

| Class | Meaning | Use |
|---|---|---|
| A | 直接使える可能性がある素材 | 条件確認・台帳記録後に使える可能性あり |
| B | 研究対象として強い素材 | 構造・テンポ・学習粒度だけ学ぶ。表現は使わない |
| C | 直接利用を避ける素材 | 見るだけ。台本・映像・字幕・図解として使わない |

### A: direct-use candidates

Aでも無条件利用ではない。必ず台帳に残す。

- 自作の文章、図、音声、画面モック。
- CC0 / Public Domain と確認できる素材。
- CC BY と確認でき、クレジット条件を満たせる素材。
- CC BY-SA と確認でき、継承条件を理解できる素材。
- 商用利用・改変可と明記されたロイヤリティフリー素材。
- 個別許諾を得た素材。
- freeCodeCampのGitHub repoなど、コード・curriculumのライセンスが明確なもの。ただし動画・記事・講義表現は別扱い。

### B: structure-only references

| Reference | What to learn | Do not do |
|---|---|---|
| freeCodeCamp | 学習ロードマップ、自走設計、プロジェクト型学習、課題の粒度 | 動画・記事・本文・台詞を日本語化しない |
| CS50 | 初心者を子ども扱いしない熱量、難しさを隠さない導入、参加感 | 講義・スライド・台詞・演出を使わない |
| Khan Academy | 急がない説明、前提を置く安心感、小さな概念分解 | 図解・説明文・画面を移植しない |
| 筋トレ系ショート | 「1回でOK」「継続が勝ち」「フォーム重視」の習慣化設計 | 台詞・構成・BGM・画面をコピーしない |
| 英語学習系ショート | 「1日1フレーズ」型の反復設計 | フォーマットを丸写ししない |
| 瞑想・メンタル系ショート | 焦りをほどく言葉、比較をやめる導線 | 情緒表現をコピーしない |

### C: avoid direct use

- TED Talks / TED-Ed の映像、字幕、台本、翻訳、音声。
- Crash Courseなど、明示許諾が確認できないYouTube動画の映像、音声、字幕、台本、図解。
- CC BY-NC / CC BY-NC-SA / CC BY-ND / CC BY-NC-ND の素材を直接使うこと。
- `NonCommercial only`, `personal use only`, `educational use only`, `no monetization`, `商用利用不可` の素材。
- 有料講座、会員限定教材、教材スライド、書籍紙面、他者のサムネイル。

## rights guard

v0では、広告収益化や将来のmebuki導線の可能性を考え、直接使う素材は商用利用可能なものに寄せる。

- NC素材は、動画に直接使わない。
- ND素材は、翻訳・編集・再構成に使わない。
- 外部動画を日本語化するだけの制作は禁止。
- 権利が曖昧なら、素材として使わず、構造だけ学ぶ。
- 参考元から得た学びは `docs/MATERIALS_LEDGER.md` または作業メモに残す。

## official references to verify

必要に応じて公式ページを確認し、確認日を台帳に残す。

- Creative Commons FAQ: https://creativecommons.org/faq/
- CS50x license: https://cs50.harvard.edu/x/2025/license/
- freeCodeCamp GitHub license: https://github.com/freeCodeCamp/freeCodeCamp/blob/main/LICENSE.md
- TED Talks Usage Policy: https://www.ted.com/about/our-organization/our-policies-terms/ted-talks-usage-policy
- YouTube Terms: https://www.youtube.com/static?template=terms
- YouTube monetization help: https://support.google.com/youtube/answer/2490020

## default decision

迷ったら、外部素材は使わない。外部素材から型だけ学ぶ。台本・図・画面・音声・字幕は自作する。

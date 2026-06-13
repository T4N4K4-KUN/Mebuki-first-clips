# RUN.sprout — mebuki starter clips v0

## SCOPE（最重要 / READ FIRST）

このファイルは、人間が読む開始手順と、Codex / Claude Code が実行する仕様を分ける。

- `## HUMAN-EXEC`：人間が使う開始手順。Codex / Claude Code は実行しない。
- `## MACHINE-EXEC`：Codex / Claude Code が実行する唯一の仕様。
- Codex / Claude Code は `## MACHINE-EXEC` 内の `### Target files` に列挙されたファイルだけを作成・更新する。
- `### File content` の各ブロックは、生成先ファイルの本文である。
- 判断が必要になった場合は、作業を止めて人間に確認する。

この sprout は、mebuki とともに成長する初心者・エンジニア返り咲き層に向けた、最初の短尺動画クリップ6本の制作を始めるためのrepoを芽吹かせる。

これは動画制作アプリ、レンダリング環境、量産システム、長期コンテンツ計画ではない。最初の6本を軽く作り、反応を見て次を決めるための、最小限の制作repoである。

---

## HUMAN-EXEC

推奨手順はこれだけ。

1. 空のリポジトリを作成し、ローカルへcloneする。
2. repo rootにこのファイルを `RUN.sprout.md` として置く。
3. Codex / Claude Code をrepo rootで開き、次を貼る。

```text
この `RUN.sprout.md` を読んでください。
`## MACHINE-EXEC` だけを実行対象にしてください。
`## HUMAN-EXEC` は実行しないでください。
`### Target files` に列挙されたファイルだけを、`### File content` の内容に従って作成してください。
既存の同名ファイルがあり、かつ空でない場合は、変更前に停止して確認してください。
install、build、test、commit、push、network、package manager command は実行しないでください。
作成またはスキップしたファイルを報告してください。
```

<details>
<summary>ローカルだけで試す場合</summary>

```bash
mkdir mebuki-starter-clips
cd mebuki-starter-clips
git init
```

その後、このファイルをrepo rootに `RUN.sprout.md` として置き、上の開始指示をCodex / Claude Codeに貼る。

</details>

---

## MACHINE-EXEC

### Goal

mebuki とともに成長する初心者・エンジニア返り咲き層に向けた、最初の短尺動画クリップ6本の制作を開始できるrepo一式を作成する。

このrepoは、まず6本だけを対象にする。大量の構想、精緻な長期計画、動画生成コード、レンダリングパイプラインは作らない。目的は、6本の企画・台本化・権利確認・軽い制作・反応確認までを小さく回せる状態にすることである。

### Target files

- `.gitignore`
- `README.md`
- `AGENTS.md`
- `TODO.md`
- `clips/README.md`
- `clips/001-error-started.md`
- `clips/002-five-minutes.md`
- `clips/003-returner-not-weak.md`
- `clips/004-ask-ai-search-ok.md`
- `clips/005-make-before-understand.md`
- `clips/006-log-to-return.md`
- `docs/PRODUCTION_RULES.md`
- `docs/RIGHTS_AND_REFERENCES.md`
- `docs/MATERIALS_LEDGER.md`
- `docs/RETROSPECTIVE.md`
- `runs/_TEMPLATE/RUN.md`

### Steps

1. 現在のディレクトリが対象リポジトリのrootであることを確認する。
2. `### Target files` に列挙された各ファイルについて、必要な親ディレクトリを作成し、対応する `### File content` の内容で作成する。
3. 同名ファイルが存在し、かつ空でない場合は、変更前に停止して人間へ確認する。
4. `### Target files` にないファイルは作成しない。
5. install、build、test、commit、push、network、package manager command は実行しない。
6. 動画ファイル、画像ファイル、音声ファイル、生成物、バイナリ、外部素材は作成しない。
7. 最後に、作成またはスキップしたファイルを報告する。

### File content

#### `.gitignore`

~~~gitignore
# local/system
.DS_Store
Thumbs.db
*.log

# generated / exported media
out/
exports/
renders/
raw/
tmp/
.cache/

# large local working files
*.mp4
*.mov
*.m4v
*.mp3
*.wav
*.aiff
*.psd
*.ai
*.prproj
*.drp
*.afdesign
*.afphoto

# keep source docs and lightweight planning files in git
!.gitignore
~~~

#### `README.md`

~~~md
# mebuki starter clips v0

初心者・エンジニア返り咲き層に向けた、mebukiの最初の短尺動画クリップ6本を作るためのrepo。

このrepoの目的は、教材を完成させることではない。まず6本だけを軽く作り、反応を見て、次に伸ばすテーマを決めること。

## v0 goal

9:16縦ショートを6本作る。

- 1080×1920を基本にする。
- 20〜35秒を目安にする。
- 字幕前提にする。
- 映像は自作の静止画・簡単なモーション・画面構成で足りる。
- 外部動画、外部字幕、外部台本、外部図解を翻訳・切り抜き・描き直しで使わない。
- 反応を見てから、継続・ピボット・横展開を決める。

## First six clips

| No | Clip | Purpose | File |
|---:|---|---|---|
| 1 | エラーが出たら、始まっている | 不安を下げる | `clips/001-error-started.md` |
| 2 | 今日は5分だけ触れば勝ち | 行動を小さくする | `clips/002-five-minutes.md` |
| 3 | 昔やめた人は、弱い人じゃない | 返り咲き層を受け止める | `clips/003-returner-not-weak.md` |
| 4 | AIに聞いていい。検索していい。 | 自力主義の呪縛を外す | `clips/004-ask-ai-search-ok.md` |
| 5 | 理解より、まず動くものを作る | 完璧主義を下げる | `clips/005-make-before-understand.md` |
| 6 | ログを残せる人は、戻ってこられる | mebukiらしい復帰導線を伝える | `clips/006-log-to-return.md` |

## Repository layout

- `clips/` — 6本それぞれの企画、台本、制作メモ。
- `docs/PRODUCTION_RULES.md` — 画角、尺、字幕、制作フローの最小ルール。
- `docs/RIGHTS_AND_REFERENCES.md` — 参考素材のA/B/C分類と権利ガード。
- `docs/MATERIALS_LEDGER.md` — 素材・参考元・権利確認の台帳。
- `docs/RETROSPECTIVE.md` — 6本公開後に見る指標とピボット判断。
- `runs/_TEMPLATE/RUN.md` — 作業単位のメモ用テンプレート。
- `TODO.md` — 今やること。
- `AGENTS.md` — Codex / Claude Code 向け作業規約。

## Working style

1. `TODO.md` から1本だけ選ぶ。
2. 対象の `clips/*.md` を開く。
3. 1メッセージ、3〜5カット、20〜35秒に収める。
4. 外部素材を使う前に `docs/MATERIALS_LEDGER.md` に記録する。
5. 権利が曖昧な素材は使わない。構造だけ参考にして自作する。
6. 6本が出るまで、長いシリーズ計画や大量の追加案を作らない。

## Success criteria for v0

6本を公開または社内確認できる形にしたら、次だけを見る。

- 最後まで見られたか。
- 保存されたか。
- コメントや反応に「自分のことだ」が出たか。

再生数だけで判断しない。mebukiに必要なのは、広く薄いバズより、続けたい人・戻ってきたい人が残る兆候である。

## Non-goals

v0では次をやらない。

- 300本の企画化。
- 横動画・長尺教材・講座化。
- レンダリング自動化。
- 素材サイトの大量探索。
- 外部動画の翻訳転載。
- 有料導線設計。
- ブランド完全設計。

6本の反応を見てから変える。
~~~

#### `AGENTS.md`

~~~md
# AGENTS.md

このリポジトリで作業するCodexおよびcoding agent向けのガイダンス。

## Project snapshot

- 目的：mebukiとともに成長する初心者・エンジニア返り咲き層に向けた、最初の短尺動画クリップ6本を制作する。
- 成果物：9:16縦ショートの企画、台本、制作メモ、権利台帳、反応確認メモ。
- v0範囲：6本だけ。大量企画、長期ロードマップ、動画生成コード、レンダリング環境は作らない。
- 主なファイル：`README.md`, `TODO.md`, `clips/*.md`, `docs/*.md`。

## Read first

作業開始時は、少なくとも次を読む。

1. `README.md`
2. `TODO.md`
3. 対象の `clips/*.md`
4. `docs/PRODUCTION_RULES.md`
5. `docs/RIGHTS_AND_REFERENCES.md`
6. 外部素材や参考元に触れる場合は `docs/MATERIALS_LEDGER.md`

## Core rule

このrepoは「小さく試す」ためのrepoである。

- 6本が終わるまで、追加の大量クリップ案を作らない。
- 長いコンテンツ戦略を勝手に作らない。
- コードや自動化を先に作らない。
- まず、1本ずつ、短く、見られる形に近づける。

## Content rules

- 1本につき、中心メッセージは1つにする。
- 20〜35秒を目安にする。
- 3〜5カットで十分。
- 字幕で意味が通るようにする。
- 難しい概念説明より、視聴後に1つ行動したくなることを優先する。
- 初心者を子ども扱いしない。
- 返り咲き層を「挫折した人」と決めつけない。
- mebukiの内部戦略や作り手側の都合を、視聴者向け台本に混ぜない。

## Rights and reference guard

外部素材や海外教材を扱うときは、次を守る。

- 外部動画の映像を使わない。
- 外部動画の音声を使わない。
- 外部字幕を翻訳して使わない。
- 外部台本を翻訳して使わない。
- 外部図解を描き直して使わない。
- 外部サムネイル、キャラクター、画面構成を似せない。
- `NC`, `ND`, `personal use only`, `educational use only`, `no monetization`, `商用利用不可` の素材は、直接素材として使わない。
- 参考元から使ってよいのは、原則として「構造」「問いの立て方」「テンポ」「学習粒度」「習慣化の型」まで。
- 具体的な表現、比喩、台詞、図、構成の並びが似すぎる場合は作り直す。

素材を使う場合は、先に `docs/MATERIALS_LEDGER.md` へ記録する。ライセンスや利用条件を推測しない。分からない場合は使わないか、人間に確認する。

## Research rules

参考にする候補は `docs/RIGHTS_AND_REFERENCES.md` にまとめてある。調査する場合も、調査結果をそのまま台本にしない。

良い使い方：

- freeCodeCampから学習ロードマップの粒度を学ぶ。
- CS50から初心者を惹き込む熱量を学ぶ。
- TED-Edから短い問いと物語の作り方を学ぶ。
- 筋トレ・英語学習・瞑想系ショートから習慣化の言葉を学ぶ。

悪い使い方：

- 英語動画を日本語化して投稿する。
- 既存動画の構成をほぼ同じ順番で作る。
- 他者の図を描き直す。
- 「教育目的だから大丈夫」と判断する。

## File editing rules

- 既存の意図を壊さない。
- 小さく、reviewしやすい変更を優先する。
- 不要なファイルを増やさない。
- 動画・音声・画像などの大きなファイルは、明示依頼がない限り作らない。
- `out/`, `exports/`, `renders/`, `raw/`, `tmp/` は生成物置き場であり、通常git管理しない。
- line numberや外部ライセンス情報を捏造しない。

## When to stop and ask

次の場合は編集を止めて人間に確認する。

- 商用利用可否が曖昧な素材を使いたい場合。
- 外部教材の翻訳・翻案に近い案になった場合。
- 6本以外の大きな展開を作りたくなった場合。
- 動画制作ツール、音声合成、BGM、フォントなどの導入判断が必要な場合。
- 既存の空でないファイルを上書きする場合。

## Completion report

作業完了時は次を報告する。

- 変更したファイル。
- 何を進めたか。
- 使った外部素材・参考元の有無。
- 権利確認で未解決の点。
- 次に人間が見るべきファイル。
~~~

#### `TODO.md`

~~~md
# TODO

このrepoのv0は、最初の6本だけを作る。

## Current focus

9:16縦ショート6本の企画・台本・簡易制作メモを整え、公開または社内確認できる状態まで進める。

## Now

- [ ] `docs/PRODUCTION_RULES.md` を読み、v0の画角・尺・制作方針を確認する。
- [ ] `docs/RIGHTS_AND_REFERENCES.md` を読み、外部素材の扱いを確認する。
- [ ] 6本それぞれの `clips/*.md` に、20〜35秒に収まる短い台本案を作る。
- [ ] 各クリップで使う予定の素材・参考元を `docs/MATERIALS_LEDGER.md` に記録する。
- [ ] 外部素材を使わずに成立する簡易ビジュアル案を各クリップに書く。

## First six

- [ ] 001 `エラーが出たら、始まっている` — draft
- [ ] 002 `今日は5分だけ触れば勝ち` — draft
- [ ] 003 `昔やめた人は、弱い人じゃない` — draft
- [ ] 004 `AIに聞いていい。検索していい。` — draft
- [ ] 005 `理解より、まず動くものを作る` — draft
- [ ] 006 `ログを残せる人は、戻ってこられる` — draft

## Before publishing

- [ ] 全クリップで外部動画・外部音声・外部字幕・外部台本・外部図解を直接使っていないことを確認する。
- [ ] BGM、画像、フォント、アイコンを使う場合、商用利用・改変・クレジット条件を台帳に記録する。
- [ ] 字幕だけで意味が通ることを確認する。
- [ ] 1本1メッセージになっていることを確認する。
- [ ] 視聴後の行動が1つに絞れていることを確認する。

## After six

6本が公開または社内確認された後だけ実施する。

- [ ] `docs/RETROSPECTIVE.md` に結果を記録する。
- [ ] 完視聴、保存、コメントの3点を見る。
- [ ] 伸ばすテーマを1つだけ選ぶ。
- [ ] 続ける / ピボットする / いったん止める を決める。

## Do not do yet

- [ ] 300本案を作らない。
- [ ] 長尺教材化しない。
- [ ] レンダリング自動化しない。
- [ ] 有料導線を設計しない。
- [ ] 外部教材の日本語化転載をしない。
~~~

#### `clips/README.md`

~~~md
# clips

最初の6本のクリップ企画を置く。

## Status values

- `idea` — 方向性だけある。
- `draft` — 台本案がある。
- `review` — 表現・権利・尺を確認中。
- `ready` — 制作に進める。
- `prototype` — 仮動画がある。
- `published` — 公開済み。
- `retired` — 反応や方針変更により止めた。

## v0 format

- 9:16 vertical
- 1080×1920
- 20〜35秒
- 字幕あり
- 1本1メッセージ
- 3〜5カット
- 外部素材なしでも成立する構成

## First six

1. `001-error-started.md` — エラーが出たら、始まっている
2. `002-five-minutes.md` — 今日は5分だけ触れば勝ち
3. `003-returner-not-weak.md` — 昔やめた人は、弱い人じゃない
4. `004-ask-ai-search-ok.md` — AIに聞いていい。検索していい。
5. `005-make-before-understand.md` — 理解より、まず動くものを作る
6. `006-log-to-return.md` — ログを残せる人は、戻ってこられる

## Clip file rule

各clip fileは、最初から完成台本にしない。まずは次が分かればよい。

- 誰のどんな心理に向けるか。
- 視聴後に何をしてほしいか。
- 何を言わないか。
- 外部素材なしでどう見せるか。
- 権利確認で何が残っているか。
~~~

#### `clips/001-error-started.md`

~~~md
# 001 — エラーが出たら、始まっている

status: idea
format: 9:16 vertical / 20〜35秒 / 字幕あり
primary audience: 開発初心者、久しぶりにコードへ戻る人

## Purpose

エラーへの恐怖を下げる。エラーは失敗ではなく、開発が始まった合図だと伝える。

## Viewer state

- エラー画面を見ると、自分には向いていないと感じる。
- 赤い文字や長いログに圧倒される。
- まだ何もできていないと思いがち。

## Core message

エラーが出たら、始まっている。

## Desired action

エラー文を1行だけコピーして、AIまたは検索に投げてみる。

## Draft constraints

- エラーを笑いにしすぎない。
- 「エラーは友達」だけで終わらせない。
- 具体行動を1つ入れる。
- 外部教材の言い回しを翻訳しない。

## Possible beats

1. エラー画面で止まる瞬間。
2. それは失敗ではなく、プログラムが返事をしている状態。
3. まず1行だけ読めばよい。
4. 今日の勝ち：エラー文を1つ貼って聞く。

## Visual idea

- 黒背景に赤いエラー風テキスト。ただし実在サービスや実在ログは使わない。
- 文字が少しずつ整理され、1行だけが強調される。
- 最後に「1行だけでいい」。

## Production TODO

- [ ] 20〜35秒の台本を書く。
- [ ] 実在ログではなく自作のサンプルエラー文にする。
- [ ] 使用フォント、BGM、効果音を台帳に記録する。
- [ ] 字幕だけで意味が通るか確認する。

## Rights notes

外部のエラー画面スクショ、教材画面、Stack Overflow等の実画面を使わない。必要なら自作モックを使う。
~~~

#### `clips/002-five-minutes.md`

~~~md
# 002 — 今日は5分だけ触れば勝ち

status: idea
format: 9:16 vertical / 20〜35秒 / 字幕あり
primary audience: 継続に不安がある初心者、時間がない返り咲き層

## Purpose

始めるハードルを下げる。毎日長時間やることではなく、今日5分だけ触ることを勝ちにする。

## Viewer state

- まとまった時間がない。
- ちゃんと勉強しなければ意味がないと思っている。
- 1日空くと戻れなくなる。

## Core message

今日は5分だけ触れば勝ち。

## Desired action

PCを開く、repoを見る、READMEを1行読む、TODOを1つだけ見る。どれか1つでよい。

## Draft constraints

- 根性論にしない。
- 「毎日必ず」と強く言いすぎない。
- 短時間でも戻れる設計が大事だと伝える。
- 筋トレ系ショートの言い回しをそのまま移植しない。

## Possible beats

1. 「今日は無理」と思う。
2. でも、5分ならできる。
3. 5分でいいのは、進めるためではなく、戻る道を消さないため。
4. 今日の勝ち：repoを開く。

## Visual idea

- 5:00のタイマー。
- PCを開く、READMEを見る、TODOにチェックを入れるような抽象モーション。
- 最後に「5分で、道はつながる」。

## Production TODO

- [ ] 20〜35秒の台本を書く。
- [ ] 5分でできる行動を1つに絞る。
- [ ] タイマーやUI素材を自作する。
- [ ] 使用素材を台帳に記録する。

## Rights notes

既存の筋トレ・英語学習ショートの台詞や構成をコピーしない。習慣化の型だけ参考にする。
~~~

#### `clips/003-returner-not-weak.md`

~~~md
# 003 — 昔やめた人は、弱い人じゃない

status: idea
format: 9:16 vertical / 20〜35秒 / 字幕あり
primary audience: 一度プログラミングを離れた人、返り咲き層

## Purpose

返り咲き層の自己否定を下げる。過去に離れたことを弱さではなく、戻るための経験として扱う。

## Viewer state

- 昔やったが続かなかった。
- もう遅いと思っている。
- 最新環境についていけないと思っている。

## Core message

昔やめた人は、弱い人じゃない。

## Desired action

以前の自分を責めず、今日の小さな再開地点を1つ決める。

## Draft constraints

- 感動させようとしすぎない。
- 「挫折」という言葉を安易に使いすぎない。
- 返り咲き層を初心者未満のように扱わない。
- メンタル系ショートの言葉をそのまま使わない。

## Possible beats

1. 昔やめたことがある。
2. でも、それは弱さの証明ではない。
3. 今はAIも、ログも、戻る道もある。
4. 今日の勝ち：前回どこで止まったかを書く。

## Visual idea

- 古いノート、閉じたPC、再び開く画面。
- 過去から現在へ線がつながる。
- 最後に「戻ってきた時点で、もう始まっている」。

## Production TODO

- [ ] 20〜35秒の台本を書く。
- [ ] 情緒に寄せすぎない表現へ調整する。
- [ ] 視聴後の行動を1つに絞る。
- [ ] 使用素材を台帳に記録する。

## Rights notes

外部の自己啓発動画やメンタル系ショートの台詞、比喩、流れをコピーしない。自己受容の型だけ参考にする。
~~~

#### `clips/004-ask-ai-search-ok.md`

~~~md
# 004 — AIに聞いていい。検索していい。

status: idea
format: 9:16 vertical / 20〜35秒 / 字幕あり
primary audience: 自力で理解しないと意味がないと思っている初心者・返り咲き層

## Purpose

自力主義の呪縛を外す。AIや検索を使うことはズルではなく、開発の普通の進め方だと伝える。

## Viewer state

- AIに聞くと実力がつかないと思っている。
- 検索しすぎる自分を責めている。
- プロは全部覚えていると思い込んでいる。

## Core message

AIに聞いていい。検索していい。

## Desired action

分からないことを、1つだけ質問文にする。

## Draft constraints

- AI万能論にしない。
- コピペだけで終わらせない。
- 「聞いて、試して、ログを残す」まで入れる。
- 特定AIサービスへの過度な誘導にしない。

## Possible beats

1. 分からないまま止まる。
2. 聞いていい。検索していい。
3. 大事なのは、答えを写すことではなく、試した結果を残すこと。
4. 今日の勝ち：質問を1つ書く。

## Visual idea

- 空の質問欄。
- 「何が分からない？」が「このエラーは何？」に変わる。
- 最後に「質問できたら、前に進んでいる」。

## Production TODO

- [ ] 20〜35秒の台本を書く。
- [ ] AI使用の注意点を1つだけ入れる。
- [ ] 実在AIサービス画面を使うかどうかは人間に確認する。基本は自作モック。
- [ ] 使用素材を台帳に記録する。

## Rights notes

実在サービス画面、検索結果画面、他者のQ&A本文は直接使わない。必要なら抽象化した自作モックにする。
~~~

#### `clips/005-make-before-understand.md`

~~~md
# 005 — 理解より、まず動くものを作る

status: idea
format: 9:16 vertical / 20〜35秒 / 字幕あり
primary audience: 勉強してからでないと作れないと思っている初心者

## Purpose

完璧主義を下げる。理解を否定するのではなく、最初は小さく動くものを作ることで理解が始まると伝える。

## Viewer state

- 先に全部理解しないと不安。
- チュートリアルを見続けて手が動かない。
- 小さな成果を軽く見ている。

## Core message

理解より、まず動くものを作る。

## Desired action

ボタン1つ、README1行、console.log 1つなど、見える小さな結果を作る。

## Draft constraints

- 理解を軽視しない。
- 雑に作ればよい、とは言わない。
- 小さな実物が理解の入口になると伝える。
- freeCodeCamp等の課題文や教材構成を直接コピーしない。

## Possible beats

1. まだ理解できていないから作れない、と思う。
2. 逆に、作るから理解が始まることがある。
3. 今日は大きなアプリではなく、1つ動けばいい。
4. 今日の勝ち：画面に1つ表示する。

## Visual idea

- 空白の画面に小さなボタンが1つ出る。
- 「完璧な理解」から「小さく動く」へ表示が切り替わる。
- 最後に「動いたら、学びが始まる」。

## Production TODO

- [ ] 20〜35秒の台本を書く。
- [ ] 具体行動を1つに絞る。
- [ ] UI素材は自作する。
- [ ] 使用素材を台帳に記録する。

## Rights notes

外部教材の演習画面、課題文、コード例を直接使わない。必要なら完全に自作した最小例にする。
~~~

#### `clips/006-log-to-return.md`

~~~md
# 006 — ログを残せる人は、戻ってこられる

status: idea
format: 9:16 vertical / 20〜35秒 / 字幕あり
primary audience: 作業が途切れると戻れなくなる初心者・返り咲き層

## Purpose

mebukiらしい「戻れる」感覚を伝える。才能や根性ではなく、短いログが次の自分を助けると示す。

## Viewer state

- 途中で止まると、次の日に何をしていたか分からない。
- 進捗が消える感覚がある。
- 作業メモを残す習慣がない。

## Core message

ログを残せる人は、戻ってこられる。

## Desired action

今日やったこと、詰まったこと、次にやることを1行ずつ残す。

## Draft constraints

- mebukiの内部思想を説明しすぎない。
- RUN.mdやrepo運用の細かい説明を入れすぎない。
- 視聴者には「戻れる」価値だけ伝える。
- 専門用語を増やさない。

## Possible beats

1. 昨日の続きが分からない。
2. それは記憶力の問題だけではない。
3. 1行のログが、明日の自分への道しるべになる。
4. 今日の勝ち：次にやることを1行書く。

## Visual idea

- 「やったこと」「詰まったこと」「次にやること」の3行メモ。
- 途切れた線が、ログによってつながる。
- 最後に「戻れる形で終わる」。

## Production TODO

- [ ] 20〜35秒の台本を書く。
- [ ] mebukiの説明を入れすぎないように調整する。
- [ ] 3行ログの自作モックを作る。
- [ ] 使用素材を台帳に記録する。

## Rights notes

実在の作業ログ、個人情報、プロジェクト情報を画面に出さない。すべて自作サンプルにする。
~~~

#### `docs/PRODUCTION_RULES.md`

~~~md
# PRODUCTION_RULES

v0は、最初の6本を軽く作るための制作ルールである。

## Format

- Primary: 9:16 vertical
- Size: 1080×1920
- Length: 20〜35秒
- Captions: required
- Audio: optional, but captions must stand alone
- Visuals: self-made stills, simple motion, abstract UI, text animation

## Why vertical first

v0の目的は、スマホ上で初心者・返り咲き層の心理に刺さるかを見ること。PC視聴や横長解説は後でよい。コード解説や長尺教材化は、6本の反応を見てから決める。

## Script shape

1本につき、次の構成で十分。

```text
Hook: 1文
Reframe: 1文
Small action: 1文
Close: 1文
```

または、3〜5カットで作る。

```text
Cut 1: 視聴者の不安
Cut 2: 見方を変える
Cut 3: 今日の小さな行動
Cut 4: 短い締め
```

## Language

- 短く言う。
- 説教しない。
- 初心者を子ども扱いしない。
- 返り咲き層を失敗者扱いしない。
- 「誰でも簡単」と言い切らない。
- 「できないのは努力不足」と言わない。
- 視聴後に1つ行動できる言葉にする。

## Visual rules

- 実在サービスの画面スクショを使わない。必要なら自作モックにする。
- 実在のエラー画面、検索結果、Q&A、教材、講義スライドを使わない。
- 読みやすい大きな文字にする。
- 1画面に詰め込みすぎない。
- 画面上の文字は、字幕と競合しないようにする。

## Asset rules

- 自作素材を優先する。
- BGM、効果音、フォント、アイコン、画像を使う場合は `docs/MATERIALS_LEDGER.md` に記録する。
- 商用利用、改変、クレジット、再配布条件が不明な素材は使わない。
- `NC`, `ND`, `personal use only`, `educational use only`, `no monetization`, `商用利用不可` は直接利用しない。

## Draft flow

1. `TODO.md` から1本選ぶ。
2. 対象の `clips/*.md` に台本案を書く。
3. 20〜35秒に収める。
4. 外部素材の有無を確認する。
5. `docs/MATERIALS_LEDGER.md` に素材・参考元を記録する。
6. 人間が確認する。
7. 必要なら動画制作ツールで仮動画を作る。
8. 公開または社内確認後、`docs/RETROSPECTIVE.md` に結果を書く。

## Definition of ready

各クリップは、次を満たしたら制作に進める。

- [ ] 中心メッセージが1つ。
- [ ] 20〜35秒に収まる見込みがある。
- [ ] 視聴後の行動が1つ。
- [ ] 外部素材の直接利用がない、または台帳で確認済み。
- [ ] 字幕だけで意味が通る。
- [ ] 初心者・返り咲き層への敬意がある。

## Stop rules

次に該当したら止める。

- 6本以外のシリーズ計画を作り始めた。
- 外部動画の日本語化に近づいた。
- ライセンスが曖昧な素材を使いたくなった。
- 長尺教材やアプリ制作へ話が膨らんだ。
- 視聴者向け台本に、作り手側の戦略や事情が混ざり始めた。
~~~

#### `docs/RIGHTS_AND_REFERENCES.md`

~~~md
# RIGHTS_AND_REFERENCES

このrepoでは、外部素材を「使う」より先に「学ぶ」。

v0の基本方針は、外部素材を翻訳・切り抜き・描き直しで使うことではない。参考元から学ぶのは、構造、テンポ、問いの立て方、学習粒度、習慣化の型まで。表現はmebuki用に自作する。

## A/B/C classification

| Class | Meaning | Use in this repo |
|---|---|---|
| A | 直接素材として使える可能性があるもの | 条件を確認し、台帳に記録してから使う |
| B | 研究・参考には強いが、直接利用しないもの | 構造・テンポ・学習粒度だけ学ぶ |
| C | 直接利用、翻訳、切り抜き、描き直しを避けるもの | 見るだけ。素材・台本・図解として使わない |

## A — direct-use candidates

Aでも、無条件に使ってよいわけではない。必ず `docs/MATERIALS_LEDGER.md` に記録する。

- 自作の文章、図、音声、画面モック。
- CC0 / Public Domain と確認できる素材。
- CC BY と確認でき、クレジット条件を満たせる素材。
- CC BY-SA と確認でき、継承条件を理解して使える素材。
- 商用利用・改変可と明記されたロイヤリティフリー素材。
- 個別許諾を得た素材。
- 公式ライセンスで利用条件を確認できたOSSコードや教材構造。ただし、動画・記事・講義表現そのものの利用可否は別に確認する。

## B — structure-only references

Bは、見て学ぶ対象。直接翻訳・転載しない。

| Reference | What to learn | Do not do |
|---|---|---|
| freeCodeCamp | 学習ロードマップ、プロジェクト型学習、初心者向け粒度 | 動画や記事を日本語化して使わない |
| CS50 | 初心者を惹き込む熱量、難しさを隠さない導入 | 講義、スライド、台詞、演出を使わない |
| Khan Academy | 急がない説明、前提を置く安心感 | 図解や説明文を移植しない |
| 筋トレ系ショート | 1回でOK、継続が勝ち、習慣化の型 | 台詞や構成をそのまま使わない |
| 英語学習系ショート | 1日1フレーズ型、短い反復 | フォーマットを丸写ししない |
| 瞑想・メンタル系ショート | 焦りをほどく、比較しない言葉 | 情緒表現をコピーしない |

## C — avoid direct use

Cは、v0では直接利用しない。

- TED Talks / TED-Ed の映像、字幕、台本、翻訳、音声。
- Crash Courseなど、明示許諾が確認できないYouTube動画の映像、音声、字幕、台本、図解。
- `CC BY-NC`, `CC BY-NC-SA`, `CC BY-ND`, `CC BY-NC-ND` の素材を直接使うこと。
- `NonCommercial only`, `personal use only`, `educational use only`, `no monetization`, `商用利用不可` の素材。
- 有料講座、会員限定教材、教材スライド、書籍紙面、他者のサムネイル。

## Practical rules

### Do

- 参考元のURL、見た日、学んだ構造を台帳に書く。
- 複数の参考元を見て、共通する型だけ抽出する。
- 台本、図、画面、音声、字幕は自作する。
- 似すぎたと感じたら作り直す。

### Do not

- 英語を日本語にするだけで投稿する。
- 外部動画を切り抜く。
- 外部字幕に日本語字幕を付ける。
- 外部図解を描き直す。
- 参考元の比喩をそのまま使う。
- 「教育目的だから大丈夫」と判断する。
- 「この動画だけ広告OFFなら必ず大丈夫」と断定する。

## Official references to verify when needed

必要になったときは、必ず公式ページを確認し、確認日を台帳に残す。

- Creative Commons FAQ: https://creativecommons.org/faq/
- freeCodeCamp GitHub license: https://github.com/freeCodeCamp/freeCodeCamp/blob/main/LICENSE.md
- TED Talks Usage Policy: https://www.ted.com/about/our-organization/our-policies-terms/ted-talks-usage-policy
- YouTube Terms / monetization / reused content policies: YouTube公式ヘルプと規約を確認する。

## Default decision

迷ったら、使わない。

ただし、学ぶことはできる。学んだ構造を、mebukiの視聴者、言葉、行動単位に変換して、自作する。
~~~

#### `docs/MATERIALS_LEDGER.md`

~~~md
# MATERIALS_LEDGER

素材・参考元・権利確認の台帳。

外部素材を使う前に記録する。外部素材を使わない場合でも、参考元から構造を学んだときは `Reference study log` に残す。

## Material ledger

| ID | Clip | Material / Source | Type | Planned use | License / permission | Commercial use OK? | Modification OK? | Attribution required? | Checked date | Evidence URL / note | Approved |
|---|---|---|---|---|---|---|---|---|---|---|---|
| SELF-TEXT-001 | all | original script | text | captions / narration | self-made | yes | yes | no | TBD | created in this repo | yes |
| SELF-VISUAL-001 | all | original text animation / mock UI | visual | video visuals | self-made | yes | yes | no | TBD | created by project | yes |

## Reference study log

| ID | Clip | Reference | Class | What was studied | What must not be copied | Checked date | URL / note |
|---|---|---|---|---|---|---|---|
| REF-FCC-001 | 005 | freeCodeCamp | B | project-based learning粒度 | 課題文、動画、記事本文、コード例 | TBD | official source to verify |
| REF-CS50-001 | 001 | CS50 | B | 難しさを隠さない導入、熱量 | 講義映像、スライド、台詞、演出 | TBD | official source to verify |
| REF-HABIT-001 | 002 | 筋トレ・英語・瞑想系shorts | B | 小さな継続の言葉 | 台詞、構成、サムネ、音楽 | TBD | source-specific notes |
| REF-TED-STRUCT-001 | optional | TED-Ed | C/B | 問いから始める短い物語構造 | 映像、字幕、台本、翻訳、図解 | TBD | official policy to verify |

## Approval meanings

- `yes` — 条件確認済み。現在の用途で使ってよい。
- `no` — 使わない。
- `pending` — 使う前に確認が必要。
- `reference-only` — 素材として使わず、構造研究のみ。

## Notes

- ライセンス条件を推測しない。
- スクリーンショットやダウンロード素材は、配布元URLと確認日を残す。
- BGM、フォント、効果音、アイコンは忘れやすいので必ず記録する。
- 収益化チャンネルで使う可能性があるため、v0でも商用利用・改変・クレジット条件を確認する。
~~~

#### `docs/RETROSPECTIVE.md`

~~~md
# RETROSPECTIVE

6本を出したあとに、次を決めるためのメモ。

v0では、再生数だけで判断しない。mebukiに必要なのは、初心者・返り咲き層が「自分のことだ」と感じ、戻ってこられる兆候である。

## Publish / review log

| Clip | Status | Published / reviewed date | Platform / place | Notes |
|---|---|---|---|---|
| 001 エラーが出たら、始まっている | TBD | TBD | TBD | TBD |
| 002 今日は5分だけ触れば勝ち | TBD | TBD | TBD | TBD |
| 003 昔やめた人は、弱い人じゃない | TBD | TBD | TBD | TBD |
| 004 AIに聞いていい。検索していい。 | TBD | TBD | TBD | TBD |
| 005 理解より、まず動くものを作る | TBD | TBD | TBD | TBD |
| 006 ログを残せる人は、戻ってこられる | TBD | TBD | TBD | TBD |

## Signals to check

| Clip | Completion / retention | Saves | Comments / replies | Strong signal? | Notes |
|---|---:|---:|---|---|---|
| 001 | TBD | TBD | TBD | TBD | TBD |
| 002 | TBD | TBD | TBD | TBD | TBD |
| 003 | TBD | TBD | TBD | TBD | TBD |
| 004 | TBD | TBD | TBD | TBD | TBD |
| 005 | TBD | TBD | TBD | TBD | TBD |
| 006 | TBD | TBD | TBD | TBD | TBD |

## Qualitative notes

見るべき反応：

- 「これならできそう」
- 「自分のことだ」
- 「戻ってみようかな」
- 「今日5分やった」
- 「エラーが怖くなくなった」
- 「ログを残してみた」

## Decision after six

6本後に、次のどれか1つを選ぶ。

- [ ] Continue: 反応が出たテーマを5本だけ横展開する。
- [ ] Pivot: 刺さった心理テーマに寄せ直す。
- [ ] Pause: 動画ではなく、README / 画像 / note / repo導線を見直す。
- [ ] Expand format: 横動画や画面共有解説を検討する。

## Do not decide from views alone

再生数が多くても、保存・コメント・完視聴が弱ければ、mebukiの伴走クリップとしては弱い可能性がある。

再生数が少なくても、コメントや保存に強い兆候があれば、その心理テーマは深掘りする価値がある。

## Next small experiment

6本後に決める。今は空欄のままにする。

```text
Next experiment:
Reason:
Target audience:
Clips to make:
Stop condition:
```
~~~

#### `runs/_TEMPLATE/RUN.md`

~~~md
# RUN

run_id: yyyymmdd-hhmmss_<short-topic>
started_at: YYYY-MM-DD HH:MM (JST)
owner: <human or agent>

## Goal

このrunで達成したいことを1〜2文で書く。

## Scope

触る予定のファイルだけを書く。

- `clips/<target>.md`
- `docs/MATERIALS_LEDGER.md` if external material or reference is involved
- `TODO.md` if task status changes

## Non-goals

このrunではやらないことを書く。

- 6本以外の企画追加。
- 外部動画の翻訳・切り抜き。
- レンダリング自動化。
- 大きなディレクトリ再編。

## Work log

- [ ] 読んだファイル：
- [ ] 変更したファイル：
- [ ] 権利確認：
- [ ] 未確認事項：

## Completion criteria

- [ ] 1本1メッセージになっている。
- [ ] 20〜35秒に収まる見込みがある。
- [ ] 外部素材の直接利用がない、または台帳に記録済み。
- [ ] 次の作業が `TODO.md` から分かる。

## Notes

判断、迷い、次に確認すべきことを書く。
~~~

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

<!-- MEBUKI-CLIPS-V0-FOCUS:START -->

## v0 focus: 6 clips, research-led, not AI-invented

このrepoのv0は、初心者・エンジニア返り咲き層に向けた短尺クリップ6本だけに集中する。

重要なのは、AIに気持ちよさそうな励まし文を書かせることではない。実在する人間の状態に合わせて、1本につき1つの心理負荷を下げ、1つの小さな行動に着地させること。

脚本や構成を作る前に必ず読む。

- `docs/RESEARCH_BASELINE.md`
- `docs/SCRIPTING_GUIDE.md`
- `docs/CLIP_BRIEFS_V0.md`
- `docs/HUMAN_REVIEW_CHECKLIST.md`

既存のclipファイルに台本案があっても、それは人間レビューを通るまで未承認ドラフトとする。

<!-- MEBUKI-CLIPS-V0-FOCUS:END -->

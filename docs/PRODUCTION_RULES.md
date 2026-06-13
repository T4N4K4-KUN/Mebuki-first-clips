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

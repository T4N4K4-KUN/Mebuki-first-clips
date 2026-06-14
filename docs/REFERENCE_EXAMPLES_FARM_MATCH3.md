# REFERENCE_EXAMPLES_FARM_MATCH3

`小さな畑アプリ` と `3つ揃えるパズル` のインスパイア元候補。

checked_date: 2026-06-15

目的:

- 人気IPをそのまま作ることではない。
- 001で「最初の1時間で自分用の小さいものが動く」を見せるため、既存作品から構造を盗む。

## Small Farm / Harvest

### 1. FarmVille

YouTube:
- https://www.youtube.com/results?search_query=FarmVille+gameplay+planting+harvesting+crops

見るポイント:

- 畑のマスが並ぶ。
- 種を植える。
- 時間経過または操作で作物が育つ。
- 収穫するとコイン/スコアが増える。
- やることが視覚的に分かる。

001で盗む核:

```text
植える
育つ
収穫する
数字が増える
```

001で削るもの:

- 時間管理
- ショップ
- フレンド
- 課金
- 大量の作物
- 保存

Mebuki 1-hour mini:

```text
3つの鉢がある。
クリックすると水をあげる。
3回水をあげると花になる。
収穫するとスコアが増える。
```

### 2. Stardew Valley

YouTube:
- https://www.youtube.com/results?search_query=Stardew+Valley+first+day+farming+harvesting

見るポイント:

- 生活/農園/収穫の気持ちよさ。
- 作物が育つことがプレイヤーの進行になる。
- 戦闘ではなく、日常行動が中心。

001で盗む核:

```text
小さい世話をすると、見た目が変わる。
```

001で削るもの:

- マップ移動
- NPC
- 時間/季節
- 道具切り替え
- インベントリ
- クラフト

Mebuki 1-hour mini:

```text
今日は畑だけ。
歩き回らない。
水やりと収穫だけ。
```

### 3. Harvest Moon / Story of Seasons

YouTube:
- https://www.youtube.com/results?search_query=Harvest+Moon+gameplay+planting+harvesting+crops
- https://www.youtube.com/results?search_query=Story+of+Seasons+gameplay+planting+harvesting

見るポイント:

- 農作業がゲームの主軸になる。
- 戦闘やスコア競争なしでも成立する。
- ループが分かりやすい。

001で盗む核:

```text
作業ループそのものが楽しい。
```

001で削るもの:

- 生活シム全体
- 会話
- 所持金/店
- 日付
- 牧場拡張

Mebuki 1-hour mini:

```text
畑3マスだけ。
1マスずつ育つ。
収穫数だけ表示。
```

## Match 3 / Three-in-a-row

### 1. Candy Crush Saga

YouTube:
- https://www.youtube.com/results?search_query=Candy+Crush+Saga+gameplay+level+1

見るポイント:

- 同じ色/形を3つ揃える。
- 消える。
- 上から補充される。
- スコアや目標が出る。
- 操作が直感的。

001で盗む核:

```text
3つ揃うと消える。
消えると点が入る。
```

001で削るもの:

- 連鎖
- 特殊キャンディ
- ステージ目標
- 手数制限
- アニメーション演出
- マップ

Mebuki 1-hour mini:

```text
5x5の盤面。
同じアイコンが3つ並んだら消える。
スコアが増える。
落下と連鎖は後でよい。
```

### 2. Bejeweled

YouTube:
- https://www.youtube.com/results?search_query=Bejeweled+gameplay+match+3

見るポイント:

- Match 3 の古典。
- 宝石を入れ替える。
- 3つ並べると消える。
- 見た目が分かりやすい。

001で盗む核:

```text
隣同士を入れ替えて、3つ揃える。
```

001で削るもの:

- 制限時間
- 連鎖演出
- 特殊ピース
- 高度なスコア計算

Mebuki 1-hour mini:

```text
クリックした2つの隣接アイコンを入れ替える。
横か縦に3つ並んだら消す。
```

### 3. Gardenscapes / Homescapes

YouTube:
- https://www.youtube.com/results?search_query=Gardenscapes+gameplay+match+3+garden
- https://www.youtube.com/results?search_query=Homescapes+gameplay+match+3

見るポイント:

- Match 3 と、庭/家の修復メタゲームを組み合わせている。
- パズル結果が、生活空間の変化につながる。
- 女性比率が高い Match 3 と、装飾/生活文脈を組み合わせる参考になる。

001で盗む核:

```text
パズルで得た点が、見た目の変化につながる。
```

001で削るもの:

- ストーリー
- キャラクター会話
- 家/庭の全体設計
- 広告的演出
- 多数ステージ

Mebuki 1-hour mini:

```text
3つ揃えると花ポイントが増える。
花ポイントが3になると、鉢に花が咲く。
```

## Beginner Implementation Reality

### Farm mini is safer

`小さな畑アプリ` は、001の実装題材として安全。

理由:

- 状態が少ない。
- クリックで変化する。
- アニメーションなしでも成立する。
- 保存なしでも成立する。
- 見た目を柔らかくできる。

### Match 3 is data-backed but harder

`3つ揃えるパズル` は、女性比率の高いジャンルという根拠がある。
ただし、初心者1時間では実装が重くなりやすい。

難所:

- 隣接判定
- 入れ替え
- 3つ以上の検出
- 消去
- 補充
- 連鎖

001でやるなら、以下まで削る。

```text
5x5固定。
4種類のアイコン。
クリックした2つを入れ替える。
3つ並んだら消えて点が入る。
落下補充は後回し。
```

## Current Recommendation

001の非ギーク向け実演としては、

```text
第一候補: 小さな畑/収穫ミニアプリ
第二候補: 好きなキャラでSnaky
第三候補: スイカゲーム系ミニ版
データ根拠は強いが実装注意: 3つ揃えるパズル
```

理由:

- 畑/収穫は Family/Farm Sim に近く、実装も簡単。
- Match 3 はデータ根拠は強いが、初回実装で沼る。
- Snaky はデータ根拠は弱いが、安定して動かせる。
- スイカ系はフックは強いが、物理が重い。


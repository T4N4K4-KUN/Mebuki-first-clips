# MEBUKI_TOPIC_SHORTLIST_EVIDENCE

001の題材を、ゲーム縛りではなく「自分用の小さいものが動く」という観点で選ぶためのショートリスト。

checked_date: 2026-06-15

## Fact Table

この表だけが「事実」。
この下の候補評価は、この表からの推論を含む。

| ID | Fact | Source | What it supports | What it does not prove |
|---|---|---|---|---|
| F1 | Quantic Foundry は 270,000+ worldwide gamers の Gamer Motivation Profile データを使って、ジャンル別の女性比率を分析した。 | https://quanticfoundry.com/2017/01/19/female-gamers-by-genre/ | ジャンル別に女性比率を見る根拠。 | 日本の初心者女性がAIで何を作りたいかは分からない。 |
| F2 | Quantic Foundry の分析では、Match 3 の 69% は「Match 3 game を挙げたゲーマーのうち女性が69%」という意味。 | https://quanticfoundry.com/2017/01/19/female-gamers-by-genre/ | Match 3 は女性比率が高い既存ゲームジャンル。 | 「女性の69%がMatch 3を遊ぶ」ではない。 |
| F3 | Quantic Foundry は、Match 3 と Family/Farm Sim を、女性比率が最も高い2ジャンルとしている。次点ジャンルより27ポイント高い。 | https://quanticfoundry.com/2017/01/19/female-gamers-by-genre/ | Farm/harvest系、Match 3系を候補に入れる根拠。 | 001で必ず刺さるとは言えない。 |
| F4 | 同分析では、Sports は女性2%、Tactical Shooter は4.3%、First-Person Shooter は7.2%。 | https://quanticfoundry.com/2017/01/19/female-gamers-by-genre/ | 競技/射撃系だけに寄せると狭くなる根拠。 | インベーダー風が全く刺さらないとは言えない。 |
| F5 | DataReportal Digital 2025 Japan は、日本のInstagram広告リーチを 57.5 million users、成人広告オーディエンスの 57.8% が女性としている。 | https://datareportal.com/reports/digital-2025-japan | Instagram/写真/見せ方文脈が女性を含む広い層に届く可能性。 | 写真アプリを作りたいという直接証拠ではない。 |
| F6 | DataReportal Digital 2025 Japan は、日本のTikTok広告リーチを18歳以上 26.9 million users、成人広告オーディエンスの 52.1% が女性としている。 | https://datareportal.com/reports/digital-2025-japan | 動画/短尺/投稿文脈が広い可能性。 | 動画編集アプリを作りたいという直接証拠ではない。 |
| F7 | DataReportal Digital 2025 Japan は、日本のPinterest広告オーディエンスの 62.8% が女性としている。 | https://datareportal.com/reports/digital-2025-japan | 画像・アイデア収集・デザイン参照文脈が女性寄りである根拠。 | 推し色カードメーカーを001で作るべきとは言えない。 |
| F8 | Zero-code LLM app development に関する研究は、LLMベースのアプリビルダーが非プログラマーのソフトウェア開発機会を広げると扱っている。 | https://arxiv.org/abs/2510.19747 / https://arxiv.org/abs/2307.16717 | mebukiをゲーム限定にしない根拠。 | どの題材が最も刺さるかは分からない。 |

## Derived Claims

ここから下は、Fact Table からの推論。

| Claim | Basis | Confidence |
|---|---|---|
| Match 3 / Farm Sim に近い題材は、女性を含む非ギーク層向け候補に入れる価値がある。 | F1, F2, F3 | medium-high |
| インベーダー風だけでは、入口として狭い可能性がある。 | F4 + 返り咲き層向け文脈 | medium |
| SNS/写真/カード系は生活文脈として候補になり得るが、001実演にはデザイン沼リスクが高い。 | F5, F6, F7 + 実例動画観察 | medium |
| ゲーム以外の小さい日常ツールもmebuki候補に入れるべき。 | F8 | medium |
| 001の本命をデータだけで一つに決めることはできない。 | F1-F8の限界 | high |

## What The Data Can Support

### 1. Game genres: Match 3 and Family/Farm Sim have strong female-skew evidence

Quantic Foundry の27万人超ゲーマー調査では、ジャンル別の女性比率に大きな差がある。

Data points:

- Match 3 は、そのジャンルに言及したゲーマーの 69% が女性。
- Match 3 と Family/Farm Sim は、調査対象ジャンルの中で女性比率が最も高い。
- Tactical Shooter や Sports は低い。
- ただし、これは「女性の69%がMatch 3を遊ぶ」という意味ではない。

Source:
- https://quanticfoundry.com/2017/01/19/female-gamers-by-genre/

Implication:

- `インベーダー風` だけに寄せるのは、データ上は狭い。
- 女性を含む非ギーク層へ広げるなら、Match 3 / Farm / Life Sim に近い題材を候補に入れる根拠がある。

### 2. Japan digital behavior: Instagram/TikTok reach women strongly, but this does not prove app-building desire

DataReportal Digital 2025 Japan:

- Instagram: 5750万人に広告リーチ。成人広告オーディエンスの 57.8% が女性。
- TikTok: 18歳以上2690万人に広告リーチ。成人広告オーディエンスの 52.1% が女性。
- YouTube: 7870万人に広告リーチ。

Source:
- https://datareportal.com/reports/digital-2025-japan

Implication:

- 写真、動画、投稿、見せ方は生活文脈として強い。
- ただし「SNSを使う」ことは「SNSアプリを作りたい」ことを意味しない。
- デザイン自由度が高い題材は、初回1時間では危険。

### 3. No-code / LLM app builders lower barriers, but use-case data is broad

Zero-code LLM app development の調査では、LLMベースのアプリビルダーが非プログラマーにソフトウェア作成機会を広げると整理されている。

Source:
- https://arxiv.org/abs/2510.19747
- https://arxiv.org/abs/2307.16717

Implication:

- `ゲーム` に限定する必要はない。
- 自動化、記録、チェックリスト、ルーレット、簡易生成ツールも mebuki の範囲に入る。
- ただし、001は「動いた感」が必要なので、完全な業務自動化より、画面上で変化が見える小物が向く。

## Candidate Evaluation

評価軸:

- Evidence: 既存データ・ヒットジャンルとの距離。
- 1-hour feasibility: AIエージェントで初回に形にしやすいか。
- Visual payoff: 見た瞬間に動いた感があるか。
- Customization: 視聴者が自分ごと化しやすいか。
- Risk: 仕様沼、デザイン沼、実装沼に落ちるか。

| Candidate | Evidence | 1-hour feasibility | Visual payoff | Customization | Risk | Judgment |
|---|---|---:|---:|---:|---|---|
| 1-screen farm / harvest mini app | Family/Farm Sim female-skew evidence | high | medium | high | low-medium | Strong candidate |
| Simple Match 3 | Match 3 female-skew evidence | medium | high | medium | medium | Strong but implementation heavier |
| Suika-like merge mini game | Existing hit, casual puzzle adjacent | medium | high | medium | physics/merge rules can grow | Candidate, not proven by gender data |
| Character Snaky | Snaky Cat / Snake pattern; customizable | high | high | high | low | Good fallback, weaker evidence |
| Meal roulette | Daily-life utility, broad no-code fit | high | medium | high | low | Good non-game candidate |
| Packing checklist / event checklist | Daily-life utility, broad no-code fit | high | low-medium | high | low | Good but less visually exciting |
| Cafe order mini game | Life/cafe theme; no direct data | medium | medium | high | medium | Possible, needs reference examples |
| Photo/card maker | SNS behavior supports context | medium | medium | high | high design precision | Not for 001 unless template-locked |
| 推し色カードメーカー | 推し活 context exists | medium | medium | high | very high design precision | Reject for 001 |
| 猫のおやつキャッチ | Cute motif, weak popularity evidence | high | medium | medium | low | Weak evidence; not a lead |
| インベーダー風 | Returner/geek nostalgia | high | high | medium | low | Good for returner segment only |

## Strongest Mebuki-Fit Candidates

### 1. 1-screen farm / harvest mini app

Why:

- Family/Farm Sim has data support as a female-skew genre.
- It is less intimidating than combat games.
- It can be made very small.
- It can become a tool/game hybrid: water, grow, harvest, count.

Beginner prompt:

```text
小さな畑アプリを作りたい。
画面に3つの鉢を並べる。
鉢をクリックすると水をあげられる。
3回水をあげると芽が花になり、収穫ボタンでスコアが増える。
最初は保存機能なしでよい。
```

001 fit:

- Good for broad audience.
- Gentle visual change.
- Easy to explain.
- Low failure pressure.

Risk:

- 派手さはスイカゲームより弱い。
- 「ゲームが動いた！」感はやや控えめ。

### 2. Simple Match 3

Why:

- Match 3 has the strongest female-skew evidence in the Quantic Foundry data.
- Rules are familiar.
- Visual payoff is clear.

Beginner prompt:

```text
6x6の盤面に、4種類のかわいいアイコンを並べる。
隣同士を入れ替えられる。
同じアイコンが3つ並んだら消えて、上から新しいアイコンが落ちる。
最初はスコアだけでよい。
```

001 fit:

- Strong evidence.
- Clear gameplay.

Risk:

- 実装が意外に重い。
- 消去、落下、補充、連鎖でバグりやすい。
- 001ではAIが詰まる可能性がある。

### 3. Suika-like merge mini game

Why:

- Existing hit.
- Casual puzzle feel.
- Visual payoff is high.
- Theme can be softened or customized.

Beginner prompt:

```text
上から丸いフルーツを落とすミニゲームを作りたい。
同じフルーツがぶつかると、一段大きいフルーツになる。
箱からあふれたらゲームオーバー。
最初はフルーツ3種類だけでよい。
```

001 fit:

- Strong hook.
- Easy to show.

Risk:

- Physics can be hard.
- Full Suika reproduction is too much.
- Must frame as "Suika-like mini version".

### 4. Character Snaky

Why:

- Snake pattern is simple.
- Character and item can be swapped freely.
- Broad personalization: dog, T-Rex, alien, rabbit,推し色ボール.

Beginner prompt:

```text
好きなキャラを動かして、アイテムを集めるゲームを作りたい。
アイテムを取るたびに体が長くなる。
壁や自分にぶつかったらゲームオーバー。
キャラとアイテムはあとで差し替えられるようにしたい。
```

001 fit:

- Reliable.
- Fast.
- Customizable.

Risk:

- Data support is weaker than Match 3 / Farm Sim.
- If Snakeを知らない層には少し古い。

### 5. Meal roulette / daily helper

Why:

- No-code/LLM app builders support non-programmers creating small applications.
- Daily-life helper avoids game-only narrowing.
- Very feasible in one hour.

Beginner prompt:

```text
今日の夕飯を決めるルーレットアプリを作りたい。
候補を追加できる。
ボタンを押すとランダムで1つ選ばれる。
肉・魚・野菜などのタグで絞り込める。
最初は保存機能なしでよい。
```

001 fit:

- Non-game users can relate.
- Easy implementation.

Risk:

- Visual hook is weaker.
- "AIで作るすごさ" はゲームより伝わりにくい。

## Recommended 001 Structure

Game-only is too narrow.
But game is useful as the clearest demo.

Use a "menu of possible first apps" before the actual build:

```text
AIに頼むと、最初の1時間で小さいものが動く。

ゲームでもいい。
生活ツールでもいい。
記録アプリでもいい。

たとえば:
- 小さな畑アプリ
- 3つ揃えるパズル
- スイカゲームみたいなミニ版
- 好きなキャラでSnaky
- 献立ルーレット
```

Then choose one demo:

```text
今日は、動いた感が一番わかりやすいものを1つ作る。
```

## Current Recommendation

Data-backed candidate pool:

```text
1. 1-screen farm / harvest mini app
2. Simple Match 3
```

Practical demo candidates:

```text
1. Character Snaky
2. Suika-like mini game
3. Meal roulette
```

Best balance for 001:

```text
冒頭で5案を見せる。
実演は Character Snaky か 1-screen farm。
```

理由:

- Match 3 は根拠が強いが実装が重い。
- Farm は根拠があり、やさしいが少し地味。
- Snaky は根拠は弱いが、1時間実演として安定する。
- Suika-like は強いフックだが、物理実装が沼る可能性がある。
- Meal roulette は非ゲーム層に届くが、映像の引きは弱い。

## What Must Not Be Claimed

以下は現時点で言わない。

```text
女性にはスイカゲームが刺さる。
女性は推し色カードメーカーを作りたい。
猫なら女性に受ける。
ゲームなら広く初心者に刺さる。
```

言えるのはここまで。

```text
女性比率が高い既存ゲームジャンルとして Match 3 と Family/Farm Sim がある。
SNS/写真/動画利用は女性比率が高いが、制作題材としては未検証。
AI/no-codeにより非プログラマーが小さいアプリを作る流れはある。
mebuki 001では、ゲームだけでなく、小さい日常ツールも見せるべき。
```

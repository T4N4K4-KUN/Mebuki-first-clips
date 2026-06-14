# REFERENCE_VIDEO_CANDIDATES_001

001 `最初の1時間で、ゲームは動く` のための参考動画候補。

目的は、NotebookLMへ入れる前に動画を選び抜くこと。
対象ユーザーは、初心者・返り咲き層。
最重要条件は「見た人にとって有益で、興味が湧き、試す理由が生まれること」。

checked_date: 2026-06-14

## Use First

001で使う本命候補。

重要:
- `Mini Galaga` と `Replit Agent` は既に文字起こし・日本語訳登録済み。
- NotebookLMへ新規投入が必要なのは `Scratch Jumping Game` と `Scratch Catch Game` の2本だけ。
- 今後は候補を出す前に `local/transcripts/README.md` と `local/transcripts/registered-lines-ja.md` の登録済みソースを照合する。

| Priority | Title | URL | Channel | Official | Length | Processing status | Why use |
|---:|---|---|---|---|---:|---|---|
| 1 | How to Make a Jumping Game in Scratch | https://youtu.be/1jHvXakt1qw | Scratch Team | yes | 304s | newly processed | 公式。冒頭で「make a jumping game」と成果物を約束し、5ステップに分解する。初心者に有益。 |
| 2 | How to Make a Catch Game in Scratch | https://youtu.be/7NN5v2wSL4U | Scratch Team | yes | 394s | newly processed | 公式。落ちてくる物をキャッチして得点するゲーム。対象物や背景を選べるため、改造導線がある。 |
| 3 | MakeCode Arcade Game of the Week: Mini Galaga | https://youtu.be/o8jrZz3L9_I | Adafruit Industries | no | 119s | already registered; do not reprocess | ユーザー投稿作品を紹介。既存ゲームから着想を得て始める、動いた後にedit codeで中を見る、改造する導線がある。 |
| 4 | What's the Replit Agent? Find out in 60 Seconds | https://youtu.be/aWBiZc5XKJM | Replit | yes | 73s | already registered; do not reprocess | 公式。`idea -> software` と `pair programmer, not code generation tool` の位置づけだけ使う。サービス売り込み色があるため限定採用。 |

## Evidence

### 1. Scratch Team — Jumping Game

Source status:

- Official Scratch Team tutorial.
- User-provided reconstructed script added at `local/transcripts/scratch-jumping-reconstructed.md`.
- Exact subtitle file exists at `local/candidate_subtitles/scratch-jumping.en.vtt`.

| Time | Evidence | Why it matters |
|---:|---|---|
| 0:04 | "show you how to make a jumping game in Scratch" | 冒頭で成果物が明確。 |
| 0:06 | "By the end of this tutorial, you'll be able to make a game like this one" | 視聴後に何ができるかを先に約束している。 |
| 0:09 | "a character jumping over moving obstacles" | ゲームの面白さが1文で分かる。 |
| 0:12 | "We'll do this in five steps" | できることを小さな手順に分ける。 |
| 0:13-0:20 | jump / moving obstacle / stop game / more obstacles / score | 成果物を機能単位で示す。 |

001に移植できる構造:

- 冒頭で「何を作れるか」を明言する。
- まず動くゲームの完成像を示す。
- 機能を小さく分解する。
- 難しい概念ではなく、動作で伝える。
- ベースが動いた後に、障害物追加・スコア・背景変更などの拡張を提案する。

### 2. Scratch Team — Catch Game

Source status:

- Official Scratch Team tutorial.
- User-provided reconstructed script added at `local/transcripts/scratch-catch-reconstructed.md`.
- Exact subtitle file exists at `local/candidate_subtitles/scratch-catch.en.vtt`.

| Time | Evidence | Why it matters |
|---:|---|---|
| 0:05 | "how to make a catch game in Scratch" | 冒頭で成果物が明確。 |
| 0:07 | "objects are falling from the sky and you catch them to score points" | ゲームの目的が一瞬で分かる。 |
| 0:12 | "It could be any object" | 改造・自分ごと化の余地がある。 |
| 0:14 | "any character or object that's catching it" | 初心者でも自分の作品にできる。 |
| 0:16-0:25 | move catcher / object to top / fall down / catch it / keep score | 小さい機能に分解している。 |

001に移植できる構造:

- 目的が単純なゲームを選ぶ。
- ユーザーが素材や見た目を変えられる余地を残す。
- まずゲームのルールを一文で伝える。
- 作る内容を5つ程度の動作へ分ける。
- 同じ基本ルールを、海のゴミ拾い、ペットのおやつキャッチなど別テーマへ変えられる。

### 3. Adafruit — Mini Galaga

Source status:

- User-provided reconstructed script.
- Not verified as verbatim transcript.
- Use as structure reference only.

Extracted structure:

- ユーザー投稿作品を紹介する。
- 既存ゲームから着想を得た作品を肯定する。
- シンプルでも遊んで楽しいと見せる。
- 動いた後に `edit code` で中を見る。
- lives / speed / projectiles を変える改造導線がある。

001に移植できる構造:

- 将来、mebukiユーザー投稿作品を紹介する型。
- 「インベーダー風」は自然な着想元として扱える。
- 動いた後に中を見る、1か所いじる、再実行する導線。

### 4. Replit Agent official

| Time | Evidence | Why it matters |
|---:|---|---|
| 0:05 | "takes you from idea to software fast" | AIエージェント時代の入口変化。 |
| 0:15 | "autonomous AI system" | 人間が全部組み立てる前提ではない。 |
| 0:15 | create database / connect front end and back end / deploy | syntaxだけでなく周辺作業まで対象。返り咲き層の障壁に対応。 |
| 0:35 | "more like a pair programmer than a code generation tool" | AIをコード生成機ではなく相棒として見せられる。 |

001に移植できる構造:

- 「AIがコードを書く」ではなく「横で進める相棒」。
- 返り咲き層が重く感じる環境・接続・共有を、AIが横で進める。
- ただし001ではサービス説明に寄せない。

## Screen Next

まだNotebookLMに入れる前の追加調査候補。
使う場合は、冒頭・成果・セリフ・対象ユーザーへの有益性を秒数付きで確認する。

| Title | URL | Channel | Length | Why screen |
|---|---|---|---:|---|
| How I learned Unity without following tutorials | https://youtu.be/vFjXKOXdgGo | Game Maker's Toolkit | 1091s | tutorial依存から抜ける、基礎->反復->実験の学習構造がありそう。返り咲き層に有益な可能性。 |
| how I learned to code personal projects | https://youtu.be/moQ625SEwmY | joowee | 336s | tutorial hellから個人プロジェクトへ移る方法。001より005向きかもしれないが、有益性が高そう。 |
| Coming Back To Programming After A Break | https://youtu.be/1L6oncFUu10 | Traversy Media | 554s | 返り咲き層そのもの。ただしゲーム・成果物先出しではないため001向きか要確認。 |
| Pro gamer plays student made games | https://youtu.be/Uy5oyUNcwz0 | Hackingtons Code School | 223s | ユーザー/学生作品を紹介する型。将来のmebuki投稿紹介に使える可能性。 |

## Reject For 001

| Source | Reason |
|---|---|
| Bolt long tutorials | サービス/機能デモ色が強い。001に使うのは「軽い自然言語プロンプト -> すぐ成果」だけ。 |
| Bolt Discuss | plan/debug/search/token節約は004/006向き。001には重い。 |
| Lovable detailed tutorial | Webサイト編集、DB連携、売り込みが中心。001では薄い。005/006向き。 |
| Supabase/API key/database videos | 001のツカミには重すぎる。 |

## Current Decision

NotebookLMに次に入れるなら、まずこの4つ。

1. Scratch Team Jumping Game
2. Scratch Team Catch Game
3. Adafruit Mini Galaga
4. Replit Agent official 60 sec

目的:

- Scratch公式2本で「初心者に有益なゲーム導入」の型を取る。
- Adafruitで「ユーザー作品・既存ゲーム着想・中を見て改造」の型を取る。
- Replitで「AIエージェント時代の入口変化」を最小限だけ取る。

この4本で、001のミクスチャーは以下に絞る。

```text
ゲーム完成像を先に見せる
↓
小さい動作へ分ける
↓
インベーダー風の着想を肯定する
↓
AIはコード生成機ではなく横で進める相棒
↓
動いた後に中を見て1か所いじる
```

# REFERENCE_VIDEO_CANDIDATES_SPEC_BRIEF

AI駆動開発時代の001/002向け追加候補。

論点:
- Scratch系は「初心者のハートを掴む」「ゲームが動く快感」の参考になる。
- ただしAIエージェント駆動では、細かいX/Y操作や言語文法よりも、依頼・仕様・受け入れ条件・MVP設計が重要になる。
- 参照すべき対象は、開発者チュートリアルだけではなく、非エンジニアが開発者/ベンダー/AIエージェントへ何をどう伝えるかを教える動画。

checked_date: 2026-06-14

## Search Result

「プチゲームを開発ベンダーに依頼してみよう」そのものに一致する初心者向け動画は、今回のYouTube検索範囲では未確認。

近い領域として、以下の4系統が見つかった。

1. 非エンジニア創業者が開発者に依頼する
2. PRDを書く
3. ユーザーストーリーと受け入れ条件を書く
4. MVPを設計する

## Candidate Set

### A. Direct Fit: Non-Technical Founder / Developer Brief

開発ベンダーへ投げる側に近い。001より002/003で使いやすい可能性が高い。

| Priority | Title | URL | Channel | Length | Why screen |
|---:|---|---|---|---:|---|
| 1 | How to Hire App Developer as a Non Technical Founder | https://youtu.be/eCbQz7XKIv8 | Startup MVP Series | 158s | 非エンジニアが開発者を雇う入口。短く、初心者向けの可能性が高い。 |
| 2 | how to approach a software developer with an app idea (from a software dev) | https://youtu.be/lLAkuOfBT_w | London Tech Studio | 556s | 「アプリ案を開発者へどう伝えるか」に直結するタイトル。 |
| 3 | The Non-Technical Founder's Introduction To Working With Outsourced Developers | https://youtu.be/sb-cpKPmspY | Tech For Non-Techies | 2216s | 外注開発者との働き方。長いので、NotebookLM投入前に章立て確認が必要。 |
| 4 | How to Hire App Developer as a Non-Technical Founder - 2025 | https://youtu.be/wZjO3L80N-E | Adrian Ching | 496s | 2025版。AI時代の前提が含まれる可能性あり。 |

### B. AI-Era Fit: PRD / Specification as Prompt

AI駆動開発に最も近い。コードではなく、AI/開発者へ渡す仕様文書が主役。

| Priority | Title | URL | Channel | Length | Why screen |
|---:|---|---|---|---:|---|
| 1 | Build Better Apps with AI Using This One Simple Document (PRD Guide) | https://youtu.be/MZjW7mlRgdw | Jordan Urbs | 1261s | AIでアプリを作るためのPRD。今回の問題意識に最も近い候補。 |
| 2 | How to Write a Product Requirements Document - Create PRD | https://youtu.be/JJzODsXsCt0 | HelloPM | 513s | 初心者向けPRD作成。アプリ企画を仕様に落とす型が取れそう。 |
| 3 | How to write a great PRD | https://youtu.be/yYtLHiB71KM | ChatPRD | 368s | PRD専門サービス色はあるが、短く要点抽出向き。 |
| 4 | Webinar: How to Write Great Product Requirements | https://youtu.be/ydHLajgdT4c | Product School | 1712s | Product School。信頼度は高いが長い。001では重い。 |

### C. Communication Fit: User Stories / Acceptance Criteria

AIエージェントや開発者に「何ができたらOKか」を伝えるための型。

| Priority | Title | URL | Channel | Length | Why screen |
|---:|---|---|---|---:|---|
| 1 | How to write good User Stories in Agile | https://youtu.be/7hoGqhb6qAs | The Agile Shop | 227s | 短い。初心者に「誰が、何を、なぜ」を伝える型として使いやすい。 |
| 2 | Beginner's Guide to Writing User Stories (Real Examples) | https://youtu.be/C_S3ygjANg4 | IT Project Managers | 705s | 実例つき。やや長いが、依頼文の型を取れそう。 |
| 3 | What is Acceptance Criteria? Definition, How To, and Best Practices | https://youtu.be/zZV6FeJ3BtE | ProductPlan | 216s | 「できた判定」を教える候補。AI駆動開発では重要。 |
| 4 | User Stories and Acceptance Criteria EXAMPLE | https://youtu.be/q26147zlcMU | The Business Analysis Doctor | 716s | user story と acceptance criteria をセットで扱う。 |

### D. Scope Fit: MVP

最初の1時間で作るゲームを「全部入り」ではなく「最小の遊べるもの」にする考え方。

| Priority | Title | URL | Channel | Length | Why screen |
|---:|---|---|---|---:|---|
| 1 | How To Create An MVP (Minimum Viable Product) - STEP BY STEP | https://youtu.be/YwEEV0wHnaA | Rob Walling | 620s | MVPを段階的に説明。サービス企画初心者向けに使える可能性。 |
| 2 | Michael Seibel - How to Plan an MVP | https://youtu.be/1hHMwLxN6EM | Y Combinator | 830s | YC。質は期待できるが、001には硬い可能性。 |
| 3 | The RIGHT WAY to Build an App MVP | https://youtu.be/jpQJ8aOThNY | ForrestKnight | 647s | アプリMVPの考え方。開発初心者より企画初心者向き。 |

## First Screening Priority

NotebookLMに入れるなら、次はこの4本から始める。

1. https://youtu.be/MZjW7mlRgdw
   - AI時代のPRD。今回の主張に最も近い。
   - processed: `local/transcripts/prd-guide-ai-apps-jordan-urbs.md`
   - Japanese translation: `local/transcripts/registered-lines-ja.md`
2. https://youtu.be/lLAkuOfBT_w
   - 開発者へアプリ案をどう伝えるか。
   - processed: `local/transcripts/approach-software-developer-app-idea.md`
   - Japanese translation: `local/transcripts/registered-lines-ja.md`
3. https://youtu.be/7hoGqhb6qAs
   - user storyの短い型。
   - processed: `local/transcripts/user-stories-agile-the-agile-shop.md`
   - Japanese translation: `local/transcripts/registered-lines-ja.md`
4. https://youtu.be/zZV6FeJ3BtE
   - acceptance criteria、つまり「何ができたら完成か」。
   - processed: `local/transcripts/acceptance-criteria-productplan.md`
   - Japanese translation: `local/transcripts/registered-lines-ja.md`

## 001への使い方

001で直接「PRD」「仕様設計」と言うと逃げる人が出る。
ただし、裏側の構造としては使う。

001の表現へ落とすなら:

```text
作りたいゲームを、AIに伝わる言葉にする。

1. 何のゲームか
2. 誰が操作するか
3. 何が落ちてくる/迫ってくるか
4. 何をしたら得点か
5. 何をしたらゲームオーバーか
6. 最初の1時間では何を作らないか
7. できた判定は何か
```

これなら、PRDやプロジェクトマネジメントという言葉を出さずに、実質的に仕様設計の入口へ入れる。

## Processed Notes

### Build Better Apps with AI Using This One Simple Document

Source: https://youtu.be/MZjW7mlRgdw

取れる核:

- AI駆動開発では、ノリで作るだけだと途中で破綻し、やり直しが発生する。
- AIに渡すドキュメントとしてPRDを作る。
- PRDはBolt、Cursor、Claude Codeのような複数ツールに渡せる。
- goals / tech stack / architecture / core features / database schema がPRDの構成要素として出てくる。
- database schema は single source of truth として扱われる。
- AIが確認質問をしながらPRD作成を助ける流れがある。
- 同じPRDを複数AIエージェントに渡して比較できる。
- デプロイで失敗しても、agenticなAIはフォルダ構成修正などを自分で進める場合がある。

001への翻訳:

- 「仕様設計」ではなく「AIに伝わるメモ」と言う。
- 「PRD」ではなく「作ってほしいゲームの注文票」と言う。
- 「single source of truth」ではなく「AIが迷わないための1枚」と言う。
- 最初の1時間では、技術スタックやDBスキーマは出さない。
- 代わりに、ゲームの目的、操作、敵/障害物、得点、ゲームオーバー、完成判定だけに絞る。

### how to approach a software developer with an app idea

Source: https://youtu.be/lLAkuOfBT_w

取れる核:

- 開発者へ最初に求めるのは参加ではなく意見。
- 技術的に可能か、どれくらい時間がかかるかを現実確認する。
- コードを書く前に、まずアイデア検証をする。
- LPやノーコードで需要を確認してから開発者へ戻る。
- 開発者のスキルや実績を確認する。
- 小さいチームでは、フロントエンドとバックエンドを一人で扱える力が重要。
- MVPでは、クールな追加機能を棚に置き、アプリが機能する最低限を決める。
- 追加機能は、顧客フィードバックに基づいて後から足す。

001への翻訳:

- 「AIにいきなり全部作れ」ではなく「まずこのゲーム案でいけるか聞く」。
- 「最初の1時間で作るもの」と「今は作らないもの」を分ける。
- かっこいい追加機能より、まず遊べる最小単位を決める。
- 人間の開発者に相談する型を、AIエージェントへの頼み方に転用する。

### What is Acceptance Criteria?

Source: https://youtu.be/zZV6FeJ3BtE

取れる核:

- 受け入れ基準は、ユーザー・顧客・システムが受け入れるために満たすべき要件。
- エンドユーザー視点の pass/fail 文で、機能や振る舞いの成功を定義する。
- 「正しいものを作っているか」「正しく作ったか」を確認するために使う。
- 良い受け入れ基準は、テスト可能、明確、簡潔、理解しやすい、ユーザー視点。
- 期待値管理、スコープ定義、曖昧さ削減、QA基準、スコープクリープ防止に効く。
- 書式は Given/When/Then または Verification List。
- 重い形式が合わない場合は、pass/fail の箇条書きでよい。

001への翻訳:

- 「受け入れ基準」ではなく「できた判定」と言う。
- AIに作らせる前に、「何が起きたら完成か」を3つだけ書く。
- 例:
  - 左右キーで自機が動く。
  - 敵に弾が当たるとスコアが増える。
  - 敵に当たるとゲームオーバーになる。
- 001では Given/When/Then という名前は出さず、必要なら裏側の設計だけ使う。

### How to write good User Stories in Agile

Source: https://youtu.be/7hoGqhb6qAs

取れる核:

- プロダクトの機能や要件を、ユーザーストーリーへ分解する。
- ユーザーストーリーは、ユーザー視点で望ましい機能を説明する。
- 各ストーリーは小さな機能のまとまりで、それ単体で価値を届ける。
- 誰にでも分かるようにシンプルに書き、解決方法や重い技術情報を含めない。
- 基本形は「誰が」「何をしたい」「なぜ」を答える。
- 受け入れ基準は、そのストーリーがいつ完了したかを知らせる。
- Given/When/Then は、前提、操作、観察できる結果に分ける。
- INVEST は、independent / negotiable / valuable / estimatable / small / testable の確認に使う。

001への翻訳:

- 「ユーザーストーリー」と言わず、「遊ぶ人の一文」と言う。
- 「プレイヤーとして、左右に動いて弾を撃ちたい。敵を倒してスコアを増やすため。」のようにする。
- 解決方法や技術情報は書かない。
- AIに渡す注文票の中で、まず「誰が、何をしたい、なぜ」を1文で決める。
- その後に「できた判定」を3つ置く。

## Current Judgment

新しい方向性は正しい。

Scratch系から盗むのは「初心者が逃げない見せ方」。
PRD/user story/acceptance criteria/MVP系から盗むのは「AIや開発者へ伝わる依頼の型」。

001はこのミックスがよい。

```text
ゲームが動く快感
×
AIに伝わる依頼文
×
最小の完成条件
```

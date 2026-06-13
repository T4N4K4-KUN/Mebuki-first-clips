# REFERENCE_TARGETS — inspiration-map source list

このファイルは、INSPIRATION MAPで「何を参考にするか」を実際の参考先に接続するためのリスト。

ここにあるリンクは、素材として使うためではない。見る対象は、構造、心理トリガー、視点反転、テンポ、学習導線だけ。映像、音声、字幕、台本、図解、キャラ、サムネ、固有の言い回しは使わない。

checked_date: 2026-06-14

## Use rule

1. 1本のclipにつき、下の参考先から2〜3件だけ見る。
2. 見たら `docs/MATERIALS_LEDGER.md` の `Reference study log` にIDを残す。
3. 台本候補には「参考にした型」を必ず書く。
4. 1つの動画や記事の順番をなぞらない。
5. 複数の参考先に共通する型だけを抽出し、mebukiの視聴者と言葉に変換する。

## Primary source targets

| ID | Source | URL | Class | Inspiration to take | Do not copy | Clips |
|---|---|---|---|---|---|---|
| REF-REPLIT-AGENT | Replit Agent overview | https://docs.replit.com/references/agent/overview | B | 普通の言葉でアイデアを伝えると、Agentが作り、確認し、直し、公開まで進める導線 | 画面、UI、文言、プロンプト例、ロゴ、サービス説明の言い回し | 001, 004, 006 |
| REF-BOLT-HOME | Bolt.new | https://bolt.new/ | B | 「何を作る？」から始める。エラー説明ではなく、作りたいものと動く結果を先に置く | UI、コピー、テンプレ、ロゴ、事例の見た目 | 001, 002, 005 |
| REF-LOVABLE-WELCOME | Lovable Docs | https://docs.lovable.dev/introduction/welcome | B | 自然言語からworking applicationへ進む。ゲーム、クイズ、シミュレーションも正当な入口にする | ドキュメント文、画面、事例、機能説明の順番 | 001, 005 |
| REF-GITHUB-SPARK | GitHub Spark | https://githubnext.com/projects/github-spark/ | B | Dream it -> see it -> ship it の流れ。自然言語、プレビュー、履歴、共有で「作る」を身近にする | GitHubの表現、画面、サンプルアプリ、コピー | 001, 005, 006 |
| REF-MAKECODE-ARCADE | Microsoft MakeCode Arcade | https://arcade.makecode.com/ | B | 初手からゲーム。小さく動く画面で「作れた」を先に作る | ゲーム名、画面、キャラ、チュートリアル構成、ブロック配置 | 001 |
| REF-HOUR-OF-AI | Hour of AI | https://hourofai.org/ | B | AIを使う側から作る側へ。短時間、ハンズオン、楽しい題材で入口を作る | カリキュラム文、教材画面、授業構成、固有表現 | 003 |
| REF-CLAUDE-CODE | Claude Code overview | https://code.claude.com/docs/en/overview | B | repoを読む、編集する、コマンド実行、複数ファイル作業をAIに任せる導線 | ドキュメント文、コマンド例、画面、機能説明の順番 | 004, 006 |
| REF-CLAUDE-CODE-WORKFLOWS | Claude Code common workflows | https://code.claude.com/docs/en/common-workflows | B | overview、plan before editing、PR、tests、docsなどの作業型 | コマンド例、プロンプト例、ワークフロー文面 | 004, 006 |
| REF-OPENAI-CODEX | OpenAI Codex | https://developers.openai.com/codex | B | multi-agent、cloud tasks、PR、review、background workの作業観 | UI、製品コピー、プロンプト例、画面 | 004, 006 |
| REF-ODIN | The Odin Project | https://www.theodinproject.com/ | B | project-based、portfolio、roadmap、community、自走 | カリキュラム文、課題文、ロゴ、画面 | 002, 003, 005 |
| REF-MDN-LEARN | MDN Learn web development | https://developer.mozilla.org/en-US/docs/Learn_web_development | B | HTML/CSS/JSを読める・直せる段階へ進める導線 | 記事本文、図解、コード例、ページ構成 | 005 |
| REF-EXERCISM | Exercism | https://exercism.org/ | B | 小課題、反復、automated analysis、メンタリングの筋トレ型 | 課題文、解答、UI、ロゴ、メンタリング文 | 002, 003 |
| REF-MISSING-SEMESTER | MIT Missing Semester | https://missing.csail.mit.edu/ | B | shell、editor、git、debuggingなど道具のセンス | 講義文、動画、演習、スライド、コード例 | 006 |
| REF-CS50-X | CS50x official course | https://cs50.harvard.edu/x/ | B | Phase 3以降で、正しさ・設計・スタイル・学び直しの軸にする | 講義映像、台詞、スライド、課題名、先生の語り口 | later, 004, 006 |
| REF-CS50-W0 | CS50x Week 0 | https://cs50.harvard.edu/x/weeks/0/ | B | Phase 3以降で、参加感と学び直しの入口にする | Scratch教材、講義構成、字幕、デモ内容 | later, 003 |
| REF-CS50-W1 | CS50x Week 1 | https://cs50.harvard.edu/x/weeks/1/ | B | Phase 3以降で、低レイヤーやCLIの怖さを学びに変える | Cの説明、コード例、問題セット | later |
| REF-FCC-LEARN | freeCodeCamp Learn | https://www.freecodecamp.org/learn | B | 小さい到達点、手を動かす順番、プロジェクト型の足場 | 課題文、記事本文、コード例、認定文面 | 002, 005, 006 |
| REF-FCC-YT | freeCodeCamp YouTube channel | https://www.youtube.com/@freecodecamp | B | 長い学習を小さな章に切る、初心者が自走できる見せ方 | 動画字幕、講師の言い回し、サムネ構成 | 005 |
| REF-KHAN-CS | Khan Academy Computer Programming | https://www.khanacademy.org/computing/computer-programming | B | 前提知識がない人を置いていかない、ここまででOKを明確にする | 画面、図解、説明文、ホワイトボード風演出 | 002, 003, 005, 006 |
| REF-TED-ED-LESSONS | TED-Ed lessons | https://ed.ted.com/lessons | C/B | 問いから始める、短く視点を反転する、1本1テーマ | アニメーション、ナレーション文、タイトル、図解、問いの言い回し | 001, 003, 004, 005 |
| REF-TED-ED-YT | TED-Ed YouTube channel | https://www.youtube.com/@TEDEd | C/B | 冒頭の問い、物語の圧縮、最後の反転 | 映像、字幕、台本、図、ナレーション | 001, 003, 004, 005 |
| REF-CRASHCOURSE-YT | Crash Course YouTube channel | https://www.youtube.com/@crashcourse | C/B | 冒頭3秒の停止力、画面切替のテンポ、章立て感 | ジョーク、キャラ、編集、BGM、字幕、台本 | all |
| REF-CRASHCOURSE-CS-SEARCH | Crash Course Computer Science search | https://www.youtube.com/results?search_query=Crash+Course+Computer+Science | C/B | コンピュータサイエンスを速いテンポで区切る編集 | 個別動画の順番、図解、画面、台詞 | all |

## Short-form pattern targets

具体動画を固定しすぎるとコピーに寄るため、short-form系は検索URLから複数本を見て、共通する型だけを抜く。

| ID | Source | URL | Class | Inspiration to take | Do not copy | Clips |
|---|---|---|---|---|---|---|
| REF-FITNESS-SHORTS | 筋トレ系ショート検索 | https://www.youtube.com/results?search_query=fitness+shorts+one+rep+consistency | B | 1回でOK、量を捨てる、実施を勝ちにする | 筋トレ映像、煽り、BGM、ビフォーアフター | 002, 006 |
| REF-LANGUAGE-SHORTS | 英語学習系ショート検索 | https://www.youtube.com/results?search_query=english+learning+shorts+one+phrase+a+day | B | 1日1フレーズ、小さい反復、とりあえず使う | フレーズ教材、カードUI、音声演出 | 002, 005 |
| REF-MEDITATION-SHORTS | 瞑想・メンタル系ショート検索 | https://www.youtube.com/results?search_query=meditation+shorts+return+to+breath+self+compassion | B | 逸れても戻る、責めずに現在地へ戻す | 癒し口調、スピリチュアル表現、抽象自己肯定 | 003, 006 |

## Clip-level watch sets

### 001 — 最初の1時間で、ゲームは動く

- REF-REPLIT-AGENT
- REF-BOLT-HOME
- REF-LOVABLE-WELCOME
- REF-GITHUB-SPARK
- REF-MAKECODE-ARCADE

Inspiration: 仕様やエラー説明で始めない。普通の言葉で「何を作る？」から入り、最初の1時間で動くゲームを見せる。作れるかも、ではなく、作れる。

### 002 — 今日は5分だけ触れば勝ち

- REF-BOLT-HOME
- REF-EXERCISM
- REF-ODIN
- REF-FCC-LEARN
- REF-KHAN-CS
- REF-FITNESS-SHORTS
- REF-LANGUAGE-SHORTS

Inspiration: 量ではなく接触を勝ちにする。5分、1行、1メモの小ささまで落とす。

### 003 — 昔やめた人は、弱い人じゃない

- REF-EXERCISM
- REF-ODIN
- REF-HOUR-OF-AI
- REF-KHAN-CS
- REF-TED-ED-LESSONS
- REF-MEDITATION-SHORTS

Inspiration: 過去の中断を弱さではなく地図に変える。恥を下げ、戻る動作へつなげる。

### 004 — AIに聞いていい。検索していい。

- REF-CLAUDE-CODE
- REF-CLAUDE-CODE-WORKFLOWS
- REF-OPENAI-CODEX
- REF-REPLIT-AGENT
- REF-FCC-LEARN
- REF-TED-ED-LESSONS

Inspiration: 自力主義を崩す。問いを立て、答えを検証し、次の1手に分解する。

### 005 — 理解より、まず動くものを作る

- REF-LOVABLE-WELCOME
- REF-GITHUB-SPARK
- REF-ODIN
- REF-MDN-LEARN
- REF-FCC-LEARN
- REF-FCC-YT
- REF-KHAN-CS
- REF-LANGUAGE-SHORTS

Inspiration: project-first、ここまででOK、文法前に1フレーズ使う。

### 006 — ログを残せる人は、戻ってこられる

- REF-CLAUDE-CODE
- REF-OPENAI-CODEX
- REF-REPLIT-AGENT
- REF-GITHUB-SPARK
- REF-MISSING-SEMESTER
- REF-CS50-X
- REF-FCC-LEARN
- REF-KHAN-CS
- REF-FITNESS-SHORTS
- REF-MEDITATION-SHORTS

Inspiration: 継続は毎日やる才能ではなく、戻れる導線を残すこと。

## Minimum reference note format

```md
Reference ID:
URL:
Clip:
What inspired this:
What I must not copy:
How it becomes mebuki:
```

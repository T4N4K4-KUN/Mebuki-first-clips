# PHASED_REFERENCE_MAP

外部意見を取り入れた、mebuki v0以降の参考先整理。
ここでいう「参考にする」は、素材・文言・画面を使うことではなく、構造、導線、心理トリガーを取り入れること。

## Phase Map

| Phase | Role | Reference | What to take | Mebuki use |
|---:|---|---|---|---|
| 0 | ツカミ | Replit Agent | 普通の言葉で言うと、Agentが作る・直す・動かす | 001。最初の1時間でゲームが動く。仕様ではなく、作れる事実を見せる。 |
| 0 | ツカミ | Bolt.new | 「何を作る？」から始める。ビジョンに集中する | 001の言い方。エラー説明で始めない。 |
| 0 | ツカミ | Lovable | 自然言語からworking applicationへ進む | 001でゲーム、クイズ、シミュレーションを入口にする。 |
| 0 | ツカミ | GitHub Spark | dream -> see -> ship、自然言語、プレビュー、共有 | 001〜002。作る、見える、公開できるの順番を取り入れる。 |
| 0 | ツカミ | v0 by Vercel | idea -> production、テンプレ、design mode、agentic build、deploy | 画面演出の後続参考。001の主参考には入れない。 |
| 0 | ゲームで掴む | Microsoft MakeCode Arcade | 初手からゲーム。小さな画面が動く快感 | 001の題材選び。Space Invaders系、Galga系、Pizza chase系。 |
| 0 | 教育導入 | Hour of AI / Code.org系 | AIを使う側から作る側へ。短時間、ハンズオン、楽しい題材 | 003以降の思想補助。学ぶより先に作る側になる。 |
| 1 | AIとの付き合い方 | Claude Code | repoを読む、編集する、コマンド実行、複数ファイル作業 | 004〜006。AIに聞いていい、差分を見て進める導線。 |
| 1 | Agent操作術 | Claude Code Common Workflows | codebase overview、plan before editing、worktrees、PR、tests、docs | 004〜006。人間がAgentに次の一言を足す導線。 |
| 1 | Agent運用 | OpenAI Codex | multi-agent、worktrees、cloud environments、PR、refactor、test、review | 006以降。AIに任せ、人間がレビュー・方向づけをする。 |
| 1 | 戻れる設計 | Replit Agent / checkpoints | Agentが作る、テストする、問題修正する。checkpointで戻れる | 006。ログを残せる人は戻ってこられる。 |
| 2 | 開発センス入口 | The Odin Project | project-based、portfolio、roadmap、community、自走 | 「動いた」の次。作品を積む・小さなportfolio化。 |
| 2 | Web基礎 | MDN Learn | beginnerからcomfortableへ。HTML/CSS/JS、challenge、Playground | AIが作ったものを読める・直せるようにする段階。 |
| 2 | 反復練習 | Exercism | 小課題、automated analysis、人間メンタリング、idiom習得 | 返り咲き層のリハビリ。1日1問、筋トレ型。 |
| 3 | 本物のCS感覚 | CS50x | correctness / design / style、ScratchからWeb、最終プロジェクト | Phase 0では使わない。後で設計・正しさ・学び直しに使う。 |
| 3 | 道具のセンス | MIT Missing Semester | shell、editor、git、debugging、packaging、AI tools | 開発者返り咲き層に強い。道具を使える人になる段階。 |
| 3 | 古典教材の再利用 | freeCodeCamp | 課題分解、project、certification、長い自走ルート | いきなり見せない。後でロードマップ化・課題粒度を参考にする。 |

## 001 Fixed Reference Set

001の参考先は、当面この5つだけに絞る。

| Priority | Reference | Core for 001 |
|---:|---|---|
| 1 | Replit Agent | 普通の言葉で、アプリは作れる |
| 2 | Bolt.new | 「何を作る？」から始める。エラー説明で始めない |
| 3 | Lovable | 自然言語でゲームやシミュレーションも作れる |
| 4 | GitHub Spark | dream -> see -> ship の流れ |
| 5 | MakeCode Arcade | 最初はゲーム。画面が動く快感 |

## Six-clip Reassignment

| No | New position | Main references |
|---:|---|---|
| 001 | 最初の1時間で、ゲームは動く | Replit / Bolt / Lovable / Spark / MakeCode |
| 002 | 今日は5分だけ触れば勝ち | Bolt / Exercism / Odin |
| 003 | 昔やめた人は、弱い人じゃない | Exercism / Odin / Hour of AI |
| 004 | AIに聞いていい。検索していい。 | Claude Code / Codex / Replit |
| 005 | 理解より、まず動くものを作る | Lovable / Spark / Odin / MDN |
| 006 | ログを残せる人は、戻ってこられる | Claude Code / Codex / Replit checkpoints / Missing Semester |

## Guardrails

- Phase 0は、AIエージェント時代の「作れる」導線に集中する。
- 001では、仕様、要件定義、エラー解説、ログ解説を前に出さない。
- CS50/freeCodeCampはPhase 3以降の強い参考先として残すが、001の入口には使わない。
- 画面、UI、ロゴ、コピー、ゲーム画面、教材順序はコピーしない。

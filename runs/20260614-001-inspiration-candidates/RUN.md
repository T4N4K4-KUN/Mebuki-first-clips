# RUN

run_id: 20260614-001-inspiration-candidates
started_at: 2026-06-14 JST
owner: codex

## Goal

001 `最初の1時間で、ゲームは動く` を、Phase 0の参考先に基づく候補A/B/Cまで進める。

## Scope

- `clips/001-game-in-first-hour.md`
- `docs/REFERENCE_TARGETS.md`
- `docs/INSPIRATION_MAP.md`
- `docs/PHASED_REFERENCE_MAP.md`
- `docs/MEBUKI_CLIPS_V0_BOARD.md`
- `docs/RIGHTS_AND_REFERENCES.md`
- `docs/MATERIALS_LEDGER.md`
- `TODO.md`

## Non-goals

- 6本全部を一気に仕上げない。
- 外部動画、字幕、台本、図解、画面を使わない。
- 完成稿を1本に決めない。
- 動画ファイル、画像、音声、レンダリングコードを作らない。

## Work log

- [x] 読んだファイル：`docs/INSPIRATION_MAP.md`, `docs/REFERENCE_TARGETS.md`, `docs/MEBUKI_CLIPS_V0_BOARD.md`, `docs/SCRIPT_QUALITY_BAR.md`, `clips/001-game-in-first-hour.md`, `docs/MATERIALS_LEDGER.md`
- [x] 参考確認：Replit Agent, Bolt.new, Lovable Docs, GitHub Spark, Microsoft MakeCode Arcade
- [x] 追加参考確認：Replit公式60秒動画、Bolt/Lovable非公式チュートリアル、Adafruit Mini Galaga紹介。
- [x] 反省：Bolt/Lovable長尺チュートリアルは売り込み・機能デモ色が強く、001への学びが薄い。今後はNotebookLM投入前に動画選定を絞る。
- [x] 方針転換：旧「エラー」起点は001から外し、AIエージェント時代の「作れる」ツカミへ変更。
- [x] 変更したファイル：`clips/001-game-in-first-hour.md`, `docs/REFERENCE_TARGETS.md`, `docs/INSPIRATION_MAP.md`, `docs/PHASED_REFERENCE_MAP.md`, `docs/MEBUKI_CLIPS_V0_BOARD.md`, `docs/RIGHTS_AND_REFERENCES.md`, `docs/MATERIALS_LEDGER.md`, `README.md`, `TODO.md`
- [x] 権利確認：外部素材は使わず、構造・心理トリガー・視点反転のみ参考。
- [ ] 未確認事項：人間レビューで Candidate A/B/C のどれを採用するか。

## Completion criteria

- [x] 参考にした型が明記されている。
- [x] 候補A/B/Cがある。
- [x] 20〜35秒に収まる見込みがある。
- [x] 外部素材の直接利用がない。
- [x] 次に人間が選ぶポイントが分かる。
- [x] 001をCandidate Aベースのready稿に固定した。

## Notes

Candidate Aを第一候補として提示。ただし最終決定ではない。
001は、仕様・要件・エラー説明を出さず、「普通の言葉で頼む -> 動くゲームを見る」を最初に置く。
その後、001はCandidate A「作れる」を採用し、制作に渡せるready稿へ更新した。
追加調査の結果、001で残す学びは限定する。Replitは `idea -> software` と `pair programmer`、Boltは「軽いプロンプトからすぐ成果」、Adafruit Mini Galagaは「ユーザー投稿・既存ゲーム着想・edit codeで改造」。Bolt Discuss、Lovable詳細、Supabase/API/DBは後段へ回す。

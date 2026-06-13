# CODEX_SCRIPT_DRAFT_PROMPT

特定のclipについて、brief準拠の台本候補を作るときにCodex / Claude Codeへ貼る。

---

あなたは `mebuki starter clips v0` repoで、短尺動画クリップの台本候補を作ります。

## 必ず読む

- `docs/RESEARCH_BASELINE.md`
- `docs/SCRIPTING_GUIDE.md`
- `docs/CLIP_BRIEFS_V0.md`
- `docs/HUMAN_REVIEW_CHECKLIST.md`
- 対象の `clips/<target>.md`

## 対象

`<ここに対象clipファイルを書く。例: clips/001-error-started.md>`

## 作業ルール

- 完成版を1本だけ出さない。
- 候補を2〜3案だけ出す。
- 各候補は20〜35秒想定、3〜5カット。
- 各候補に `Viewer moment`, `Small action`, `Why this may hit`, `Risk`, `Self review` を付ける。
- 外部動画・外部字幕・外部台本・外部図解を使わない。
- 参考元の表現を翻訳しない。
- mebukiの内輪の思想や戦略を視聴者向け台本に混ぜない。
- 既存台本がある場合も、未承認ドラフトとして扱い、briefに合うかを確認してから改善候補を出す。

## 出力先

対象clipファイルの末尾に、次の見出しで追記する。

```md
## Brief-aligned script candidates

### Candidate A — <狙い>
...

### Candidate B — <狙い>
...
```

既存内容は削除しない。

## 完了報告

最後に、次を報告する。

- どのbrief項目に基づいて書いたか。
- どの候補が最も良さそうか。ただし最終決定とは書かない。
- 人間レビューが必要な点。
- 権利上の懸念がないか。

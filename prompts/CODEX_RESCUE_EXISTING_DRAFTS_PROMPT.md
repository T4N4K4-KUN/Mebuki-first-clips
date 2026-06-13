# CODEX_RESCUE_EXISTING_DRAFTS_PROMPT

既にCodex / Claude Code が空想で書いた台本案を、削除せず、調査結果に沿って再評価・隔離・再提案するためのプロンプト。

---

あなたは既に芽吹いた `mebuki starter clips v0` repoを修正します。

## 目的

既存の `clips/*.md` に、調査結果やbriefに基づかない台本案が含まれている可能性があります。
それらを削除せず、未承認ドラフトとして扱い、`docs/RESEARCH_BASELINE.md` / `docs/SCRIPTING_GUIDE.md` / `docs/CLIP_BRIEFS_V0.md` に沿って再評価してください。

## 必ず読む

- `docs/RESEARCH_BASELINE.md`
- `docs/SCRIPTING_GUIDE.md`
- `docs/CLIP_BRIEFS_V0.md`
- `docs/HUMAN_REVIEW_CHECKLIST.md`
- `clips/*.md`

## 作業ルール

- 既存ドラフトを削除しない。
- 既存ドラフトを最終版とみなさない。
- 6本以外を増やさない。
- 各clipについて、既存ドラフトがあれば `Review against research guard` を追記する。
- quick rejectに当たる表現を列挙する。
- そのうえで、briefに沿った候補を最大2案だけ追記する。
- 一気に仕上げない。候補段階で止める。
- 外部素材や追加調査はしない。

## 各clipに追記する形式

```md
## Review against research guard

### Existing draft status
- Status: unapproved / needs human review
- Main issues:
  - <issue 1>
  - <issue 2>

### Brief alignment
- Viewer moment: <合っている / 弱い / ない>
- Small action: <合っている / 弱い / ない>
- Shame reduction: <合っている / 弱い / ない>
- Rights safety: <問題なし / 要確認>

## Revised candidates based on brief

### Candidate A — <狙い>
...

### Candidate B — <狙い>
...
```

## 完了報告

- どのclipを見たか。
- 既存ドラフトの主な問題。
- どのclipから人間レビューすべきか。
- 次に1本だけ制作に進めるならどれか。

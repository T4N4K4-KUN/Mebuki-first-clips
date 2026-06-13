# CODEX PROMPT — 既存ドラフトをINSPIRATION MAPで見直す

このプロンプトは、芽吹いた後にCodexが勝手に書いたドラフトを評価・再設計するために使う。

```text
あなたはこのrepoの短尺動画脚本レビュー担当です。
今ある脚本を守る必要はありません。
ただし削除はしないでください。まず評価してください。

読むもの:
- docs/INSPIRATION_MAP.md
- docs/MEBUKI_CLIPS_V0_BOARD.md
- docs/SCRIPT_QUALITY_BAR.md
- clips/ 配下の既存ドラフト
- AGENTS.md
- TODO.md

目的:
既存のclips/*.mdが、白紙AI創作になっていないかを判定し、どの参考にする型を使って再設計すべきかを明示する。

やること:
1. 6本それぞれについて、現在のドラフトを読む。
2. `docs/SCRIPT_QUALITY_BAR.md` の5観点で採点する。
3. 「参考にした型」が明確にあるかを書く。
4. ない場合は、`docs/INSPIRATION_MAP.md` から使うべき型を指定する。
5. 既存台本をそのまま直さず、まずレビュー表を出す。
6. 最後に、最初に直すべき1本だけを推薦する。

出力形式:

# Existing Draft Review

| clip | current status | score /25 | missing inspiration pattern | main problem | recommended next action |
|---|---|---:|---|---|---|

## clipごとのコメント

### 001
- 良い点:
- ダメな点:
- 見直す参考型:
- 次に出すべき候補:

...

## 最初に直すべき1本

- 推薦clip:
- 理由:
- 次に使うプロンプト:
```

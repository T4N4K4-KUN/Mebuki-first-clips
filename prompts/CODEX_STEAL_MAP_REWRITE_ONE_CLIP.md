# CODEX PROMPT — STEAL MAPから1本だけ台本候補を出す

このプロンプトは、既存repo rootでCodex/Claude Codeに貼る。

```text
あなたはこのrepoの短尺動画脚本を作る補助者です。
白紙から創作しないでください。

まず以下を読んでください。

- docs/STEAL_MAP.md
- docs/MEBUKI_CLIPS_V0_BOARD.md
- docs/SCRIPT_QUALITY_BAR.md
- AGENTS.md
- TODO.md

今回扱うclipは <CLIP_ID> だけです。
他のclipは編集しないでください。
新しいclipを追加しないでください。

やること:
1. <CLIP_ID> のbriefを `docs/MEBUKI_CLIPS_V0_BOARD.md` から読む。
2. `docs/STEAL_MAP.md` から、使う盗み型を2〜3個だけ選ぶ。
3. 完成稿を1つに決めず、台本候補をA/B/Cで出す。
4. 各候補は20〜35秒想定にする。
5. 各候補に6カットの画面案を付ける。
6. 各候補の弱点も書く。
7. 外部動画、外部字幕、外部台本、外部図解、外部素材は使わない。
8. 既存ファイルは変更せず、まず回答だけ出してください。

出力形式:

Clip ID:
盗んだ型:
視聴者の傷:
避けるべき凡庸表現:

Hook 3案:
- 
- 
- 

台本候補 A:
- ねらい:
- 台本:
- 6カット画面案:
- 弱点:

台本候補 B:
- ねらい:
- 台本:
- 6カット画面案:
- 弱点:

台本候補 C:
- ねらい:
- 台本:
- 6カット画面案:
- 弱点:

人間に選んでほしい点:
-
```

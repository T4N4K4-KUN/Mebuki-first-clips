# Reference Transcripts

Transcripts and fact extraction for reference clip analysis.

This directory is committed so reference scripts and Japanese translations are visible from the remote repository.

## Files

| File | Source | Status |
|---|---|---|
| `replit-agent.md` | https://youtu.be/aWBiZc5XKJM | transcript added |
| `bolt-new-darrel-wilson.md` | https://youtu.be/5zfOitaKfmM | transcript added |
| `bolt-discuss-no-code-mba.md` | https://youtu.be/d8JTs12rxT0 | transcript added |
| `lovable-darrel-wilson-reconstructed.md` | https://youtu.be/mOak_imYmqU | reconstructed script added; not verbatim |
| `adafruit-mini-galaga-reconstructed.md` | https://youtu.be/o8jrZz3L9_I | reconstructed script added; not verbatim |
| `registered-lines-ja.md` | synthesis | Japanese translation of registered lines |
| `scratch-jumping-reconstructed.md` | https://youtu.be/1jHvXakt1qw | reconstructed script added; official source, not verbatim |
| `scratch-catch-reconstructed.md` | https://youtu.be/7NN5v2wSL4U | reconstructed script added; official source, not verbatim |
| `prd-guide-ai-apps-jordan-urbs.md` | https://youtu.be/MZjW7mlRgdw | user-provided script added; AI/PRD reference |
| `approach-software-developer-app-idea.md` | https://youtu.be/lLAkuOfBT_w | user-provided script added; developer brief reference |
| `acceptance-criteria-productplan.md` | https://youtu.be/zZV6FeJ3BtE | user-provided script added; acceptance criteria reference |
| `user-stories-agile-the-agile-shop.md` | https://youtu.be/7hoGqhb6qAs | subtitles downloaded; user story reference |

## Duplicate Guard

Before asking for NotebookLM work, check this list first.

Already registered sources:

| Source | Registered file | Japanese translation |
|---|---|---|
| https://youtu.be/aWBiZc5XKJM | `replit-agent.md` | yes |
| https://youtu.be/5zfOitaKfmM | `bolt-new-darrel-wilson.md` | yes |
| https://youtu.be/d8JTs12rxT0 | `bolt-discuss-no-code-mba.md` | yes |
| https://youtu.be/mOak_imYmqU | `lovable-darrel-wilson-reconstructed.md` | yes |
| https://youtu.be/o8jrZz3L9_I | `adafruit-mini-galaga-reconstructed.md` | yes |
| https://youtu.be/1jHvXakt1qw | `scratch-jumping-reconstructed.md` | yes |
| https://youtu.be/7NN5v2wSL4U | `scratch-catch-reconstructed.md` | yes |
| https://youtu.be/MZjW7mlRgdw | `prd-guide-ai-apps-jordan-urbs.md` | yes |
| https://youtu.be/lLAkuOfBT_w | `approach-software-developer-app-idea.md` | yes |
| https://youtu.be/zZV6FeJ3BtE | `acceptance-criteria-productplan.md` | yes |
| https://youtu.be/7hoGqhb6qAs | `user-stories-agile-the-agile-shop.md` | yes |

Do not send an already registered source back to NotebookLM unless the explicit goal is to verify or replace the existing transcript.

## NotebookLM Prompt

```text
このノートブック内のソースだけを使ってください。
推測は禁止です。
ソースにない情報は「未確認」と書いてください。

以下の形式で表にしてください。

1. クリップ一覧
- クリップ名
- URL
- チャンネル名
- 長さ
- 公式/非公式
- 001で参考にできる要素

2. セリフ一覧
- クリップ名
- 秒数
- 実際のセリフ
- 画面で起きていること
- 001で使える要素

3. 狙い
各クリップが何を狙っているか。
必ずソース内の根拠を付けてください。

4. 成果
各クリップで最終的に何ができる、何が見える、何が伝わるか。
推測は禁止です。

5. 001へのミクスチャー戦略
ここだけは提案として書いてください。
事実と提案を混ぜないでください。
```

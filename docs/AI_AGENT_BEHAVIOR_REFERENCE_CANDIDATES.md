# AI_AGENT_BEHAVIOR_REFERENCE_CANDIDATES

AIエージェント駆動開発で、人間の開発者への依頼術とズレる部分を扱う参考候補。

checked_date: 2026-06-14

## Problem

人間の開発者は、曖昧な仕様や深みにハマりそうな開発に対して、経験から警戒する。

AIエージェントは違う。

- 曖昧でも、質問せずに進めることがある。
- 「できそうですね」と軽く引き受けることがある。
- 逆に、ユーザーがリスク回避を強く示すと、急に保守的にリスク列挙へ寄ることがある。
- 実装できるかどうかと、運用・保守・安全に耐えるかどうかを分けて考えないことがある。
- 自律実行へ最適化されているため、質問すべき場面でも実行へ寄ることがある。

この論点は、従来の「開発者に見積もってもらう」教材だけでは足りない。

## Strong References

### 1. Ask or Assume? Uncertainty-Aware Clarification-Seeking in Coding Agents

URL: https://arxiv.org/abs/2603.26233

使える核:

- LLMエージェントは、ソフトウェアエンジニアリングのようなオープンエンド領域で、文脈不足の指示に頻繁に遭遇する。
- 人間の開発者は自然に確認質問をする。
- 現在のエージェントは、自律実行に最適化されがち。
- 不確実性検出とコード実行を分ける設計で、解決率が上がる。

001/002への翻訳:

- AIにすぐ作らせる前に、「足りない情報を3つ聞いて」と頼む。
- AIを「実行係」だけにしない。
- まず「質問係」として使う。

### 2. Interactive Agents to Overcome Ambiguity in Software Engineering

URL: https://arxiv.org/abs/2502.13069

使える核:

- AIエージェントは曖昧な指示に対して、勝手な仮定を置くことがある。
- 確認質問をしないと、悪い結果、安全リスク、計算資源の無駄につながる。
- モデルは「十分指定された指示」と「不足した指示」の区別が苦手。
- ただし、対話で不足情報を得られると性能は上がる。

001/002への翻訳:

- 「AIが質問してこないなら、こちらから質問モードに切り替える」。
- 「この注文票で足りない点を聞いて」と言う。
- 「勝手に決めて進めないで」と明示する。

### 3. Large Language Models Should Ask Clarifying Questions to Increase Confidence in Generated Code

URL: https://arxiv.org/abs/2308.13507

使える核:

- LLMはコード生成ができるが、トップレベルのソフトウェアエンジニアとは差がある。
- 良いエンジニアは、要件や解決策の曖昧さを減らすために確認質問をする。
- LLMにも同じことをさせるべき。
- 意図の不明確さ、計算的思考の不足、望ましくないコード品質を、質問によって減らせる可能性がある。

001/002への翻訳:

- 「作って」ではなく「作る前に、確認質問をして」と言う。
- AIに「あなたが不安な点」を聞くのではなく、「実装前に確定すべき点」を聞く。

### 4. Knowing but Not Showing: LLMs Recognize Ambiguity but Rarely Ask Clarifying Questions

URL: https://arxiv.org/abs/2605.25284

使える核:

- モデルは、曖昧さを認識できることがある。
- しかし通常の回答場面では、確認質問ではなく直接回答へ寄りがち。
- つまり「曖昧さを分かっている」と「質問として表に出す」は別能力。

001/002への翻訳:

- AIが質問しないからといって、仕様が十分とは限らない。
- 「この仕様に曖昧さがあるか判定してから、質問が必要なら質問して」と明示する。

### 5. Vibe Coding in Practice: Flow, Technical Debt, and Guidelines for Sustainable Use

URL: https://arxiv.org/abs/2512.11922

使える核:

- Vibe codingはMVPやプロトタイピングに使える。
- ただし、速い生成は技術的負債、設計不整合、セキュリティ脆弱性、保守負担につながる。
- 問題の一部は、設計理由の不足や、速いコード生成を優先することから来る。

001/002への翻訳:

- 最初の1時間は「動く」でよい。
- ただし、そのあと「なぜこの作りにしたか」をAIに説明させる。
- 作品化する段階では、設計理由とリスク確認を入れる。

### 6. Is Vibe Coding Safe? Benchmarking Vulnerability of Agent-Generated Code in Real-World Tasks

URL: https://arxiv.org/abs/2512.03262

使える核:

- 実世界タスクで、AIエージェント生成コードの安全性を評価している。
- 機能的には正しくても、安全ではないケースが多い。
- 「動く」と「安全」は別。

001/002への翻訳:

- 001では怖がらせすぎない。
- ただし「動いたら完成」ではなく、「公開する前に確認」が必要だと後続回で扱う。

### 7. Measuring the Permission Gate: A Stress-Test Evaluation of Claude Code's Auto Mode

URL: https://arxiv.org/abs/2604.04978

使える核:

- Claude Code auto mode の権限判定を、曖昧な認可シナリオで評価。
- ユーザー意図は明確でも、対象範囲・影響範囲・リスクレベルが不足していると問題が出る。
- 危険操作はシェルだけでなく、ファイル編集経由でも起こる。

001/002への翻訳:

- AIエージェントには「触ってよい範囲」を明示する必要がある。
- 「このフォルダだけ」「既存ファイルは変更前に確認」など、範囲指定は初心者にも必要。

## Secondary References

### Vibe Coding: convenience, risk and the future of software development

URL: https://www.techradar.com/pro/vibe-coding-convenience-risk-and-the-future-of-software-development

使える核:

- Vibe codingは参入障壁を下げる。
- ただし、未検証コード、セキュリティ、組織固有文脈の不足がリスクになる。

### When AI agents go rogue: why IT can't afford blind trust

URL: https://www.techradar.com/pro/when-ai-agents-go-rogue-why-it-cant-afford-blind-trust

使える核:

- AIエージェントは従来ソフトウェアより挙動が柔軟で、予期しない行動を取りうる。
- ロールバック、権限制限、ログ、人間の確認が重要。

## Video Candidate Check

今回の検索では、この論点を初心者向けに真正面から扱うYouTube動画は未確定。

近い動画候補:

| Title | URL | Why screen |
|---|---|---|
| Vibe Coding Fundamentals in 19 Minutes With Emergent AI | https://youtu.be/sdH7YPAmHes | vibe coding入門として、AI開発の流れを確認する候補。ただしリスク/曖昧さまで踏み込むか未確認。 |
| Essential AI prompts for developers | https://youtu.be/H3M95i4iS5c | プロンプト設計の型を拾える可能性。AIエージェント特有の過信/保守化まで扱うかは未確認。 |
| Claude Code Tutorial - Build Apps 10x Faster with AI | https://youtu.be/IuyVVtr1uhY | Claude Code実務チュートリアル。長いので、計画・確認・リスク制御の章があるか確認が必要。 |
| How to Write Perfect PRD for AI App Development | https://youtu.be/EZwLq21uAkA | AIアプリ開発向けPRD。仕様をAIに渡す型として追加調査候補。 |

## Editorial Takeaway

001で言うべきこと:

```text
AIは、怖がらずに作り始めてくれる。
でも、迷ったときに勝手に決めて進むこともある。
だから最初に、作るものを小さくして、できた判定を書く。
そして作る前に、「足りない情報があれば質問して」と言う。
```

002以降で扱うべきこと:

```text
AIに聞くべき3つ:

1. この注文票で曖昧なところは？
2. 最初の1時間で削るべき機能は？
3. 公開前に確認すべきリスクは？
```

人間の開発者との違い:

```text
人間の開発者は、経験から嫌な予感を持つ。
AIエージェントは、嫌な予感を自動では出さないことがある。
だから、AIには「不安を言え」ではなく「曖昧さを検出しろ」と頼む。
```


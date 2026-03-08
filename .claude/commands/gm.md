Morning Briefingを実行します。

`agents/secretary.md` の役割定義に従い、Morning Briefing Protocolを実行してください。

## 実行手順

### 1. データ取得（並行取得）
以下をすべて確認してください：
- Notion MCP → 今日のスケジュール・タスク（GTD[DB]: `1f55aab73db480a4a446d1f50e76cca3`）
- Notion MCP → 今週の習慣トラッキング実績（Habit_DB: `29a5aab73db480dea37ed74fdb01192b`、data_source_id: `29a5aab7-3db4-81a6-82b8-000ba10b54d7`）
  - 当週分（月曜〜今日）を date フィルタで取得
- Obsidian → 昨日のDaily Note（パスは secretary.md の Data Sources 参照）
- Notion MCP → 昨日完了したタスク
- `management/strategy/okr.md` → 今週の優先事項

### 2. Morning Briefing を出力
secretary.md の「Morning Briefing Protocol」のフォーマットに従って出力してください。

習慣トラッカーセクションでは以下の週目標と実績を対比してください：

| Category | 習慣 | 週目標 |
|----------|------|--------|
| 健康 | 平均睡眠時間 | 6.75時間 |
| 健康 | 筋トレ | 3回 |
| 健康 | No Masturbate | 7日 |
| 健康 | 歩数 | 平均 7,000歩 |
| 思考 | 読書ページ数 | 70P |
| 思考 | 日記（Daily Note作成） | 7日 |
| 社交 | デート | 1回 |
| 社交 | SEX | 1回 |
| 学習 | 英語 | 3回 |
| 学習 | スペイン語 | 7回 |
| 学習 | 数学 | 7回 |
| 資産 | 週間Spend | ¥20,000以内 |

出力フォーマット（習慣トラッカー部分）：
- 各項目に「実績 / 目標」と達成率を表示
- 未達成かつペースが遅い項目には ⚠️ を付けてアドバイスを添える
- 達成済みまたはペースが良い項目には ✅ を付ける

### 3. 今日のアジェンダ確認
ブリーフィング後、「今日は何から始めますか？」と問いかけてください。

リサーチを実行します。

**引数**: `$ARGUMENTS`
（例: `/research SNS運用代行市場の競合` / `/research 宇宙事業の参入機会`）

---

## 実行手順

以下のAgentを順番に呼び出して実行してください。

### Step 1: 問いの構造化
`agents/specialists/strategy/framer.md` の役割で、リサーチテーマを構造化してください：
- 調査目的（何を知りたいか・なぜ必要か）
- 調査範囲（何を調べるか・何は調べないか）
- 成功基準（どんな情報が得られれば十分か）

### Step 2: 情報収集
`agents/specialists/strategy/researcher.md` の役割で調査を実施してください：
- 一次情報源を3つ以上参照
- 信頼度を3段階で評価
- 出典を明記

### Step 3: 結果の構造化
`agents/specialists/strategy/content-creator.md` の役割でレポートを作成してください。

### Step 4: 保存
調査結果を以下に保存してください：
- `management/knowledge/market-research/YYYY-MM-DD_[テーマ].md`

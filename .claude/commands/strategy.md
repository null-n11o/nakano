戦略立案セッションを開始します。

**引数**: `$ARGUMENTS`
（例: `/strategy SNS運用代行の価格戦略` / `/strategy Doberの成長戦略`）

---

## 実行手順

COOの指揮のもと、以下のAgentを順番に呼び出して実行してください。

### Step 1: 問いの構造化 — Framer
`agents/specialists/strategy/framer.md` の役割で実行：
- テーマ: **$ARGUMENTS**
- 真の問いを特定する
- 目的・制約・評価軸を設定する
- 不足情報があれば逆質問リストを出力する

（不足情報がある場合はユーザーに確認してから次へ進む）

### Step 2: 情報収集 — Researcher
`agents/specialists/strategy/researcher.md` の役割で実行：
- Framerの構造に基づき必要な情報を収集する

### Step 3: 戦略立案 — Strategist
`agents/specialists/strategy/strategist.md` の役割で実行：
- 選択肢3案を設計する
- 各案にPros/Cons/Riskを付ける
- 推奨案を1案選び、理由を述べる

### Step 4: 批判検証 — Red Team
`agents/specialists/strategy/red-team.md` の役割で実行：
- 推奨案の反論・リスクを最低3つ提示する
- 各リスクに発生確率・影響度・対策を付ける

### Step 5: 意思決定サポート
上記を踏まえた最終提案をまとめてユーザーに提示する。

### Step 6: 記録
決定内容を `management/strategy/decisions/YYYY-MM-DD_[タイトル].md` に保存する。

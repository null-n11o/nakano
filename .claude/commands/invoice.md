請求書を作成します。

**引数**: `$ARGUMENTS`
（例: `/invoice kyohei` / `/invoice amano`）

---

## 実行手順

`agents/specialists/finance/accountant.md` の役割で以下を実行してください。

### Step 1: 情報確認
クライアント名: **$ARGUMENTS**

以下を確認してください：
- クライアントの BRIEF.md（契約金額・支払条件）
- 今月完了した業務内容

### Step 2: 不足情報の確認
以下の情報をユーザーに確認してください（BRIEF.mdに記載がない場合）：
- 請求金額・内訳
- 請求対象期間
- クライアントの会社名・住所

### Step 3: 請求書作成

```markdown
# 請求書
請求書番号: YYYY-MM-[連番]
発行日: YYYY-MM-DD
支払期日: YYYY-MM-DD（発行から30日後）

## 請求元
[KCPの情報をここに記載]

## 請求先
[クライアント情報]

## 請求内容
| 項目 | 数量 | 単価 | 金額 |
|------|------|------|------|
| [サービス名] | 1 | ¥X,XXX | ¥X,XXX |

小計: ¥X,XXX
消費税（10%）: ¥X,XXX
**合計: ¥X,XXX**

## 振込先
[銀行情報]
```

### Step 4: 保存
`management/finance/invoices/YYYY-MM-[クライアント名].md` に保存してください。

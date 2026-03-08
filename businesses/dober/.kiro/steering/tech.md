# Technology Stack

## Architecture

コンテンツビジネスのオートメーションスタック。コードを書くのではなく、ノーコード/ローコードツールを組み合わせてファネルを自動化する。

## Core Tools

- **自動化エンジン**: n8n（Threads投稿自動化済み。DM分岐は未実装）
- **コンテンツ配布**: Notion公開ページ or PDF（LM配布先）
- **メディア**: Threads（メイン集客）、note（ブログ記事）
- **メールリスト**: 使用中のメールサービス（未確定）

## Workflow Patterns

### n8n自動化フロー
```
Threads投稿スケジューラ（実装済み）
  ↓
キーワードリプライ検知 → 分岐判定 → LM別DM送信（未実装）
  ↓
メールリスト誘導CTA
```

### LMフロー設計原則
- キーワード1つにつきLM1種を対応させる（評価→LM-A、資産→LM-B、規律→LM-C）
- DM文は短く・即価値提供・CTA1点に絞る

## Spec-Driven Development

AIとの協業でスペックを先行定義してから実行する。
- `requirements.md` → `design.md` → `tasks.md` → 実行の順
- AIが実行できるタスクとケンタロウが判断するタスクを明確に分離する

## Development Standards

### コンテンツトーン
- 断定調・命令調（「〜しろ」「〜だ」）
- 感情的表現は排除。数字と観察事実のみ。
- 自己啓発系の「やさしい喝」ではなく、冷徹なシステム思考

### スペック管理
- ステータスは🔴 Not started / 🟡 In progress / 🟢 Done で統一
- ブロッカーは明示してから次のスペックを着手しない

---
_Document standards and patterns, not every dependency_

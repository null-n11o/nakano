# Project Structure

## Organization Philosophy

スペック単位でディレクトリを切る。各スペックは `requirements.md → design.md → tasks.md` の3ドキュメントで完結する。コンテンツ成果物と自動化テンプレートは専用ディレクトリで管理。

## Directory Patterns

### Specs（実行単位）
**Location**: `specs/[spec-name]/`
**Purpose**: 1機能または1成果物に対するRequirements → Design → Tasksの3点セット
**Example**: `specs/lm-a-grm-sheet/requirements.md`

### Content（コンテンツ成果物）
**Location**: `content/drafts/` / `content/published/`
**Purpose**: ドラフト段階と公開済みを分離して管理
**Example**: `content/drafts/lm-a-grm-sheet-v1.md`

### Workflows（n8n設計・テンプレート）
**Location**: `workflows/`
**Purpose**: n8nフロー設計書・DM送信テンプレートの保管
**Example**: `workflows/dm-template-lm-a.md`

### Assets（ブランドリソース）
**Location**: `assets/`
**Purpose**: ブランドガイドライン等の静的リソース

## Naming Conventions

- **スペックディレクトリ**: `kebab-case`（例: `lm-a-grm-sheet`, `n8n-dm-automation`）
- **コンテンツファイル**: `[spec-id]-[type]-v[N].md`（例: `lm-a-grm-sheet-v1.md`）
- **ワークフローテンプレート**: `[type]-template-[lm-id].md`（例: `dm-template-lm-a.md`）

## Spec Structure Convention

各スペックディレクトリ内のファイル命名と役割：

```
specs/[feature]/
  requirements.md   # 目的・成功基準・制約条件（承認必須）
  design.md         # 詳細設計・構成・トーン設計（承認必須）
  tasks.md          # Phase別タスクリスト・ブロッカー明示
```

## Spec Dependency Rule

スペック間の依存はタスクファイルの「依存関係」セクションで明示する。
URLや成果物が確定しないと次スペックを着手しないルールを守る。

---
_Document patterns, not file trees. New files following patterns shouldn't require updates_

# claude-skills-pack-ja

Manabuの個人用Claudeスキル集。Claude Code / Claude Desktop / claude.ai で使用。

## ディレクトリ構造

```
skills/
├── anti-ai-writing/     # AI生成文パターンの検出・除去
├── cire-minutes/        # CIRE議事録作成（CIRE専用）
├── daily-report/        # 日報アップデート
├── email-triage/        # メール仕分け・要約
├── general-minutes/     # 汎用議事録作成（CIRE以外）
├── monthly-report/      # UoC月報生成
├── morning-setup/       # 朝のTODOセットアップ
├── notion-cleanup/      # Notion巡回整理
├── notion-integration/  # Notion連携ユーティリティ
├── plaud-import/        # Plaud文字起こしのNotion取り込み
└── weekly-report/       # 週次振り返りレポート
```

## スキル一覧

| スキル | トリガー | 概要 |
|---|---|---|
| anti-ai-writing | 文章執筆時 | Wikipedia「Signs of AI writing」ベース。日本語20項目チェックリスト |
| cire-minutes | 「CIRE議事録」、CIRE文字起こしアップロード | CIRE専用の議事録生成。固有名詞辞書つき |
| daily-report | 「日報」 | カレンダー・ミーティング記録から日報を生成 |
| email-triage | メール確認時 | 3アカウントのメール仕分け・優先度判定 |
| general-minutes | 「議事録」、文字起こしアップロード | CIRE以外の全ミーティング議事録生成 |
| monthly-report | 「月報」 | 日報DBから月報をUoCフォーマットで生成 |
| morning-setup | 「朝」 | TODO更新、ルーティンリセット、メール・Slack確認 |
| notion-cleanup | 「整理して」「巡回して」 | Tactiq受信箱処理、DB棚卸し、重複検出 |
| notion-integration | Notion操作時 | Notion API連携のユーティリティ |
| plaud-import | Plaud txtアップロード | Plaud録音の文字起こしをNotionミーティングDBに登録 |
| weekly-report | 「週報」 | 日報DBから週次振り返りレポートを生成 |

## 管理方針

- source of truth はこのリポジトリ
- `~/.claude/skills` はこのリポジトリの `skills/` へのシンボリックリンク
- claude.ai側のスキルは別途アップロードが必要（ローカルファイルを直接参照できないため）
- 両方にあるスキルは、更新日が新しいほうを正とする

## 環境

- Claude Code: `~/.claude/skills/` → シンボリックリンクで自動参照
- Claude Desktop: 同上
- claude.ai: Project設定からアップロード。memoryにも要点を記録済み

## 関連

- anti-ai-writing: [blader/humanizer](https://github.com/blader/humanizer), [Wikipedia:Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)

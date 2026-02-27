# インストールガイド / Installation Guide

## Claude.ai でスキルを使う方法

### ステップ1: スキルファイルをダウンロード

このリポジトリの `skills/` ディレクトリから、使いたいスキルの `SKILL.md` をダウンロードします。

- [議事録スキル](../skills/meeting-minutes/SKILL.md)
- [日報スキル](../skills/daily-report/SKILL.md)
- [朝セットアップスキル](../skills/morning-setup/SKILL.md)
- [Notion連携スキル](../skills/notion-integration/SKILL.md)
- [メール仕分けスキル](../skills/email-triage/SKILL.md)

### ステップ2: Claude.ai にアップロード

1. [Claude.ai](https://claude.ai) にログイン
2. 左サイドバーで使いたいプロジェクトを選択（なければ新規作成）
3. プロジェクト設定の「Project Knowledge」セクションを開く
4. 「Upload」ボタンでダウンロードした `SKILL.md` をアップロード

### ステップ3: 使う

新しい会話を開始し、トリガーフレーズを使います。

- 議事録: 「議事録作って」+ 文字起こしテキストを貼り付け
- 日報: 「日報作って」
- 朝セットアップ: 「おはよう、今日のセットアップして」

## 複数のスキルを同時に使う

1つのプロジェクトに複数の `SKILL.md` をアップロードできます。Claude はトリガーフレーズから適切なスキルを自動判定します。

**推奨の組み合わせ:**
- 朝セットアップ + メール仕分け + 日報 → 1日のワークフローをカバー
- 議事録 + Notion連携 → 会議後のフォローアップを自動化

## MCP連携が必要なスキル

以下のスキルは MCP サーバーの設定が必要です:

| スキル | 必要なMCPサーバー |
|--------|------------------|
| 朝セットアップ | Google Calendar, Gmail（オプション） |
| Notion連携 | Notion |
| メール仕分け | Gmail |

MCP の設定方法は [claude-mcp-cookbook](https://github.com/manabuozato/claude-mcp-cookbook) を参照してください。

## トラブルシューティング

### スキルが反応しない

- SKILL.md がプロジェクトの Project Knowledge にアップロードされているか確認
- 新しい会話（同じプロジェクト内）で試す
- トリガーフレーズを変えて試す

### 出力が期待と異なる

- SKILL.md 内のカスタマイズポイントを確認
- 「〜の形式で」と明示的に指定して試す

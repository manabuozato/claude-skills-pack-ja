# Claude Skills Pack JA

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![GitHub stars](https://img.shields.io/github/stars/manabuozato/claude-skills-pack-ja.svg?style=social)](https://github.com/manabuozato/claude-skills-pack-ja/stargazers)

日本のビジネスワークフロー向けに設計された **Claude.ai スキル**のコレクションです。議事録作成、日報、朝のルーティン、メール仕分けなどに対応しています。

## これは何？

Claude.ai では、プロジェクトナレッジとしてカスタム指示（「スキル」）をアップロードできます。スキルは、会話中に関連するコンテキストを検出すると自動的に発動する再利用可能なプロンプトです。

**このリポジトリ**は、日本のビジネス環境に合わせたすぐに使えるスキルファイル（`.md`）を提供します。敬語、会議の進め方、和暦など、日本のビジネス慣習を理解したスキルです。

## スキル一覧

| スキル | 説明 | 対象ユーザー |
|--------|------|-------------|
| [議事録作成](skills/meeting-minutes/SKILL.md) | 文字起こしから構造化された議事録を自動生成 | 会議に参加する全ての人 |
| [日報作成](skills/daily-report/SKILL.md) | カレンダーとメモから日報を自動作成 | オフィスワーカー、管理職 |
| [朝のセットアップ](skills/morning-setup/SKILL.md) | 朝のルーティン：カレンダー、メール、タスク整理 | 仕事を始める全ての人 |
| [Notion連携](skills/notion-integration/SKILL.md) | Notion MCP連携テンプレート集 | Notion + MCP利用者 |
| [メール仕分け](skills/email-triage/SKILL.md) | 複数アカウントのメール仕分けと優先度分類 | 多忙なビジネスパーソン |

## クイックスタート

1. 使いたいスキルの `SKILL.md` ファイルを **ダウンロード**
2. [Claude.ai](https://claude.ai) を開き、プロジェクトに移動
3. プロジェクトナレッジに `SKILL.md` ファイルを **アップロード**
4. **チャット開始** — トリガーフレーズを検出すると自動的にスキルが発動

以上です。コーディング不要、APIキー不要、セットアップ不要。

### 使用例

`meeting-minutes/SKILL.md` をアップロード後、会議の文字起こしを貼り付けて：

> 議事録にまとめて

と言うだけで、日本のビジネス形式に沿った構造化された議事録が生成されます。

## 各スキルの詳細

### 議事録作成（`meeting-minutes/`）

会議の文字起こし（Tactiq、Otter.ai、手動メモなど）を構造化された議事録に変換します。

- 会議メタデータ（会議名、日時、出席者）
- 発言者名付きの議論ポイント
- 決定事項・アクションアイテム（担当者・期限付き）
- 敬語の正規化、です・ます → である調への変換オプション

### 日報作成（`daily-report/`）

以下の情報を統合して日報を作成します。

- カレンダーの予定と会議の成果
- プロジェクト別のタスク完了状況
- 明日の予定と優先事項
- 振り返りと懸念事項

### 朝のセットアップ（`morning-setup/`）

朝のルーティンをアシストします。

- 今日の日付コンテキストを更新
- カレンダーで今日のスケジュールを確認
- 未読メールのサマリー
- 優先度順のタスク整理
- 今日のフォーカス設定

### Notion連携（`notion-integration/`）

Claude + Notion MCP 連携のテンプレート集です。

- TODOマネジメントパターン
- 日報データベース更新
- プロジェクトトラッキングワークフロー

### メール仕分け（`email-triage/`）

複数アカウントのメール管理です。

- 全アカウントの未読チェック
- 緊急度・重要度による自動分類
- 適切なトーンでの返信ドラフト生成

## 日常使いから生まれたスキル集

これらは机上のテンプレートではありません。このパックに含まれる全てのスキルは、作者が実際に毎日の業務で使っているものです。会議の管理、レポートの作成、朝の準備、複数アカウントのメール対応など、日本のビジネス現場での数ヶ月の実用を経て磨き上げられました。

実践的で意見が入っていると感じたら、それは意図的なものです。

## サンプル

[examples/](examples/) ディレクトリにサンプル入出力があります。

- [議事録の例](examples/meeting-minutes-example.md)
- [日報の例](examples/daily-report-example.md)
- [朝のセットアップの例](examples/morning-setup-example.md)

## ドキュメント

- [インストールガイド](docs/installation.md) — Claude.ai へのスキルのインストール方法
- [カスタマイズガイド](docs/customization.md) — ワークフローに合わせたスキルの調整方法

## コントリビュート

コントリビュートを歓迎します！プルリクエストを送る前に [CONTRIBUTING.md](CONTRIBUTING.md) をお読みください。

特に歓迎するもの：
- 日本のビジネスワークフロー向けの新しいスキル
- 翻訳・ローカライゼーションの改善
- バグ修正・ドキュメントの改善

## ライセンス

MIT License — 詳細は [LICENSE](LICENSE) をご覧ください。

## 作者

**大里学 / Manabu Ozato** ([@manabuozato](https://github.com/manabuozato))
プロデューサー / 研究者、北陸先端科学技術大学院大学（JAIST）博士後期課程

---

[English README is here](README.md)

# CLAUDE.md — Daily Academic English Project

## プロジェクト概要

このリポジトリは、丸井健（Takeru Marui）が国際学会・英語論文執筆に向けて、
毎日Claudeと行う学術英語トレーニングの記録です。

## ディレクトリ構成

```
learning-english/
├── CLAUDE.md                  # このファイル
├── README.md                  # プロジェクト説明
├── logs/
│   └── YYYY-MM-DD.md          # 毎日のセッション記録
├── progress/
│   └── summary.md             # 累積進捗サマリー
└── .github/
    └── workflows/
        └── save-log.yml       # GitHub Actions ワークフロー
```

## 毎日のセッション構成

| Step | 内容 |
|------|------|
| Step 1 | Claudeが出す英文を日本語に翻訳する |
| Step 2 | その英文に対して英語でコメントを書く |
| Step 3 | Claudeが翻訳・英文コメントの両方にフィードバックを行う |

## .mdファイルのフォーマット

各日のログは `logs/YYYY-MM-DD.md` に保存。
フォーマットは `logs/template.md` を参照。

## テーマ方針

健さんの研究領域（防災・土木計画・VR・地域研究・教育）から
英文を選定し、専門的語彙と学術文体を同時に習得する。

## GitHub Actions について

セッション終了後に「今日の記録をGitHubに保存して」と送ると、
Claudeが当日の.mdファイルを生成し、`save-log.yml` ワークフローが
自動的にcommit/pushを実行する。

## 継続のルール

- サボった日は翌日「サボりました」と申告する
- 3日以上空いた場合はClaudeが叱る or 励ます（健さんの希望による）
- 継続こそが唯一の正解

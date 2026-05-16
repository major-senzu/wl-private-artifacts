# WL Private Artifacts

Wanderlust 内部用の成果物置き場（**Private リポジトリ**）。
機密情報（クライアント名・社員名・契約金額・戦略情報など）を含む成果物を格納する。

## 構成

```
wl-private-artifacts/
├── pwc/                    PwC関連
│   ├── issue-map.html      課題マップ（8課題の進捗トラッカー）
│   └── 課題マップ.html     同上（日本語ファイル名）
└── （将来）optage/, panasonic-homes/ など
```

## 機密扱いに関するルール

- このリポジトリは **Private**。Public に切り替える前に必ず内容を匿名化すること
- 公開可能な成果物は `claude-artifacts`（Public）に置く
- 人名・契約金額・戦略情報などはこちらに格納

## ローカル閲覧

```bash
cd /Users/major/Documents/wl-private-artifacts/pwc
python3 -m http.server 8765
# ブラウザで http://localhost:8765/issue-map.html
```

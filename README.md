# WL Artifacts

Wanderlust 内部用の成果物置き場。

> ⚠️ **このリポジトリは Public です**。GitHub Pages を使うために当初 Private から Public に変更しました。
> 機密情報（クライアント名・社員名・契約金額・戦略情報など）を含むため、**URL を不用意に共有しないこと**。
> 命名「wl-private-artifacts」は当初 Private で作成した経緯のままです（リネームすると公開URLが変わるため保持）。

## URL

- GitHub: https://github.com/major-senzu/wl-private-artifacts
- Pages トップ: https://major-senzu.github.io/wl-private-artifacts/
- PwC 課題マップ: https://major-senzu.github.io/wl-private-artifacts/pwc/issue-map.html
- Fulmark アプリUI: https://major-senzu.github.io/wl-private-artifacts/fulmark/

## 構成

```
wl-private-artifacts/
├── pwc/                    PwC関連
│   ├── issue-map.html      課題マップ（8課題の進捗トラッカー）
│   └── 課題マップ.html     同上（日本語ファイル名）
├── optage/                 Optage関連（org-chart.html）
├── fulmark/                Fulmark（CCG ENTERTAINMENT）関連
│   ├── index.html          プロジェクトページ（成果物一覧）
│   └── app-ui.html         簡易アプリケーションUI（ポスター自動生成プロトタイプ）
└── （将来）panasonic-homes/ など
```

## ルール

- このリポジトリは Public だが、 **URL を不用意に共有しないこと**
- 公開可能な成果物は `claude-artifacts` に置く
- 業務トラッカー・社内向け資料はこちらに格納

## 更新方法

```bash
cd /Users/major/Documents/wl-private-artifacts
# ファイル更新後...
git add -A
git commit -m "Update: ..."
git push
```

## ローカル閲覧

```bash
cd /Users/major/Documents/wl-private-artifacts/pwc
python3 -m http.server 8765
# ブラウザで http://localhost:8765/issue-map.html
```

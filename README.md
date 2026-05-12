# Pe☆rappella 公式サイト

東京理科大学アカペラサークル Pe☆rappella の公式サイト。素の HTML / CSS / JavaScript で構成。

## ローカル確認

```sh
cd ~/Documents/perappella-site
python3 -m http.server 8080
# → http://localhost:8080
```

## GitHub Pages への公開手順

1. このフォルダを GitHub リポジトリにする
   ```sh
   cd ~/Documents/perappella-site
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin git@github.com:<USER>/<REPO>.git
   git push -u origin main
   ```
2. GitHub のリポジトリ画面 → **Settings** → **Pages**
3. **Source** を `Deploy from a branch`、**Branch** を `main` / `/ (root)` に設定して保存
4. 数分後 `https://<USER>.github.io/<REPO>/` で公開される

## ファイル構成

```
.
├── index.html      # ページ本体
├── styles.css      # Cafe Jazz テーマ
├── script.js       # ナビ開閉 + フェードイン
├── assets/
│   └── logo.png    # サークルロゴ
├── .nojekyll       # Jekyll の処理をスキップ
└── README.md
```

## 編集ポイント

- ライブ情報：`index.html` の `<section id="live">` 内のチケット部分
- SNS リンク：`index.html` の `<section id="info">` と `<footer>` の 2 箇所
- 年間予定：`index.html` の `<ol class="timeline">`
- 色味の変更：`styles.css` 冒頭の `:root` 変数

# Pe☆rappella 公式サイト

東京理科大学アカペラサークル Pe☆rappella の公式サイト。素の HTML / CSS / JavaScript で構成。

1. GitHub のリポジトリ画面 → **Settings** → **Pages**
2. **Source** を `Deploy from a branch`、**Branch** を `main` / `/ (root)` に設定して保存
3. 数分後 `https://<USER>.github.io/<REPO>/` で公開される

## ファイル構成

```
.
├── index.html      # ページ本体 (サイトの構造や文字)
├── styles.css      # ページcss (サイトの見た目)
├── script.js       # ナビ開閉 + フェードイン (サイトの動き)
├── assets/
│   └── logo.png    # サークルロゴ
└── README.md       # この説明文
```

## 編集ポイント

- ライブ情報：`index.html` の `<section id="live">` 内のチケット部分
- SNS リンク：`index.html` の `<section id="info">` と `<footer>` の 2 箇所
- 年間予定：`index.html` の `<ol class="timeline">`
- 色味の変更：`styles.css` 冒頭の `:root` 変数

## 編集方法

1. github上で編集してコミットする。
2. コマンドラインで git clone し、AIで編集してからプッシュ

サイト中の文字を変更するだけなら1がおすすめ。
サイトの構造を変えたいなら2がおすすめ。やり方はAIに聞くか有識者に頼んだ方がいいと思います。

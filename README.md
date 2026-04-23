# KENKO Service Reform — 指針・実装書

経営・スタッフ共有用の社内文書。パスワード保護された静的 HTML。

## サイト構成

```
.
├── index.html      ← staticrypt で暗号化された本体
├── robots.txt      ← 検索エンジン除外
├── .nojekyll       ← Jekyll 無効化（GitHub Pages 用）
└── README.md       ← このファイル
```

## 更新方法

1. 手元で `KENKO_Service_Reform.html`（原本）を編集
2. https://robinmoisson.github.io/staticrypt/ で暗号化
3. 出力された HTML を `index.html` としてリポジトリに上書きコミット
4. GitHub Pages が数分以内に自動反映

## パスワードを変更する場合

1. 原本 HTML を用意（編集していなければそのまま）
2. staticrypt で **新しいパスワード** で再暗号化
3. 新しい `index.html` をコミット → push
4. チームに新パスワードを別チャネルで共有

## 注意事項

- パスワードは WhatsApp / Slack など、URL とは別のチャネルで共有する
- 人事異動・退職があった時は、必ずパスワードを変更する
- URL は検索エンジンには載らないが、URL とパスワードがあれば誰でも閲覧可能

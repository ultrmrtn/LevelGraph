# LevelGraph

日付ごとの進捗実績から、今後の進捗を予測するブラウザアプリです。グラフを PNG で保存できます。

[アプリを開く](https://ultrmrtn.github.io/LevelGraph/)

## ローカルで使う

`index.html` をブラウザで開いてください。ビルドやパッケージのインストールは不要です。

## 公開設定

GitHub Pages の公開元は `main` ブランチの `/ (root)` です。
設定はリポジトリの **Settings → Pages** で確認できます。
`.nojekyll` は Jekyll による処理を省略するためのファイルです。

## 更新する

変更をコミットして `main` に push すると、Pages が更新されます。

```powershell
git add index.html
git commit -m "Update LevelGraph"
git push origin main
```

## 参考

- [GitHub Pages の公開元の設定](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
- [コミット用メールアドレスの設定](https://docs.github.com/en/account-and-profile/how-tos/email-preferences/setting-your-commit-email-address)

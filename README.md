# LevelGraph

日付ごとの進捗実績から、今後の進捗を予測するブラウザアプリです。グラフを PNG で保存できます。

## ローカルで使う

`index.html` をブラウザで開いてください。ビルドやパッケージのインストールは不要です。

## GitHub への初回アップロード

以下はリポジトリ名を `LevelGraph`、公開範囲を Public にする場合の手順です。
GitHub のユーザー名とコミット用メールを確認してから実行してください。

1. `gh auth login --hostname github.com --web --git-protocol https` で公開先のアカウントにログインします。
2. `gh auth status` でログイン先を確認します。
3. このフォルダでコミット情報を設定します。メールは GitHub の Settings → Emails に表示される `@users.noreply.github.com` のアドレスを使用してください。

   ```powershell
   git config --local user.name "kuro"
   git config --local user.email "YOUR_GITHUB_NOREPLY_EMAIL"
   ```

4. 最初のコミットを作り、リポジトリを作成してアップロードします。

   ```powershell
   git add index.html README.md .gitignore .nojekyll
   git commit -m "Prepare LevelGraph for GitHub Pages"
   gh repo create LevelGraph --public --source . --remote origin --push
   ```

## GitHub Pages で公開する

1. 作成したリポジトリで **Settings → Pages** を開きます。
2. **Build and deployment → Source** を **Deploy from a branch** にします。
3. **Branch** を `main`、フォルダを `/ (root)` にして **Save** を押します。
4. デプロイ完了後、Pages に表示される URL を開きます。

公開 URL は通常 `https://GITHUB_USERNAME.github.io/LevelGraph/` です。
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

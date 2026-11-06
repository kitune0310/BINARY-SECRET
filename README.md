# BINARY SECRET — Web Edition

HTML/CSS/JavaScriptで動く、ブラウザ内完結型の暗号化・復号デモです。

## GitHub Pagesで公開する方法
1. GitHubで新しいPublicリポジトリ `BINARY-SECRET` を作成
2. `index.html` と `README.md` をアップロード
3. リポジトリの Settings → Pages を開く
4. Build and deployment の Source を `Deploy from a branch` にする
5. Branch を `main`、Folder を `/(root)` にして Save
6. 公開URLが表示されるまで待つ

## 方式
UTF-8 → パスワードを繰り返してXOR → 各byteのビット順を反転 → 16進数文字列化。`BS1` を先頭に付けます。

**注意:** これは学習用の難読化方式であり、暗号学的に安全ではありません。重要な情報には使わないでください。

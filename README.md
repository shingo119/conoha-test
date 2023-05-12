# ConoHa WING でのサーバー構築
### やったこと
1. テストアプリケーション作成
2. GitHub Actions用のymlファイル作成
3. ConoHa WINGでyubaseサーバーにドメイン設置
4. GitHubでSecretsの設定
5. GitHub Actionsでデプロイ
6. ConoHa WINGのファイルマネージャーを開き、ディレクトリ構成を確認
7. GitHub Actionsのymlファイルを、初回はgit clone、２回目以降はgit pullになるように修正
8. git clone失敗
9. ConoHa WINGのデプロイすべきフォルダに既にerrorフォルダがあったため削除して再度デプロイ
10. サーバーにphp実行環境がないため、composerコマンドが通らず
11. 推奨はサーバー側(ConoHa WING)にphpの実行環境をインストールすることだけど、やっていいかわからないのでプロジェクト内にインストールする
12. deploy.ymlの内容を修正
13. 
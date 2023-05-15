# ConoHa WING でのサーバー構築

## 初回デプロイ時に必要な作業
1. ConoHaへSSH接続
2. git clone
3. .envの修正
4. key:generateの実行
5. php artisan migrateの実行
6. シンボリックリンクの作成

## 作業記録
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
13. git cloneできた
14. composer installできず
15. サーバーのディレクトリ内を全部削除
16. git cloneできた
17. composer installできた
18. 403forbiddenエラー
19. .htaccessファイルは設定
20. internal server error

### 坂尻さんからのアドバイスを元に修正
1. .envの修正（DBの情報をConoHaのダッシュボードからコピペ）
2. key:gernerateを実施
3. php migrateを実施
4. シンボリックリンクの作成
5. デプロイ完了

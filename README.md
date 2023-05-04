# Wordpressのdocker-compose
1. duckdnsでドメイン取得
2. 以下のような.envファイルを作成
   ```
    URL=url
    MYSQL_ROOT_PASSWORD=password1
    MYSQL_PASSWORD=password2
    ```
3. `docker compose --env-file .env up -d`を実行
4. ポート8080に接続してwordpressをインストール
5. 設定からURLを`http://wordpress.<duckdnsで取得したurl>`に設定
6. ToolsのSite Healthからhttpsにアップデート

# README
cloneが終わったら、以下の手順でアプリを立ち上げてみてください。

```
docker-compose build
```

アプリとデータベースサーバの起動

```
docker-compose up -d
```

ターミナルで別のタブを開いて以下のコマンドを入力し、データベースを作成

```
docker-compose run web rake db:create
```

以下のURLにアクセスし、アプリが正常に起動できることを確認

```
http://localhost:3000
```

アプリの終了

```
docker-compose exec web down
```

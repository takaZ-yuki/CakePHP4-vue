# php-blog

## 実行方法

docker-compose初回起動時はjavascriptのパッケージを取得できていない為
watchコンテナーは起動に失敗する。

```
  docker-compose up -d
  docker exec -it app composer install
  docker exec -it app npm install -y
```
watchコンテナーを再起動する

```
docker-compose up watch
```

## 確認方法

[ここ](http://localhost/)にアクセスする

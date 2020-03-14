# docker-laravel4

## 参考
[Dockerを使ってLaravel開発環境構築][link1]

## メモ
- 起動
  ```
  # docker起動
  docker-compose up -d

  # phpコンテナに入ります
  docker-compose exec php bash

  # Laravelプロジェクト作成
  laravel new
  ```

- これでartisan makeでホスト側のユーザでファイルが作れる
  ```
  docker-compose exec -u 1000 php bash
  ```


[link1]:https://qiita.com/A-Kira/items/1c55ef689c0f91420e81
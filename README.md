# install_laravel_on_docker

## composition
- Nginx
- Laravel
- MySQL

## install and Usage
1. コンテナ起動
```
docker-compose build
docker-compose up -d
```

2. コンテナ確認
```
docker ps
docker-compose ps
```

3. コンテナ上でLaravelインストール
```
docker-compose exec app bash
cd /var/www/app
composer create-project laravel/laravel:^9 --prefer-dist .
```

4. ブラウザアクセス
```
http://localhost:8080/
```

5. コンテナ停止
```
docker-compose down
```
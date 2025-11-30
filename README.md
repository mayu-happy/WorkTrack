# 勤怠管理アプリ WorkTrack

## 環境構築

### 1. リポジトリをクローン
git clone git@github.com:mayu-happy/worktrack.git
cd worktrack

### 2. Dockerビルド＆起動
docker compose up -d --build

### 3. Laravelセットアップ
docker compose exec php bash
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate --seed

### 4. URL

アプリ本体: http://localhost/

phpMyAdmin: http://localhost:8080/

### 使用技術
PHP 8.1
Laravel 10
MySQL 8.0
Docker / docker-compose

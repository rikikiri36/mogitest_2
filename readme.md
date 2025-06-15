# coachtech 勤怠管理アプリ
## プロジェクト概要
---
- サービス名：coachtech 勤怠管理アプリ
- サービス概要：ある企業が開発した独自の勤怠管理アプリ
- 制作の背景と目的：ユーザーの勤怠と管理を目的とする
- 制作の目標：初年度でのユーザー数1000人達成

## 環境構築
---
### 1.Dockerビルド
1. git clone https://github.com/rikikiri36/mogitest1
2. docker compose up -d --build

### 2.Laravel環境構築
1. composer install
2. 「.env.example」をコピーして「.env」ファイルを作成し、下記環境変数の変更をする
　　-  DB_HOST=mysql
　　-  DB_DATABASE=laravel_db
　　-  DB_USERNAME=laravel_user
　　-  DB_PASSWORD=laravel_pass
1. php artisan key:generate
2. php artisan migrate:fresh
3. php artisan db:seed

## 使用技術
---
- PHP 8.4.1
- Laravel Framework 8.83.29
- MySQL 8.0.41
- Docker 27.5.1

## URL
---
### 開発環境
1. 一般ユーザーログイン
   http://localhost/login
2. 管理者ログイン
   http://localhost/admin/login

### phpMyAdmin
   http://localhost:8080/

## テストアカウント
---
### 一般ユーザー
name: 一般太郎  
email: user1@test.com
password: password  
-------------------------
name: 一般花子  
email: user2@test.com  
password: password  
-------------------------
### 管理者
name: 管理三郎  
email: kanri1@test.com  
password: password  
-------------------------
name: 管理四郎  
email: kanri2@test.com  
password: password  
-------------------------


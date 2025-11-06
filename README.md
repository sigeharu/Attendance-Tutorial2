# 勤怠システム - Attendance Tutorial

これはセレブエンジニアサロンの教材で作られた学習用サンプルアプリケーションです。

## 概要

基本的な勤怠管理機能を持つWebアプリケーションです。ユーザー認証、出退勤記録、勤怠の一覧・編集機能を実装しています。

**注意**: このプロジェクトは学習・ポートフォリオ目的で作成されたものです。

## 使用技術

* Ruby 3.1.6
* Rails 6.1.7
* PostgreSQL (本番環境)
* SQLite3 (開発環境)
* Bootstrap
* Render (デプロイ先)

## 主な機能

* ユーザー認証（サインアップ、ログイン、ログアウト）
* 管理者権限システム
* 出勤・退勤の打刻
* 月次カレンダー表示
* 勤怠記録の一括編集
* 在社時間の自動計算

## ローカル開発環境のセットアップ

```bash
# リポジトリのクローン
git clone [repository-url]
cd Attendance-Tutorial2

# 依存関係のインストール
bundle install

# データベースのセットアップ
rails db:migrate
rails db:seed

# サーバーの起動
rails server
```

## Renderへのデプロイ

このアプリケーションはRenderでホスティングできるように設定されています。

### デプロイ手順

1. Renderアカウントにログイン
2. 「New +」→「Blueprint」を選択
3. リポジトリを接続
4. `render.yaml`が自動検出されます
5. 環境変数を設定（必要に応じて）
6. デプロイを実行

### 必要な環境変数

本番環境では以下の環境変数が必要です：

* `DATABASE_URL` - PostgreSQLの接続URL（Renderが自動設定）
* `SECRET_KEY_BASE` - Railsのシークレットキー（Renderが自動生成）
* `RAILS_ENV=production`
* `RAILS_SERVE_STATIC_FILES=true`
* `RAILS_LOG_TO_STDOUT=true`

## 開発履歴

* AWS Cloud9で初期開発
* Herokuデプロイ用に設定
* Rails 6.1 + Ruby 3.1にアップグレード
* Renderデプロイ対応
# Inspection App（点検登録アプリ）

## 概要
自動車点検内容を登録・管理するためのDjango製Webアプリです。

## 主な機能
- 点検一覧表示
- 点検詳細表示
- 点検登録
- 点検編集
- 点検削除
- フォームバリデーション（必須・数値チェック）
- エラーメッセージ表示（Django messages framework）

## 使用技術
- Python
- Django
- SQLite3
- HTML / CSS

## セットアップ手順
```bash
git clone https://github.com/kz-MobilIT/inspection-app.git
cd inspection-app
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

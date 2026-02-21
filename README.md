# Inspection App（点検登録アプリ）

## 概要
## 概要
自動車整備・点検業務を想定し、点検内容を登録・管理できる
Django製のWebアプリです。

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

## 工夫した点・学習ポイント
- DjangoのClass Based Viewを使わず、Function Based ViewでCRUDを実装し、処理の流れを理解することを重視しました
- フォームバリデーションをforms.pyで管理し、viewsをシンプルに保つようにしています
- base.htmlを作成し、テンプレート継承で共通レイアウトを管理しています
- Django messages frameworkを使い、ユーザーに分かりやすいエラー表示を実装しました

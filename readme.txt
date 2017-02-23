1.起動手順
①logisticsフォルダに遷移して
②source ./env/bin/activate を実行して
③python app.py を実行する

2.以下のPythonパッケージが必要
sudo pip install flask-mysql


3.DBについて
DB設定ファイルはlogisticsフォルダの下のconfigure.pyになる。
ファイル内容として、以下が必要

# -*- coding: utf-8 -*-
MYSQL_DATABASE_USER = 'XXX'
MYSQL_DATABASE_PASSWORD = 'XXXXXX'
MYSQL_DATABASE_DB = 'DB名'
MYSQL_DATABASE_HOST = 'ホストIPまたはホスト名'

4.ログインページについて
url/showLogin
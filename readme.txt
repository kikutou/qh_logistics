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
url/show_login

5.pycharmのインポートエラー表示について
pathになるフォルダをpycharmのProject表示欄に右クリックして、
選択肢の「Mark Directory as」の「Sources root」を選択する。

6.debugモード切り替え
デバッグモード：logistics/app.pyのapp.config['DEBUG']をTrueに設定する
実行モード：logistics/app.pyのapp.config['DEBUG']をFalseに設定する

7.app設定
ICONITアプリをダウンロードして、
設定の「アカウント」の「アプリ設定」の「商品検索」
その中に、倉庫管理用の商品追加のURLを追加する。


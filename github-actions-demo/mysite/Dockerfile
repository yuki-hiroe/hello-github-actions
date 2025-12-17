# ベースイメージの指定
FROM python:3.10

# ワーキングディレクトリの作成
RUN mkdir /code

# ワーキングディレクトリの設定
WORKDIR /code

# カレントディレクトリ配下のファイルをワーキングディレクトリに追加
ADD . /code

# 8000番ポートでリッスン
EXPOSE 8000

# 必要なパッケージのインストール
RUN pip install -r requirements.txt

# 起動コマンド
CMD python manage.py runserver 0.0.0.0:8000

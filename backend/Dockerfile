FROM python:3.8

WORKDIR /app

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

# 必要なファイルをコピー
COPY . .

ENV FLASK_APP=app/app.py

# コンテナが外部に公開するポートの指定
EXPOSE 5000

# コンテナ起動時に実行するコマンドの指定
CMD ["flask", "run", "--host=0.0.0.0"]
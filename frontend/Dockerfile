# ベースイメージとして node を使用
FROM  node:14

# 作業ディレクトリを /app に設定
WORKDIR /app

# 必要なファイルをコピー
COPY package.json ./
COPY package-lock.json ./

# 依存関係をインストール
RUN npm install

# アプリケーションのソースコードをコピー
COPY . .

# コンテナが外部に公開するポートを指定
EXPOSE 3000

# コンテナ起動時に実行するコマンドを指定
CMD ["npm", "start"]
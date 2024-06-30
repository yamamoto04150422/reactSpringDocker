フロントはreactでバックはspring boot

# デタッチで起動

docker compose up -d

# 停止

docker compose down

## 起動を確認

docker compose ps

# バックエンドの起動までのプロセス

docker compose exec api bash

cd /workspace

./gradlew bootRun

## バックエンド単体の確認

http://localhost:8080/api/hello

# フロントの起動プロセス

docker compose exec web bash

cd /workspace

npm install

npm run start 

## フロントの確認

http://localhost:3000/
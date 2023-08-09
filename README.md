## 手順

1.git clone https://github.com/tsubasahirakida/docker_react_rails.git

2. Docker Desktopの立ち上げ

3. cd docker_react_rails

4. docker-compose build

5. docker-compose up -d --build
※ `-dオプション` バックグラウンドでコンテナが起動

6. localhost:3000にRails、localhost:8000にReactのサーバー起動

7. docker-compose down
※コンテナはメモリ容量大きいので、作業が終われば、コンテナを削除

8.再度コンテナを起動する際は、`docker-compose up -d`
※Dockerイメージは5の手順で作成されているため、再度コンテナ起動する際は、--buildオプション不要

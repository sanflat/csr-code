Dockerイメージのビルド
```
docker build -t linux-basic-image .
```

Dockerコンテナの起動
```
docker run -it --rm --name linux-basic-container -v ./:/workspace linux-basic-image
```

起動中のDockerコンテナに入る
```
docker exec -it linux-basic-container /bin/bash
```

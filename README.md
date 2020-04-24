# my-c-compiler
自作cコンパイラ

## Dockerによる開発環境の作成
ソースコードの編集やgitの操作はDockerの外、ビルドやテストはDockerの中で行う(Linux開発環境をセットアップする)

セットアップ手順

```
$ docker build -t compilerbook .
```

Dockerイメージの取得

```
docker run --rm -it -v $HOME/my-c-compiler compilerbook
```

コンテナをインタラクティブに呼び出し、ビルドする
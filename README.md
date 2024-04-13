# 概要

このプロジェクトは、Ruby on RailsとVue.jsをDocker内で動作させることにより、環境構築のコストを削減することを目的としています。Dockerコンテナ内でアプリケーションを実行することで、開発者は環境構築にかかる手間を軽減し、素早く開発を始めることができます。

Ruby on Rails：`/app`  
Vue：`/vue`

# 環境構築

1. **makeコマンドの利用（Macはデフォルトで入っているか確認）**: プロジェクトの起動やコンテナの管理には、`make`コマンドを使用しています。`make`コマンドを使用することで、簡単にコンテナのビルド、起動、停止などを行うことができます。Macユーザーは通常、`make`コマンドを使用できますが、インストールされていない場合は別途インストールする必要があります。

2. **Docker for Desktopのインストール**: プロジェクトを実行するには、Docker for Desktopが必要です。Docker for Desktopをインストールすることで、ローカルマシンでDockerコンテナを実行し、開発を行うことができます。

# 初回実行時

初回実行時には、以下の手順に従ってプロジェクトをセットアップします。

1. プロジェクトのルートディレクトリに移動します。
2. `make build`コマンドを実行して、Dockerイメージをビルドします。
3. `make up`コマンドを実行して、コンテナを起動します。
4. 起動が完了したら、指示に従ってブラウザでアプリケーションにアクセスします（デフォルトでは[http://localhost:8080/](http://localhost:8080/)）。

# 主なコマンド

- `make up`: コンテナを起動します。
- `make up-d`: コンテナをバックグラウンドで起動します。
- `make down`: コンテナを停止します。
- `make exec-vue`: Vue.jsコンテナに入ります。
- `make exec-rails`: Railsコンテナに入ります。
- `make exec-db`: データベースコンテナに入ります。

これらのコマンドを使用することで、開発やデバッグをより効率的に行うことができます。

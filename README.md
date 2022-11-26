# playwright_sample

## 概要

Playwrightを利用したサンプルプロジェクト。

## 前提環境

* Poetry
  * ローカルで実行する場合は必要。
* Docker
  * dockerコンテナ上で実行する場合は必要。

## 環境構築

ローカルで実行する場合は、以下の環境構築手順の実施が必要。

1. 仮想環境を作成し、依存パッケージをインストールする
    ```bash
    poetry install
    ```
1. 仮想環境を有効にする
    ```bash
    poetry shell
    ```
1. Playwrightで利用するブラウザをインストールする
    ```bash
    playwright install
    ```

## 実行方法

### ローカルで実行

1. 仮想環境が有効でない場合は有効にする
    ```bash
    poetry shell
    ```
1. サンプルコードを実行する
    ```bash
    python -m playwright_sample.sample
    ```

### dockerコンテナ上で実行

1. サンプルコードを実行するdockerコンテナを起動する
    ```bash
    docker-compose up -d
    ```

コンテナを削除する場合は以下のコマンドを実行する。
```bash
docker-compose down
```

## 参考サイト

* [Pythonで記述されたPlaywrightの実行環境をDockerで用意する](https://nainaistar.hatenablog.com/entry/2021/07/12/120000)
* [Poetryをサクッと使い始めてみる](https://qiita.com/ksato9700/items/b893cf1db83605898d8a)
* [Installation | Poetry](https://python-poetry.org/docs/#installing-with-the-official-installer)
* [Poetryのインストールと仮想環境作成先の変更](https://medium.com/music-and-technology/poetry%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB%E3%81%A8%E4%BB%AE%E6%83%B3%E7%92%B0%E5%A2%83%E4%BD%9C%E6%88%90%E5%85%88%E3%81%AE%E5%A4%89%E6%9B%B4-96e1bab83725)

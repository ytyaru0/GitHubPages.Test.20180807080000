# このソフトウェアについて

GitHubPagesの使い方まとめ。

GitHubでリポジトリごとにWebSiteを構築する方法をまとめる。

* [URL](https://ytyaru.github.io/GitHubPages.Test.20180807080000)
    * [ReadMe.md](https://ytyaru.github.io/GitHubPages.Test.20180807080000/ReadMe.md)
    * [index.html](https://ytyaru.github.io/GitHubPages.Test.20180807080000/index.html)

# 前提

* GitHubのアカウントを作成する

# 方法

1. サイト用ファイルを作成
1. 1をGitHubへpushする（`git add`, `git commit`, `git push`）
1. サイト公開設定する（GitHubのリポジトリページで`Settings`参照）
1. 確認（URL参照すると公開されていることが確認できる）

## 手順

### 1. サイト用ファイルを作成

* RootRepo/
    * _config.yml
    * ReadMe.md
    * index.html

ディレクトリ名は任意。ディレクトリ名はリポジトリ名やURLのサブディレクトリ名になる。

### 2. GitHubへpushする

RootRepoディレクトリを任意GitHubユーザのリポジトリとしてpushする。

```
$ cd RootRepo
$ git init
$ git add .
$ git commit "init commit."
$ git push
```

### 3. サイト公開設定する

#### 3-1. リポジトリ設定ページへ遷移する

1. ブラウザを起動する
1. GitHubのサイトへアクセスする
1. pushしたアカウントでログインする
1. pushしたリポジトリのページへ遷移する
1. リポジトリページで`Settings`をクリックする

#### 3-2. リポジトリ設定する

1. `GitHubPages`の項目で`None`になっているリストボタンをクリックする
1. `master branch`, `master branch /doc folder`, `None`の3つの項目が表示されることを確認する
1. `master branch`をクリックする
1. 隣にある`Save`ボタンをクリックする
1. URLが表示されることを確認する

### 4. 確認

1. 表示されたURLをクリックする
1. サイトが表示される

表示されないなら数秒待ってからクリックするか、キャッシュ削除してからクリックする。

# 参考

* http://yoshikyoto.github.io/text/git/gh_pages_md.html

# 開発環境

* [Raspberry Pi](https://ja.wikipedia.org/wiki/Raspberry_Pi) 3 Model B
    * [Raspbian](https://www.raspberrypi.org/downloads/raspbian/) GNU/Linux 8.0 (jessie)
        * ブラウザ
            * Chromium
                * バージョン 56.0.2924.84 Built on Ubuntu 14.04, running on Raspbian 8.0

# ライセンス

このソフトウェアはCC0ライセンスである。

[![CC0](http://i.creativecommons.org/p/zero/1.0/88x31.png "CC0")](http://creativecommons.org/publicdomain/zero/1.0/deed.ja)


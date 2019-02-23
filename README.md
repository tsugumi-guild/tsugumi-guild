つぐみギルドに関係する文書やメディアなどを保管するリポジトリです。

Gitのインストール
----

参照: https://git-scm.com/book/ja/v1/%E4%BD%BF%E3%81%84%E5%A7%8B%E3%82%81%E3%82%8B-Git%E3%81%AE%E3%82%A4%E3%83%B3%E3%82%B9%E3%83%88%E3%83%BC%E3%83%AB

* Windowsなら [git for windows](https://gitforwindows.org/ )をダウンロード
* Macなら`brew install git`
* UbuntuなどDebian系Linuxなら`apt install git`

クローン
----

このリポジトリの内容を手元のコンピュータに移す。

```sh
git clone git@github.com:tsugumi-guild/tsugumi-guild
```

コミット & プッシュ
----

HOGE.txtを追加したい場合:

```sh
git fetch # 内部データを同期する
git checkout -B add-hoge origin/master # ブランチ(変更の草案)を作成
git add HOGE.txt # 変更部分を指定
git commit # ブランチに変更を追加
git push -u origin add-hoge # GitHubに送信する
```

https://github.com/tsugumi-guild/tsugumi-guild/pulls に移動し、プルリクエストを投稿する。

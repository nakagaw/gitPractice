# gitPractice

1. A をリモートにプッシュ
2. B をリモートにプッシュ
3. C をリモートにプッシュ
4. D をローカルでコミット
5. E をローカルでコミット

４，５をgit rebaseでsquashしてみたリポジトリです。



```
git rebase -i コミットID
```
とコマンドをうつと、

```
pick コミットID
pick コミットID
pick コミットID
```
といったリストが出てくるので、「pick」の部分を以下のコマンドに書き換えることでそれぞれのコマンドが使える。

>- pick（コミットを採用）
- reword（コミットを採用するが、コミットメッセージを変更）
- edit（コミットを採用するが、ファイルを修正する）
- squash（一個前のコミットと合体させる）
- fixup（コミットメッセージを変更しない点以外、squashと同じ）
- exec（shellでコマンドを実行する）<br>
引用元：<a href="http://liginc.co.jp/web/tool/79390" target="_blank">"初心者でも分かる！git rebaseの使い方を解説します | 株式会社LIG</a>




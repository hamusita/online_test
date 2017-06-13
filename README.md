# とある会社の技術テストで出された問題の解答
最近とある会社の技術テストを受けたんですが、３問あるうちの３問とも答えられなくて悔しかったので解き直したもののコードを上げておきます。

## Base64に関する問題
１問目はBase64に関する出題でした。  
これはBase64/ に入れてあります。


```./base.py```で実行できます。
オプションは以下の通りです。

| オプション      | オプションの説明                                                                     |
| :-------------: | :----------------------------------------------------------------------------------: |
| -i [FILEPATH]   | base64でエンコード、もしくはデコードしたい文字列が書かれた入力ファイルのパスを指定   |
| -o [FILEPATH]   | base64でエンコード、もしくはデコードした文字列の出力先のファイルのパスを指定         |
| -e              | 変換のタイプの指定 -e はエンコード                                                   |
| -d              | 変換のタイプの指定 -d はデコード                                                     |

-i と -o は必須です。
-e と -d のどちらも使用しなかった場合はエンコードになるようにしてあります。

```
ex) $ ./base64.py -i input.txt -o output.txt

    $ cat output.txt
    SGVsbG8gd29ybGQK
    $ ./base64.py -i output.txt -o revers.txt -d

    $ cat revers.txt
    Hello world

    $
```

## 逆ポーランド記法に関する問題

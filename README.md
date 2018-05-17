# Markdownに関するメモ
* 以下の記法で大体綺麗に書けるはず
* `*`とか`#`の直後のスペースはMarkdownの文法上意味があるので省くと正しく表示できない。
```Markdown
# Header level1
* list
** list
*** list
1. 番号付きlist
2. 番号つきlist
## Header level2
### Header level3
#### Header level4
##### Header level5
###### Header level6
```
* 上のMarkdownは[こんな感じ](https://ensemble-project.github.io/header_list)になる
## Header levelの注意
```
# Header level1
#### Header level4 のつもり -> 実際にはHeader level2となる
```
* 一つの.mdファイルの中で途中のHeader levelが一つも使われない場合は、Header levelが繰り上がるので注意
* 上の例では`## Header level2`と `### Heder level3`が現れないので `#### `は自動的に繰り上がってHeader level2 となってしまう。

## 表の挿入
```

| ここに(中央寄せ) | 表の(中央寄せ) | 項目を(右寄せ) | 入れる(左寄せ) |
|:----------------:|:--------------:| --------------:|:-------------- |
| ここに           | 表の           | 要素を         | 入れる         |
| 123              | 456            | 789            | 012            |

```

| ここに(中央寄せ) | 表の(中央寄せ) | 項目を(右寄せ) | 入れる(左寄せ) |
|:----------------:|:--------------:| --------------:|:-------------- |
| ここに           | 表の           | 要素を         | 入れる         |
| 123              | 456            | 789            | 012            |

* うまくいかないときは前後に空行を入れると良いかも
* 2行目の`:- `:-:` ` -:`で右寄せ中寄せ左寄せを制御できる
* 縦線`|`は位置を揃える必要はない

## リンク
* リンクは`[リンクしたい文字](http://リンク先)`みたいに書く

## その他
* Markdown でググる

# スタイルの変更
* 大元の[merlot](https://github.com/pages-themes/merlot)からの変更点
  * `_sass/screen.scss` 内のヘッダレベルを調整
  * `assets/css/mobile.css`でスマホからページを参照した時のヘッダレベルを調整
* もっと詳しい方いたら適宜変更してください

# テストページ
* [テストページ](https://ensemble-project.github.io/test)があるので、ここで好きに試してみると良いと思います。`test.md`がテストページの内容です。
* 変更して30秒くらいで反映されるっぽい
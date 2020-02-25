jinmei-neologd
====

[mecab-ipadic-neologd](https://github.com/neologd/mecab-ipadic-neologd)の辞書データから人名だけを抜き出しました。  
フリガナをキーとして、候補となる書き文字をリストで保持するようなJSON形式に整形しています。

## Description

`sei.json`は姓のデータです。`mei.json`は名のデータです。  
現在は`mecab-user-dict-seed.20200130.csv`からデータを抜き出しました。

scriptsフォルダ以下には人名データを抜き出してJSONに整形するスクリプト（Python）があります。  
使い方は以下のとおりです。

1. [mecab-ipadic-neologd](https://github.com/neologd/mecab-ipadic-neologd)から辞書データをダウンロード、解凍します。
2. scripts/jinmei_neologd.pyを実行します。（Python3）
```
python jinmei_neologd.py '~/mecab-user-dict-seed.yyyyMMdd.csv'
```

## Usage

GitHub Pagesで[サイト](https://s1r-j.github.io/jinmei-neologd/)を作成しているので、
姓または名のリンクを押せばそれぞれのJSONファイルが返却されます。

## Licence

[Apache-2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

## Author

[s1r-J](https://github.com/s1r-J)
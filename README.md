# xls-to-csv-or-csv-to-xls
http://www.kunst1080.net/entry/2013/03/31/165215
上記URLのものを忘備録としてGitにアップさせていただいています。

概要

BATファイルを作成し、コマンドラインからxls→csvやcsv→xlsの変換を行う。
テキストの解析やEXCELの解析を実装するのが面倒なので、極力EXCELの機能を使用するコンセプトで。

使い方

BATファイルはPATHの通ってる場所においてね！

hoge.xlsをfuga.csvに変換する場合(xls → csv)

xls2csv hoge.xls fuga.csv

fuga.csvをhoge.xlsに変換する場合(csv → xls)

(CSVの1列目が標準、2列目と3列目が文字、4列目が標準 で変換の場合)

csv2xls -f "1,2,2,1" fuga.csv hoge.xls
※-f の引数は、USAGEにも書いていますが、

1 … 標準
2 … 文字列
5 … 日付
9 … 削除(非表示)

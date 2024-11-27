可変長引数について調べる
slice(index, length) は、配列の指定した位置から指定した長さの要素を取り出すメソッドです。
次のコードの実行

```
count = 0
begin
  1 / count
rescue NameError
  count += 1
  retry
rescue NoMethodError
  count += 2
  retry
rescue ZeroDivisionError
  count += 3
  retry
else
  puts 4
ensure
  puts "count: #{count}"
end
```

Object#eql?メソッドはレシーバと引数の同値性を検証します。
Object#equal?メソッドはレシーバと引数のオブジェクトIDを比較し同一性を検証します。


次のプログラムの実行結果として正しいものを選択してください。
```
arr = [
  true.equal?(true),
  nil.eql?(NilClass),
  String.new.equal?(String.new),
  1.equal?(1)
]

p arr.collect { |a| a ? 1 : 2 }.inject(:+)
```
inject(:+)は配列の要素を合計します。
```
1: io = File.open('list.txt')
2: 
3: while not io.eof?
4:   io.readlines
5:   io.seek(0, IO::SEEK_CUR)
6:   p io.readlines
7: end
```
&&

&&は、Rubyにおける論理 AND 演算子です。条件分岐や論理演算で使用され、両方の条件が真 (true) の場合にのみ全体が真 (true) になります。それ以外の場合は偽 (false) となります。

|| 演算子は

左辺が true の場合、右辺は実行しません。
左辺が false の場合は、右辺は実行します。
&& 演算子は

左辺が true の場合、右辺は実行します。
左辺が false の場合は、右辺は実行しません。
&& 演算子は、両方が真でないときに偽を返すため、1 && nil の結果は nil になります。
```
str = <<EOS
よりニッチに。よりユニークに。
  IT市場はもちろん、ヘルスケア・医療・介護など
    次世代市場における企業や生活者のユーザビリティを向上させる
      サービス、ソフトウェアを開発しています。
    #{1 + 1}
EOS
puts str
```
```
klass = Class.new

hash = {klass => 100}

puts hash[klass]
```
```
arr = ["c", 2, "a", 3, 1, "b"]
arr.sort
p arr
```

productの例
```
[1, 2].product([3, 4])
```
実行結果
 [[1, 3], [1, 4], [2, 3], [2, 4]]
transposeはレシーバーの配列から行と列を入れ替えた配列を作成し返します。

transposeの例
```
[[1, 3],
 [1, 4],
 [2, 3],
 [2, 4]
].transpose
```
実行結果
[[1, 1, 2, 2], [3, 4, 3, 4]]
```
次のプログラムの期待値を得られるように正しいメソッドを選択肢から選んでください。

hash = {price: 100, order_code: 200, order_date: "2018/09/20", tax: 0.8}

p hash.__(1)__
期待値

[100, 0.8]

```
```
IO.writeメソッドは第1引数に指定したファイルを開き、第2引数に指定した文字列の書き込みを行った後ファイル閉じます。第3引数で書き込み開始位置を指定できます。

IO.readlinesメソッドは引数に指定したファイルの内容を全て読み込み、各行を要素に持つ配列を返します。
```
```
Hashクラスについて適切な記述を選びなさい（複数選択）

選択
選択肢
member?でハッシュがキーをもつか判断できる

選択
選択肢
to_aでハッシュから配列を生成できる

選択肢
updateは破壊的メソッドである

選択肢
clearの戻り値は空のハッシュ
```
```
Array#eachはレシーバの各要素に対してブロックの処理を行います。

Array#each_indexはレシーバの各要素のインデックスを渡しブロックの処理を繰り返します。

Enumerable#each_with_indexはレシーバの各要素とインデックスを渡しブロックの処理を繰り返します。
```
```
w+は新規作成・読み込み + 書き込みモードで開きます。
既にファイルが存在する場合は、空になります。
IO#seekはファイルポインタを指定の位置に移動します。IO:SEEK_SETがファイルの先頭からの位置を指定する識別子です。

wは書き込みモードで開きます。
その他はw+と同様です。

a+はファイルを読み込みモード + 追記書き込みモードで開きます。
ファイルの読み込みは、ファイルの先頭から行いますが、書き込みは、ファイルの末尾に行います

aはファイルを追記書き込みモードで開きます。
ファイルの読み込みを行うことはできません。読み込みを行なった場合は、not opened for reading (IOError)が発生します。
```

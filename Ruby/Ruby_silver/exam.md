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

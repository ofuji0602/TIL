
### Part1:  
rakeコマンドについて  
rakeコマンドとはmakeコマンド風にタスクを実行する為のタスクランナー

実行する処理のことをRakeタスクと呼ぶ
RakefileにRakeタスクを記述する。

Rakefile
```
dese"Hello Rake task"
task :hello do
    puts "hello world"
end
```
コマンドで実行するとき

% rake helloで実行できる

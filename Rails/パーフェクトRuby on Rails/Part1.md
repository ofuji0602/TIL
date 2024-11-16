
### Part1:  
## rakeコマンドについて  
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

## Gemfileについて
 
Gemfile
このプロジェクトで利用するgemファイルを定義したファイル

Gemfile.lock
依存関係を解決した結果を保存する


## configディレクトリについて
アプリケーションの設定ファイルなど、アプリケーション起動時に必要な情報を定義するディレクトリ
routes.rbやdatebase.ymlなどがある。

## railsコマンドについて
rails db:drop データベースを削除する。

rails db:setup　データベースを作成し、スキーマの読み込みとシードデータの読み込みを行う。

rails routes　URLとコントローラーを紐づけてルーティング情報を出力する

## CRUDについて
データの基本的な操作を表す概念
Create（作成）Read（読み取り）Update（更新）Delete（削除）

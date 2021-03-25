コードを自動生成する___scaffold（スキャフォールド）___
# 作ってくれるもの
ルーティング    routes.rb内に記述してくれる
コントローラー  resourcesのアクション全て定義してくれる
モデル         マイグレーションファイルも同時に作成してくれる
ビュー         コントローラーで定義したアクションに対応するビューファイルを作成してくれる

# 作る方法

```
% rails g scaffold モデル名 カラム名1:型1 カラム名2:型2...
% rails g scaffold money saving_amount:integer day:date...
```

たくさんのファイルが自動生成される
最後にテーブルを作成する

```
rails db:migrate
```
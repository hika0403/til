# Prefixとは
URIパターンを名前をつけて変数化したもので`rails routeコマンド`で1番左に表示されている。
link_toの遷移はPrefixを使用することが一般的である。

```
URLPatternでの記述
<%= link_to '削除', "/tweets/#{tweet.id}", method: :delete %>

Prefixでの記述
<%= link_to '削除', tweet_path(tweet.id), method: :delete %>
```

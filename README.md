# django + graphql + react
## 目標
1. いろんなクエリを送ってみる
2. どんな場合GraphQLを使った方がいいなのかちゃんと理解する。
3. 依存性などを会社のプロジェットにインストールするため必要なのは？

## セッチング順番
### GraphQL稼働
 * graphQLインストール
 * アプリケーションにschema.py追加 → projectの直下にschema.py追加＆中にアプリケーションのschema.pyをimport → settings.pyにGRAPHENE = {"SCHEMA": "myproject.schema.schema"}追加
 * アプリケーションのurls.pyにpath("graphql/", csrf_exempt(GraphQLView.as_view(graphiql=True))),追加
 * /graphqlに入るとクエリを送れる。

### Reactとの連携




# CSSフレンズ #4「CSSで失敗した暴露話とリファクタリング」

```
$ npm i
$ npm run server
```

## ダメなポイント一覧

- id を重複して使用する
- .adという名前を使ってAdblockにブロックごと抹消される
- 命名規則が直接的すぎる
- HTML 要素に依存したスタイルの適用
- 同じ見た目なのに別名でスタイルあたってる
- `!important` の嵐
- `.mt-10` で、15px 開ける
- キャメルケースとスネークケースを混在する

## Github Pages

`/docs` ディレクトリがそのまま公開されてます。  
<https://cssfriends.github.io/cssfriends-vol4-groupwork/>

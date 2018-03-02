# CSSフレンズ #4「CSSで失敗した暴露話とリファクタリング」

```
$ npm i
$ npm run server
```

## Github Pages

`/docs` ディレクトリがそのまま公開されてます。  
<https://cssfriends.github.io/cssfriends-vol4-groupwork/>

## ダメなポイント一覧

- id を重複して使用する
- .adという名前を使ってAdblockにブロックごと抹消される
- 命名規則が直接的すぎる
- HTML 要素に依存したスタイルの適用
- 同じ見た目なのに別名でスタイルあたってる
- `!important` の嵐
- `.mt-10` で、15px 開ける
- キャメルケースとスネークケースを混在する
- ネストが深すぎる
- 同じスタイルの中で値を上書き
- あまり使うことのない Utility クラス達
- （特殊）`.ad` という名前を使って Adblock にブロックごと抹消される
- `font-size` の指定が px や % や em が混在している

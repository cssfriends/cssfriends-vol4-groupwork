# メンター枠専用

```
$ npm i
$ npm run server
```

## Github Pages

`/docs` ディレクトリがそのまま公開されてます。  
<https://cssfriends.github.io/cssfriends-vol4-groupwork/>

## グループワークで語り合っていただきたいところ

[公開してるページ](https://cssfriends.github.io/cssfriends-vol4-groupwork/) には以下、ダメなポイントがすべて実装されてます。  
これらのソースがどうダメなのか、こうあったほうのでは？等のアドバイスなどを参加者の方と議論・共有していただければと思います。  
CSS の書き方に正解はないと思いますので、メンター様ご自身の経験でお話していただければ幸いです。

また CSS の一部ソースを変更していただきたいです。  
その際にこうすると、こういう変更に弱い等、ダメなポイントを踏まえながらお話していただければと思います。

### ダメなポイント一覧

- id を重複して使用する
	- ダメ → `<section id="section" class="***">`
- px で `width` の値指定
	- `.twitter_btn`
- 命名規則が直接的すぎる
	- 住所 → `.jyuusyo`
- Twitter のリンクに使用しているボタンではない
	- `.twitter_btn`
- HTML 要素に依存したスタイルの適用
	- `section`, `p`, `li`
- 同じ見た目なのに別名でスタイルあたってる
	- `.member .card` と `.member .box`
- `!important` の使用
	- `.hoge .moge` と `.moge`
- `.mt-10` で、15px 開ける
	- `.mt-15 { margin-top: 15px; }`
- キャメルケースとスネークケースを混在する
	- `.hogeMoge` と `.hoge__moge`
- ネストが深すぎる
	- `.member .row .col .box .thumbnail.thumbnail_1 img`
- 同じスタイルの中で値を上書き
	- `.twitter_btn` で `width` 上書き
- あまり使うことのない Utility クラス達
	- 賛否あるかと思いますがみなさまどうされてますか？
- （特殊）`.ad` という名前を使って Adblock にブロックごと抹消される
	- らしいです。
- `font-size` の指定が px や % や em が混在している
	- 統一してほしい。
- メディアクエリがスマホファーストなのか PC ファーストなのかわからない

### 変更してほしい箇所

- `font-size` を body タグのフォントサイズを変更するだけで対応してほしい(CSS)
- 同じスタイルのボタン風なリンクのクラス名を変更してほしい（HTML）
- `!important` を使わない運用

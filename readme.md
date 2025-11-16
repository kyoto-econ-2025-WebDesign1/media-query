# メディアクエリの基礎
## メディアクエリを使って600px以下の時にデザインを変更させることを目的とする

### ファイル構成
このページのファイル構成は以下のようになっている。<br>
/（ルートフォルダ）<br>
├── index.html<br>
└── style.css

### HTMLコードへの必須事項
レスポンシブデザインの必須設定であるViewport の `<meta>` タグが含まれていることに注目してください。
```html
<!DOCTYPE html>
<html lang="ja">
<head>
  ,,,,
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  ,,,,
</head>
<body>
  ,,,,,
</body>
</html>
```

### CSSコード
CSSファイル内で **Media Query** を使用し、デザインを切り替えています。<br>
`@mediaルール`を使って「画面幅が600px以下」という条件を指定し、その条件を満たしたときだけ、以下のスタイルを上書きして適用します。
|`@media (max-width: 600px)`|条件: 画面の最大幅が600px、つまり**600px以下の画面**（スマートフォンなど）で適用されます。|
|:---|:---|
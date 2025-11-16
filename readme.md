#メディアクエリの基礎
##メディアクエリを使って600px以下の時にデザインを変更させることを目的とする

###ファイル構成
このページのファイル構成は以下のようになっている。
/（ルートフォルダ）
├── index.html
└── style.css

###HTMLコードへの必須事項
レスポンシブデザインの必須設定であるViewport の `<meta>` タグが含まれていることに注目してください。
```html
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>簡単なレスポンシブテスト</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="container">
        <h1>画面サイズを変えてみよう！</h1>
        <p>ブラウザの幅を狭くしたり広げたりしてみてください。</p>
        <p>画面幅が 600px 以下になると、背景色と文字の大きさが変わります。</p>
    </div>
</body>
</html>
```
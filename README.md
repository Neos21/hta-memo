# HTA Memo

Windows の HTA (HTML Application) を利用してメモアプリを作りした。


## System Requirements

- Windows 環境 … Windows10 にて動作確認しています。
- Internet Explorer 11 … Edge モードで動作させるため、IE11 推奨です。
- Excel … 最前面表示処理に使用。なくても動作します。Excel 2007 にて動作確認しています。

## How To Use

- `Main.hta` が本体です。直接実行すると、通常の HTA としてウィンドウを開きます。
- `Execute.hta` を実行すると、枠線のないウィンドウを開き、常に最前面に表示させます (最前面表示は内部的に Excel の API を利用するため、Excel がインストールされている必要があります)。
- `Execute.hta` を経由して開いた場合のみ、「Save」ボタン右側の余白部分をドラッグするとウィンドウを移動できます。
- `Main.hta` が開くと、同フォルダに `Memo_YYYY-MM-DD.md` という当日日付のテキストファイルを生成します。
- テキストエリアに文章を入力し、「Save」ボタンもしくは `Ctrl + S` を押下すると、当日日付のテキストファイルに内容を保存します。
- HTA を再起動すると、当日日付のテキストファイルを読み込み再表示します。
- 翌日になると新たに当日日付のテキストファイルを作成するので、日付ごとにメモを残せます。
- テキストエリアで `Tab` キーを押下すると、インデント用に半角スペース2つを入力します。


## Author

[Neo](http://neo.s21.xrea.com/) ([@Neos21](https://twitter.com/neos21))


## Links

- [Neo's World](http://neo.s21.xrea.com/)
- [Corredor](http://neos21.hatenablog.com/)
- [Murga](http://neos21.hatenablog.jp/)
- [El Mylar](http://neos21.hateblo.jp/)
- [Bit-Archer](http://bit-archer.hatenablog.com/)
- [GitHub - Neos21GitHub](https://github.com/Neos21GitHub/)

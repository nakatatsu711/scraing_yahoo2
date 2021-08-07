## 概要
Yahoo検索を自動化するプログラムです。

<br>

検索キーワードが入力されたテキストファイルを読み込みます。  
[Yahoo!JAPAN](https://www.yahoo.co.jp)のトップページから読み込んだ検索キーワードで検索します。  
1番目にヒットしたページに遷移し、URLを取得します。  
検索キーワードとURLをセットにしてテキストファイルに書き出します。



## システム環境
以下で動作確認済みです。  
OS：macOS 10.15.6  
Python：3.6.9



## 実行方法
### ライブラリインストール
以下の2通りの方法がありますので、どちらかでインストールしてください。
```
$ pip install selenium
```
```
$ pip install -r requirements.txt
```


### ChromeDriverについて
ブラウザはGoogleChromeを使用します。  
ブラウザを自動操作するためにはChromeDriverが必要です。

以下から自分のGoogleChromeと同じバージョンのドライバーをダウンロードします。  
https://sites.google.com/a/chromium.org/chromedriver/downloads

ChromeDriverをダウンロードしたら解凍して、任意の場所に配置します。  
そして、`chromedriver_path`のところに自分がダウンロードした場所を指定します。


### 読み込み用のテキストファイル
読み込み用のテキストファイルは、`yahoo2_data.txt`のファイル名でPythonの実行ファイルと同じ場所に配置します。


### 実行
コマンドラインで実行します。
```
$ python scraping_yahoo2.py
```

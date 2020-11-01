# HTML5_CSS_JavaScript_Programing

- [HTML5_CSS_JavaScript_Programing](#html5_css_javascript_programing)
  - [第１章 HTML入門](#第１章-html入門)
    - [Sample1.html](#sample1html)
      - [文字化けが発生する](#文字化けが発生する)
    - [Sample4.html](#sample4html)
      - [imgタグの画像サイズを変更する](#imgタグの画像サイズを変更する)
    - [Sample5.html](#sample5html)
      - [開発者ツールでDOMの操作を行う。](#開発者ツールでdomの操作を行う)
  - [第2章 CSS入門](#第2章-css入門)
    - [Sample12.html](#sample12html)
    - [Sample13.html](#sample13html)
    - [Sample14.html](#sample14html)
  - [第3章 JavaScript入門](#第3章-javascript入門)
    - [変数の宣言](#変数の宣言)
    - [Sample19](#sample19)
    - [Sample20](#sample20)
      - [JavaScriptメソッド](#javascriptメソッド)
  - [参考](#参考)

## 第１章 HTML入門

### Sample1.html

#### 文字化けが発生する

文字コードの指定が必要。
```html
<head>
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
</head>
```
[W3C:HTMLで文字エンコーディングを指定する](https://www.w3.org/International/questions/qa-html-encoding-declarations.ja)

### Sample4.html

#### imgタグの画像サイズを変更する

- width
- height

### Sample5.html

#### 開発者ツールでDOMの操作を行う。

1. Sample5.htmlをブラウザで開く
2. F12キーを押す
3. コンソールタブをクリック
4. 下記を入力
5. ```document.getElementById("title").textContent="hello"```
6. 表示される文字列が変更されることを確認する。

## 第2章 CSS入門

### Sample12.html

2-5-1 ブロックレベル要素とインライン要素  

HTMLタグにはインライン要素とブロックレベル要素がある。

インライン要素は横に並ぶ。親要素の幅に達すると改行され、次の行の先頭から開始される。
- インライン要素
  - a
  - span
  - button
  - input
  - img
  - etc...

ブロックレベル要素は縦にに並ぶ。（矩形領域を確保する。）
- ブロックレベル要素
  - h1
  - h2
  - p
  - div
  - ol
  - ul
  - li
  - etc...

書籍から転記
```
・p要素 = 子要素としてテキストを含む場合
・div要素 = 小要素としていろいろな要素を含む場合
```

### Sample13.html

2-5-2 ボックスモデル  

ボックスモデルでスタイルを指定できるのはブロックレベル要素のみ。

- height : 要素自体の高さ
- width : 要素自体の幅
- padding : 要素自体からborderまでの長さ
- border : 境界線のスタイル
- margin : 要素のborderからほかの要素までの長さ

### Sample14.html

2-5-3 ボックスの位置指定

topとleftスタイルを使ってボックスの位置を調整できる。  
topとleftは親要素からの距離を指定する。  
topは縦。leftは横。  
top, leftを使用する場合は、```position: absolute;```を指定する必要がある。

## 第3章 JavaScript入門

### 変数の宣言

varを使用するのが一般的だったが、意図しない動作を作りやすい問題が知られており、ECMAScript[2015]で```const```と```let```が導入された。

- const
  - 再代入できない変数を宣言する。
  - 代入しようとした場合、TypeErrorが発生する。
- let
  - 再代入可能な変数を宣言する。
- var
  - 再代入可能な変数を宣言する。
  - 変数の再宣言ができてしまう。

### Sample19

デバッグを行う。  
F12キーを押下する。

### Sample20

3-10 DOMの操作  

JavaScriptで番号付きリストに追加/削除する。

#### JavaScriptメソッド

Next  
3-10-2 文書ツリーをたどるためのプロパティ

- .appendChild(li)
  - 番号付きリストに追加する。
- .removeChild(li)
  - 番号付きリストから指定したitemを削除する。
- .appendChild(li)
  - 番号付きリストの末尾に指定したitemを追加する。



## 参考

[ゲームを作りながら楽しく学べるHTML5+CSS+JavaScriptプログラミング［改訂版］](https://nextpublishing.jp/book/8499.html)

[JavaScript Primer](https://jsprimer.net/)  
JavaScriptの参考
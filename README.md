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

## 参考

[ゲームを作りながら楽しく学べるHTML5+CSS+JavaScriptプログラミング［改訂版］](https://nextpublishing.jp/book/8499.html)


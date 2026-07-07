# char-counter
# 文字数カウンター（Char Counter）

入力した文章の **文字数・単語数・割合・残り文字数** をリアルタイムで表示する Web アプリです。  
最大文字数を自由に設定でき、進捗バーやダークモードなどの UI 機能も備えています。

GitHub Pages で公開中：  
https://miyaaak.github.io/char-counter/

---

##  主な機能

###  文字数カウント
入力した文字数をリアルタイムで表示。

###  単語数カウント
スペース区切りで単語数を自動計算。

###  最大文字数の設定
任意の最大文字数を入力可能。

###  割合表示
現在の文字数が最大値の何％かを表示。

###  残り文字数表示
最大値まであと何文字入力できるかを表示。

###  進捗バー（色変化）
- 〜70%：緑  
- 〜100%：オレンジ  
- 超過：赤  

視覚的に分かりやすい進捗バー。

###  ダークモード
ワンクリックでライト／ダークを切り替え。

###  クリアボタン
入力内容をで消去。

###  自動保存（localStorage）
ページを閉じても入力内容が保持される。

---

##  使用技術

- HTML  
- CSS  
- JavaScript（Vanilla JS）  
- GitHub Pages（ホスティング）

---

##  コード概要（主要部分）

```html
<textarea id="text"></textarea>
<p>文字数：<span id="count">0</span></p>
<p>単語数：<span id="words">0</span></p>
<p>割合：<span id="percent">0</span>%</p>
<p>残り：<span id="remain">0</span>文字</p>
<div id="bar-bg"><div id="bar"></div></div>

# char-counter
# 文字数カウンター（Character Counter）

シンプルな文字数カウンター Web アプリです。  
テキストを入力すると、リアルタイムで文字数を表示します。

---

## 📌 公開ページ
GitHub Pages で公開しています：

https://miyaaak.github.io/char-counter/

---

## 🧰 機能
- 入力した文字数をリアルタイムでカウント
- シンプルで軽量な UI
- スマホでも使えるレスポンシブデザイン（textarea を大きめに設定）

---

## 🖥 使用技術
- HTML
- JavaScript（Vanilla JS）

---

## 📄 コード概要

```html
<textarea id="text" placeholder="ここに入力" style="width:100%; height:300px;"></textarea>
<p>文字数：<span id="count">0</span></p>

<script>
  const text = document.getElementById('text');
  const count = document.getElementById('count');

  text.addEventListener('input', () => {
    count.textContent = text.value.length;
  });
</script>

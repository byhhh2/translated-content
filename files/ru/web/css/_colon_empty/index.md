---
title: ':empty'
slug: 'Web/CSS/:empty'
tags:
  - CSS
  - CSS Pseudo-class
  - Layout
  - Reference
  - Web
  - Псевдоклассы
translation_of: 'Web/CSS/:empty'
---
<p>{{ CSSRef() }}</p>

<h2 id="Summary">Описание</h2>

<p>{{ Cssxref("pseudo-classes", "Псевдокласс") }} <code>:empty</code> находит любой элемент, у которого нет потомков. Учитываются элементы и текст (включая пробелы). Комментарии не повлияют на то, что элемент будет рассматриваться как не пустой.</p>

<h2 id="Syntax">Синтаксис</h2>

<pre class="syntaxbox">&lt;element&gt;:empty { <em>/* стили</em> */ }
</pre>

<h2 id="Examples">Примеры</h2>

<pre class="brush: css">.box {
  background: red;
  height: 200px;
  width: 200px;
}

.box:empty {
  background: lime;
}
</pre>

<pre class="brush: html">&lt;div class="box"&gt;&lt;!-- Я буду лаймовым --&gt;&lt;/div&gt;
&lt;div class="box"&gt;Я буду красным&lt;/div&gt;
&lt;div class="box"&gt;
    &lt;!-- Я буду красным, так как перед комментарием стоят пробелы --&gt;
&lt;/div&gt;</pre>

<h2 id="Specifications">Спецификации</h2>

{{Specifications}}

<h2 id="Поддержка_браузерами">Поддержка браузерами</h2>

<p>{{Compat}}</p>
---
title: ':first-of-type'
slug: 'Web/CSS/:first-of-type'
tags:
  - Псевдоклассы
translation_of: 'Web/CSS/:first-of-type'
---
<div>{{CSSRef}}</div>

<h2 id="Описание">Описание</h2>

<p><a href="/ru/docs/CSS" title="CSS">CSS</a> <a href="/ru/docs/Web/CSS/Псевдо-классы" title="Pseudo-classes">псевдокласс</a> <code>:first-of-type</code> находит первого потомка своего типа среди детей родителя.</p>

<h2 id="Синтаксис">Синтаксис</h2>

<pre class="syntaxbox">element:first-of-type { <em>/* стили</em> */ }
</pre>

<h2 id="Пример">Пример</h2>

<p>Этот пример показывает, как применится универсальный селектор, если простой селектор не написан.</p>

<pre class="brush: css">div :first-of-type {
  background-color: lime;
}</pre>

<pre class="brush: html">&lt;div&gt;
  &lt;span&gt;Это span первый!&lt;/span&gt;
  &lt;span&gt;Это span нет. :(&lt;/span&gt;
  &lt;span&gt;что насчёт этого &lt;em&gt;вложенного элемента&lt;/em&gt;?&lt;/span&gt;
  &lt;strike&gt;Это другой тег&lt;/strike&gt;
  &lt;span&gt;Грустно, это тоже нет...&lt;/span&gt;
&lt;/div&gt;
</pre>

<p>...сработает так:</p>

<div>{{EmbedLiveSample('Пример','100%', '120')}}</div>

<h2 id="Спецификации">Спецификации</h2>

{{Specifications}}

<h2 id="Поддержка_браузерами">Поддержка браузерами</h2>

<p>{{Compat}}</p>

<h2 id="Смотрите_также">Смотрите также</h2>

<ul>
 <li>{{Cssxref(":nth-of-type")}}, {{Cssxref(":last-of-type")}}</li>
</ul>
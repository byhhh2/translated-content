---
title: ':left'
slug: 'Web/CSS/:left'
tags:
  - Вёрстка
  - Псевдоклассы
translation_of: 'Web/CSS/:left'
---
<div>{{ CSSRef() }}</div>

<p><a href="/en-US/docs/Web/CSS/Pseudo-classes">Псевдокласс</a> <a href="/en-US/docs/Web/CSS">CSS</a> <strong><code>:left</code></strong> используется с <a href="/en-US/docs/Web/CSS/At-rule">at-правилом</a> {{cssxref("@page")}}, предоставляет все левые страницы печатного документа.</p>

<pre class="brush: css no-line-numbers">/* Выбирает все левые страницы при печати */
@page :left {
  margin: 2in 3in;
}</pre>

<p>Является ли данная страница "левой" или "правой" определяется основным направлением документа. Например, если первая страница имеет основное направление слева направо, то это будет страница с page {{Cssxref(":right")}} ; если первая страница имеет основное направление справа налево, то это будет страница с page <code>:left</code>.</p>

<div class="note">
<p><strong>Примечание:</strong> Этот псевдокласс можно использовать только для изменений следующих свойств элементов страницы: {{ Cssxref("margin") }}, {{ Cssxref("padding") }}, {{ Cssxref("border") }}, и{{ Cssxref("background") }} . Все остальные свойства будут игнорироваться; изменены будут только свойства элементов страницы без изменения содержимого документа.</p>
</div>

<h2 id="Синтаксис">Синтаксис</h2>

{{csssyntax}}

<h2 id="Примеры">Примеры</h2>

<h3 id="Выставляем_отступы_для_левых_страниц">Выставляем отступы для левых страниц</h3>

<pre class="brush: css">@page :left {
  margin: 2in 3in;
}
</pre>

<h2 id="Спецификации">Спецификации</h2>

{{Specifications}}

<h2 id="Поддержка_браузерами">Поддержка браузерами</h2>
<p>{{Compat}}</p>

<h2 id="Смотрите_также">Смотрите также</h2>

<ul>
 <li>{{ Cssxref("@page") }}</li>
 <li>Другие псевдоклассы, связанные с @page: {{ Cssxref(":first") }}, {{ Cssxref(":right") }}</li>
</ul>
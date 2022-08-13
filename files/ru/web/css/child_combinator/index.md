---
title: Селектор дочерних элементов
slug: Web/CSS/Child_combinator
translation_of: Web/CSS/Child_combinator
---
<p>{{CSSRef("Selectors")}}</p>

<h2 id="Summary">Описание</h2>

<p><code>Комбинатор &gt;</code> разделяет 2 селектора, находит элементы заданные вторым селектором, являющие <strong>прямыми </strong>потомками для элементов отобранных первым селектором. Напротив, два селектора в <a href="/ru/docs/Web/CSS/Descendant_selectors">селекторе потомков</a>  находят элементы не обязательно являющиеся прямыми потомками, т.е. несмотря на количество "прыжков" до них в DOM.</p>

<h2 id="Syntax">Синтаксис</h2>

<pre class="eval">selector1 &gt; selector2 { <em>style properties</em> }
</pre>

<h2 id="Example">Пример</h2>

<pre class="brush: css">span { background-color: white; }
div &gt; span {
  background-color: DodgerBlue;
}
</pre>

<pre class="brush: html">&lt;div&gt;
  &lt;span&gt;Span 1 в div
    &lt;span&gt;Span 2 в span, который в div&lt;/span&gt;
  &lt;/span&gt;
&lt;/div&gt;
&lt;span&gt;Span 3. Не в div вообще&lt;/span&gt;
</pre>

<p>{{ EmbedLiveSample('Example', 200, 100) }}</p>

<h2 id="Specifications">Спецификации</h2>

{{Specifications}}

<h2 id="Поддержка_браузерами">Поддержка браузерами</h2>

<p>{{Compat}}</p>
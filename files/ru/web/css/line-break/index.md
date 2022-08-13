---
title: line-break
slug: Web/CSS/line-break
tags:
  - разрыв строки
translation_of: Web/CSS/line-break
---
<div>{{CSSRef}}</div>

<p>CSS-свойство <strong><code>line-break</code></strong> устанавливает способ разрыва строки текста на китайском, японском или корейском (CJK) при работе с пунктуацией и символами.</p>

<pre class="brush:css no-line-numbers">/* Значения ключевым словом */
line-break: auto;
line-break: loose;
line-break: normal;
line-break: strict;

/* Глобальные значения */
line-break: inherit;
line-break: initial;
line-break: unset;
</pre>

<div>{{cssinfo}}</div>

<h2 id="Синтаксис">Синтаксис</h2>

<h3 id="Значения">Значения</h3>

<dl>
 <dt><code>auto</code></dt>
 <dd>Разрыв текста, используя правило разрыва строки по умолчанию.</dd>
 <dt><code>loose</code></dt>
 <dd>Разрыв текста, используя правило разрыва строки с наименьшими ограничениями. Обычно используется для коротких строк, например, в газетах.</dd>
 <dt><code>normal</code></dt>
 <dd>Разрыв текста, используя наиболее распространённое правило разрыва строки.</dd>
 <dt><code>strict</code></dt>
 <dd>Разрыв текста, используя самое строгое правило разрыва строки.</dd>
</dl>

<h3 id="Формальный_синтаксис">Формальный синтаксис</h3>

{{csssyntax}}

<h2 id="Спецификации">Спецификации</h2>

{{Specifications}}

<h2 id="Поддержка_браузерами">Поддержка браузерами</h2>



<p>{{Compat}}</p>
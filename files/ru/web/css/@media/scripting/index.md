---
title: scripting
slug: Web/CSS/@media/scripting
translation_of: Web/CSS/@media/scripting
---
<div>{{cssref}}</div>

<p><a href="https://developer.mozilla.org/ru/docs/Web/CSS">CSS</a> <a href="https://developer.mozilla.org/ru/docs/Web/CSS/Media_Queries/Using_media_queries">медиа функция</a> <code><strong>scripting</strong></code> может использоваться для проверки доступности скриптов (таких как JavaScript)</p>

<h2 id="Синтаксис">Синтаксис</h2>

<p>Функция <code><strong>scripting</strong></code> указывается в качестве значения ключевого слова, выбранного из списка ниже.</p>

<dl>
 <dt><code>none</code></dt>
 <dd>Скрипты полностью недоступны в текущем документе.</dd>
 <dt><code>initial-only</code></dt>
 <dd>Скрипты включаются во время начальной загрузки страницы, но не после.</dd>
 <dt><code>enabled</code></dt>
 <dd>Скрипты поддерживаются и активны в текущем документе.</dd>
</dl>

<h2 id="Пример">Пример</h2>

<h3 id="HTML">HTML</h3>

<pre class="brush: html">&lt;p class="script-none"&gt;You do not have scripting available. :-(&lt;/p&gt;
&lt;p class="script-initial-only"&gt;Your scripting is only enabled during the initial page load. Weird.&lt;/p&gt;
&lt;p class="script-enabled"&gt;You have scripting enabled! :-)&lt;/p&gt;
</pre>

<h3 id="CSS">CSS</h3>

<pre class="brush: css">p {
  color: lightgray;
}

@media (scripting: none) {
  .script-none {
     color: red;
  }
}

@media (scripting: initial-only) {
  .script-initial-only {
    color: red;
  }
}

@media (scripting: enabled) {
  .script-enabled {
    color: red;
  }
}</pre>

<h3 id="Result">Result</h3>

<p>{{EmbedLiveSample("Пример")}}</p>

<h2 id="Спецификация">Спецификация</h2>

{{Specifications}}

<h2 id="Совместимость_с_браузерами">Совместимость с браузерами</h2>



<p>{{Compat}}</p>
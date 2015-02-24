## Nesting

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS
a {
  color: #009;
  &:hover {
    color: #00C;
  }
}

header {
  background-color: #CCC;
  a {
    color: #00A;
  }
}</code></pre>
  </div>
  <div>
<pre><code class="language-css">/\* Compiled CSS \*/
a {
  color: #009;
}
a:hover {
  color: #00C;
}

header {
  background-color: #CCC;
}
header a {
  color: #00A;
}</code></pre>
  </div>
</div>

<p class="small">Nest CSS selectors like you nest the hierarchy of your HTML. Super useful, but tread lightly.</p>

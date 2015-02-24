## Vertical Centering

Vertical centering has always been difficult, but with CSS3's Translate
transformation, it has gotten a lot easier. Toolkit provides a shortcut
mixin for this technique:

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS:
.vc-item {
  @include vertical-center();
}
</code></pre>
  </div>
  <div>
<pre><code class="language-css">/\* Compiled CSS: \*/
.vc-item {
  top: 50%;
  position: relative;
  -webkit-transform: translateY(-50%);
  -ms-transform: translateY(-50%);
  transform: translateY(-50%);
}
</code></pre>
  </div>
</div>

## CSS-Only Triangles

Triangles are easy to make with CSS borders; Toolkit provides a mixin.

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS:
.triangle {
  @include triangle($color: black, $height: 4em, $width: 6em, $angle: 180);
}
</code></pre>
<span style="display: block; margin-top: 2em;"></span>
<span class="triangle"></span>
  </div>
  <div>
<pre><code class="language-css">/\* Compiled CSS: \*/
.triangle {
  display: block;
  width: 0;
  height: 0;
  border: 0 solid transparent;
  border-top-color: black;
  border-width: 4em 3em 0 3em;
}
</code></pre>
  </div>
</div>

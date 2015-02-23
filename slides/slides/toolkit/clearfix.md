## Clearfixes

Toolkit provides a better <code>clearfix</code> mixin than Compass, too.

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS:
@import 'compass';

.container {
  @include clearfix();
}

/\* Compiled CSS: \*/
.container {
  overflow: hidden;
  \*zoom: 1;
}

</code></pre>
  </div>
  <div>
<pre><code class="language-scss">// SCSS:
@import 'compass';
@import 'toolkit';
.container {
  @include clearfix();
}

/\* Compiled CSS: \*/
.container:after {
  content: "";
  display: table;
  clear: both;
}
</code></pre>
  </div>
</div>

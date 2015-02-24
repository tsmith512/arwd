## Creating a 960-esque Layout

Align to columns using the _Grid Span_ mixin: <br />
<code>$span</code> &ndash; number of columns to span &ensp;&bull;&ensp; <code>$position</code> &ndash; starting position

<pre><code class="language-scss">
@include grid-span($span, $position);
</code></pre>

<div class="columns">
  <div>
    <pre class="small scroll-y"><code class="language-scss">// SCSS:
#container {
  @include clearfix; 	// Clear floats
  max-width: 960px;   // Outer Container
  padding: 0 10px;    // Side Gutter
  margin: 0 auto;     // Center Container
}

.left {
  @include grid-span(6,1);
}

.right {
  @include grid-span(6,7);
}
    </code></pre>
  </div>
  <div>
    <pre class="small scroll-y"><code class="language-css">/\* Compiled CSS \*/
#container {
  max-width: 960px;
  padding: 0 10px;
  margin: 0 auto;
  overflow: hidden;
  *zoom: 1;
}

.left {
  width: 48.93617%;
  clear: right;
  float: left;
  margin-left: 0;
  margin-right: 2.12766%;
}

.right {
  width: 48.93617%;
  clear: right;
  float: right;
  margin-right: 0;
}
    </code></pre>
  </div>
</div>

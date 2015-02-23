## Intrinsic Ratios

**[Intrinsic Ratios](http://alistapart.com/article/creating-intrinsic-ratios-for-video):**
a CSS technique to constrain child elements to a particular aspect ratio based on the parent.

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS:

@import "toolkit";

.ratio-16-9 {
  @include intrinsic-ratio;
}

</code></pre>

<p class="small centered">This mixin is applied to the <strong>parent</strong>; <br /> these items will need a wrapper.</p>

  </div>
  <div>

<pre><code class="language-css">/\* Compiled CSS: \*/
.ratio-16-9 {
  position: relative;
  height: 0;
  padding-top: 56.25%; /\* &larr; MAGIC \*/
  width: 100%;
}
.ratio-16-9 > * {
  display: block;
  position: absolute;
  width: 100% !important;
  height: 100% !important;
  top: 0;
  margin: 0;
  padding: 0;
}
</code></pre>

  </div>
</div>

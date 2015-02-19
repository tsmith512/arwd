## Global Contexts

When using the <code>breakpoint</code> mixin, Singularity determines the current
global context to use for the <code>grid-span</code> mixin.

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS:
@include add-grid(2);
@include add-grid(4 at 500px);
@include add-gutter(1/6);

#nav {
  @include grid-span(1,1);

  @include breakpoint(500px) {
    @include grid-span(3, 2);
  }
}

</code></pre>
  </div>
  <div>
<pre><code class="language-css">/\* Compiled CSS: \*/
#nav {
  width: 46.15385%;
  float: left;          clear: none;
  margin-right: -100%;  margin-left: 0;
}
@media (min-width: 500px) {
  #nav {
    width: 74.07407%;
    float: right;       clear: none;
    margin-left: 0;     margin-right: 0;
  }
}
</code></pre>
  </div>
</div>

<p class="small">
  See this example on <a href="http://sassmeister.com/gist/b592e7567fd4bf2eba18" target="_blank">SassMeister</a>.
</p>

## Overriding Global Contexts

If you need to override the global contexts to change the grid you're using (useful to nest a grid), use the <code>layout</code> mixin.

<pre><code class="language-scss">
@include add-grid(12);
@include add-gutter(1/3);

#main {
  @include grid-span(8, 1);

  @include layout(snap((6 2), 1/3)) {
    .left {  @include grid-span(1, 1); }
    .right { @include grid-span(1, 2); }
  }
}
</code></pre>

<p class="small">
  See a built-out working example on <a href="http://sassmeister.com/gist/352e2db3382d1c306cbf" target="_blank">SassMeister</a>.
</p>

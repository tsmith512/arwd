## Global Contexts

<strong>Grids</strong> and <strong>gutters</strong> exist in a global context. <br/>
Declare them once; they're available to reuse each time they're needed.

You can set <em>different global contexts</em> to use at different
<code>min-width</code> breakpoints.

<pre><code class="language-scss">
@include add-grid(12);
@include add-grid(2 8 2 at 500px);

@include add-gutter(1/3);
@include add-gutter(.25 at 532px);
</code></pre>

## Use the Background Grid to visualize the columns

Singularity provides a <code>background-grid</code> mixin to visualize the custom
grid:

<div class="columns">
  <div>
    <pre><code class="language-scss">// SCSS:

// Turn on debugging:
@include sgs-change('debug', true);

#container {
  @include background-grid();
  // ^^ Optional argument: $color: #ddd
}</code></pre>
  </div>
  <div>
    <img src="img/bg-grid.png" alt="Sample background grid" height="339" width="977" />
    <p class="small centered">Grid is approximate</p>
  </div>
</div>

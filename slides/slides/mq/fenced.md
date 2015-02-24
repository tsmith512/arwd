## Fenced Values

Two values creates a <code>min-width</code> / <code>max-width</code> query.

<div class="columns">
  <div><pre><code class="language-scss">// SCSS:
$medium-header: 460px 780px;

#header {
  font-size: 2em;
  @include breakpoint($medium-header) {
    font-size: 2.5em;
  }
}
</code></pre></div>
  <div><pre><code class="language-css">/\* Compiled CSS \*/
#header {
  font-size: 2em;
}
@media (min-width: 460px) and (max-width: 780px) {
  #header {
    font-size: 2.5em;
  }
}
</code></pre></div>
</div>

## Single Value &rarr; <code>min-width</code>

Pass Breakpoint one number to get a min-width query.

<div class="columns">
  <div><pre><code class="language-scss">// SCSS:
$big-btn: 720px;

header a {
  padding: 0.5em;
  font-size: 0.875em;
  @include breakpoint($big-btn) {
    padding: 2em;
    font-size: 1em;
  }
}</code></pre></div>
  <div><pre><code class="language-css">/\* Compiled CSS \*/
header a {
  padding: 0.5em;
  font-size: 0.875em;
}
@media (min-width: 720px) {
  header a {
    padding: 2em;
    font-size: 1em;
  }
}
</code></pre></div>
</div>

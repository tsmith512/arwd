## Explicit Test / Value

Pass a string and a value for a feature / value pair.

<div class="columns">
  <div><pre><code class="language-scss">// SCSS:
$tiny-pager: max-width 620px;

#pager {
  @include breakpoint($tiny-pager) {
    // Drop all the other pager links
    a:not(.prev):not(.next):not(.current) {
      display: none;
    } } }
</code></pre></div>
  <div><pre><code class="language-css">/\* Compiled CSS \*/
@media (max-width: 620px) {
  #pager a:not(.prev):not(.next):not(.current) {
    display: none;
  }
}



</code></pre>

  </div>
</div>

<p class="small">
  This example is the opposite of mobile-first; these styles are
  <strong>specific</strong> to small screens. But this can be useful when
  building specific styles that would be difficult to override.
</p>

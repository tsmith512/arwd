## Combine Tests

String tests together to create more complex media queries.

<div class="columns">
  <div><pre><code class="language-scss">// SCSS:
$tighten-text: (max-width 1000px) (orientation portrait);

#main-article {
  font-size: 1em;
  line-height: 1.375;

  @include breakpoint($tighten-text) {
    line-height: 1.25;
  }
}
</code></pre></div>
  <div><pre><code class="language-css">/\* Compiled CSS \*/
#main-article {
  font-size: 1em;
  line-height: 1.375;
}
@media (max-width: 1000px) and (orientation: portrait) {
  #main-article {
    line-height: 1.25;
  }
}

</code></pre>

  </div>
</div>

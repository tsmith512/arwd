## No-query Fallbacks, Output

<div class="columns">
  <div><p class="filename">&rarr; /style.scss</p>
  <pre><code class="language-scss">// SCSS:
$breakpoint-no-queries: false;
$breakpoint-no-query-fallbacks: false;
@import "config/variables";
@import "components/nav";


</code></pre>
  <p class="filename">&rarr; /style-ie8.scss</p>
  <pre><code class="language-scss">// SCSS:
$breakpoint-no-queries: true;
$breakpoint-no-query-fallbacks: true;
@import "config/variables";
@import "components/nav";</code></pre>
  </div><div>
  <p class="filename">&rarr; /style.css</p>
  <pre><code class="language-css">/\* Compiled CSS \*/
@media (min-width: 500px) {
  nav {
    width: 60%;
    margin-right: 4%;
  }
}</code></pre>
  <p class="filename">&rarr; /style-ie8.css</p>
  <pre><code class="language-css">/\* Compiled CSS \*/
.lte-ie8 nav {
  width: 60%;
  margin-right: 4%;
}</code></pre>
</div></div>

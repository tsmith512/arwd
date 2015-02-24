## No-query Fallbacks, Setup

Breakpoint can also output [fallbacks](https://github.com/at-import/breakpoint/wiki/No-Query-Fallbacks) for when media queries are unsupported.

<div class="columns">
  <div>

<p class="filename">&rarr; /style.scss</p>
<pre><code class="language-scss">// SCSS:
$breakpoint-no-queries: false;
$breakpoint-no-query-fallbacks: false;
@import "config/variables";
@import "components/nav";</code></pre>
<p class="filename">&rarr; /style-ie8.scss</p>
<pre><code class="language-scss">// SCSS:
$breakpoint-no-queries: true;
$breakpoint-no-query-fallbacks: true;
@import "config/variables";
@import "components/nav";</code></pre>
</div><div>
<p class="filename">&rarr; /config/_variables.scss</p>
<pre><code class="language-scss">$nav-lg: 500px, 'no-query' '.lte-ie8';</code></pre>
<p class="filename">&rarr; /components/_nav.scss</p>
<pre><code class="language-scss">// SCSS:
nav {
  @include breakpoint($nav-lg) {
    width: 60%;
    margin-right: 4%;
  }
}
</code></pre>
  </div>
</div>

<p class="small">Just add a conditional class to your <code>&lt;html></code> element.</p>

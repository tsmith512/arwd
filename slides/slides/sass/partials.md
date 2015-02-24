## Partials

<div class="columns">
  <div>
    <p class="filename">&rarr; /style.scss</p>
    <pre><code class="language-scss">@import 'config/variables';
@import 'partials/typography';</code></pre>
    <p class="filename">&rarr; /config/_variables.scss</p>
    <pre><code class="language-scss">$brand-color: #006DAF;</code></pre>
    <p class="filename">&rarr; /partials/_typography.scss</p>
    <pre><code class="language-scss">h1 {
  color: $brand-color
}</code></pre>
  </div>
  <div>
    <p class="filename">&rarr; /style.css</p>
    <pre><code class="language-css">h1 {
  color: #006DAF;
}</code></pre>
  </div>
</div>

<p class="small">Split up Sass into Partials (separate files) to get organized. <br/>
<code class="language-scss">@import "filename";</code> directives <strong>run
server-side</strong>.</p>

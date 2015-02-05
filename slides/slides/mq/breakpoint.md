## Breakpoint

<a href="https://github.com/Team-Sass/breakpoint">Breakpoint</a>, a Compass
extension, <br /> makes media queries easier to write and maintain.

<div class="columns">
  <div><pre><code class="language-scss">@import "breakpoint";

$two-columns: 680px;

.first-column {
  width: 100%;

  @include breakpoint($two-columns) {
    width: 50%;
    float: left;
  }
}</code></pre></div>
  <div><pre><code class="language-css">.first-column {
  width: 100%;
}
@media (min-width: 680px) {
  .first-column {
    width: 50%;
    float: left;
  }
}



</code></pre></div>
</div>

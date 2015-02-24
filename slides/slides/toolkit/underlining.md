## Fancy Underlines

Typographically, underlining text is not ideal, a holdover from typewriters.
<em>Italics</em> are preferred. But on the web, underlining is a
common UX necessity. Toolkit provides a mixin for fancy underlines which
respect descenders.


<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS:
.fancy-underlines {
  @include underline($background: #fff, $color: #00F, $clear-descenders: true, $distance: 0.925, $width: 1);
}
</code></pre>
<span style="display: block; margin-top: 3em;"></span>
<a class="fancy-underlines">typography++</a>
  </div>
  <div>
<pre><code class="language-css">/\* Compiled CSS: \*/
.fancy-underlines {
  text-decoration: none;
  background-repeat: repeat-x;
  background-image: linear-gradient(to top, #fff 75%, #00F 75%);
  background-size: 0.125em 0.125em;
  background-position: 0 0.9875em;
  text-shadow: 0.0625em 0.0625em 0 #fff, -0.0625em 0 0 #fff;
}
</code></pre>
  </div>
</div>

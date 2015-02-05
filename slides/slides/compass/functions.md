## Functions

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS:
@import "compass";

#{headings(1,3)} {
  text-transform: uppercase;
}

#{nest('header, footer', 'ul, ol')} {
  font-size: 0.75em;
}
</code></pre>
  </div>
  <div>
<pre><code class="language-scss">/\* Compiled CSS \*/
h1, h2, h3 {
  text-transform: uppercase;
}

header ul, header ol,
footer ul, footer ol {
  font-size: 0.75em;
}

</code></pre>
  </div>
</div>

<p class="small">
  Learn more about
  <a href="http://compass-style.org/reference/compass/helpers/">helpers</a>,
  <a href="http://compass-style.org/reference/compass/helpers/sprites/">spriting</a>,
  <a href="http://compass-style.org/reference/compass/helpers/urls/">URL handling</a>,
  and a ton of other stuff.
</p>

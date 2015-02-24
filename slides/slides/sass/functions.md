## Functions

<pre><code class="language-scss">@function pixel-to-em($pixel-size, $inherited-font-size: 16px) {
  @return $pixel-size / $inherited-font-size * 1em;
}

button {
  font-size: pixel-to-em(12px); // Returns 0.75em
}</code></pre>

<p class="small">Functions return a single <strong>value</strong>, just like PHP or JS.</p>

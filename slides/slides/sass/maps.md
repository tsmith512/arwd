## Maps

<pre><code class="language-scss">$colors: (
  background: #1A1610,
  foreground: #E6D6BC,
  highlight:  #F05983,
);

body {
  background: map-get($colors, background);
  color: map-get($colors, foreground);
}</code></pre>

<p class="small">Only available in Sass 3.3+. Most like an associative array. Required by Singularity.</p>

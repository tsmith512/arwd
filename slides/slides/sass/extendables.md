## Extendables

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS
.message {
  margin: 1em;
  padding: 1em;
  border: 1px solid #000;
  font-size: 1.2em;
}
.error {
  @extend .message;
  color: #600;
  border-color: #C00;
}</code></pre>
  </div>
  <div>
<pre><code class="language-css">/\* Compiled CSS \*/
.message, .error {
  margin: 1em;
  padding: 1em;
  border: 1px solid #000;
  font-size: 1.2em;
}

.error {
  color: #600;
  border-color: #C00;
}
</code></pre>
  </div>
</div>

<p class="small">Extendables allow you to build upon a common style.</p>

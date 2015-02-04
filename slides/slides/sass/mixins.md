## Mixins

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS
@mixin my-button($color: #0000FF) {
  background-color: $color;
  border-width: 2px solid;
  border-color: lighten($color, 20%);
}
.button-one {
  @include my-button;
}
.button-two {
  @include my-button(#AA0000);
}</code></pre>
  </div>
  <div>
<pre><code class="language-css">/\* Compiled CSS \*/
.button-one {
  background-color: #0000FF;
  border-width: 2px solid;
  border-color: #6666ff;
}

.button-two {
  background-color: #AA0000;
  border-width: 2px solid;
  border-color: #ff1111;
}</code></pre>
  </div>
</div>

<p class="small">Mixins are like functions, but they return blocks of CSS.</p>

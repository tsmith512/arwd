## Mixins

<div class="columns">
  <div>
<pre><code class="language-scss">// SCSS:
@import "compass";

.modal {
  @include box-shadow(1px 1px 2px rgba(0,0,0,0.5));
}

.overlay {
  @include opacity(0.5);
}

</code></pre>
  </div>
  <div>
<pre><code class="language-scss">/\* Compiled CSS \*/
.modal {
  -moz-box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
  -webkit-box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
  box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
}

.overlay {
  filter: progid:DXImageTransform.Microsoft.Alpha(Opacity=50);
  opacity: 0.5;
}</code></pre>
  </div>
</div>

<p class="small">CSS3 mixins add vendor prefixing. There are <a href="http://compass-style.org/index/mixins/" target="_blank">many many more</a>.</p>

## The Box Model

<div class="mid-columns">
  <div>
    <img src="img/boxmodel.png" alt="Box Model" width="485" height="393" />
  </div>
  <div>
    <pre><code class="language-scss">// SCSS:
\*, \*:before, \*:after {
  @include box-sizing('border-box');
}

/\* Compiled CSS \*/
\*, \*:before, \*:after {
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
}
    </code></pre>
  </div>
</div>



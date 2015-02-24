## A Review: The Box Model

<div class="mid-columns">
  <div style="width:60%" />
    <img src="img/box-sizing.png" alt="Box Model" width="650" height="500" style="border:0; box-shadow: none" />
  </div>
  <div style="width:40%" />
    <pre class="small"><code class="language-scss">// SCSS:
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



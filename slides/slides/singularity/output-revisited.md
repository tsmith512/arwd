# Hint: Remember this?
## Grid Output Styles

Out-of-the-box, Singularity offers two output styles. <strong>We were using <em>Float</em>.</strong>

<div class="mid-columns">
  <div>
    <ol class="list-big">
      <li><strong>Isolation</strong>
        <small>Uses negative margins without clears to pull elements into place.</small>
      </li>
      <li><strong>Float</strong>
        <small>Uses floats and clears to stack elements horizontally, like other grid systems.</small>
      </li>
    </ol>
  </div>
  <div>
    <pre><code class="language-scss">
// Change this:
@include sgs-change('output', 'float');

// To this: (or just remove; this is default)
@include sgs-change('output', 'isolation');

// Then try the Gold Challenge again.
</code></pre>
  </div>
</div>




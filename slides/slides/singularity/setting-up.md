## Setting Up The Grid


<pre><code class="language-scss">@include add-grid(12);     // Number of Columns
@include add-gutter(1/3); // Gutter to Column ratio, 20px/60px = 1/3</code></pre>

<ul class="list-big">
  <li><code class="language-scss">@include add-grid()</code>  <strong>Grid Definition:</strong>
    <small>
      For <strong>symmetric grids</strong>, a single integer: the number of equal-width columns. <br/>
      For <strong>asymmetric grids</strong>, a list of integers: each represents a column and the value represents its width relative to other columns.
    </small>
  </li>
  <li><code class="language-scss">@include add-gutter()</code>  <strong>Gutter Definition:</strong>
    <small>The width of a single gutter in relation to a column of width 1.</small>
  </li>
</ul>

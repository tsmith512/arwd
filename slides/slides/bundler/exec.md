## Using Gems in a Bundler-managed Project

Instead of running <code class="language-bash">compass watch</code> or
<code class="language-bash">compass compile</code>, you should use:

<pre><code class="language-bash">
bundle exec compass watch
</code></pre>

Bundler will only use the gem versions selected within the <code>.lock</code> file

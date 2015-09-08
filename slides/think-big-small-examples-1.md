## <em>Big Ideas</em><small> Small Examples</small>

<pre class="fragment"><code>
function curry(fn, arg) {...}

</code></pre><pre class="fragment"><code>function add(a, b) { return a + b }

</code></pre><pre class="fragment"><code>let addTen = curry(add, 10);
addTen(12); // => 22

</code></pre>

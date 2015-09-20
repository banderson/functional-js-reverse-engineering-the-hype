## <em>Big Ideas</em><small> Small Examples</small>

<pre><code>
function curry(fn, arg) {...}

</code></pre><pre><code>function add(a, b) { return a + b }

</code></pre><pre><code>let addTen = curry(add, 10);

addTen(12); // => 22

</code></pre>

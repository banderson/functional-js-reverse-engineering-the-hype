# <em>Functional Components</em>

<code class="javascript"><pre style="text-align: left; font-size: 0.6em">
export function Checkbox({ checked = true, width }) {
  return (
    &lt;input type="checkbox" checked={checked} style={{width}} /&gt;
  );
}
//...
export function WideCheckbox(props) {
  return (
    &lt;Checkbox {...props} style={...props.styles, width: 100} /&gt;
  );
}
</pre></code>


note:
    Put your speaker notes here.
    You can see them pressing 's'.

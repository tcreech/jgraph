FreeBSD supports hierarchical, nested jails.
The `jgraph` tool uses the system `jls(8)` to build a simple Graphviz digraph.

The output can be visualized in a "live" fashion with something like:

```sh
while true; do jgraph ; sleep 2 ; done | dot -Txlib
```

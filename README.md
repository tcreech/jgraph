FreeBSD supports hierarchical, nested jails.

The `jgraph` tool uses the system `jls(8)` to build a Graphviz digraph of this hierarchy.

One use is to visualize the state of all jails in a live fashion:

```sh
while jgraph; do sleep 2 ; done | dot -Txlib
```

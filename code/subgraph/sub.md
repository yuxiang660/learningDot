``` dot
digraph G {
compound=true
subgraph cluster0 { label = " A ";
    a -> b;
    a -> c;
    b -> d;
    c -> d;
}

subgraph cluster1 { label = " B ";
    e -> g;
    e -> f;
}

{rank=same; d; f}
a -> g [constraint=true];
}
```

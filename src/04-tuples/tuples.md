# Tuples
* A tuple is a typed array with a pre-defined length and types for each index.

```
let details: [number, string, boolean] = [21, "PDN", true];
```

## readonly tuple
```
let details: readonly [number, string, boolean] = [21, "PDN", true];
```

## Named tuples
* Provide context for our values at each index.
```
const graph: [x: number, y: number] = [55.2, 41.3];

// but can't access with x, only for annotations for developers and editors 
```

## Destructuring tuples
```
const graph: [number, number] = [55.2, 41.3];
const [x, y] = graph;
```

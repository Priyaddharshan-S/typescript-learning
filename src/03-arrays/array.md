# Arrays
* It can be either explicit or type inference.
* Arrays are type specific in TS. Can't add other datatypes.

```
// Explicit

const names: string[] = ["Priyaddharshan", "leo"]
```

```
// Type inference

const names = ["Priyaddharshan", "leo"]
```

## readonly
* It can prevent arrays from being changed.

```
const names readonly string[] = ["Marry"];
names.push("gold"); // error show
```
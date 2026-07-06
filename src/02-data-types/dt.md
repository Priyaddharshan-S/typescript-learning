
Basic types similair to js:
1. string
2. number
3. boolean
4. null
5. undefined
```
let name = "Priyaddhrshan";
let age = 21;
let positive_mindset = true;
let drawbacks = null;
let girlfriend = undefined;
```

Also contains:
1. any
2. unknown 
3. never
4. void

## any
* Store any type of value, able to change its type whenever needed.
```
let value: any;

value = 10;
value = "Hello";
value = true;
value = [1, 2, 3];

console.log(value);
```
* Use When really needs like calling third-party libraries.
 ## never
 * Similair to any but safer because can't just use it directly without checking or narrowing its type first. 
```
let value: unknown = "Hello";
console.log(value.toUpperCase()); // cause error
```

```
let value: unknown = "Hello";

if (typeof value === "string") {
    console.log(value.toUpperCase());
}
```
## Void
* returns nothing, mostly used for functions.
```
function greet(): void {
    console.log("hello");
}
```

## Never
* represents a values that never occur. It’s used to indicate situations where something is impossible or a function never successfully returns.

### Common Uses;
* Functions that always throw an error.
* Functions that run forever.
* Exhaustive type checking to ensure all possible cases are handled in a switch or conditional statement.
* Preventing impossible property combinations in object types.







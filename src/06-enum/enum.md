# Enums
* An enum is a special class that represents a group of constants.
* IT has String and number

## Numberic enums
* By default, enums will initialize the first value to 0 and add 1 to each additional value.
```
enum count {
    e,  // 0
    t,  // 1
    e   // 2
}
```
* If initialize the first value to 0 means then remaing values are increamented.
```
enum count {
    e=30
    t,  // 31
    e   // 32
}
```
* We can provide custom values to it.
```
enum count {
   e=5
   t=33
   e=22222
}
```

## String Enums
```
enum CardinalDirections {
  North = 'North',
  East = "East",
  South = "South",
  West = "West"
};
// logs "North"
console.log(CardinalDirections.North);
// logs "West"
console.log(CardinalDirections.West);
```
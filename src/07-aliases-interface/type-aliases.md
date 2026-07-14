# Type Aliases
* Type Aliases allow defining types with a custom name (an alias).

```
type Age = number;

let myAge: Age = 25;  // same as let myAge: number

```

## Object Alias
```
type User = {
  id: number;
  name: string;
};

const u: User = { id: 1, name: "Alice" };

```

## Union Types
* A union means “either this type or that type (like or).
```
type ID = string | number;

let userId: ID = "abc123";
let anotherId: ID = 42;

```

## Intersection types
* Intersection means Must satify both at once.
```
type Name = { name: string };
type Age = { age: number };

type Person = Name & Age;

const p: Person = {
  name: "Alice",
  age: 30
};

```
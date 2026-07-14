# Interface
* Interface is a way to define the structure or shape of an object.
* Interfaces are similar to type aliases, except they only apply to object types.
* Doesn't provide actual implementation used to enforce consistency and type safety in code.

```
interface User {
  id: number;
  name: string;
  age?: number; // optional property
}
```
IMPLEMENTATION
```
const u1: User = { id: 1, name: "Alice" };          // valid

const u2: User = { id: 2, name: "Bob", age: 30 };   // valid

const u3: User = { id: 3 };                         // ❌ error, name missing

```

## Interface Merging
* Declaring the same name more than once, ts will automatically merge them into a single definition/
```
interface User {
  id: number;
  name: string;
}

// Declared again with extra properties
interface User {
  age?: number;
}

const u: User = {
  id: 1,
  name: "Alice",
  age: 30
};

```

## Extending Interfaces
An interface can inherit properties from another interface using extends, creating a new type with all the parent’s members plus its own.

```
interface Person {
  name: string;
  age: number;
}

interface Employee extends Person {
  department: string;
}

const emp: Employee = {
  name: "Bob",
  age: 25,
  department: "HR"
};

```
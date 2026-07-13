# Object
```
// Explict typing

const user : {name: string, age: number, city: string} = {
    name: 'leo',
    age: 32,
    city: 'ODY'
}
```

## Optional Properties
* ## Optional Properties
* By default, TypeScript requires all properties in an object to have values. If you want a property to be optional (so it can be left out), you mark it with `?:` .

```
const {name: string, age: number, city?: string} = {
    name: 'leo'
}
```

## Index signature
* Index signatures can be used for objects without a defined list of properties, if changed means show error.
```
const nameAgeMap: { [index: string]: number } = {};
```
* All the values in this object must have key in string and their values in number.
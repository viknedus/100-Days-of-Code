# 100 days of code, day 14

## 1. Testing objects for properties

### A simple Javascript Object

```javascript
var obj = {
  name: "Victor",
  age: 69,
  pic: "https://randompicurl.com",
  friends: ["Frank", "Jim"],
};

console.log(obj.name); // output: Victor
```

Sometimes it is useful to check if the property of a given object exists or not. We can use the `.hasOwnProperty(propname)` method of objects to determine if that object has the given property name. `.hasOwnProperty()` returns `true` or `false` if the property is found or not.

_Example_

```javascript
var myObj = {
  top: "hat",
  bottom: "pants",
};
myObj.hasOwnProperty("top");
myObj.hasOwnProperty("middle");
```

- The first `hasOwnProperty` returns `true`, while the second returns `false`.

_Another Example_

```javascript
function checkObj(obj, checkProp) {
  if (obj.hasOwnProperty(checkProp) == true) return obj[checkProp];
  else return "Not Found";
}
```

- `checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "gift")` should return the string `pony`.
- `checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "pet")` should return the string `kitten`.
- `checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "house")` should return the string `Not Found`.

## 2. Manipulating complex Objects

### Accessing Nested Objects

```javascript
var ourStorage = {
  desk: {
    drawer: "stapler",
  },
  cabinet: {
    "top drawer": {
      folder1: "a file",
      folder2: "secrets",
    },
    "bottom drawer": "soda",
  },
};

ourStorage.cabinet["top drawer"].folder2; // secrets
ourStorage.desk.drawer; // stapler
```

- `ourStorage.cabinet["top drawer"].folder2` would be the string `secrets`, and `ourStorage.desk.drawer` would be the string `stapler`

Here is an example of how to access a nested array:

```javascript
var ourPets = [
  {
    animalType: "cat",
    names: ["Meowzer", "Fluffy", "Kit-Cat"],
  },
  {
    animalType: "dog",
    names: ["Spot", "Bowser", "Frankie"],
  },
];
ourPets[0].names[1]; // Fluffy
ourPets[1].names[0]; // Spot
```

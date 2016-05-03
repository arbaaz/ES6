### ES6
```javascript
let firstName = "John";
let lastName = "Lindquist";

let person = {firstName, lastName}

console.log(person);

let mascot = "Moose";

let team = {person, mascot};

console.log(team);
```
output
----
```javascript
[object Object] {
  firstName: "John",
  lastName: "Lindquist"
}
[object Object] {
  mascot: "Moose",
  person: [object Object] {
    firstName: "John",
    lastName: "Lindquist"
  }
}
```

# Default Values for Function Parameters

### ES5
```javascript
function greet(greeting, name){
  console.log(greeting + ", " + name);
}
greet();

---
output 

undefined, undefined
```

### ES6
```javascript
function greet(greeting, name='Arbaaz'){
  console.log(greeting + ", " + name);
}
greet('hello');

---
output

hello, Arbaaz
```

### ES6
```javascript
var color = "red";
var speed = 10;
var drive = "go";
var car = {
    color,
    speed,
    [drive]: function(){
        console.log("vroom");
    }
};


console.log(car.color);
console.log(car.speed);

car[drive]();

```
output
---
```javascript
"red"
10
"vroom"
```

### ES5
```javascript
var fs = [];
for(var i = 0; i <= 10; i++){
 fs.push(function () {
  console.log(i);
 })
}
fs.forEach(function (f){
  f();
});

output
---
10
10
10
10
10
10
10
10
10
10
10
```
 
```javascript
var fs = [];
for(let i = 0; i <= 10; i++){
 fs.push(() => {
  console.log(i);
 })
}
fs.forEach(f => f() );

output
---
0
1
2
3
4
5
6
7
8
9
10
```


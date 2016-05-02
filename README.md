#Learning ES6

## Arrow Function => in ES6
### ES5
```javascript
var createGreeting = function(message, name){
  return message + name
}
```

### ES6
```javascript
var arrowGreeting = (message, name) => {
 return message + name;
}
```

```javascript
var arrowGreeting = (message, name) => message + name;
```

### ES5
```javascript
var deliveryBoy = {
  name:'John',
  
  handleMessage: function (message, handler){
    handler(message);
  },

  receive:function () {
    var that = this;
    
    this.handleMessage('Hello, ', function (message){
      that.name;//get the proper name
      console.log(message + that.name);
    });
  }
}

deliveryBoy.receive();

```
### ES6

```javascript
var deliveryBoy = {
  name:'John',
  
  handleMessage: function (message, handler){
    handler(message);
  },

  receive:function () {
    this.handleMessage('Hello, ', (message) => {
      console.log(message + this.name);
    });
  }
}

deliveryBoy.receive();

```

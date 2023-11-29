# Javascript Logical Coding Questions
This repository contains questions related to Javascript

> Click :star:if you like the project. Follow me [@krishnateja](https://in.linkedin.com/in/krishna-teja-medam-3320a6135) for more updates. 




### 1. What is the output for the below code and why?

```javascript
(function(){
var a = b = 3;
})();

console.log("a defined? " + (typeof a !== 'undefined'));
console.log("b defined? " + (typeof b !== 'undefined'));

```  

### 2. What is the output for the below code and why?

```javascript
(function() {
    console.log(1); 
    setTimeout(function(){console.log(2)}, 1000); 
    setTimeout(function(){console.log(3)}, 0); 
    console.log(4);
})();
```

### 3. Write a single function that need to satisfy both consoles

```javascript
console.log(sum(2,3));   // Outputs 5
console.log(sum(2)(3));  // Outputs 5
```

### 4. What is the output for the below code

```javascript
console.log(1 +  "2" + "2");
console.log(1 +  +"2" + "2");
console.log(1 +  -"1" + "2");
console.log(+"1" +  "1" + "2");
console.log( "A" - "B" + "2");
console.log( "A" - "B" + 2);
```


### 5. What is the output for the below code

```javascript

console.log(typeof typeof null);
console.log(typeof {});
console.log(typeof []);
```

### 6. What is the output to the console and why?


```javascript
    var myObject = {
        foo: "bar",
        func: function() {
            var self = this;
            console.log("outer func:  this.foo = " + this.foo);
            console.log("outer func:  self.foo = " + self.foo);
            (function() {
                console.log("inner func:  this.foo = " + this.foo);
                console.log("inner func:  self.foo = " + self.foo);
            }());
        }
    };
    myObject.func();
```
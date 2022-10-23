# How to compare two JSON have the same properties without order?


- var obj1={Name: ”Person1”, Age: 5};
- var obj2={Age: 5, Name: ”Person2”};


## Object:
Object are variables which can `store many values`.
Object values are written as `name: value pairs` separated by a comma.

I have tried to compare those two JSON objects. Here, we have two objects such as _obj1 and obj2_. Each object has some properties which is inorder. By using _=== operator_, we are gonna compare those two objects.

_Example:_

```js
var obj1={
    name: "person1",
    age: 5
};
var obj2={
    age: 5,
    name: "person2"
};
console.log(obj1===obj2); 	//false
```

_Output:_

`false`

The output is _False_, because an object is a `non-primitive datatypes`. In non-primitive, it returns the _address of an object_ whereas in primitive datatypes such as Number, String, Boolean,. It returns the value of an object.

_Example:_

```js
var obj1={
    name: "person1",
    age: 5
};
var obj2={
    age: 5,
    name: "person2"
};
var obj1=obj2; 		//gets assigned
console.log(obj1===obj2); 	//true
```
	
_Output:_

	true

Here, we have used an `assignment operator` to assign the values of obj2 in obj1. So that, it holds the same value and gets the output as true.


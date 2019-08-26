# Objects

An object data structure is a pair of curly brackets around zero or more name/value pairs called members.

```js
let exampleObject = {
    name: 'value', // member
    foo: true,
    color: 'red',
    // ...
    count: 12
};
```

 
Each name is a string (like `name` in the example above) with a single colon separating it from the value. Note that all members aside from the very last end with a comma.
 
Names should be unique by convention, so the following example is invalid:

```js
let badNames = {
    title: 'Chef',
    title: 'Teacher',
    color: 'red',
    color: 'blue',
    title: 'Engineer'
};
```
 
All names in an object must be distinct so that any program interacting with the object knows how to parse it. When an object contains duplicate names, you often get unexpected results or an error message.

 
For example, when receiving the `badNames` object from above, some programs reproduce duplicates:
![reproduced duplicates](https://github.com/ellisken/writing_samples/blob/master/staysTheSame.jpg)


 
Other programs take the object and remove all duplicates except for the last name/value pair:

![duplicates removed](https://github.com/ellisken/writing_samples/blob/master/JSFiddle.png)


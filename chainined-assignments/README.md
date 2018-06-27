## Chained Assignments

It is possible to do more than one assignment in a single line. You can have any number of equals signs in a row.  

You can think of chained assignments like passing a note in class.  
* The note is whatever value is written on the far right hand side of the line.
* That value is passed from variable to variable, going from right to left until each one has been assigned the same value.
* When JS has finished executing the chained line, each variable will contain the same value.

If there is anything but a variable
___

### The Code

```js
let var_1 = 1;
let var_2 = 2;

let var_3 = var_2 = var_1 = 3;

let var_4 = 4 = var_3;

let var_5 = var_4 = var_6;
```

[PyTut Link](https://goo.gl/HESWxP)

___

### The Sketches
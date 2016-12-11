##Quarter Checker

<span>A simple JavaScript project which allows to identify a point
quarter based on input values of its 'x' and 'y' axis.</span>

Here is its code:

```javascript
if(isNaN(x) || isNaN(y)) {
   print('Some coordinate was passed with incorrect value');
}

if(x == '' || y == '') {
   print('Some coordinate value is empty');
} else if(x == 0 && y > 0) {
   print('Point is in 2nd or in 1st quarter');
} else if(x == 0 && y < 0) {
   print('Point is in 3rd or in 4th quarter');
} else if(x > 0 && y == 0) {
   print('Point is in 1st or in 4th quarter');
} else if(x < 0 && y == 0) {
   print('Point is in 2nd or in 3rd quarter');
} else if(x > 0 && y > 0) {
   print('Point is in the first quarter!');
} else if(x < 0 && y > 0) {
   print('Point is in the second quarter!');
} else if(x < 0 && y < 0) {
   print('Point is in the third quarter!');
} else if(x > 0 && y < 0) {
   print('Point is in the fourth quarter!');
} else if (x == 0 && y == 0) {
   print('Point is in the beginning of coordinate system!');
}
```
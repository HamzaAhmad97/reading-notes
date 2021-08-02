## Lists and keys

1. The **map()** method returns a new array where each element in the array undergoes some process, or inother workd, we map the original elements and return them in a new array.
2. To loop through an array to display each value in JSK, you will have to use the map method, inside the callback funciton, you will usually return elements containing data or attribute from the original elements in the array, of course you will need to use curly braces if you are doing that inside JSX.

3. Each list item needs a unique **key**.
4. The purpose of key is to help React identify which items have changed, added or removed.

--------------

## The spread operator

1. The spread operator is a unary operator that is used with iterables like lists, when used in the right context, it should return the elements inside that iterable, the iterable itself is a single item or value, but with the spread operator, a number of values get returned.

2.Among the many things the spread operator can do or help with are: 

* Copying arrays:
```
let arr = [1,2,3];
let secondArr = [...arr];
```
* Using arrays as arguments:
```
let arr = [1,2,3];
const func= (a,b,c) => a+b+c;
func(...arr); // this will work is if we passed the arguments individually.
```
* Adding an item to a list:
```
let arr = [1,2,3];
let secondArr = [1,2,...arr];
```
* Combining objects:
```
let objA = { key: val };
let objB = { KEY: VAL};
let objC = {...objA, ...objB};
```
3. An example of using the spread operator to combine two arrays:
```
let arr = [1,2,3];
let ARR = [4,5,6];
let combine = [...arr, ...ARR];
```
4. An example of using the spread operator to add a new item to an array:
```
let arr = [1,2,3];
let secondArr = [1,2,...arr];
```
5. An example of using the spread operator to combine two objects into one:
```
let objA = { key: val };
let objB = { KEY: VAL};
let objC = {...objA, ...objB};
```
--------------

## Passing functions between components

1. The first thing to do to pass functions between components is to define the function inside the component body (before rendering), and then passing it as an attribute, so that it gets referenced via props.
2. In the video, the increment function is is used to check for the card that was clicked by using a map and matching the name stored in the component and the passed name, and if they match, the callback function will increment the count key for that very card, and that will be shown.
3. Via props, by passing the function or the method as an attribute.
4. By making use of props, like `this.props.someFunction()'.

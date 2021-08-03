## React Docs - Forms

1. A controlled component is a component that its state is maintained by React in such away that the state is the signle source of truth from the perspective of React since form fields for example maintain thier own state based on the user input, but to deal with them in React, the React state will be the one to be trusted or controlled.
2. We should update the state as the user types or fills the form fields because we are making the react state the source of truth which also happens to be updated for every change regardless of its size.
3. We target what the user is entering if we have an event handler on an input field by adding an event listener 'onChange()', and assigning it a callback function that will work on changing or updating the state, so eveytime the user changes or modifies his entry, the state will immediately get updated.

-------------------------------
## The Conditional (Ternary) Operator Explained

1. The ternary operator is bit faster than the regular if/ else statements, it also provides a faster way to retrieve values from expressions, so for example, we can just type the value we want to return directly after the **?** in a ternary operator, while in a if/ else statement we will have to type more code that can be avoided. It also allows us to nest more ternary operators with ease.
2. Original code:
```
  if(x===y){
 console.log(true);
  } else {
 console.log(false);
  }
```
New Code:
```
x===y ? console.log(true) : console.log(false);
``` 
note here that the returned value will be undefined since the log method does not return anything.

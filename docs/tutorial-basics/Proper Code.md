---
sidebar_position: 4
---

# Proper Code

Proper Code Etiquette isn't required in ChitChat, but can improve compile time and just make it easier to read. 

## Tests 

When you are defining a test, make sure to make the first word of a test name capitalized, and do not end with punctuation, capital, and or a space. This makes running tests harder to read. This just improved readability. An example of this is:

``` javascript
var test = require('chitchatsjs')
function add(num1, num2) {
  return num1 + num2;
}
// bad
test.TestCase('THIS IS MY FIRST TEST!! ', add(1, 1), () => {
  // ..
  return expectToBeNum(2);
});
// good 
test.TestCase('This is my first test', add(2, 2), () => {
  // ..
  return expectToBeNum(4)
});
```
:::important
While this may only improve readability, it is important to follow this to make it easy on people to look at the tests.
:::
## Expecting

When you are making an expectation, you need to follow proper ChitChat rules. 

When you expect something, always put a return statement in front of it, this improves readability and compile time! An example of this is:

``` javascript
var test = require('chitchatsjs')
function add(num1, num2) {
  return num1 + num2;
}
// bad
test.TestCase('This is an example test', add(10, 10), () => {
  // ..
  test.expectToBeNum(20);
});
// good 
test.TestCase('This is an example test', add(20, 20), () => {
  // ..
  return test.expectToBeNum(40);
});
```
You also should avoid putting more than one expectation in one test, this improves readability. 

That's it for coding etiquette. You should **ALWAYS** follow these rules to improve your tests!

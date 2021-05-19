---
sidebar_position: 1
---

# First Test 

This will be your very first test with `ChitChatjs`! With your newly setup enviorment, it should be easy! 

In your `index.js`, put in the following code:

``` javascript
function add(num1, num2) {
  return num1 + num2;
}
module.exports = add;
```

And in your `tests/mytest.js` file:

``` javascript
var test = require("chitchatsjs");
var add = require("../index.js");
test.TestCase('First Test', add(2, 6), () => {
  return test.expectToBeNum(8); // You don't have to put return, but it is proper etiquette in ChitChatjs to do so
});
```
Then when you run `npm run test`, you should see the prompt:
```
✅  First Test Passed!
```
There you go! That was your first test! If you didn't get any of the stuff that was done, don't worry! In the next page a lot of it will be explained!

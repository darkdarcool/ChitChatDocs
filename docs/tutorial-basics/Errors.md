---
sidebar_position: 3
---

# Errors

Obviously, your going to make some mistakes, like accidentally not filling out a parameter, using incorrect types, ect. So, instead of giving you 15 errors with ChitChatjs for not filling out a parameter, we'll give you one error about one not being filled out. One example of an error is:

``` javascript
var test = require('chitchatsjs')
function divide(num1, num2) {
  return num1 / num2
}
test.TestCase('Example Error Test', () => {
  return expectToBeText(5)
});
```

Did you catch the error? If you didn't, here's a hint, it has something to do with types...

Did you catch it now? If you didn't, no worries! I'll explain it! 

The error is on line **`6`** of the example. The error is an incorrect type. And the error is that you are expecting text! If you look at the function expectation on line **`6`**, you'll see that we are expecting text, and that the error shown in the terminal is:

```
Error: Type given to number function in Example Error Test is not text.
```
This is caused because we made ChitChat think we are expecting text, but then we told it to expect a number! This breaks up type rules, and ChitChat is forced to throw an error at you! This is an example of an error, some errors are on your end and cannot be found by ChitChat.

## Expectation Error

Of course, maybe a function you ae testing at one point doesn't work. That's okay! ChitChatjs let's you know what went wrong! Here is a sample error:

``` javascript
var test = require('chitchatsjs');
function add(num1, num2) {
  return num1 + num2 + 0; // 0 is the error, it is meant to be 1 as + 1
}
test.TestCase('Example test', add(2, 2), () => {
  return test.expectToBeNum(5);
});
```
Of course, the answer your expecting is 5, but the value the function is returning is 4. So, ChitChat will tell you that your function didn't work as expected.

Here is an example TestCase failure:
```
❌  Example test failed.
Expected number:
   5
but received number:
   4
```
You can then go back and look at why your function was returning that value, this let's you know that your function isn't good, and you need to remake it, or, you just have to do a simple bug fix, like this one!

ChitChat will also let you know what type was returned by the function. In the case above, it's a number, but it can be a string, number, and many more!

:::important
If you have a type returned that ChitChat doesn't have a function to catch, please let us know in out [GitHub Repo](https://github.com/darkdarcool/chitchat) so we can fix it as soon as possible!

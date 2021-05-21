---
sidebar_position: 1
---
# Passes

In a TestCase, ChitChat will actually return a value if your test succeeded or not. This can be used for executing code if you test succeeded, or executing another test if it succeeded. This can be used like this:

``` javascript
var isSucceeded;
function add(num1, num2) {
  return num1 + num2
}
TestCase("Example test", add(2, 2), () => {
  return isSucceeded = expectToBeNum(4)
});
if (isSucceeded == true) {
  console.log("Our test succeeded, wahoo!");
}
else {
  console.log("Our test failed :(")
}
```
Since our test succeeded, it prints `Our test succeeded, wahoo!`! You don't have to put a `console.log` there, but that was the example. You can put whatever you want!

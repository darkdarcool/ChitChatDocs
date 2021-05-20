# Passes

In a TestCase, ChitChat will actually return a value if your test succeded or not. This can be used for exacuting code if you test succeded, or exacuting another test if it succeded. This can be used like this:

``` javascript
const test = require("chitchatsjs");
var isSucceded;
function add(num1, num2) {
  return num1 + num2
}
test.TestCase("Example Test", add(2, 2), () => {
  isSucceded = test.expectToBeNum(4)
});
if (isSucceded == true) {
  console.log("Our test succeded, wahoo!");
}
else {
  console.log("Our test failed :(")
}
```
Since our test succeded, it prints `Our test succeded, wahoo!`! You don't have to put a `console.log` there, but that was the example. You can put whatever you want!

### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function(hungry, availableTime) {
  if (hungry && availableTime < 20) {
    console.log("Pick something to eat and eat it in the kitchen.");
  } else if (hungry && availableTime > 30) {
    console.log("Have lunch bit take a shorter time as I'm in bootcamp and here to work hard.");
  } else if (hungry && (availableTime >= 20 && availableTime < 30)) {
    console.log("I deserve a break for lunch, I can go check something out in Kits.");
  } else {
    console.log("Wait to eat until I am actually hungry.");
  }
};

console.log("I'm hungry and I have 20 minutes for lunch.");
whatToDoForLunch(true, 20);
console.log("---");

console.log("I'm hungry and I have 50 minutes for lunch.");
whatToDoForLunch(true, 50);
console.log("---");

console.log("I'm not hungry and I have 30 minutes for lunch.");
whatToDoForLunch(false, 30);
console.log("---");

console.log("I'm hungry and I have 15 minutes for lunch.");
whatToDoForLunch(true, 15);
```
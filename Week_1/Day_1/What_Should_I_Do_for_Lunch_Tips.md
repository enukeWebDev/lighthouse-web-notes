### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
const whatToDoForLunch = function (hungry, availableTime) {
  console.log("I don't know what to do!");
  if (hungry && availableTime < 20) {
    console.log('Not a lot of time... Just pick up something to eat. Sit and eat in the kitchen. Get to know more of your peers!');
  } else if (hungry && (availableTime >= 20 && availableTime <= 30)) {
    console.log('You deserve a break for working hard! Perhaps lunch at Gastown 😀...');
  } else if (hungry && availableTime > 30) {
    console.log('Reminder! This is an intense Bootcamp. Please be mindful of the time you wil spend for lunch!');
  } else {
    console.log("Get back to work!");
  }
};



/*
 * This is some test runner code that's simply calling our whatToDoForLunch function
 * defined above to verify we're making the right decisions. Do not modify it!
 */

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
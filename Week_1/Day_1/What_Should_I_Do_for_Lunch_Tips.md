### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
function whatToDoForLunch(hungry, availableTime) {
  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
}
```

Once you have given it your best go, your code should look something like this:

``` javascript
const whatToDoForLunch = function(hungry, availableTime) {

  if (hungry === true && availableTime < 20) {
    console.log("Pick something up and eat it in the lab.");
  } else if (hungry === true && availableTime >= 20 && availableTime <= 30) {
    console.log("Try a place nearby.");
  } else if (hungry === true && availableTime > 30) {
    console.log("You're in a bootcamp and you should reconsider how much time you have to spare.");
  } else {
    console.log("Get back to work.");
  }
  
}
```
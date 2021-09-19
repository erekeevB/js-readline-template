# js-readline-template

``` javascript
const readline = require("readline");
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

let input = [];

rl.on("line", line => {
  input.push(line.split(" ").map(x => parseInt(x)));
});

rl.on("close", () => {
});
```

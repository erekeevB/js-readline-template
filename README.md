# js-readline-template

``` javascript
const readline = require("readline");
const rl = readline.createInterface({
  input: process.stdin,
  output: process.stdout
});

let input = [];

rl.on("line", line => input.push(line.split(" ").map(x => parseInt(x))));

rl.on("close", () => {
});
```

``` javascript
process.stdin.resume();
process.stdin.setEncoding("utf-8");
let inputs = []
process.stdin.on("data", input => inputs.push(input.split(' ').map(x => parseInt(x));
process.stdin.on("end", () => main(inputs));
```

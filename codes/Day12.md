# 100 days of code, day 11

## Switch statement samples

```javascript
function randomSwitchStatements(val) {
  var answer = "";

  switch (val) {
    case 1:
      answer = "one";
      break;
    case 2:
      answer = "two";
      break;
    default:
      answer = "some random number";
      break;
  }
}
randomSwitchStatements(1); // output: one
randomSwitchStatements(8); // output: three
```

```javascript
function randomSwitchStatements(val) {
  var answer = "";

  switch (val) {
    case 1:
      answer = "one";
      break;
    case "a":
      answer = "apple";
      break;
    case 3:
      answer = "three";
      break;
  }
}
randomSwitchStatements("a"); // output: apple
randomSwitchStatements(3); // output: three
```

```javascript
function randomSwitchStatements(val){
    var answer = "";

    switch(val){
        case 1:
        case 2:
        case 3: answer="one, two, and three!"; break;
        case 4: answer="only four!"; break;
        case 5:
        case 6: answer="five and six!" break;
        default: answer="some random number smh"; break;
    }
}
randomSwitchStatements(1); // output: one, two, and three!
randomSwitchStatements(3); // output: one, two, and three!
randomSwitchStatements(5); // output: five and six!
```

```javascript
function randomSwitchStatements(val) {
  var answer = "";

  switch (val) {
    case "a":
      answer = "apple";
      break;
    case "b":
      answer = "ball";
      break;
    case "c":
      answer = "cat";
      break;
  }
}
randomSwitchStatements("a"); // output: apple
randomSwitchStatements("b"); // output: ball
```

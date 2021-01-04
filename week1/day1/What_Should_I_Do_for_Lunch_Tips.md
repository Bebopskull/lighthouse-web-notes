### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

```javascript
function whatToDoForLunch(hungry, availableTime) {
  if(hungry && availableTime>30){
    console.log(`You are on a bootcamp, please consider if you really want to spend all those ${availableTime} minutes out there!.`);
  }else if(hungry && (availableTime>=20 && availableTime<=30)){
    console.log(`Use those ${availableTime} minutes wisely, probably going to a near place is a good idea.`);
  }else if(hungry && availableTime<20){
    console.log(`${availableTime} minutes is not enought, starve!!.`);
  }else{
    console.log(`Don't even think about it, keep the good work!.`);
  }

  console.log("hungry is", hungry);
  console.log("availableTime is", availableTime);
}
```
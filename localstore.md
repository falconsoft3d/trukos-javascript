```
var colors = ["red","blue","green"];
localStorage.setItem("my_colors", JSON.stringify(colors)); //store colors

var storedColors = JSON.parse(localStorage.getItem("my_colors")); //get them back
console.log(storedColors)
```

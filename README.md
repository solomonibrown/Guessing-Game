# Guessing-Game
<html>
<head>

</head>
<body>
<h3>
I have chosen a number between 1 and 10. Try to guess it
</h3>
<br>
<label>Your Guess</label> <input class="numbers" type="number">
<button onclick="checkInput()"> Submit</button>
  <div id="div1">

  </div>
</body>

<script>

var Usernumber= 10;
var Randomnumber= math.floor(math.random() * Usernumber);

function checkInput(){
  var Attempts = prompt( "I have chosen a number between 1 and 10. Try to guess it");
  var Attempt =  parseInt(Attempts);
while (Attempt != Randomnumber && Attempts != null) {
  var para = document.createElement("p");
  var node = document.createTextNode("This answer i wrong.  "${Attempts}" ");
  para.appendChild(node);
  var element = document.getElementById("div1");
  element.appendChild(para);
  Attempts = prompt( "I have chosen a number between 1 and 10. Try to guess it" , "gang");
  Attempt = parseInt(Attempts);
//while (userInput != Randomnumber) {
  //= document.getElementById('id');
//}

}
var pa = document.createElement("p");
var nod = document.createTextNode("This answer i right.  "${Attempts}" ");
pa.appendChild(nod);
var elemen = document.getElementById("div1");
elemen.appendChild(pa);
console.log("gg");
//var Attempts = prompt( "I have chosen a number between 1 and 10. Try to guess it");
}

</script>
</html>

## HTML Move Cursor To End Of Text
```
function moveCursorToEnd(el){
  var elValue = el.value;
  el.value = null;
  el.value = elValue;
}

//Usage example
var input = document.getElementById("input");
input.addEventListener("focus", function(){
  moveCursorToEnd(input);
});
```

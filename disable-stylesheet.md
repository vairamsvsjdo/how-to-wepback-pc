```
// this disable all style of the website...
var cant = document.styleSheets.length
for(var i=0;i<cant;i++){
    document.styleSheets[i].disabled=true;
}

//this is the same disable all stylesheets
Array.prototype.forEach.call(document.styleSheets, function(element){
  try{
    element.disabled = true;
  }catch(err){}
});
```
# Disable Stylesheet 

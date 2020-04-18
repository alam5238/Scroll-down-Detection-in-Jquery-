# Scroll-down-Detection-in-Jquery-
Scroll down Detection in Jquery for all devices


## Add this function into Jquery document ready body (This script no work for Windows EDGE Browser). 

```

window.onscroll = function() {
  var d = document.documentElement;
  var offset = d.scrollTop + window.innerHeight;
  var height = d.offsetHeight;

  console.log('offset = ' + offset);
  console.log('height = ' + height);

  if (offset >= height) {
  //  var y = $(document).height()/2; 
  //  window.scrollTo(0, y);             //Set scroll-bar position to middle;
    alert('at the bottom');
  }
}
```
## Working edge browser script but it not work for other browser.

```
function getDocumentHeight() {
return Math.max(
    Math.max(document.body.scrollHeight, document.documentElement.scrollHeight),
    Math.max(document.body.offsetHeight, document.documentElement.offsetHeight),
    Math.max(document.body.clientHeight, document.documentElement.clientHeight)
);
}
$(window).scroll(function() {
     var docHeight = getDocumentHeight();
     if($(window).scrollTop() + window.innerHeight == docHeight)
                 {
                  alert('at the bottom');
                 }
        });
```

## please add `<meta name="viewport" content="width=device-width, initial-scale=1, minimum-scale=1, maximum-scale=1">` in `<head>` section of your webpage.

)- **Thank you** -(

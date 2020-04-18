# Scroll-down-Detection-in-Jquery-
Scroll down Detection in Jquery for all devices


## Add this function into Jquery document ready body. 

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

)- **Thank you** -(

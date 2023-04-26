# Welcome to the Web Notifications wiki!

## # Introduction
The package provides services for displaying native web notifications and browser notifications.

NG1 implementation is based on the JQuery library Toastr. You can find information about this library here: [https://github.com/CodeSeven/toastr](https://github.com/CodeSeven/toastr). 

NG2 implementation is based on the NGX-TOASTR. You can find information about this library here: [https://github.com/scttcper/ngx-toastr](https://github.com/scttcper/ngx-toastr)

Example of NG1 toastr options configuration:
```javascript
var options = {
  "closeButton": false,
  "newestOnTop": false,
  "positionClass": "toast-top-full-width",
  "showDuration": "300",
  "hideDuration": "1000",
  "hideEasing": "linear",
  "showMethod": "fadeIn",
  "hideMethod": "fadeOut",
  "progressBar": false
}

plugins.webnotificationsToastr.info("This is my first notification", "Hello Toastr", options);
```

Please consider that:

Two configuration options are missing now in NG2 (showMethod, hideMethod) and [will be added](https://support.servoy.com/browse/SVY-16471) soon (if possible) in a new minor release.


The easing types for NG2 are now based on the CSS animation timings. So in NG1 you can use only "swing" or "linear" for the showEasing and hideEasing options but now in NG2 you have more options like: "ease", "ease-in", "ease-out", "ease-in-out", "linear", "step-start", "step-end". Check the full list here: [https://developer.mozilla.org/en-US/docs/Web/CSS/animation-timing-function](https://developer.mozilla.org/en-US/docs/Web/CSS/animation-timing-function)


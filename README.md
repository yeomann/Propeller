![Propeller.js](http://pixelscommander.com/polygon/propeller/logo.gif "JavaScript library to rotate HTML elements by mouse or touch gestures")

JavaScript library to rotate elements by mouse. Supports inertia and stepwise rotation. It is also compatible with touch devices.

[Demo](http://pixelscommander.com/polygon/propeller/)

##Usage

####Easy-to-use as jQuery plugin:
    $(nodeOrSelector).propeller(options);

####or zero-dependancy library 
    new Propeller(nodeOrSelector, options)

##Performance
Propeller uses requestAnimationFrame and GPU compositing for better performance.
    
##Options
- **inertia** is the most valueble option. It is a number between 0 and 1. 0 means no rotation after mouse was released. 1 means infinite rotation. For this demo we use inertia equals to 0.99.
- **speed** - initial speed of rotation. It also can be used as property in runtime.
- **step** allows to set step in degrees for stepwise mode.
- **stepTransitionTime** enables CSS transition to move from step to step. This makes steps smooth and allows to use CSS transitions easing.
- **stepTransitionEasing** CSS easing mode for transition when in stepwise mode and stepTransitionTime is more than zero. [A bit more about easing functions](http://www.w3schools.com/cssref/css3_pr_transition-timing-function.asp)
- **onRotate** callback executed when rotated. You can easily get current angle as **this.angle** inside of callback function.

##Public properties
- **angle** current propellers angle.
- **speed** current speed of rotation. Degrees per frame.

##License

MIT: http://mit-license.org/

Copyright 2014 Danish Raza [DanishRaza](http://danishraza.info)

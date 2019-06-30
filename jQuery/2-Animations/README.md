# Animations

Animations in jQuery are quite easy to work with and make development incredibly easy once you understand it. Vanilla JavaScript does not have the advanced functions that jQuery has to tackle Animations.

## How

The main animation function of jQuery has 4 parts and I have divided this lesson into those parts. These parts are:
 - [Element](#element)
 - [Parameters](#parameters)
 - [Speed](#speed)
 - [Callback](#callback)

 ## Element

The first part of the animate function is the element. You have to first grab an element by id or class to use the animate funtion on it. For example:
```js
$("#demo").animate();
```
Keep in mind we are missing the other parts of this function so you would experience the error: ``1 argument required, but only 0 present.``

## Parameters
The parameters are the most important part of the animate function. An object is used to define the parameters for this particular function. All css styles are possible to be used in the core animation paramaters but to manipulate color you will need an extra plugin. An example to move an element to the right and and change the height and left margin you would do this:
```js
$("#demo").animate({
    right: "100px",
    height: "20px",
    marginLeft: "10%"
});
```
It is important to remember as demonstrated that css styles with a dash are converted to camel case so margin-left became marginLeft.

## Speed
The speed in jQuery can be used two different ways. The first way is to specify the time in MS, so one second would be 1000. Another way is to use the predefined "fast" or "slow". The speed is how long it will animate for and slow down/speed up to compensate for the time frame. Here is an example of a slow and 1 second animation:
```js
$("#demo").animate({
    right: "100px",
    height: "20px",
    marginLeft: '10%'
}, 1000); // 1000 being 1000 milliseconds or 1 second
$("#demo").animate({
    right: "100px",
    height: "20px",
    marginLeft: '10%'
}, "slow");
```

## Callback
As in most cases of jQuery there is a callback to the animation that fires once the animation has finished or completed. For example:

```js
$("#demo").animate({
    right: "100px",
    height: "20px",
    marginLeft: '10%'
}, "slow", function() {
    console.log("Animation finished!")
});
```

## Other
There are many other animation functions that I have demonstrated below that can also be used:
```js
//Hide/Show
$("#demo").hide("slow");
$("#demo").show("fast");

//Fading
$("#demo").fadeOut("slow");
$("#demo").fadeIn("fast");

//Sliding
$("#demo").slideUp("slow");
$("#demo").slideDown("fast");
```

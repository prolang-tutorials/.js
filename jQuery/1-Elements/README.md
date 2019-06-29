# Elements

jQuery has a very advanced and versatile way of retreiving and using elements. A key point to know about jQuery is that most of it is very different to vanilla JavaScript (Plain JavaScript). For example to get the inner text of a element in JavaScript you would use the object value of .innerText whereas in jQuery you would use .text(); 

# Document and body
Now to get an element in jQuery lets start with something basic, document and body. To use the document in jQuery you run this:
```js
$(document);
```
This immediately retreives the document so you can use it as a jQuery object. The same thing goes for the body of the document:
```js
$(body);
```
# Element by ID
Now for something slightly harder. If you want to retreive an element by ID, rather than use getElementById as used in vanilla JS you would use a # and the element id as shown here:
```js
$("#demo");
```
# Element by Class
This is one of the advantages of jQuery as you can easily fetch an element in much less code than vanilla JS. Now classes are a little different as they can be assigned to multiple elements. Therefore just like with JavaScript's getElementsByClassName we receive an array. To get the first element with the class demo we would do this:
```js
$(".demo")[0];
```
# Examples
The prefixes are exactly like in css with .class and #id. Here are a couple functions you might need in web development:
```js
$("#demo").val(); // The value of the element such as in an input
$("#demo").text(); // The text inside of an element
$("#demo").html(); // The html inside of an element
$("#demo").attr("data-demo"); // The value inside of an attribute such as data-demo
$("#demo").css('display', 'none') // Manipulate the element's css style
```

# Conclusion
In all, elements in jQuery are easy to work with and make web development faster in less lines of code.

# Ajax

Ajax stands for Asynchronous Javascript And Xml. Ajax is just a means of loading data from the server to the web browser without reloading the whole page.
Ajax isn't something new in web development. It is basically just creating a new XMLHttpRequest object to send and receive information to and from a web server asynchronously, in the background!

jQuery is "just" another library that tries to make its implementation easy. Let's see how it works.

Syntax:

```js
$.get(URL,callback)
```

A real-world example:

```js
$.get("/test", function(data, status) {
  alert("Data: " + data + "\nStatus: " + status);
});
```

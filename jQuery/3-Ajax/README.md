
# Ajax

Ajax stands for Asynchronous Javascript And Xml. Ajax is just a means of loading data from the server to the web browser without reloading the whole page.
Ajax isn't something new in web development. It is basically just creating a new XMLHttpRequest object to send and receive information to and from a web server asynchronously, in the background!

jQuery is "just" another library that tries to make its implementation easy. Let's see how it works.
It provides several methods for smooth ajax calls.

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

Alright. But what if you want to pass some data to the server?

Pass some data to the server:

```js
$.ajax({
  method:"GET", // can be lowercase too
  data: {
    some_dumb_info: "this_is_the_info"
  }
}).done(function (response){
  console.log(response)
})
```

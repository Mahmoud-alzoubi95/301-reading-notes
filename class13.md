# Read 13 : Update/Delete

## Client/server architecture

Definition : a client (usually a web browser) sends a request to a server (most of the time a web server like Apache, Nginx, IIS, Tomcat, etc.), using the HTTP protocol. The server answers the request using the same protocol.

## On the client side: defining how to send the data
The `<form>` element defines how the data will be sent and The two most important attributes are action and method.

The method attribute:

The method attribute defines how data is sent.the most common being the `GET` method and the `POST` method

1. The GET method

The `GET` method is the method used by the browser to ask the server to send back a given

2. The POST method

The `POST` method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request


## On the server side: retrieving the data

Whichever HTTP method you choose, the server receives a string that will be parsed in order to get the data as a list of key/value pairs. The way you access this list depends on the development platform you use and on any specific frameworks you may be using with it.

## Security issues

* Each time you send data to a server, you need to consider security. HTML forms are by far the most common server attack vectors

* All data that comes to your server must be checked and sanitized. Always. No exception.



## Summary

* Sending form data is easy, but securing an application can be tricky.
* Front-end developer is not the one who should define the security model of the data


 ## The End
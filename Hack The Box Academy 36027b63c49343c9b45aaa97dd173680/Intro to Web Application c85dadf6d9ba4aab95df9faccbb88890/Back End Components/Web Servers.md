# Web Servers
A web server is an application that runs on the back end server, which handles all of the HTTP traffic from the client side browser, routes it to the requested pages, and finally respond to the client-side browser. Web Servers usually run on port 80 and 443 and are responsible for connecting end-users to various parts of the web application, in addition to handling their various responses.

# Workflow
A typical Web server accepts HTTP request from the client side and respond with different HTTP response code, like a code **200 ok** response for a successful request, a code **404 Not Found** when requesting page that doesn't exist, code **403 Forbidden** for requesting access to restricted pages and so on.

![[Pasted image 20211108102853.png]]

||
--|--
**Code** | **Description**
*suceessful request*|
**200 Ok**	| Request has succeeded
*Redirected Message* |
**301 Moved Permanently** | The URL of requested resource has been changed permanently
**302 Found** | The URL of requested resource has been changed temporarily.
*Client error Message* |
**400 Bad Request** | The server couldn't understand the request due to invalid syntax.
**401 Unauthorized** | Unauthenticated attempt to access page
**403 Forbidden** | The client doesn't have access rights to the content.
**404 Not Found** | The server can not find the requested resource.
**405 Method Not Allowed** | The request method is known by the server but has been disabled and cannot be used.
**408 Request Timeout** | This response is sent on an idle connection by some servers, even without any previous request by the client 
*Server error Responses* |
**500 Internal Server Error** | The Server has encountered a situation it doesn't know how to handle.
**502 Bad Gateway** | The server, while working as a gateway to get a response needed to handle a request , received an invalid response.
**504 Gateway timeout** | The server is acting as a Gateway and cannot get a response time.

Web server also accept various types of user inputs within HTTP request including text **JSON** and even binary data(i.e. for file uploads)
Once a web server receive a web request it is then responsible for routing it to it's destination, run any processes needed for the request and return the response to the user on the client-side. The page and file are that web server processes and routes traffic to are the web application core files.

## Apache or httpd
Apache or httpd is the most common webserver on the internet. 
Apache is usually used with **PHP** for web application development, but it also supports all other languages like **.Net, Python, Perl** and even Os language like **bash** through **CGI**. 

## Nginx
Nginx is second most common web server on the internet. 

## IIS or Internet Information Services
IIS is developed and maintained by **Microsoft .Net framework** 

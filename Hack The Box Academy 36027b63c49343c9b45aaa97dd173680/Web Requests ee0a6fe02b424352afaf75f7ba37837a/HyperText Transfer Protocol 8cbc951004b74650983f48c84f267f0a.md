# HyperText Transfer Protocol

# HTTP

- **HTTP** is an application level protocol.
- HTTP is used to access the resource over the World Wide Web.
- The **hypertext** stands for text containing links to other resources and text that can be easily explain by readers.
- HTTP consist of the client and server , where the client request server for resources.
- The default port for HTTP is 80 *but it can be changed.*
- We entered **Fully Qualified Domain Name(FQDN)** as a **URL(Uniform Requested Locator)** to reach the desired website.

The URL offers much more than just specifying the website.

[[Pasted image 20210921235316.png]]

[Untitled](HyperText%20Transfer%20Protocol%208cbc951004b74650983f48c84f267f0a/Untitled%20Database%201bf7c079c8cd4039933839ad8a213beb.csv)

---

# What happens when we enter URL in browser

[[Pasted image 20210922005508.png]]

- When we enter the url in browser it’s firstly go to DNS to resolve the domain.
- The DNS gives the IP address of the requested website.
- Server can’t communicate without an IP Address we need it.
- [x]  Work with DNS done
- The browser sends the GET request to the default HTTP port; 80 , asking for the root */* folder.
- GET is the request method.
- When a request received for **/** by default server gives an index file.
- As an HTTP response server read and return the content of **index.html**
- The response also give us information such as **200, OK** means request processed successfully.`
# HEADERS

# HEADERS

HTTP Headers provide an additional way to pass information between client and the server. Headers can have one or multiple values appends after the header name and separated by colon. There are different headers used for different categories :

`General Headers` `Entity Headers` `Request Headers` `Response Headers` `Security Headers`

---

## General Headers

The headers don’t belong especially to any request or response. They are contextual and are used to describe a message rather than its contents.

[[Pasted image 20210922123254.png]]

[Untitled](HEADERS%20b695dbc1ea134dde8ed3d6b3ae89717f/Untitled%20Database%20e4b905e8298e4c2683a52662143fdb38.csv)

---

## Entity Headers

Entity headers are similar to general header they are common to both the request and response. These headers are used to describe the entity(content) being transferred by a message.

- *Found in response and PUT or POST request (ex. upload a file)

[[Pasted image 20210922173724.png]]

[Untitled](HEADERS%20b695dbc1ea134dde8ed3d6b3ae89717f/Untitled%20Database%20f4cbb1a2098f474094e24ad926ab7a6f.csv)

[[Pasted image 20210922192753.png]]

---

## Request Headers

The client send request headers in HTTP transaction. These headers are used in an HTTP request and do not relate to the content of the message. Headers such as **Accept, Accept-* and IF-*** allow for conditional requests. Headers such as **Cookie** or **User-agent** are sent so that server can tailor the response.

[Untitled](HEADERS%20b695dbc1ea134dde8ed3d6b3ae89717f/Untitled%20Database%20a0471618cb354f74b6e77ef935bead0d.csv)

[[Pasted image 20210922203215.png]]

---

## Response Headers

Response headers are used in HTTP response and don’t relate them with message content. Certain response headers such as **Age, Location, Server** are used to provide more context about the response.

[Untitled](HEADERS%20b695dbc1ea134dde8ed3d6b3ae89717f/Untitled%20Database%207b2494f3c2cd40e69d5fa5b91e80aa84.csv)

[[Pasted image 20210922210601.png]]

---

## Security Headers

With the increase variety of browser or web based attacks , it was necessary to define certain header that enhance the security. HTTP Security headers are a class of response header used to clarify certain rules and policies to be followed by the browser while accessing the website.

[Untitled](HEADERS%20b695dbc1ea134dde8ed3d6b3ae89717f/Untitled%20Database%20e321c48e119e4c4980823b01c6fc8fa7.csv)

[[Pasted image 20210922213142.png]]

For more [headers](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers)

---
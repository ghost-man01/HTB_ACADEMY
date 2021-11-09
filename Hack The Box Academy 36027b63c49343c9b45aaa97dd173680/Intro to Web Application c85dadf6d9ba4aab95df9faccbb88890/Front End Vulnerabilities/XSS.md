# XSS

HTML injection vulnerabilities can often be used utilized to also perform Cross-site Scripting attacks by injecting JavaScript Code to be executed on the client-side.
Once we can execute code on victim's machine, we can potentially gain access to the victim's account or even their machines. 
XSS very similar to HTML injection in practice. However, XSS involves the injection of JavaScript code to perform more advanced attacks on the client-side, instead of merely injecting HTML code.  There are three main types of XSS:

||
--|--
**Reflected XSS** | Occurs when user input is displayed on the page after processing (e.g. search result or error message.)
**Stored XSS** | Occurs when user input is stored on the back end databases  and then displayed upon retrieval (e.g posts or comments)
**DOM XSS** | Occurs when user input directly shown in the browser and is written to an HTML DOM object (e.g. vulnerable username or page title).

We are trying to inject following **DOM XSS JavaScript** code as a payload which should show us the cookie value for the current user:
```jsx
"><img src=/ onerror=alert(document.cookie)> 
```
This payload is accessing the HTML document tree and retrieving the cookie object's value. 

An attacker can leverage to steal this cookie session and send them to themselves and attempt to use the cookie value to authenticate to the victim's account. The same attack can be used to perform various types of other attacks against a web application's users.  



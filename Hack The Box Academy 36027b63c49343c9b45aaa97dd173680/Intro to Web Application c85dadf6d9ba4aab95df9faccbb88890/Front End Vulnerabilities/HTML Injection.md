# HTML Injection
Another major aspect of front end security and sanitizing accepted user input. In many cases, user input validation and sanitization is carried out on the back end. 
HTML injection occurs when unfiltered user input is displayed on the page. This can either through retrieving previously submitted code, like retrieving a user comment from the back end database, or by directly displaying unfiltered user input through JavaScript on the front end.

When a user has complete control of how their input will be displayed , they can submit HTML code, and the browser may display it as part of the page. This may include a malicious HTML code, like an external login form which can be used to trick user into logging into in while actually sending their login credentials to a malicious server to be collected for other attacks.

Another example of  HTML Injection is a web page defacing. This consists of injecting new HTML code to change the web page's appearance, inserting malicious ads, or even more completely changing the page. This type of attack can result in servere reputational damage to the company hosting on the web application.

If no input sanitization is in place, this is potentially an easy target for HTML injection and XSS

\<style> body { background-image: url(https://image.com/); } \</script>



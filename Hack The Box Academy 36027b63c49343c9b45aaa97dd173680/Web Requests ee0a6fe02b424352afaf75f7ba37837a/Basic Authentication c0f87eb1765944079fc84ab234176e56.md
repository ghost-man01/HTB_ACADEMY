# Basic Authentication

# Basic Access Authentication

Basic access authentication is a method for an HTTP user agent (eg web browser) to provide user name and password when making a request. In basic authentication a request contains a header field in the form of `Authorization:Basic <credentials>` where credentials are Base64 encoding of ID and password joined by single colon`:`

## features

HTTP Basic Authentication implementation is simplest technique for enforcing access control to web resources because it doesn’t require cookie, session identifiers and login pages rather HTTP authentication uses standard fields in the HTTP header.

## Security

The BA mechanism doesn’t provide confidentially protection for the transmitted protocols. They are only encoded with Base65 in transit and not encrypted or hashed in any way. Therefore BA is used in conjunction with HTTPS to provide confidentially. Because the BA needs the header in every HTTP request, so that web browser cached the credentials for a reasonable period of time to avoid the constantly promoting user their username and password.
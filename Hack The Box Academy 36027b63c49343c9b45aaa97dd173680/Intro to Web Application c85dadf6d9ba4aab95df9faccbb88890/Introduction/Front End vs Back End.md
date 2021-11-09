# Front End Development
Aside from frontend code development, the following are some of the other tasks related to front end web development.

- Visual Concept Web Design
- User Interface (UI) design
- User Experience (UX) design

## Back-End Server
The back end of a web application drives all of the core web application functionalities, all of which is executed at the back end server, which process everything required for the web application to run correctly.

||
--|--
**Component** | **Description**
**Back end Servers** | The hardware and operating system that hosts all other component and are usually run on operating system like **Linux, windows and containers.**
**Web Servers**  | Web servers handle HTTP requests and connection. Some examples are **Apache, Nginx and IIS**.
**Databases** | Databases(DBs) store and retrieve the web applications data. Some examples of relational databases are **MySQL, MSSQL, ORACLE, PostgreSQL**, while examples of non-relational databases include **NoSQL and MongoDB.**
**Development Frameworks** | Development frameworks are used to develop the core Web Application. Some well-known frameworks include **PHP, C# , JAVA, PYTHON & NodeJS JavaScript. 

![[Pasted image 20211107181228.png]]

It's also possible to host each component of the back end on it's own isolated server, or in isolated containers, by utilizing services such as **Docker.** 
Some of main jobs  performed by back end components include :
- Develop the main logic and services of the back end of the web application.
- Develop the main code and functionalities of the web application.
- Develop and maintain the back end database.
- Develop and implement libraries to be used by the web applications.
- Implement technical/business needs for the web application
- Implement the main **API** for the front end component communications.
- Integrate remote servers and cloud services into the web application.

## Securing front/back end
In most cases we don't have access to back end code to analyze individual functions and the structure of the code, it doesn't make the application invulnerable. **SQL injection** and **Command Injection** are front end attacks.
**Local File Inclusion** could allow us to obtain the source code from the back end server. 

The Top 20 most common mistakes web developers make that are essential for us as penetration testers are :

1. Permitting invalid data to enter database.
2. Focusing on the system as a whole.
3. Establishing personally developed security methods
4. Treating security to be your last step
5. Developing plain text password storage.
6.  Creating weak passwords.
7.  Storing unencrypted data in the database
8.  Depending excessively on the client side.
9.  Being too optimistic
10.  Permitting variables via the URL path name.
11.  Trusting third-party code.
12.  Hard-coding backdoor accounts.
13.  Unverified SQL injections.
14.  Remote file inclusion
15.  Insecure data handling 
16.  Failing to encrypt data properly
17.  Not using a secure cryptographic system
18.  Ignoring layer 8
19.  Review user actions
20.  Web application firewall misconfigurations

These mistakes lead to OWASP TOP 10 vulnerabilities :

1. Injection 
2. Broke Authentication
3. Sensitive Data Exposure
4. XML External Entities (XXE)
5. Broken Access Control
6. Security Misconfiguration
7. Cross-site Scripting (XSS)
8. Insecure Deserialization
9. Using Component with known Vulnerabilities 
11. Insufficient Logging & Monitoring 


# Introduction

- Web applications are interactive application that run on web browsers.
- Web applications usually adopts **client-server architectures** to run interactions.

![Untitled](HTB_ACADEMY/Hack%20The%20Box%20Academy%2036027b63c49343c9b45aaa97dd173680/Intro%20to%20Web%20Application%20c85dadf6d9ba4aab95df9faccbb88890/Introduction/Untitled.png)

Client-server Architecture

- They have front end components [ "The website interface or what users see" ] that run on client-side(browsers) and other back end components (web application source code) that run on server side (back-end server/databases)

  

# Web Application vs Web sites :

## Web Sites :

- The websites that are static cannot be changed in real-time.
- Traditional websites were statically created to represent specific information, they cannot be  change with our interactions.
- To change these websites content, the corresponding page has to edited by developers manually.
- These types of static pages do not contain functions, and therefore do not produce real time changes.
- These types of websites also known as **web 1.0**

![Untitled](HTB_ACADEMY/Hack%20The%20Box%20Academy%2036027b63c49343c9b45aaa97dd173680/Intro%20to%20Web%20Application%20c85dadf6d9ba4aab95df9faccbb88890/Introduction/Untitled%201.png)

## Web Application :

- Most websites run web application or **web 2.0**
- They present dynamic content based on user experience.
- Fully functional and can perform various functionalities for the end-user
- Being modular running on any display size
- Running on any platform without being optimized.

## Web Applications vs Native Operating System Application :

### Advantages of WEB APPLICATIONS over Native OS Applications

- **Unlike Native OS application Web Applications are platform-independent**
    - Native OS application can run only on native OS.
    - Web applications are platform-independent and can run in a browser on any OS.
    - Web Applications don't need to install on user's OS and hence do not consume any space in end user's hard drive.
    - Web applications have functionality an executed remotely on the remote server.

  

- **Web applications are** **Version unity**.
    - All users accessing a web application use the same version and the same web application.
    - Which can be continuously update and modified without pushing updates to each user.
    - Web application can be updated from single location (webserver), without developing different builds for each platform.
    - It reduces maintenance and support costs removing the need to communicate changes to all users individually.
    

### Advantages of Native OS Application over Web Application

Mainly their operation speed and the ability to utilize native operating system libraries and local hardware.

Native application are built to utilize Native OS libraries they are much faster to load and interact with.

Native OS are more capable than web applications, as they have deeper integration to the operating system and are not limited to the browser's capabilities only.

> Most recently, **hybrid and progressive web application** are becoming more common. They utilize modern frameworks to run web applications using native OS capabilities and resources, making them faster than regular web applications and more capable.
> 

**Content Management System (CMS) such as Wordpress.**

We often find SQL injection vulnerabilities that uses Active Directory for authentication. 

A successful Password Spraying can often lead access to sensitive data such as email or even foothold directly into the corporate network environment.

||
--|--|--
**Flaw** | **Real world scenario** Status
**SQL  Injection** | Obtaining active directory username and performing password spraying attack against via VPN or email portal.,
**File Inclusion** | Reading source code to find hidden pages or directory which exposes additional functionality that can be used to gain RCE,
**Unrestricted File Upload** | A web application that allows a user to upload a profile picture that allows any file type to be uploaded (not just images). This can be leveraged to gain full control of the web application server by uploading malicious code.",
**Insecure Direct Object Referencing** | When combined with a flaw such as broken access control, this can often be used to access user's file or functionality. Editing your user profile browsing to a page such as /user/701/edit-profile. If we change 701 to 702 we may edit another user's profile.",REAL WORLD SCENARIO
**Broken Access Control** | Another example is an application that allows a user to register a new account. If the account registration functionality is designed poorly, a user may perform privilege escalation when registering. Consider the POST request when registering a new user, which submits the data username=bjones&password=Welcome1&email=bjones@inlanefreight.local&roleid=3. What if we can manipulate the roleid parameter and change it to 0 or 1. We have seen real-world applications where this was the case, and it was possible to quickly register an admin user and access many unintended features of the web application.",



# Web Enumeration

## Gobuster

To check there is no hidden directories or files that are not intended for the public access.
#Tools -- ffuf or gobuster
Sometimes we will find hidden functionality  or pages/directories sensitive data that can leverage to the web application or remote code execution on the web server itself.

## Directory file enumeration

**Gobuster allow:** -- **perfoming DNS, vhost and Directory brute-forcing**.

**Additional functionality** -- **enumeration of public AWS S3  buckets**

**switch** -- for directory/files brute-forcing mode specified with ** dr **

### **#Http Status codes**

200 -- Resources request was successful
403 -- We are forbidden to access the resource.
301 -- We have been redirected

## Subdomain Enumeration

#Tools -- Seclist

There is may be subdomain contain resources such as admin panel or application that can be exploited.

To enumerate subdomains using the gobuster we use flag`dns` to specify dns mode.

**Seclists** contain many lists for fuzzing or exploitation.

After installing seclist, Adding dns 1.1.1.1 to **/etc/resolv.conf**

## Banner Grabbing / Web server headers

#Tools  -- 	cUrl

We can use the **curl** to retrieve the server header from the command line.

**`curl -IL website/ip`**

#Tools  -- **Eyewitness** which is used to take screenshots of target web application.

## What Web

#Tools  --- What web

**Work** -- To extract the version of web servers , supporting frameworks, and application

This information can helpful us  at pinpoint the technologies in use and begin to search for potential vulnerabilities.

What-web is a handy tool and contain much functionality to automate web application enumeration across a network .

## SSl/Tls

Ssl / Tls are another valuable source of information if HTTPS in use.

## Robots.txt

<s class=aside-hide>Robots.txt is a common website file whose purpose is to instruct search engines web crawlers, which resources can or cannot be accessed for indexing. </s>

**Information Provide**  --   **location of private files and admin pages**.
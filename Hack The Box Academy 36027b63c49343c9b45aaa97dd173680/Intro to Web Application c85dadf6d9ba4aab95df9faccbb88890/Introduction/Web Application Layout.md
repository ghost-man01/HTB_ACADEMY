# Web Application Layout.
No web applications are identical. 
Web Application layout consists of many different layer that can be summarized with the following three main categories :
||
--|--
**Category** | **Description**
**Web Application Infrastructure** | Describes structure of required components, such as the databases, needed for web application to function as intended. Since the web application can be set up to run on a separate server, it is essential to know which databases server it needs to access.
**Web Application Components** | The components that make up a web application represents all the components that the web application interact with. These are divided into three three areas : **UI/UX , Client and Server** Components. 
**Web Application Architecture** | Architecture compromises all the relationship between various web application components.

## Web Application Infrastructure
Web Application Infrastructure can use many different infrastructure steps. These are also called **Models**. The most common ones can be grouped into following four types :

- Client-Server
- One Server
- Many Servers - One database 
- Many Servers - Many databases 

### Client Server
Web application often adopt the **client-server** model. A server hosts the web application in a client-server model and distributes it to any clients trying to access it.

![[Pasted image 20211107105031.png]]

In this model web application model have two types of components, those in the front end which are usually interpreted and executed on the client-side(browser) and components in the back end, usually compiled, and executed by the hosting server.

- When client visits the web application's URL (web address i.e., https://acme.local), the server uses the main web application interface (**UI**).
- Once a user clicks on a button or request a specific function the browser sends a HTTP web request to the server, which interprets the request and perform the necessary tasks to complete the request (i.e logging user in , adding an item to cart).
- Once server has required data, it sends the result back to the client-browser.
- However even though most web application utilize a client-server front-back end architecture , there are many design implementations.

## One Server
In this architecture the entire web application or even several web application and their components, including the database are hosted on a single server. Though this design is straightforward and easy to implement, it is also riskiest design. 

![[Pasted image 20211107111029.png]]

If any of the hosted web application is vulnerable, the entire webserver becomes vulnerable.

## Many Servers - One database
This model separates the database onto its own database server and allows the web applications' hosting server to access the database server to store and retrieve data. It can be seen as many-server to one-database and one-server to one-database as long as database is separated on it's own database server.

![[Pasted image 20211107112036.png]]

This model can allow several web application to access a single database to have access to the same data without syncing the data between them. The web application can be replicates  of one main application (i.e primary/backup) or they can be separate web application that share common data.

This model 's main advantage is (from security point of view) is **segmentation**, where each of the main components of a web application is located  and hosted separately. 
In case one webserver is compromised other is not affected directly. Similarly if the database is compromised (sql injection) the web application itself is not directly affected.
There are still access control measure that need to be implemented after asset segmentation, such as limiting web application access to only data needed to function as intended.

## Many Servers - Many Databases
This model builds upon the **Many Servers, one database** model. However within the database server each web application's data is hosted in a separated database. The web application only access private data and only common data that is across web applications. It is also possible to host each web application's database on it's separate database server.

![[Pasted image 20211107114234.png]]

This design is also widely used for redundancy purpose, so if any web server or database goes offline, a back up will run it's place to reduce downtime as much as possible. Although this may be more difficult to implement and may require tools like **load balancers** to function appropriately, this architecture is one the best choices in the terms of security due to it's proper access control measure and proper segmentation. 

Aside from  these models, there are other web application models available such as **serverless** we application or web application that utilizes **microservices**. 

# Web Application Components
Each web application can have a different number of components. 
1. **Client**
2. **Server**
	1. Webserver 
	2. Web Application Logic
	3. Database

3. **Services** (Microservices)
	1. Third Party Integrations
	2. Web Application Integrations

4. **Functions** (Serverless)

# Web Application Architecture
The components of a web application are divided into three different layers.

||
--|--
**Layer** | **Description**
**Presentation Layer** | Consists of UI process components that enable communication with the application and the system. These can be accessed by the client via web browser and are returned into the form of HTML, JavaScript and CSS.
**Application Layer** | This layer ensures that all client request(web browser) are correctly processed. Various criteria are checked, such as authorization privileges and data passed on the client. 
**Data Layer** | The data layer works closely with the application layer to determine exactly where the required data is stored and can be accessed.

![[Pasted image 20211107165309.png]]

## Microservices
 We can think of microservices as independent components of the web application, which in most cases programmed for one task only. For example for an online store we can decompose core task into following components :
 - Registration 
 - Search 
 - Payments 
 - Rating 
 - Reviews

 These components communicate with the client and with each other. The communication between the microservices is **stateless** which means that the request and response are independent.  This is because the stored data is **stored separately** from the respective microservices. The use of microservices is considered **service-oriented architecture(SOA)** 
 Another essential and efficient microservices components is that they can be written in different programming languages and still interact. Microservices benefit from easier scaling and faster development of application, which encourage innovation and speeds upmarket delivery of new features. Some benefits of microservices include :
 - Agility 
 - Flexibility 
 - Easy development
 - Reusable Code
 - Resilence

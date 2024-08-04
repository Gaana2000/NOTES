# Serverless Security 

Serverless security is the layer of protection added to the applications to secure code functions within the applications hosted by cloud providers, giving developers compliance and security posture over applications they are developing. 
Serverless security could have risks when it comes to increased attack surfaces, insecure configurations, and broken authentication.


# How does security work in Serverless?

When you go serverless, it's the serverless provider (eg. AWS lambda, Google Cloud Functions etc) that's responsible for securing all the cloud components such as data center, network, servers, operating systems and its configurations.However this merely reduces the security burden shouldered by the developer and doesn't negate it. From the application side of things, the application developer is still responsible for application logic, code, data, and application-layer configurations, making it is a shared security responsibility.

1. **Broken Authentication**

Serverless applications are architected in microservice-like system design which often contain hundreds of distinct serverless functions with their own purposes. Some may expose public web APIs, while others may serve as a proxy to different functions or processes. It's mandatory to apply robust authentication schemes, which provides proper access control and protection to every relevant function, event type and trigger.An example of such an attack would be “Exposing Unauthenticated Entry Point via S3 Bucket with Public Access”.


2. **Insecure Serverless Deployment Configuration**

Serverless architecture is still new and provides different customisation and configuration settings for any specific need, task and environment. The probability of misconfiguring critical configuration settings are quite high and can lead to catastrophic data losses. It's vital to make functions stateless while designing serverless architectures and also to make sure that sensitive data isn't exposed to the any unauthorized personnel. It's also recommended to properly make use of cloud hardening methods and proper ACL configurations.


3. **Over-Privileged Function Permissions and Roles**


It's always wise to follow the Principle of “Least Privilege”. Which technically means serverless functions should only be given necessary privileges to perform the intended logic. Provisioning over privileges to a serverless function could end up being abused to perform unintended operations such as ‘Executing System Functions’.

4. **Denial of Service & Financial Resource Exhaustion**

Denial of Service (DoS) attacks can also be targeted within serverless architectures as they're a pay-per function based model. Denial of Service attacks on serverless application can cause financial and resource unavailability disasters. To avoid such financial disasters and service downtime, It is vital for the application developer to properly define execution limits while deploying the serverless application in the cloud.
 

5. **Improper Exception Handling and Verbose Error Messages**


In all serverless applications, performing line-by-line debugging is more complicated and limiting compared to standard applications. However, the above factor forces developers to adapt the use of verbose error messages, enabling debugging environment variables and eventually forgetting to clean the code when moving it to production environment.Verbose error messages such as stack traces or syntax errors, expose internal logic of the serverless function revealing potential weakness, flaws or sensitive data.


# Hosting

✓ A web hosting service is a type of Internet hosting service that hosts websites for clients, i.e. it offers the facilities required for them to create and maintain a site and makes it accessible on the World Wide Web. Companies providing web hosting services are sometimes called **web hosts.**

✓ Web hosting is a service that provides storage for the files that make up your website and the software, physical hardware, and network infrastructure that makes your website available to others on the internet.

**Typically,  hosting requires -** 

• One or more servers to act as the hosts for the sites; servers may be physical or virtual

• Colocation for the servers, providing physical space, electricity, and Internet connectivity;

• Domain Name System configuration to define names for the sites and point them to the hosting servers;

• A web server running on the host;

• For each site hosted on the server -  space on the servers to hold the files making up the site

 
• Site-specific configuration.

• often, a database;

• Software and credentials allowing the client to access these, enabling them to create, configure, and modify the site;

• Email connectivity allowing the host and site to send email to the client.

[**Hosting Services**]


**Static page hosting**

The most basic is web page and small-scale file hosting, where files can be uploaded via File Transfer Protocol (FTP) or a web interface. The files are usually delivered to the Web as is  or with minimal processing. Many Internet service providers (ISPs) offer this service free to subscribers. Individuals and organizations may also obtain web page hosting from alternative service providers.

**Peer-to-peer hosting**

Peer-to-peer web hosting is using peer-to-peer networking to distribute access to webpages. This is differentiated from the client–server model which involves the distribution of web data between dedicated web servers and user-end client computers. Peer-to-peer web hosting may also take the form of P2P web caches and content delivery networks.

**Larger hosting services**

Many large companies that are not Internet service providers need to be permanently connected to the web to send email, files, etc. to other sites. The company may use the computer as a website host to provide details of their goods and services and facilities for online orders.
A complex site calls for a more comprehensive package that provides database support and application development platforms (e.g. ASP.NET, ColdFusion, Java EE, Perl/Plack, PHP or Ruby on Rails). These facilities allow customers to write or install scripts for applications like forums and content management. Web hosting packages often include a web content management system, so the end-user does not have to worry about the more technical aspects. Secure Sockets Layer (SSL) is used for websites that wish to encrypt the transmitted data.

# Types of hosting

Internet hosting services can run web servers.

1. **Shared web hosting service** –

  One's website is placed on the same server as many other sites, ranging from a few sites to hundreds of websites. Typically, all domains may share a common pool of server resources, such as RAM and the CPU. The features available with this type of service can be quite basic and not flexible in terms of software and updates. Resellers often sell shared web hosting and web companies often have reseller accounts to provide hosting for clients.
  
  
2. **Reseller web hosting** – 

Allows clients to become web hosts themselves. Resellers could function, for individual domains, under any combination of these listed types of hosting, depending on who they are affiliated with as a reseller. Resellers' accounts may vary tremendously in size: they may have their own virtual dedicated server to a colocated server. Many resellers provide a nearly identical service to their provider's shared hosting plan and provide the technical support themselves.


3. **Virtual Dedicated Server** – 

Also known as a Virtual Private Server (VPS), divides server resources into virtual servers, where resources can be allocated in a way that does not directly reflect the underlying hardware. VPS will often be allocated resources based on a one server to many VPSs relationship, however virtualisation may be done for a number of reasons, including the ability to move a VPS container between servers. The users may have root access to their own virtual space. Customers are sometimes responsible for patching and maintaining the server (unmanaged server) or the VPS provider may provide server admin tasks for the customer (managed server).


4. **Grid hosting** –

This form of distributed hosting is when a server cluster acts like a grid and is composed of multiple nodes.

5. **Managed hosting service** – 

The user gets their own web server but is not allowed full control over it (user is denied root access for Linux/administrator access for Windows); however, they are allowed to manage their data via FTP or other remote management tools. The user is disallowed full control so that the provider can guarantee quality of service by not allowing the user to modify the server or potentially create configuration problems. The user typically does not own the server. The server is leased to the client.


# Security

Because web hosting services host websites belonging to their customers, online security is an important concern. When a customer agrees to use a web hosting service, they are relinquishing control of the security of their site to the company that is hosting the site. The level of security that a web hosting service offers is extremely important to a prospective customer and can be a major factor when considering which provider a customer may choose.
Web hosting servers can be attacked by malicious users in different ways, including uploading malware or malicious code onto a hosted website. These attacks may be done for different reasons, including stealing credit card data, launching a Distributed Denial of Service Attack (DDoS) or spamming.
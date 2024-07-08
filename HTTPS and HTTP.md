# HTTPS AND HTTP

HTTPS is just HTTP with encryption. The primary distinction between these two names is that HTTPS is more secure than HTTP since it uses **TLS (SSL)** encryption for all HTTP requests and answers, even the standard ones.

# HyperText Transfer Protocol (HTTP)

1. **HyperText Transfer Protocol (HTTP)** is a protocol using which hypertext is transferred over the Web.

2. Due to its simplicity, HTTP has been the most widely used protocol for data transfer over the Web but the data (i.e. hypertext) exchanged using HTTP isn’t as secure as we would like it to be.

3. In fact, hyper-text exchanged using HTTP goes as plain text i.e. anyone between the browser and server can read it relatively easily if one intercepts this exchange of data.

4. The acronym for **Hypertext Transfer Protocol** is HTTP.

5. The web server delivers the desired data to the user in the form of web pages when the user initiates an HTTP request through their browser. Above the TCP layer lies an application layer protocol called HTTP. It has given web browsers and servers certain standard principles that they can use to talk to one another.

6. Because each transaction on the **HTTP** protocol is carried out independently of the others and without reference to the history, the connection between the web browser and the server ends after the transaction is finished. This makes HTTP a stateless protocol.


# Advantages of HTTP

● Because there are fewer connections running at once, it delivers reduced CPU and memory utilization.

● It allows requests and answers to be pipelined via HTTP.

● Because there are fewer TCP connections, it provides less network congestion.

● During the first stage of connection establishment, handshakes are exchanged. Because there is no handshaking, it provides lower latency for subsequent requests.

● Without terminating the TCP connection, it reports problems.


# Disadvantages of HTTP

● It is applicable to point-to-point connections.

● It isn’t mobile-friendly.

● It is not capable of being pushed.

● It uses far too many words.

● It doesn’t provide trustworthy exchange (in the absence of retry mechanism).

● When the client receives all the data it requires, the connection is not terminated. Therefore, the server won’t be accessible during this time.


# Hypertext Transfer Protocol Secure (HTTPS)

1. Hypertext Transfer Protocol Secure (HTTPS) is an extended version of the Hypertext Transfer Protocol (HTTP). It is used for secure communication.

2. In HTTPS, the communication protocol is encrypted using Transport Layer Security.

3. HTTPS stands for Hypertext Transfer Protocol Secure.

4. While HTTP guarantees data security, the HTTP protocol does not provide data security. 

5. As a result, HTTPS can be defined as a secure variant of the HTTP protocol. Data can be transferred using this protocol in an encrypted format.

6. In most cases, the HTTPS protocol must be used while entering bank account information.

7. The HTTPS protocol is mostly utilised in situations when entering login credentials is necessary. Modern browsers like Chrome distinguish between the HTTP and HTTPS protocols based on distinct markings.

8. HTTPS employs an encryption mechanism called **Secure Sockets Layer (SSL)**, also known as Transport Layer Security, to enable encryption.  


# Advantages of HTTPS

● Provides in-transit data security.

● Shields your website from data breaches, phishing, and  MITM attacks.

● Increases the visitors’ trust to your website.

● Eliminates the “NOT Secure” alerts.

● Assist you in raising your website’s ranking.

# Disadvantages of HTTPS

● When switching to HTTPS, an SSL certificate needs to be bought. Even though website hosts often give SSL certificates, these should be renewed annually by paying a charge.

● Encrypting and decrypting data across HTTPS connections requires a lot of computation.

● There will be issues with caching some information over HTTPS. Public caching of those that previously took place won’t happen again.

● Certain proxy servers and firewalls prevent users from accessing HTTPS websites. Both deliberate and inadvertent actions might result from this.

● If there are configuration issues, HTTP will be used by your website to obtain files rather than HTTPS.


# Difference Between HTTP and HTTPS

1. HTTP stands for HyperText Transfer Protocol.	HTTPS for HyperText Transfer Protocol Secure.

2. In HTTP, URL begins with “http://”.	In HTTPs, URL starts with “https://”.

3. HTTP uses port number 80 for communication.	HTTPs uses 443 port number for communication.

4. HTTP is considered to be unsecure.	HTTPs is considered as secure.

5. HTTP works at Application Layer.	HTTPS works at Transport Layer.

6. In HTTP, Encryption is absent.	Encryption is present in HTTPS.

7. HTTP does not require any certificates.	HTTPS needs SSL Certificates.

8. HTTP does not improve search ranking	HTTPS helps to improve search ranking.

9. HTTP faster than HTTPS	HTTPS slower than HTTP.

10. HTTP does not use data hashtags to secure data.	While HTTPS will have the data before sending it and return it to its original state on the receiver side.

11. In HTTP Data is transfer in plaintext.	In HTTPS Data transfer in ciphertext.

12. HTTP Should be avoided.	HTTPS Should be preferred.
Search engines do not favour the insecure website.	Improved reputation of the website in search engine.

13. HTTP Does not require SSL/TLS or Certificates	HTTPS Requires SSL/TLS implementation with Certificates.

14. In HTTP Users ar  worried about their data.	In HTTPS Users are  confident about the security of their data.
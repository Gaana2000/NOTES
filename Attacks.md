# PHISHING ATTACKS

**PHISHING**

Phishing is another type of cyber attack. Phishing got its name from “phish” meaning fish. It’s a common phenomenon to put bait for the fish to get trapped. Similarly, phishing works. It is an unethical way to dupe the user or victim to click on harmful sites. The attacker crafts the harmful site in such a way that the victim feels it to be an authentic site, thus falling prey to it. The most common mode of phishing is by sending spam emails that appear to be authentic and thus, taking away all credentials from the victim. The main motive of the attacker behind phishing is to gain confidential information like:

●Password

●Credit card details

●Social security numbers

●Date of birth

The attacker uses this information to further target the user impersonate the user and cause data theft. The most common type of phishing attack happens through email. Phishing victims are tricked into revealing information that they think should be kept private. The original logo of the email is used to make the user believe that it is indeed the original email. But if we carefully look into the details, we will find that the URL or web address is not authentic. 

# How is Phishing Carried Out?

Below mentioned are the ways through which Phishing generally occurs. Upon using any of the techniques mentioned below, the user can lead to Phishing Attacks.

☆ **Clicking on an unknown file or attachment**


☆ **Using an open or free wifi hotspot**


☆ **Responding to social media requests**


☆ **Clicking on unauthenticated links or ads**


# TYPES OF  PHISHING ATTACKS

1. **Email Phishing**


2. **Spear Phishing**


3. **Whaling**


4. **Smishing**


5. **Vishing**


6. **Clone Phishing**



# IMPACT OF PHISHING 

¤ **Financial Loss**: 

Phishing attacks often target financial information, such as credit card numbers and bank account login credentials. This information can be used to steal money or make unauthorized purchases, leading to significant financial losses.


¤ **Identity Theft**: 

Phishing attacks can also steal personal information, such as Social Security numbers and date of birth, which can be used to steal an individual’s identity and cause long-term harm.


¤ **Damage to Reputation**: 

Organizations that fall victim to phishing attacks can suffer damage to their reputation, as customers and clients may lose trust in the company’s ability to protect their information.


¤ **Disruption to Business Operations**: 

Phishing attacks can also cause significant disruption to business operations, as employees may have their email accounts or computers compromised, leading to lost productivity and data.


¤ **Spread of Malware**: 

Phishing attacks often use attachments or links to deliver malware, which can infect a victim’s computer or network and cause further harm.


¤ **Signs of Phishing** 

It is very important to be able to identify the signs of a phishing attack to protect against its harmful effects. These signs help the user to protect user data and information from hackers. Here are some signs to look out for include:

¤ **Suspicious email addresses**:

Phishing emails often use fake email addresses that appear to be from a trusted source, but are controlled by the attacker. Check the email address carefully and look for slight variations or misspellings that may indicate a fake address.

¤ **Urgent requests for personal information**: 

Phishing attacks often try to create a sense of urgency to trick victims into providing personal information quickly. Be cautious of emails or messages that ask for personal information and make sure to verify the authenticity of the request before providing any information.

¤ **Poor grammar and spelling**: 

Phishing attacks are often created quickly and carelessly, and may contain poor grammar and spelling errors. These mistakes can indicate that the email or message is not legitimate.

¤ **Requests for sensitive information**: 

Phishing attacks often try to steal sensitive information, such as login credentials and financial information. Be cautious of emails or messages that ask for sensitive information and verify the authenticity of the request before providing any information.

¤ **Unusual links or attachments**: 

Phishing attacks often use links or attachments to deliver malware or redirect victims to fake websites. Be cautious of links or attachments in emails or messages, especially from unknown or untrusted sources.

¤ **Strange URLs**: 

Phishing attacks often use fake websites that look similar to the real ones, but have slightly different URLs. Look for strange URLs or slight variations in the URL that may indicate a fake website.

**How To Stay Protected Against Phishing?**

1. **Authorized Source**: Download software from authorized sources only where you have trust.

2. **Confidentiality**: Never share your private details with unknown links and keep your data safe from hackers.

3. **Check URL**: Always check the URL of websites to prevent any such attack it will help you not get trapped in Phishing attacks.

4. **Avoid replying to suspicious things**: If you receive an email from a known source but that email looks suspicious, then contact the source with a new email rather than using the reply option.

5. **Phishing Detection Tool**: Use phishing-detecting tools to monitor the websites that are crafted and contain unauthentic content.

6. **Try to avoid free wifi**: Avoid using free Wifi, it will lead to threats and Phishing.

7. **Keep your system updated**: It’s better to keep your system always updated to protect from different types of Phishing Attacks. 

8. **Keep the firewall of the system ON**: Keeping ON the firewalls helps you filter ambiguous and suspicious data and only authenticated data will reach you.




# DDOS (DISTRIBUTED DENIAL OF  SERVICE) ATTACK

**Distributed Denial of Service (DDoS)** is a type of DOS attack where multiple systems, which are trojan infected, target a particular system which causes a DoS attack. 

A DDoS attack uses multiple servers and Internet connections to flood the targeted resource. A DDoS attack is one of the most powerful weapons on the cyber platform. When you come to know about a website being brought down, it generally means it has become a victim of a **DDoS attack.** This means that the hackers have attacked your website or PC by imposing heavy traffic. Thus, crashing the website or computer due to overloading. 

# Types of DDoS Attacks

There are various types of DDoS attacks.

1. **Volumetric Attacks**

 
2. **Protocol Attacks**

  
3. **Application Attacks**


4. **Fragmentation Attacks**


# How do DDoS Attacks Work?

The logic of a DDoS attack is very simple, although attacks can be highly different from each other. Network connections consist of various layers of the OSI model. Various types of DDoS attacks focus on particular layers. Examples are illustrated below:

**Layer-3**:
**Network layer**
– Attacks are known as Smurf Attacks, ICMP Floods, and IP/ICMP Fragmentation.

**Layer-4**:
**Transport layer**
– Attacks include SYN Floods, UDP Floods, and TCP Connection Exhaustion.

**Layer-7**:
**Application layer**
– HTTP-encrypted attacks.


# How to Protect from DDoS Attacks?

1. **Take quick action**


2. **Configure firewalls and routers**


3. **Consider artificial intelligence**


4. **Secure your Internet of Things devices**




# CODE INJECTION ATTACK

**Code injection** is the malicious injection or introduction of code into an application. The code introduced or injected is capable of compromising database integrity and or compromising privacy properties, security and even data correctness. It can also steal data and or bypass access and authentication control. Code injection attacks can plague applications that depend on user input for execution.

▪ Code Injection differs from Command Injection. Here an attacker is only limited by the functionality of the injected language itself. For example, if an attacker is able to inject PHP code into an application and have it executed, he is only limited by what PHP is capable of.

▪ Code injection vulnerabilities range from easy to difficult-to-find ones. Many solutions have been developed for thwarting these types of code injection attacks, for both application and architecture domain. Some examples include input validation, parameterization, privilege setting for different actions, addition of extra layer of protection and others.
  
  
#   Example

▪ When a developer uses the PHP eval() function and passes it untrusted data that an attacker can modify, code injection could be possible.

The example below shows a dangerous way to use the eval() function:

// A dangerous way to use the eval() function  
// in PHP 

$myvar = "varname"; 

$x = $_GET['arg']; 

eval("\$myvar = \$x"); 
As there is no input validation, the code above is vulnerable to a Code Injection attack.

For example:

/index.php?arg=1; phpinfo()
Above will show all the info of php.

While exploiting bugs like these, an attacker may want to execute system commands. In this case, a code injection bug can also be used for command injection, for example:

/index.php?arg=1; system('id')
This will tell the ids of the process.
uid=33(www-data) gid=33(www-data) groups=33(www-data)

# Mitigation

● Ideally, a developer should use existing API for their language. 
For example (Java): Rather than use **Runtime.exec()** to issue a **‘mail**’ command, use the available Java API located at **javax.mail.***

● If no such available API exists, the developer should scrub all input for malicious characters. Implementing a positive security model would be most efficient. Typically, it is much easier to define the legal characters than the illegal characters.


# SCRIPT ATTACK

**Cross Site Scripting (CSS/ XSS)** is a vulnerability in a web application that allows a third party to execute a script in the user’s browser on behalf of the web application. Cross-site Scripting is one of the most prevalent vulnerabilities present on the web today. The exploitation of XSS against a user can lead to various consequences such as account compromise, account deletion, privilege escalation, malware infection and many more.

There are **Two types of XSS**

1. **Reflected XSS** 

If the input has to be provided each time to execute, such XSS is called reflected. These attacks are mostly carried out by delivering a payload directly to the victim. Victim requests a page with a request containing the payload and the payload comes embedded in the response as a script. An example of reflected XSS is XSS in the search field.

2. **Stored XSS**

When the response containing the payload is stored on the server in such a way that the script gets executed on every visit without submission of payload, then it is identified as stored XSS. An example of stored XSS is XSS in the comment thread.
  
3. **Dom Based XSS** 

There is another type of XSS called **DOM based XSS** and its instances are either reflected or stored. DOM-based XSS arises when user-supplied data is provided to the DOM objects without proper sanitizing.


There are two aspects of XSS (and any security issue) –

1. **Developer**


2. **Security researchers**


# How does XSS work?

Cross-site scripting works by manipulating a vulnerable web site so that it returns malicious JavaScript to users. When the malicious code executes inside a victim's browser, the attacker can fully compromise their interaction with the application.


..................................................................................................
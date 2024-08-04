# METASPLOIT 

Metasploit is the world’s leading open-source penetrating framework used by security engineers as a penetration testing system and a development platform that allows to create security tools and exploits. The framework makes hacking simple for both attackers and defenders. The various tools, libraries, user interfaces, and modules of Metasploit allow a user to configure an exploit module, pair with a payload, point at a target, and launch at the target system. Metasploit’s large and extensive database houses hundreds of exploits and several payload options.

A Metasploit penetration test begins with the information gathering phase, wherein Metasploit integrates with various reconnaissance tools like Nmap, SNMP scanning, and Windows patch enumeration, and Nessus to find the vulnerable spot in your system. Once the weakness is identified, choose an exploit and payload to penetrate the chink in the armor. If the exploit is successful, the payload gets executed at the target, and the user gets a shell to interact with the payload. One of the most popular payloads to attack Windows systems is Meterpreter – an in-memory-only interactive shell. Once on the target machine, Metasploit offers various exploitation tools for privilege escalation, packet sniffing, pass the hash, keyloggers, screen capture, plus pivoting tools. Users can also set up a persistent backdoor if the target machine gets rebooted.

# What Is the Purpose of Metasploit?

Metasploit is a powerful tool used by network security professionals to do penetration tests, by system administrators to test patch installations, by product vendors to implement regression testing, and by security engineers across industries. The purpose of Metasploit is to help users identify where they are most likely to face attacks by hackers and proactively mend those weaknesses before exploitation by hackers. 

# Who Uses Metasploit?

With the wide range of applications and open-source availability that Metasploit offers, the framework is used by professionals in development, security, and operations to hackers. The framework is popular with hackers and easily available, making it an easy to install, reliable tool for security professionals to be familiar with even if they don’t need to use it. 

# Metasploit Uses and Benefits


* Open Source and Actively Developed 



* Ease of Use  

 

* Easy Switching Between Payloads 


* Cleaner Exits 



* Friendly GUI Environment 



# What Tools Are Used in Metasploit?


Metasploit tools make penetration testing work faster and smoother for security pros and hackers. Some of the main tools are Aircrack, Metasploit unleashed, Wireshark, Ettercap, Netsparker, Kali, etc.


# How to Download and Install Metasploit?


•If you are using Kali Linux for presentation testing, Metasploit is preinstalled in your system. So you don’t need to download and install it. 

•The Github repository helps to download and install Metasploit in both Windows and Linux systems. It is available in the GUI version, but you have to purchase for full access to Metasploit licensed version.   


**What Is Metasploitable?**

Metasploitable refers to a vulnerable machine that enables the learning and practice of Metasploit. It is illegal to hack or attack any system without the owner’s consent. So, the metasploitable machine enables users to set up a penetration testing environment to learn and practice hacking.   


**Metasploit Framework**

Following is the filesystem of Metasploit Framework (MSF):

Data – contains editable files for storing binaries, wordlist, images, templates, logos, etc

Tools – contains command utilities including plugins, hardware, memdump

Scripts – contains Meterepreter scripts, resources to run functionalities

Modules – contains actual MSF modules 

Plugins – additional extensions for automating manual tasks

Documentation – documents and pdfs concerning Metasploit framework

Lib – contains libraries required to run Metasploit from start to end.


# BURP SUITE

Burp or Burp Suite is a set of tools used for penetration testing of web applications. It is developed by the company named Portswigger, which is also the alias of its founder Dafydd Stuttard. BurpSuite aims to be an all in one set of tools and its capabilities can be enhanced by installing add-ons that are called BApps.
It is the most popular tool among professional web app security researchers and bug bounty hunters. Its ease of use makes it a more suitable choice over free alternatives like OWASP ZAP. Burp Suite is available as a community edition which is free.


**The tools offered by Burp Suite are:**


1. **Spider**


2. **Proxy**


3. **Intruder**


4. **Repeater**


5. **Sequencer**


6. **Decoder**


7. **Extender**


8. **Scanner**



# WIRESHARK

• Wireshark is an open-source packet analyzer, which is used for education, analysis, software development, communication protocol development, and network troubleshooting.

• It is used to track the packets so that each one is filtered to meet our specific needs. It is commonly called as a sniffer, network protocol analyzer, and network analyzer. It is also used by network security engineers to examine security problems.

• Wireshark is a free to use application which is used to apprehend the data back and forth. It is often called as a free packet sniffer computer application. It puts the network card into an unselective mode, i.e., to accept all the packets which it receives.


# WIRESHARK USES

•It is used by network security engineers to examine security problems.

•It allows the users to watch all the traffic being passed over the network.

•It is used by network engineers to troubleshoot network issues.

•It also helps to troubleshoot latency issues and malicious activities on your network.

•It can also analyze dropped packets.

•It helps us to know how all the devices like laptop, mobile phones, desktop, switch, routers, etc., communicate in a local network or the rest of the world.

**A Packet**

A packet is a unit of data which is transmitted over a network between the origin and the destination. Network packets are small, i.e., maximum 1.5 Kilobytes for Ethernet packets and 64 Kilobytes for IP packets. The data packets in the Wireshark can be viewed online and can be analyzed offline.


# Features of Wireshark

•It is multi-platform software, i.e., it can run on Linux, Windows, OS X, FreeBSD, NetBSD, etc.

•It is a standard three-pane packet browser.

•It performs deep inspection of the hundreds of protocols.

•It often involves live analysis, i.e., from the different types of the network like the Ethernet, loopback, etc., we can read live data.

•It has sort and filter options which makes ease to the user to view the data.

•It is also useful in VoIP analysis.

•It can also capture raw USB traffic.

•Various settings, like timers and filters, can be used to filter the output.

•It can only capture packet on the PCAP (an application programming interface used to capture the network) supported networks.

•Wireshark supports a variety of well-documented capture file formats such as the PcapNg and Libpcap. These formats are used for storing the captured data.

•It is the no.1 piece of software for its purpose. It has countless applications ranging from the tracing down, unauthorized traffic, firewall settings, etc.


**What is color coding in Wireshark?**

•The packets in the Wireshark are highlighted with blue, black, and green color. These colors help users to identify the types of traffic. It is also called as packet colorization. The kinds of coloring rules in the Wireshark are temporary rules and permanent rules.

•The temporary rules are there until the program is in active mode or until we quit the program.
The permanent color rules are available until the Wireshark is in use or the next time you run the Wireshark.
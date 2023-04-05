# **CyberSecurity Essentials notes**

&nbsp;


# **1 - Threats Vulnerabilities and Attacks**
&nbsp;

**Types of cyber threats**
- **Software attacks** : Virus, DoS...
- **Software errors** : bug, app going offline, cross-site script, illegal file server share.
- **Sabotage** : backdoor, worms, authorized user compromising an org's database, ...
- **Human error**
- **Theft**
- **Hardware failures**
- **Utility interruption**
- **Natural disasters**
- **Internal threats** : carried out by current/former employee and/or contract partners who accidentally mishandle confidential data, threathen infra, etc...
- **External threats** : Typically stems from an amateur or skilled attackers who can exploit vulnerabilities

Internal threats have the potential to cause greater damage because an employee has direct access to the organisation premises/devices. They also have inside knowledge.

**APT** : Advanced Persistent Threat. Continuous attack that was elaborate espionage tactics involving multiple actors and/or sophisticated malware to gain access to and analyze a target's network. Typically target high level orgs.

**Algorithm attacks** : takes advantage of an algorithm in a piece of legitimate software to generate unintended behaviors.
&nbsp;

#### **Social engineering**

**Types of attacks** : 
- **Pretexting** : to lie to gain access to privileged data
- **Something for something (quid pro quo)** : request for info in exchange for a gift for example
- **Identity fraud**

**Tactics** : 
Authority, intimidation, consensus, scarcity, urgency, familiarity, trust.
&nbsp;

#### **Piggybacking/Tailgating**

Occurs when a criminal follows an authorized person to gain physical entry into a secure location or restricted area.
Criminals can achieve this by :
- Giving the appearance of being escorted into the facility by an authorized person
- Joining and pretending to be part of a large crowd that enters the facility
- Targeting an authorized person who is careless about the rules of the facility

Two sets of doors is a way to prevent this. Referred to as a mantrap.

#### **Deception methods**

- **Invoice scam**
- **Watering hole attack** : describes an exploit in which an attacker observes or guesses what websites an org uses most often and infects one of them.
- **Typosquatting** : relies on common mistakes such as typos made by individuals when inputting a website URL in their browser
- **Prepending** : Removing the EXTERNAL tag used by orgs to warn the recipient that the email is external. Tricks individuals into believing that a malicious email was sent from inside the org.
- **Influence campaign**

&nbsp;


## **1.3 - Cyber Attacks**
&nbsp;

### **1.3.1 - Three most common types of hardwares used by hackers :**

- **Viruses** : A virus is a type of computer program that, when executed, replicates and attaches itself to other files, such as a legitimate program, by inserting its own code into it. Some viruses are harmless yet others can be destructive, such as those that modify or delete data. Most viruses require end-user interaction to initiate activation, and can be written to act on a specific date or time.

- **Worms** : A worm is a malicious software program that replicates by independently exploiting vulnerabilities in networks. Unlike a virus, which requires a host program to run, worms can run by themselves. Other than the initial infection of the host, they do not require user participation and can spread very quickly over the network, usually slowing it down. Worms share similar patterns: they exploit system vulnerabilities, they have a way to propagate themselves and they all contain malicious code (payload) to cause damage to computer systems or networks.

- **Trojan horses** : A trojan horse is a malware that carries out malicious operations by masking its true intent. It might appear legitimate but is, in fact, very dangerous. Trojans exploit the privileges of the user who runs them. Unlike viruses, trojans do not self-replicate but often bind themselves to non-executable files, such as images, audio or video files, acting as a decoy to harm the systems of unsuspecting users.

&nbsp;

### **1.3.2 - Logic bombs**


A logic bomb is a malicious program that waits for a trigger, such as a specified date or database entry, to set off the malicious code. Until this trigger event happens, the logic bomb will remain inactive.
Once Activated, a logic bomb implements a malicious code that causes harm to a computer in various ways (sabotage data records, erase files, attack OS or applications, destroy hardware of a desktop/server with methods such as overheating parts).

&nbsp;

### **1.3.3 - Ransomware**


Designed to hold a computer system or the data it contains captive until payment is made. Files are encrypted until the payment is made, you cannot access it until then.
Payment is made through an untraceable payment system and once done hackers will supply you the program to decrypt your data (often doesn't happen, victims never gain access again). Some versions of ransomware can take advantage of specific system vulnerabilities to lock it down. Ransomware is often spread through phishing emails that encourage you to download a malicious attachment, or through a software vulnerability.

&nbsp;

### **1.3.4 - Denial of Service attacks**

Type of network attack that is relatively simple to conduct. These attacks can either overwhelm their target's network with overwhelming traffic or they can send maliciously formatted packets which can cause systems to crash. **DDoS** attacks are similar but originate from multiple originated sources, such as a network of bots or botnet which is a network of infected hosts called zombies, here is how it works :
- The attacker builds his botnet which are controlled by handler systems
- Zombie computers consanstly scan and infect more hosts, creating more and more zombies
- Once ready, the attacker will instruct the handler systems to make the zombies carry out the DDoS attack.

&nbsp;

### **1.3.5 - Domain Name System**

Prime targets for attacks : routing, addressing and domain naming.
- **DNS Spoofing** : DNS spoofing or DNS cache poisoning is an attack in which false data is introduced into a DNS resolver cache — the temporary database on a computer’s operating system that records recent visits to websites and other Internet domains.
- **Domain hijacking** : When an attacker wrongfully gains control of a target’s DNS information, they can make unauthorized changes to it. This is known as domain hijacking. The most common way of hijacking a domain name is to change the administrator’s contact email address through social engineering or by hacking into the administrator's email account. The administrator’s email address can be easily found via the WHOIS record for the domain, which is of public record.
- **URL** : A uniform resource locator (URL) is a unique identifier for finding a specific resource on the Internet. Redirecting a URL commonly happens for legitimate purposes. For example, you have logged into an eLearning portal to begin this Cybersecurity Essentials course. If you log out of the portal and return to it another time, the portal will redirect you back to the login page. It is this type of functionality that attackers can exploit. Instead of taking you to the eLearning login page, they can redirect you to a malicious site. 

&nbsp;

### **1.3.7 - Layer 2 Attacks**

Layer 2 refers to the data link layer in the OSI model. This layer is used to move data accross a linked physical network. In its simplest terms, the MAC address identifies the intended receiver of an IP address sent over the network, and ARP resolves IP addresses to MAC addresses for transmitting data.
Examples of exploits attackers take advantage of in the layer 2.

**Spoofing**

Spoofing or poisoning is a type of impersonation attack that takes advantage of a trusted relationship between two systems.
- **MAC address spoofing** occurs when an attacker disguises their device as a valid one on the network
- **ARP spoofing** sends spoofed ARP messages accross a LAN.
- **IP spoofing** sends IP packets from spoofed source address in order to disguise it

**MAC Flooding**

MAC Flooding compromises the data transmitted to a device. An attacker floods the network with fake MAC addresses, compromising security of the NW switch.

&nbsp;

### **1.3.9 - Man-in-the-Middle and Man-in-the-Mobile Attacks**

Attackers can intercept or modify communications between two devices to steal information from or to impersonate one of the devices.
- **Man in the Middle (MitM)** : happens when a cybercriminal takes control of a device without the user’s knowledge. With this level of access, an attacker can intercept, manipulate and relay false information between the sender and the intended destination.
- **Man in the Mobile (MitMo)** : A variation of man-in-the-middle, MitMo is a type of attack used to take control over a user’s mobile device. When infected, the mobile device is instructed to exfiltrate user-sensitive information and send it to the attackers. ZeuS is one example of a malware package with MitMo capabilities. It allows attackers to quietly capture two-step verification SMS messages sent to users.

A **replay attack** occurs when an attacker captures communication between two hosts and then retransmits the message to the recipient to trick him.

&nbsp;

### **1.3.10 - Zero day attacks**

Exploits a software vulnerability before they become known or before they are disclosed. A network is extremely vulnerable to attack between the time an exploit is discovered (zero hour) and the time it takes for the software vendor to develop and release a patch that fixes this exploit.

&nbsp;

### **1.3.11 - Keyboard logging**

Keylogging, etc.

&nbsp;

### **1.3.13 - Defending against attacks**

- Configure firewalls to remove any packets from outside the NW that have addresses indicated that they originated from inside the network.
- Ensure patches/updates
- Distribute workload accross servers/network
- To prevent DoS and DDoS attacks, organizations can block external ICMP packets with their firewalls.

&nbsp;

## **1.4 - Wireless and mobile device attacks**

&nbsp;

### **1.4.1 - Grayware and SMiShing**

**Grayware** is any unwanted application that behaves in an annoying or undesirable manner. And while grayware may not carry any recognizable malware, it may still pose a risk to the user by, for example, tracking your location or delivering unwanted advertising.
**Short message service phishing or SMiShing** is another tactic used by attackers to trick you. Fake text messages prompt you to visit a malicious website or call a fraudulent phone number, which may result in malware being downloaded onto your device or personal information being shared. 

&nbsp;

### **1.4.2 - Rogue access point**

A rogue access point is a wireless access point installed on a secure network without explicit authorization.
- An attacker will often use social engineering tactics to gain physical access to an organization’s network infrastructure and install the rogue access point.
- Also known as a criminal’s access point, the access point can be set up as a MitM device to capture your login information. This works by disconnecting the rogue access point, which triggers the network to send a deauthentication frame to disassociate the access point. This process is then exploited by spoofing your MAC address and sending a deauthentication data transmission to the wireless access point.

&nbsp;

### **1.4.3 - Radio Frequncy Jamming**

Wireless signals are susceptible to electromagnetic interference (EMI), radio frequency interference (RFI) and even lightning strikes or noise from fluorescent lights.
Attackers can take advantage of this fact by deliberately jamming the transmission of a radio or satellite station to prevent a wireless signal from reaching the receiving station.

&nbsp;

### **1.4.4 - Bluejacking and Bluesnarfing**

Bluetooth exploits.
- Bluejacking uses wireless Bluetooth technology to send unauthorized messages or shocking images to another Bluetooth device.
- Bluesnarfing occurs when an attacker copies information, such as emails and contact lists, from a target’s device using a Bluetooth connection.

&nbsp;

### **1.4.5 - Attacks against WiFi protocols**

Wired equivalent privacy (WEP) and Wi-Fi protected access (WPA) are security protocols that were designed to secure wireless networks that are vulnerable to attacks.

WEP was developed to provide data transmitted over a wireless local area network (WLAN) with a level of protection comparable to what is usually expected of a traditional wired network. It added security to wireless networks by encrypting the data.

WEP used a key for encryption. The problem, however, was that WEP had no provision for key management and so the number of people sharing the same key continually grew, giving criminals access to a large amount of traffic data. Furthermore, WEP’s initialization vector (IV), one of the key components of its encryption key, was too small, readable and static.

To address this and replace WEP, WPA and then WPA2 were developed as improved security protocols. Unlike with WEP, an attacker cannot recover WPA2’s encryption key by observing network traffic. However, they can still use a packet sniffer to analyze the packets going between an access point and a legitimate user.

**Evil twin attack** consists of, for example, going in a public area which has a public WiFi hotspot and setup your phone as an access point with the same name. You can then monitor the network from your laptop.

&nbsp;

### **1.4.7 - WiFi and mobile defense**

There are several steps that organizations and users need to take to defend against wireless and mobile device attacks. These include the following:
- Take advantage of basic wireless security features such as authentication and encryption by changing the default configuration settings.
Restrict access point placement by placing these devices outside the firewall or within a demilitarized zone — a perimeter network that protects an organization’s LAN from untrusted devices.
- Use WLAN tools such as NetStumbler to detect rogue access points or unauthorized workstations. 
- Develop a policy for guest access to an organization’s Wi-Fi network.
- Employees in an organization should use a remote access VPN for WLAN access.

&nbsp;

## **1.5 - Other attacks**

&nbsp;

### **1.5.1 - Cross-site scripting**

Cross-site scripting (XSS) is a common vulnerability found in many web applications. This is how it works:

- Cybercriminals exploit the XSS vulnerability by injecting scripts containing malicious code into a web page.
- The web page is accessed by the victim, and the malicious scripts unknowingly pass to their browser. 
- The malicious script can access any cookies, session tokens or other sensitive information about the user, which is sent back to the cybercriminal.
- Armed with this information, the cybercriminal can impersonate the user.

&nbsp;

### **1.5.2 - Code injection**

Most modern websites use a database, such as a Structured Query Language (SQL) or an Extensible Markup Language (XML) database, to store and manage data. Injection attacks seek to exploit weaknesses in these databases.
- **XML injection attack** : An XML injection attack can corrupt the data on the XML database and threaten the security of the website.It works by interfering with an application’s processing of XML data or query entered by a user. A cybercriminal can manipulate this query by programming it to suit their needs. This will grant them access to all of the sensitive information stored on the database and allows them to make any number of changes to the website.
- **SQL injection attack**
- **DLL injection attack** : A dynamic link library (DLL) file is a library that contains a set of code and data for carrying out a particular activity in Windows. Applications use this type of file to add functionality that is not built-in, when they need to carry out this activity.DLL injection allows a cybercriminal to trick an application into calling a malicious DLL file, which executes as part of the target process.
- **LDAP injection attack** : An LDAP injection attack exploits input validation vulnerabilities by injecting and executing queries to LDAP servers, giving cybercriminals an opportunity to extract sensitive information from an organization’s LDAP directory.  

&nbsp;

### **1.5.3 - Buffer overflow**

Buffers are memory areas allocated to an application. A buffer overflow occurs when data is written beyond the limits of a buffer. By changing data beyond the boundaries of a buffer, the application can access memory allocated to other processes. This can lead to a system crash or data compromise, or provide escalation of privileges.
These memory flaws can also give attackers complete control over a target’s device. For example, an attacker can change the instructions of a vulnerable application while the program is loading in memory and, as a result, can install malware and access the internal network from the infected device.

&nbsp;

### **1.5.4 - Remote code execution**

Remote code execution allows a cybercriminal to take advantage of application vulnerabilities to execute any command with the privileges of the user running the application on the target device.
Privilege escalation exploits a bug, design flaw or misconfiguration in an operating system or software application to gain access to resources that are normally restricted.

Check **metasploit project**.

&nbsp;

### **1.5.5 - Other application attacks**

- **Cross Site Request Forgery (CSRF)** : CSRF describes the malicious exploit of a website where unauthorized commands are submitted from a user’s browser to a trusted web application.
A malicious website can transmit such commands through specially-crafted image tags, hidden forms or JavaScript requests — all of which can work without the user’s knowledge.

- **Race condition attack** : Also known as a time of check (TOC) or a time of use (TOU) attack, a race condition attack happens when a computing system that is designed to handle tasks in a specific sequence is forced to perform two or more operations simultaneously.

- **Improper input handling attack** : Data inputted by a user that is not properly validated can affect the data flow of a program and cause critical vulnerabilities

- **Error handling attack** : Attackers can use error messages to extract specific information such as the hostnames of internal systems and directories or files that exist on a given web server — as well as database, table and field names that can be used to craft SQL injection attacks.

- **API attack** : An API delivers a user response to a system and sends the system’s response back to the user. An API attack occurs when a cybercriminal abuses an API endpoint.

- **Replay attack** : This describes a situation where a valid data transmission is maliciously or fraudulently repeated or delayed by an attacker, who intercepts, amends and resubmits the data to get the receiver to do whatever they want.

- **Directory traversal attack** : Directory traversal occurs when an attacker is able to read files on the webserver outside of the directory of the website. An attacker can then use this information to download server configuration files containing sensitive information, potentially expose more server vulnerabilities or even take control of the server !

- **Resource exhaustion attack** : These attacks are computer security exploits that crash, hang or otherwise interfere with a targeted program or system. Rather than overwhelming network bandwidth like a DoS attack, resource exhaustion attacks overwhelm the hardware resources available on the target’s server instead.

&nbsp;

### **1.5.10 - Vishing, Pharming and Whaling**

- **Vishing** : Often referred to as voice phishing, this type of attack sees criminals use voice communication technology to encourage users to divulge information, such as their credit card details.
Criminals can spoof phone calls using voice over Internet protocol (VoIP), or leave recorded messages to give the impression that they are legitimate callers.
- **Pharming** : This type of attack deliberately misdirects users to a fake version of an official website. Tricked into believing that they are connected to a legitimate site, users enter their credentials into the fraudulent website.
- **Whaling** : Whaling is a phishing attack that targets high profile individuals, such as senior executives within an organization, politicians and celebrities.

&nbsp;

### **1.5.13 - More attacks**

- **Physical attacks** : Malicious USB keys, unauthorized physical access...
Fitting cables and plugs such as generic USB cables, mobile device charging cables and wall or power adapters with advanced technologies, such as a wireless chip, to allow an attacker to control or provide instructions to a device. Copying or skimming data from a credit or debit card using a specialized terminal to create a cloned card, which can be used to gain unauthorized access to the victim’s accounts. 

- **Adversarial artificial intelligence attacks** : Machine learning uses mathematical models to predict outcomes. However, these models are dependent on the data that is inputted. If the data is tainted, it can have a negative impact on the predicted outcome. Attackers can take advantage of this to perpetrate attacks against machine learning algorithms. For example, using tainted data to trick an autonomous vehicle into misinterpreting street signs.

- **Supply chain attacks** : Many organizations interface with a third party for their systems management or to purchase components and software. Organizations may even rely on parts or components from a foreign source.
Attackers often find ways to intercept these supply chains. For example, software can be based on specific support agreements and subject to an end-of-life (EOL) date. Changing this date could mean that an organization is no longer eligible for service and maintenance support.

- **Cloud based attacks** : Attackers are constantly leveraging ways to exploit sensitive data stored on the cloud, as well as applications, platforms and infrastructure that is cloud-based, as we saw with SaaS, PaaS and IaaS.


---
&nbsp;

# **2 - Principles, Practices and Processes**

&nbsp;

## **2.1 - The three dimensions**
&nbsp;


### **2.1.1 - The cybersecurity cube**

#### **1 - Security Principles**

Data confidentiality prevents the disclosure of information to unauthorized people, resources, or processes.
Data integrity refers to the accuracy, consistency, and trustworthiness of data.
Data availability ensures that information is accessible by authorized users when needed.
You can use the acronym CIA to remember these three principles.

#### **2 - Data States**

- Data in transit.
- Data at rest or in storage.
- Data in process.

#### **3 - Safeguards**

The third dimension of the cybersecurity cube defines the pillars on which we need to base our cybersecurity defenses in order to protect data and infrastructure in the digital realm. These are technology, policy and practices, and improving education, training and awareness in people

&nbsp;

### **2.1.2 - CIA Triad - Principle of confidentiality**

To accomplish confidentiality without using encryption, tokenization is a substitution technique that can isolate data elements from exposure to other data systems. A random value with no mathematical relationship replaces original data. Outside the system, a token has no value and is meaningless. Tokenization can preserve the data format (its type and data length), which makes it useful for databases and card payment processing.
Rights management covers both digital rights management (DRM) and information rights management (IRM). Both protect data from unauthorized access by using encryption.
- DRM protects copyrighted material like music albums, films or books. When any such content appears in digital form — for instance on CD, mp3 or e-book — it is encrypted, so the media cannot be copied without the decryption key, which is available only to licensed parties.
- IRM is used in email and other files relevant to the activities and communications of an organization that need to be shared with others. With IRM, the document owner, the organization or one of its members, controls and manages access to the document.

&nbsp;

### **2.1.3 - Data privacy**

- Personal information is anything that can be traced back to an individual, such as medical records, credit card numbers or social security numbers.
- Business information contains anything that poses a risk to an organization if discovered by the public or by a competitor, such as acquisition plans, customer information or trade secrets.
- Classified information may belong to a government body or similar and is considered secret, confidential or restricted access.

**Privacy enhancement techologies** :
- **Anonymization** (works by obscuring privately identifiable data stored in a clear format, and turning that data into irreversible anonymous information)
- **Data minimization**
- **Tokenization**

&nbsp;

### **2.1.4 - Data integrity**

Integrity is the accuracy, consistency and trustworthiness of data across its entire lifecycle.
Data undergoes several operations such as capture, storage, retrieval, update and transfer, and must remain unaltered by unauthorized entities during all these operations.
Methods used to ensure data integrity include hashing, data validation checks, data consistency checks and access controls. Data integrity systems can include one or more of these methods.

**Levels of need for data integrity** :
- **Critical** : Healthcare organization for example. All data is continuously validated, tested and verified.
- **High** : E-commerce or analytics-based organization. All data is validated and verified at frequent intervals.
- **Medium** : Online sales and search engines. Little verification is performed, and data is not completely trustworthy.
- **Low** : Blogs, forums, personal pages on social media. Data may not be verified at all, therefore there is a low level of trust in the content.

&nbsp;

### **2.1.5 - Availability**

Availability refers to the need to maintain availability of information whenever it is needed. Cyberattacks and systems failures can prevent access to information, systems and services.
Methods used to ensure high availability include system redundancy, system backups, increased system resiliency, equipment maintenance, operating system and software updates and patches, and proactive plans for swift recovery from unforeseen disasters.

&nbsp;

### **2.1.6 - Ensuring availabiity**

**Measures that organizations can implement to ensure the availability of their services and systems** :
- **Equipment maintenance**
- **Operating systems and softwares updates and patches**
- **Backup testing**
- **Disaster planning**
- **New technologies implementation**
- **Activity monitoring**
- **Availability testing**

&nbsp;

### **The McCumber Cube**

The McCumber Cube was developed by John McCumber in 1992. It is a framework that is used to establish and evaluate information and information systems security. The framework relies on the cybersecurity professional to identify information assets with a focus on the core principles of cybersecurity: confidentiality, integrity, and availability. The model is based on three dimensions, each having three elements :

- **1 - Principles** :
    - **Confidentiality**
    - **Integrity**
    - **Availability**
- **2 - Information (data) states** :
    - **Storage**
    - **Transmission**
    - **Processing**
- **3 - Security Countermeasures or safeguards** :
    - **Policy and practices**
    - **Human factors**
    - **Technology**

&nbsp;

### **2.1.8/9 - Packet Tracer Practice Lab**

| md5sum to display the hash of the current file.
hmac to encrypt with secret key

&nbsp;

## **2.2 - States of data**
&nbsp;

### **2.2.1 - Data at rest**

Refers to data that is in storage. Is it the state data is in when it no user or process is accessing it.
Storage options :
- Direct attached storage (DAS)
- Redudant Array of Independent Disks (RAID)
- Network Attached Storage (NAS)
- Storage Area Network (SAN)
- Cloud

&nbsp;

### **2.2.2 - Challenges of Protecting Stored Data**

Data at rest also includes backup data (when not being written or in transit).
Network storage offer a more secure option.

&nbsp;

### **2.2.3 - Methods of Transmitting Data**

Data in transit is the second state of data we are going to look at, referring simply to data which is being transmitted — it is not at rest nor in use.
Data transmission involves sending information from one device to another, and protecting data in transit poses challenges. There are numerous ways to transmit information between devices.
- **A sneaker net** : A sneaker net uses removable media to physically move data from one computer to another. Organizations will never be able to fully eliminate the use of a sneaker net as a way to capture data.
- **Wired networks**
- **Wireless networks**

&nbsp;

### **2.2.4 - Challenges of Data In Transit**

The protection of data in transit is one of the most challenging jobs of a cybersecurity professional.
We have several challenges to deal with if we want to protect this data :
- **Protecting the confidentialty of data in transit** : VPN, SSL, IPsec, ...
- **Protecting the integrity of data in transit** : hashing, data redudancy...
- **Protecting the availability of data in transit** : Cybercriminals can use rogue or unauthorized devices to interrupt data availability, capturing it in transit. A simple mobile device can pose as a local wireless access point and trick unsuspecting users into associating with it. Network security professionals can implement mutual authentication systems to counter these actions.

&nbsp;

### **2.2.5 - Data in Process**

Data in process refers to data during initial input, modification, computation or output. It is the state that data is in when it is neither in transit nor at rest — in simple terms, it is data that is being processed.
- **Input** : Protection of data integrity starts with the initial input of data. Corruption during the input process may include mislabeling and incorrect or mismatched data formats, data entry errors or disconnected and/or malfunctioning or inoperable systems.
- **Modification** : Data modification is any change made to original data, such as users manually modifying data, and programs processing and changing data. When data is modified in a way that stops it from being readable or usable, this is often referred to as data corruption.
- **Output** : Data output refers to outputting data to output devices, such as printers, electronic displays and speakers. The accuracy of output data is critical because output provides information and influences decision-making.

&nbsp;

### **2.2.6 - Challenges of Protecting Data in Process**

Invalid data modification during processing can have an adverse impact, and mitigating against such cases is important to organizations of all sizes. Software errors are the reason for many such mishaps and disasters.

&nbsp;

## **2.3 - Cybersecurity Countermeasures**

&nbsp;

### **2.3.1 - HW-Based and Software-Based Technologies**

In the world of cybersecurity, both software and hardware is utilized to protect the data and systems of organizations.

**Software countermeasures technologies** :
- **Software FW**
- **NW and port scanners**
- **Protocol analyzers** : Otherwise known as signature analyzers, these are devices that collect and examine network traffic. They identify performance problems, detect misconfigurations, identify misbehaving applications, establish baseline and normal traffic patterns and debug communication problems.
- **Vulnerability scanners**
- **Host based intrusion detection system (IDS)** : These examine activity on host systems only. An IDS generates log files and alarm messages when it detects unusual activity. A system storing sensitive data or providing critical services is a candidate for host-based IDS.

**HW countermeasures technologies** :
- **FW**
- **Proxy**
- **HW based access control** : This term refers to devices that utilize biometric technology, such as fingerprint or iris scanners, to confirm the identity of anyone trying to access servers, data and systems.
- **Network switches**

&nbsp;

### **2.3.3 - Policies**

A security policy sets out the security objectives, rules of behavior and system requirements to be adhered to :

**Identification and authentication policies**

**Password policies**

**Acceptable use policies**

**Remote access policies**

**Network maintenance policies**

**Incident handling policies**


&nbsp;

### **2.3.4 - Standards**

One of the most important security principles is consistency. Standards help IT staff maintain consistency in operating the network. Standards documents provide the technologies that specific users or programs need in addition to any program requirements or criteria that an organization must follow. This helps IT staff improve efficiency and simplicity in design, maintenance and troubleshooting.

&nbsp;

## **2.4 - Access controls**
&nbsp;

### **2.4.2 - Logical Access Controls**

- Encryption is the process of taking plaintext and creating ciphertext.
- Smart cards have an embedded microchip.
- Passwords are protected strings of characters.
- Biometrics are users’ physical characteristics.
- Access control lists (ACLs) define the type of traffic allowed on a network.
- Protocols are sets of rules that govern the exchange of data between devices.
- Firewalls prevent unwanted network traffic.
- Routers connect at least two networks.
- Intrusion detection systems monitor a network for suspicious activities.
- Clipping levels are certain allowed thresholds for errors before triggering a red flag.

&nbsp;

### **2.4.3 - Administrative Access Controls**

- Policies are statements of intent.
- Procedures are the detailed steps required to perform an activity.
- Hiring practices define the steps an organization takes to find qualified employees.
- Background checks are a type of employee screening that includes information of past employment verification, credit history and criminal history.
- Data classification categorizes data based on its sensitivity.
- Security training educates employees about the security policies at an organization.
- Reviews evaluate an employee’s job performance.

&nbsp;

### **2.4.4 - Administrative Access Control in Details**

Also called AAA.
The concept of administrative access control involves three security services : 

- **Authentication** : Authentication verifies the identity of each user, to prevent unauthorized access. Users prove their identity with a username or ID. In addition, users need to verify their identity by providing one of the following: something they know (password), something they have (token, card), something they are (fingerprint).
- **Authorization** : Authorization services determine which resources users can access, along with the operations that users can perform.
- **Accounting** : Not related to financial accounting, accounting in AAA keeps track of what users do — including what they access, the amount of time they access resources, and any changes they make.

These services provide the primary framework to control access, preventing unauthorized access to a computer, network, database or other data resource.

&nbsp;

### **2.4.6 - Federated Identity Management**

Refers to multiple enterprises that let their users use the same identification credentials to gain access to the networks of all enterprises in the group. Unfortunately, this broadens the scope and increases the probability of a cascading effect should an attack occur. The goal of federated identity management is to share identity information automatically across castle boundaries. From the individual user’s perspective, this means a single sign-on to the web.

&nbsp;

### **2.4.7 - Authentication Methods**

- **What you know** : Password, PIN, ...
- **What you have** : Smart card, keys, ...
- **What you are** : Fingerprints, ...

&nbsp;

### **2.4.12 - Implementing Accountability**

**What is accountability ?** Accountability traces an action back to a person or process making this change to a system. Accountability then collects this information and reports the usage data. The organization can use this data for such purposes as auditing or billing.

&nbsp;

## **2.5 - Cryptography**

&nbsp;

### **2.5.2 - Creating ciphertext**

Key management is the most difficult part of designing a cryptographic system. Many cryptosystems have failed because of mistakes in their key management, and all modern cryptographic algorithms require key management procedures. In practice, most attacks on cryptographic systems involve attacking the key management system, rather than the cryptographic algorithm itself.

A cipher is a series of well-defined steps used to encrypt and decrypt messages. There are several methods of creating ciphertext :
- **Start with the plaintext** — the phrase you want to encrypt.
- **Transposition** — the letters are rearranged.
- **Substitution** — letters are replaced.
- **One-time pad** — plaintext combined with a secret key creates a new character, which then combines with the plaintext to produce ciphertext.

&nbsp;

### **2.5.3 - Types of cryptography**

Today, the most common types of cryptography use block ciphers and stream ciphers. Each method differs in the way that it groups bits of data to encrypt it.

**Block ciphers** transform a fixed-length block of plaintext into a common block of ciphertext of 64 or 128 bits. Block size is the amount of data encrypted at any one time. To decrypt this ciphertext, we apply the reverse transformation to the ciphertext block, using the same secret key. Block ciphers usually result in output data that is larger than the input data, because the ciphertext must be a multiple of the block size. For example, Data Encryption Standard (DES) is a symmetric algorithm that encrypts blocks in 64-bit chunks using a 56-bit key. To accomplish this, the block algorithm takes data one chunk at a time — for example, 8 bytes per chunk — until the entire block is full. If there is less input data than one full block, the algorithm adds artificial data, or blanks, until it uses the full 64 bits

**Stream ciphers** encrypt plaintext one byte or one bit at a time. Think of stream ciphers as a block cipher with a block size of one bit. With a stream cipher, the transformation of these smaller plaintext units varies, depending on when they are encountered during the encryption process. Stream ciphers can be much faster than block ciphers, and generally do not increase the size of the message being encrypted, because they can encrypt an arbitrary number of bits. For instance, A5 is a stream cipher that provides voice privacy and encrypts cell phone communications. It is also possible to use DES in stream cipher mode. Complex cryptographic systems can combine block and stream in the same process.

&nbsp;

### **2.5.4 - The Two Encryption Approaches**

The first is to protect the algorithm. If the security of an encryption system depends on the secrecy of the algorithm itself, the most important protection is to guard the algorithm at all costs. Every time someone found out the details of the algorithm, every party involved would need to change the algorithm. That approach does not sound very secure or manageable.

The second approach is to protect the keys. In modern cryptography, the algorithms are public. It is the cryptographic keys that ensure the secrecy of the data.

**Symmetric encryption** : Used the same pre-shared key, sometimes called a secret key pair to encrypt and decrypt data. Both the sender and recipient know the key before any encrypted communication begins.

**Asymmetric encryption** : Uses one key to encrypt and one to decrypt. One is public and the other is private. In a public-key encryption system, any person can encrypt a message using the public key of the receiver and the receiver is the only one that can decrypt it using their private key. Parties exchange secure messages without needing a pre-shared key.

&nbsp;

### **2.5.6 - Symmetric Encryption Algorithms**

- **3DES** : Digital Encryption Standard (DES) is a symmetric block cipher with 64-bit block size that uses a 56-bit key. It takes a 64-bit block of plaintext as input and outputs a 64-bit block of ciphertext. It always operates on blocks of equal size and it uses both permutations and substitutions in the algorithm. Triple DES encrypts data three times and uses a different key for at least one of the three passes, giving it a cumulative key size of 112 to 168 bits. 3DES is more resistant to attack, but it is much slower than DES.
The encryption cycle is as follows : 
    - Data encrypted by first DES
    - Data decrypted by second DES
    - Data re-encrypted by third DES
- **IDEA** : The International Data Encryption Algorithm (IDEA) uses 64-bit blocks and 128-bit keys. IDEA performs eight rounds of transformations on each of the 16 blocks that results from dividing each 64-bit block. IDEA was the replacement for DES, and now PGP (Pretty Good Privacy) uses it. PGP is an encryption program that provides privacy and authentication in data communication. GNU Privacy Guard (GnuPG) is a licensed, free version of PGP.
- **AES** : The Advanced Encryption Standard (AES) has a fixed block size of 128 bits with a key size of 128, 192, or 256 bits. The National Institute of Standards and Technology (NIST) approved the AES algorithm in December 2001. The U.S. government uses AES to protect classified information. AES is a strong algorithm that uses longer key lengths. AES is faster than DES and 3DES, so it provides both a solution for software applications as well as hardware use in firewalls and routers.

Other block ciphers include Skipjack (developed by the NSA), Blowfish and Twofish.

&nbsp;

### **2.5.7 - Asymmetric Encryption Process**

Also called public key encryption, asymmetric encryption uses one key for encryption that is different from the key used for decryption. A criminal cannot calculate the decryption key based on knowledge of the encryption key, and vice versa, in any reasonable amount of time.

&nbsp;

### **2.5.8 - Asymmetric Encryption Algorithms**

Asymmetric algorithms use formulas that anyone can look up. The pair of unrelated keys is what makes these algorithms secure.

- **RSA (Rivest-Shamir-Adleman)** : Uses the product of two very large prime numbers with an equal length of between 100 and 200 digits. Browsers use RSA to establish a secure connection.
- **Diffie-Hellman** : Provides an electronic exchange method to share the secret key. Secure protocols, such as Secure Sockets Layer (SSL), Transport Layer Security (TLS), Secure Shell (SSH), and Internet Protocol Security (IPSec) use Diffie-Hellman.
- **ElGamal** : ElGamal uses the US government standard for digital signatures. This algorithm is free for use because no one holds the patent.
- **Elliptic Curve Cryptography (ECC)** : Uses elliptic curves as part of the algorithm. In the US, the National Security Agency (NSA) uses ECC for digital signature generation and key exchange.

&nbsp;

### **2.5.10 - Key Management**

Key management includes the generation, exchange, storage, use and replacement of keys used in an encryption algorithm.
It is the most difficult part of designing a cryptosystem. Many cryptosystems have failed because of mistakes in their key management procedures. In practice, most attacks on cryptographic systems target the key management level, rather than the cryptographic algorithm itself.
There are several essential characteristics of key management to consider :
- **Symmetric Encryption Algorithm** : 
    - Best known as shared-secret key algorithms
    - The usual key length is 80 to 256 bits
    - A sender and a receiver must share a secret key
    - Algorithms are usually quite fast (wire speed) because they are based on simple mathematical operations
    - Examples include 3DES, DES, AES, IDEA, RC2/4/5/6 and Blowfish
- **Asymmetric Encryption Algorithm** :
    - Best known as public key algorithms
    - The usual key length is 512 to 4096 bits
    - A sender and a receiver do not share a secret key
    - Algorithms are relatively slow because they are based on difficult computational operations
    - Examples include RSA, ElGamal, elliptic curves and DH

Two terms used to describe keys are :
- **Key length** - Also called the key size, this is the length of the key in bits
- **Keyspace** - This is the number of possibilities that a specific key length can generate.

As key length increases, the keyspace increases exponentially. The keyspace of an algorithm is the set of all possible key values. Longer keys are more secure; however, they are also more resource intensive.

&nbsp;

### **2.5.11 - Comparing Encryption Types**

- Symmetric encryption systems are more efficient and can handle more data. However, key management with symmetric encryption systems is more problematic and harder to manage.
- Asymmetric cryptography is more efficient at protecting the confidentiality of small amounts of data, and its size and speed make it more secure for tasks such as electronic key exchange, which involves a small amount of data rather than encrypting large blocks of data. It is more complex and requires more resources.

Maintaining confidentiality is important for both data at rest and data in motion. In both cases, symmetric encryption is favored because of its speed and the simplicity of the algorithm. Some asymmetric algorithms can significantly increase the size of the object encrypted. Therefore, in the case of data in motion, public key cryptography should be used to exchange the secret key, and then symmetric cryptography to ensure the confidentiality of the data sent.

&nbsp;

### **Notes**

Common key for encryption and decryption : Symmetric
Faster and uses less resources : Symmetric
Key management can become an issue as the number of users increases : Symmetric
Typically requires a third party key management service : Asymmetric
Use a public key to encrypt and a private key to decrypt : Asymmetric

&nbsp;

## **2.6 - Hashing**

&nbsp;

### **2.6.1 - What is hashing ?**

Hash functions are one-way functions used to verify and ensure data integrity. A hash tool can also verify authentication. It works by using a cryptographic hashing function to replace clear text passwords or encryption keys. If a password is hashed with a specific hashing algorithm, it will always result in the same hash digest. It is considered one-way because with hash functions, it is computationally infeasible for two different sets of data to come up with the same hash digest or output.
Every time the data changes, the hash value also changes. As a result, cryptographic hash values are often called digital fingerprints.

&nbsp;

### **2.6.2 - Hashing properties**

The one-way mathematical function of hashing is relatively easy to compute, but significantly harder to reverse. Grinding coffee is a good analogy for one-way functions: it is easy to grind coffee beans, but it is impossible to put all the tiny pieces back together to rebuild the original beans.
A cryptographic hash function has the following properties :
- The input can be any length.
- The output has a fixed length.
- The hash function is one-way and is not reversible.
- Two different input values will almost never result in the same hash.

&nbsp;

### **2.6.3 - Hashing algorithms**

Hash functions help to ensure that a user or communication error does not change data accidentally.

**ASCII code - character to binary** : The 8-bit checksum is the simplest form of a hash function. It calculates the hash by converting the message into binary numbers.

**Simple hash algorithm** : The algorithm adds up the 8-bit values and calculates the result using a process called 2’s complement. This process transforms a binary to its opposite value — zero converts to one, and one converts to zero. The final step of the process is to add 1 to produce an 8-bit checksum.

&nbsp;

### **2.6.4 - Modern hashing algorithms**

Many used today but most populars are MD5 and SHA.

**Message digest 5 (MD5) algorithm** : MD5 is a one-way function that makes it easy to compute a hash from the given input data but makes it very difficult to compute input data from a hash value. MD5 produces a 128-bit hash value.

**Secure Hash Algorithm (SHA)** : The U.S. National Institute of Standards and Technology (NIST) developed SHA, the algorithm specified in the Secure Hash Standard (SHS). NIST published SHA-1 in 1994. SHA-2 replaced SHA-1 with four additional hash functions to make up the SHA family:
- SHA-224 (224 bit)
- SHA-256 (256 bit)
- SHA-384 (384 bit)
- SHA-512 (512 bit)

SHA-2 is a stronger algorithm, and it is replacing MD5. SHA-256, SHA-384 and SHA-512 are the next-generation algorithms.

&nbsp;

### **2.6.5 - Hashing Files and Digital Media**

The field of digital forensics uses hashing to verify all digital media that contains files. For example, the examiner creates a hash and a bit-for-bit copy of the media containing the files to produce a digital clone. The examiner compares the hash of the original media with the copy. If the two values match, the copies are identical. The fact that one set of bits is identical to the original set of bits establishes fixity.

&nbsp;

### **2.6.10 - Salting**

Salting makes password hashing more secure. If two users have the same password, they will also have the same password hashes. A salt, which is a random string of characters, is an additional input added to the password before hashing. This creates a different hash result even when the two passwords are identical, as shown here. Then, the database stores both the hash and the salt. The same password generates a different hash for different users, because the salt in each instance is different. Meanwhile, the salt does not have to be secret since it is a random number.

&nbsp;

### **2.6.11 - Implementing salting**

A cryptographically secure pseudo-random number generator (CSPRNG) is the best way to generate salt. CSPRNGs generate a random number that has a high level of randomness and is completely unpredictable, so it is cryptographically secure.
The following recommendations will help ensure successful implementation of salting :
- The salt needs to be unique for every user password / Never reuse a salt
- The length of the salt should match the length of the hash function’s output.
- Always hash on the server, in a web application.

Using a technique called **key stretching** will also help to protect against attack. Key stretching makes attempts to figure out passwords work very slowly. This makes high-end attacker hardware that can attempt to crack billions of hashes per second less effective.

&nbsp;

### **2.6.12 - Preventing attacks**

Salting prevents an attacker from using a dictionary attack to try to guess passwords. Salting also makes it impossible to use lookup tables and rainbow tables to crack a hash.
- **Lookup tables** : A lookup table stores the pre-computed hashes of passwords in a password dictionary, along with the corresponding password. A lookup table is a data structure that processes hundreds of hash lookups per second.
- **Reverse lookup tables** : This attack allows the cybercriminal to launch a dictionary or brute-force attack on many hashes without the pre-computed lookup table. The cybercriminal creates a lookup table that plots each password hash from the breached account database to a list of users. The cybercriminal hashes each password guess and uses the lookup table to get a list of users whose password matched the cybercriminal’s guess. Since many users have the same password, the attack works well.
- **Rainbow tables** : Rainbow tables sacrifice hash-cracking speed to make the lookup tables smaller. A smaller table means that the table can store the solutions to more hashes in the same amount of space.

&nbsp;

### **2.6.12 - What is an HMAC operaion ?**

The next step in preventing a cybercriminal from launching a dictionary or brute-force attack on a hash is to add a secret key to the hash. Only the person who knows the hash can validate a password. One way to do this is to include the secret key in the hash using a hash algorithm called keyed-hash message authentication code (HMAC or KHMAC).

&nbsp;

## **2.7 - Obscuring Data**

&nbsp;

### **2.7.1 - Data Masking Techniques**

Data masking technology secures data by replacing sensitive information with non-sensitive versions of it. The non-sensitive version looks and acts like the original so that an organizational process can use non-sensitive data with no change needed to the supporting applications or data storage facilities.
Masking most commonly limits the propagation of sensitive data within IT systems by distributing surrogate data sets for testing and analysis. Information can be dynamically masked on the spot if the system or application detects a risky user request for sensitive information.
Several data masking techniques can be used :
- **Substitution** : replaces data with authentic-looking values to apply anonymity to the data records
- **Shuffling** : derives a substitution set from the same column of data that a user wants to mask. This technique works well for financial information in a test database, for example.
- **Nulling out** : applies a null value to a particular field, which completely prevents visibility of the data.

&nbsp;

### **2.7.2 - Steganography**

Steganography conceals data — e.g. a message — in another file such as a graphic, audio or video file. The advantage of steganography over cryptography is that the secret message does not attract any special attention. There are several components involved in hiding data. First, there is the embedded data, which is the secret message. The cover-text (or cover-image or cover-audio) hides the embedded data producing the stego text (or stego image or stego audio). A stego key controls the hiding process.

**Steganography techniques**

The approach used to embed data in a cover-image is using least significant bits (LSB). This method uses bits of each pixel in the image.
- A pixel is the basic unit of programmable color in a computer image.
- The specific color of each pixel is a blend of three colors; red, green and blue (RGB).
- Three bytes of data specify a pixel’s color (one byte for each color). Eight bits make up a byte so a 24-bit color system uses all three bytes.
- LSB uses a bit of each of the red, green and blue color components. Each pixel can store three bits.

On average, no more than half of the bits in an image will need to change to hide a secret message effectively.

**Social steganography**

Social steganography hides information in plain sight by creating output that can be read a certain way by some to get the secret message, based on previously set rules and/or definitions.

**Detection**

Steganalysis follows the discovery that hidden information exists. The goal of steganalysis is to discover this hidden information. Patterns in the stego image create suspicion. For example, a disk may have unused yet reserved areas, which are reserved because they hide information. Disk analysis utilities can report on hidden information in unused clusters of storage devices. Filters can capture data packets that contain hidden information in packet headers. Both of these methods use steganography signatures.

&nbsp;

### **2.7.3 - Packet Tracer**

steghide tool for steganography

&nbsp;

# **3 - System and Network Defense**

&nbsp;

## **3.1 - Defending Systems and Devices**

&nbsp;

### **3.1.4 - Patch Management**

**What are patches ?** Patches are code updates that prevent a new virus, worm or other malware from making a successful attack. Patches and upgrades are often combined into a service pack. 

&nbsp;

### **3.1.5 - Endpoint Security**

A host-based solution is a software application that runs on a local device (or endpoint) to protect it. The software works with the operating system to help prevent attacks.
- **Host-based firewalls** : A host-based firewall runs on a device to restrict incoming and outgoing network activity for that device. It can allow or deny traffic between the device and the network. The software firewall inspects and filters data packets to protect the device from becoming infected. Windows Firewall, installed by default during Windows installation, is an example of a software firewall.
- **Host intrusion detection system (HIDS)** : HIDS software is installed on a device or server to monitor suspicious activity. It monitors system calls and file system access to detect malicious requests. It can also monitor configuration information about the device held in the system registry.
- **Host intrusion prevention system (HIPS)** : HIPS is software that monitors a device for known attacks and anomalies (deviations in bandwidth, protocols and ports), or finds red flags by assessing the actual protocols in packets. If it detects malicious activity, the HIPS tool can send you an alarm, log the malicious activity, reset the connection and/or drop the packets.
- **Endpoint detection and response (EDR)** : EDR is an integrated security solution that continuously monitors and collects data from an endpoint device. It then analyzes the data and responds to any threats it detects. An antivirus can only block against threats, while EDR can do that and find threats on the device.
- **Data loss prevention (DLP)** : DLP tools provide a centralized way to ensure that sensitive data is not lost, misused or accessed by unauthorized users.
- **Next generation firewall (NGFW)** : NGFW is a network security device that combines a traditional firewall with other network-device-filtering functions. For example, an application firewall using in-line deep packet inspection (DPI) on an intrusion protection system (IPS).

&nbsp;

### **3.1.6 - Host encryption**

The Windows Encrypting File System (EFS) feature allows users to encrypt files, folders or an entire hard drive. Full disk encryption (FDE) encrypts the entire contents of a drive (including temporary files and memory). Microsoft Windows uses BitLocker for FDE. To use BitLocker, the user needs to enable Trusted Platform Module (TPM) in the BIOS. The TPM is a specialized chip on the motherboard that stores information about the host system, such as encryption keys, digital certificates and passwords. When enabled, BitLocker can use the TPM chip.

&nbsp;

### **3.1.7 - Boot integrity**

Boot integrity ensures that the system can be trusted and has not been altered while the operating system loads. Firmware — software instructions about basic computer functions — is stored on a small memory chip on the motherboard. The basic input/output system (BIOS) is the first program that runs when you turn on the computer.  Unified Extensible Firmware Interface (UEFI), a newer version of BIOS, defines a standard interface between the operating system, firmware and external devices. A system that uses UEFI is preferred over one that uses BIOS because a UEFI system can run in 64-bit mode.

*How does secure boot works ?*

Secure Boot is a security standard to ensure that a device boots using trusted software. When a computer system boots, the firmware checks the signature of each piece of boot software, including UEFI firmware drivers, UEFI applications and the operating system. If the signatures are valid, the system boots, and the firmware gives control to the operating system.

&nbsp;

### **3.1.8 - Physical protection of devices**

- **Computer equipment** : Use cable locks, keep telecommunications rooms locked, use security cages (faraday cages) around equipment to block electromagnetic fields.
- **Door locks** : A standard keyed entry lock is the most common type of door lock. They are often easy to force open. A deadbolt lock can be added for extra security. Any lock that requires a key is vulnerable if the keys are lost, stolen or duplicated. A cipher lock uses buttons that are pressed in a given sequence to open the door. It can be programmed so that a user’s code may only work during certain days or times. It can also keep a record of when the door opened, and the code used to open it.
- **Radio frequency identification (RFID) systems** : RFID uses radio waves to identify and track objects. RFID tags can be attached to any item that an organization wants to track. The tags contain an integrated circuit that connects to an antenna. RFID tags are small and require very little power, so they do not need a battery to exchange information with a reader. RFID can help automate asset tracking, or wirelessly lock, unlock or configure electronic devices.

&nbsp;

### **3.1.10 - Harden a linux system (ex)**

Lynis for system auditing.
iptables is the firewall installed by default on ubuntu.

&nbsp;

## **3.2 - Application Security**

&nbsp;

### **3.2.1 - Application development**

To maintain security at all stages of application development, a robust process needs to be followed :
- **Developing and testing** : Software is developed and updated in a development environment, where it can be developed, tested and debugged before being deployed. A development environment is less restrictive than the live environment and has a lower security level. Version control software helps track and manage changes to the software code. During testing, developers look at how the code interacts with the normal environment.
- **Staging and production** : Staging environments should closely match the organization’s production environment. By testing in a staging environment, developers can verify that the software runs under the required security settings. After the developer runs and tests security, the program can be deployed to production.
- **Provisioning and deprovisioning** : Provisioning is the creation or updating of software. Deprovisioning is its removal. An organization can use a self-service portal to automate software provisioning and deprovisioning.

&nbsp;

### **3.2.2 - Security Coding Techniques**

Developers use several techniques to validate that all security requirements have been met :
- **Normalization** : used to organize data in a database and help maintain data integrity. Converts an input string to its simplest known form to ensure that all strings have unique binary representation and that any malicious input is identified.
- **Stored procedure** : group of precompiled SQL statements stored in a database that execute a task. If you use a stored procedure to accept input parameters from clients using different input data, you will reduce network traffic and get faster results.
- **Obfuscation and camouflage** : Prevents software from being reverse-engineered. Obfuscation hides original data with random characters or data. Camouflage replaces sensitive data with realistic fictional data.
- **Code reuse** : means using existing software to build new software, saving time and development costs. Care must be taken, though, to avoid the introduction of vulnerabilities.
- **SDKs** : Third-party libraries and software development kits (SDKs) provide a repository of useful code to make application development faster and cheaper. The downside is that any vulnerabilities in SDKs or third-party libraries can potentially affect many applications.

&nbsp;

### **3.2.3 - Input validation**

Input validation is key to maintaining a database integrity. Many attacks run against a database and insert malformed data. Hackers can automate such kind of attacks to flood a web application.

&nbsp;

### **3.2.4 - Validation rules**

Validation rules can help ensure the security of databases by checking to see if data meets certain rules when entered into a field. A validation rule checks that data falls within the parameters defined by the database designer. This helps to ensure the completeness, accuracy and consistency of data.
The criteria used in a validation rule include the following:

- **Size** : checks the number of characters in a data item.
- **Format** : checks that the data conforms to a specified format.
- **Consistency** : checks for the consistency of code in related data items.
- **Range** : checks that data lies within a minimum and maximum value.
- **Check digit** : provides for an extra calculation to generate a check digit for error detection.

&nbsp;

### **3.2.5 - Integrity checks**

Compromised data can threaten the security of your devices and systems. The integrity check performs a **hash function**. A checksum is an example of a hash function.

**How a checksum works ?** : A checksum verifies the integrity of files, or strings of characters, before and after they transfer between devices across a local network or the Internet. Checksums convert each piece of information to a value and sum the total. To test the data integrity, a receiving system repeats the process. If the two sums are equal, the data is valid.

**Hash functions** : *See chapter 2.6*

**Version control** : Organizations use version control to prevent authorized users from making accidental changes. Version control means that two users cannot update the same object, such as a file, database record or transaction, at the exact same time.

**Backups** : Accurate backups help to maintain data integrity if data becomes corrupted.

**Authorization**

&nbsp;

### **3.2.6 - Other application security practices**

**Code signing** : proves that a piece of software is authentic. 

**Secure cookies** : Using secure cookies protects information stored in cookies from hackers. When your client system interacts with a server, the server sends a HTTP response that instructs your browser to create at least one cookie. The cookie then stores data for future requests while you are browsing that website. Web developers should use cookies with HTTPS, to secure cookies and prevent them from being transmitted over unencrypted HTTP.

&nbsp;

### **3.2.7 - Managing threats to applications**

Organizations can implement various measures to manage threats to the application domain.
- Unauthorized access to data centers, computers rooms and wiring closets
- Server and system downtime
- Network operating system software vulnerability
- Unauthorized access to systems
- Data loss
- Software development vulnerabilities

&nbsp;

## **3.3 - Network hardening : services and protocols**

&nbsp;

### **3.3.1 - Network and routing services**

- **DHCP** : Attackers can target DHCP servers to deny access to devices on the network, but security measures like DHCP snooping prevent rogue DHCP servers from providing IP addresses to clients by validating messages from sources that are not trusted. Ensure that the DHCP is physically secure, up to date, patched, unused ports are closed, logging, etc...
- **DNS** : Attackers can target DNS servers to deny access to network resources or redirect traffic to rogue websites. To secure it, prevent version string from revealing information, separate internal and external DNS, restrict allowed transactions by client IP addr, use transaction signatures, disable or restrict zone transfers and dynamic updates as much as possible, logging, use domain name system security extensions (DNSSEC), sign zones.
- **ICMP** : Cybercriminals can alter the use of ICMP to run reconnaissance, denial of service (DoS) and covert channel attacks. Many networks filter ICMP requests to prevent such attacks.
- **Routing information protocol (RIP)** : RIP is a routing protocol that limits the number of hops from source to destination that are allowed in a network path. The maximum number of hops allowed for RIP is fifteen. RIP is used to exchange routing information about which networks each router can reach and how far away those networks are. RIP calculates the best route based on hop count, but cybercriminals can also target routers and the RIP protocol. Such attacks on routing services can affect performance and availability, some attacks can even result in traffic redirection. Use secure services with authentication and implement system patching and updates to protect routing services.
- **NTP** : Cybercriminals attack timeservers to disrupt secure communication that depends on digital certificates and to hide attack information. Use NTP Authentication to verify that the server is trusted.

&nbsp;

### **3.3.2 - Telnet, SSH and SCP**

SSH uses port 22.

Secure Copy (SCP) securely transfers files between two remote systems. SCP uses SSH for data transfer and authentication, ensuring the authenticity and confidentiality of the data in transit.

&nbsp;

### **3.3.3 - Secure protocols**

- **Simple Network Management Protocol (SNMP)** : SNMP collects statistics from TCP/IP devices to monitor network and computer equipment. SNMPv3 is the current standard — it uses cryptography to prevent eavesdropping and make sure data hasn’t been tampered with while in transit.
- **HTTP** : Limited built-in security, can be made more secure with the use of other protocols :
    - **Secure Sockets Layer (SSL)** manages encryption by using an SSL handshake at the beginning of a session to provide confidentiality.
    - **TLS** prevents eavesdropping and tampering
    - SSL/TLS encrypts communication between the client and the server. Where it’s used, the user will see **HTTPS** in the URL field of a browser instead of HTTP.
- **FTP** : uses plaintext username/password. **FTPS** is more secure — it adds support for TLS and SSL to prevent eavesdropping, tampering and forgery on exchanged messages.
- **POP, IMAP and MIME** : Email uses Post Office Protocol (POP), Internet Message Access Protocol (IMAP) and Multipurpose Internet Mail Extensions (MIME) to attach non-text data, such as an image or video, to an email message. To secure POP (port 110) or IMAP (port 143), use SSL/TLS to encrypt mail during transmission. The Secure/Multipurpose Internet Mail Extensions (S/MIME) protocol provides a secure method of transmission. It sends digitally signed and encrypted messages that provide authentication, message integrity and nonrepudiation.

&nbsp;

## **3.4 - Network hardening : Securing network devices**

&nbsp;

### **3.4.1 - Switches, routers and network appliances**

Network switches are subject to ARP/STP attacks. Other protocols can be attacked too. Firewalls are subject to ACLs attacks. Routers are subject to routing protocols attacks.

A UTM can be connected to the main network to provide maximum security against all incoming viruses. A UTM appliance carries out a diverse range of functions. It:
- Balances the load in a network.
- Prevents data leaks that might occur.
- Provides a gateway antivirus solution.
- Provides network intrusion prevention and on-appliance reporting.

Multiple types of firewalls : 

- A **stateless firewall** provides basic traffic filtering capabilities using access control lists (ACLs). Administrators use ACLs to stop traffic or permit only specified traffic on their networks. An ACL is a sequential list of permit or deny statements that apply to addresses or protocols.
- A **stateful firewall** inspects traffic leaving the network and monitors the establishment of a stateful connection. Traffic associated with the established (stateful) connection is then permitted.
- A **content-filtering firewall** works by specifying content patterns (text strings or objects within images) that, if matched, indicate undesirable content that is to be screened out. 
- A **web application firewall (WAF)** filters, monitors and blocks HTTP traffic to and from a web service.
- A **next-generation firewall (NGFW)** combines a traditional firewall with other network device filtering functions, such as an application firewall using in-line deep packet inspection to examine the actual data within the packets transmitted.

&nbsp;

### **3.4.3 - Intrusion detection systems**

An IDS monitors the traffic on a network to identify threats. An IDS-enabled device copies network traffic and analyzes the copy rather than the actual forwarded packets.

*How does an IDS work ?*

Working offline, compares network traffic with known malicious signatures.
- Works passively
- Physically positioned in the network so that traffic must be mirrored to reach it
- Network traffic doesn't reach the IDS, only copies of it that are mirrored.

An IDS is passive and operates in promiscuous mode, meaning it monitors and reports on traffic but does not take any action. 

*Advantages of an IDS*

The advantage of operating with a copy of the traffic is that the IDS does not negatively affect the packet flow of the forwarded traffic.

*Disadvantages of an IDS*

The disadvantage of operating on a copy of the traffic is that the IDS cannot stop malicious single-packet attacks from reaching their target before it responds to the threat. An IDS often requires assistance from other networking devices, such as routers and firewalls, to respond to an attack.

&nbsp;

### **3.4.4 - Intrusion prevention systems**

An IPS builds on IDS technology but works inline, within the data stream. This means that all traffic must flow through it for processing. Unlike IDS, an IPS does not allow packets to enter the trusted side of the network unless it has analyzed them first. An IPS can detect and immediately address a network problem.

*How does an IPS work ?*

An IPS monitors network traffic and analyzes packets for malicious activities. Some systems use a blend of detection technologies, including signature-based, profile-based and protocol analysis-based intrusion detection. This deeper analysis enables the IPS to identify, stop and block attacks that would have passed through a traditional firewall. When a packet comes through an interface on an IPS, the outbound or trusted interface does not receive that packet until the IPS analyzes it and signals it can go through.

*Advantages of an IPS*

The advantage of operating in inline mode is that the IPS can stop single-packet attacks from reaching the target system.

*Disadvantages of an IPS*

The disadvantage of this technology is that a poorly configured IPS can negatively affect the packet flow of the forwarded traffic.

&nbsp;

### **3.4.5 - NetFlow and IPFIX**

NetFlow is a Cisco IOS technology that provides statistics on packets flowing through a Cisco router or multilayer switch. NetFlow is the standard for collecting operational data from networks. The Internet Engineering Task Force (IETF) used Cisco’s NetFlow Version 9 as the basis for IP Flow Information Export (IPFIX).

IPFIX is a standard format for exporting router-based information about network traffic flows to data collection devices. IPFIX works on routers and management applications that support the protocol.

Collecting, storing and analyzing information from IPFIX-supported devices helps:
- Secure the network against internal and external threats.
- Troubleshoot network failures quickly and precisely.
- Analyze network flows for capacity planning.

&nbsp;

### **3.4.6 - Network access control**

Network Access Control (NAC) is a networking solution that protects a private network from unauthorized users and devices. NAC only allows authorized users with security-compliant systems to access the network. For example, a laptop that is part of a home wireless network may not be allowed to connect remotely to the office network. A NAC framework can use the existing network infrastructure and third-party software to enforce security-policy compliance for all devices. A NAC appliance controls network access, evaluates compliance and enforces security policy. A common NAC systems checklist includes:
- Updated virus detection.
- Operating systems patches and updates.
- Complex password enforcement.
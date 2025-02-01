# Malware

### Viruses

 Computer virus :  These are the malicious programs that made of malicious code that runs on a machine without the user's knowledge and this allow the code to infect the computer whenever it has been run.

 10 Different types of Viruses
 
 - Boot sector : This is the virus that is stored in the first sector of a hard drive and is then loaded into the memory whenever the computer boots up.
 
 - Macro : This is a form of code that allows a virus to be embedded inside another document so that when the document is opened by the user, the virus is executed.
 
 - Program : This type of virus tries to find executable or a application file to infect with their malicious code.
 
 - Multipartite : This a combination of boot sector type virus and a program virus. This type of virus place itself in the boot sector and is loaded every time the computer is boots. It can install a program where it can be run every time the system boots up.
  
 - Encrypted : It is designed to hide itself from being detected by encrypting it's malicious code or payloads to avoid detection by any antivirus software. 
 
 - Polymorphic : This is a type of an encrypted virus, but instead of just encryption of the code it also changes the virus code each time when it is executed by altering the decryption module in order for it evade detection. 
 
 - Metamorphic : This type of virus is able to re-write themself entirely before it infects a given file. 
 
 - Stealth : This is a technique that is used to prevent the virus from being detected by the anti-virus software.
 
 - Armored : This type of virus have a layer of protection to confuse a program or a person who's trying to analyse it.
 
 - Hoax : It is a from of technical social engineering that attempts to scare our end user into taking some kind of undesirable action on their system.
### Worms
These are the piece of malicious software, much like a virus, but it can replicate itself without any user interaction. These software are able to self replicate and spread throughout your network without user's consent or their action. 
Worms are dangerous for 2 reasons:
- They infect your workstation and other computing assets 
- These causes disruption to your normal network traffic as they are constantly trying to replicate and spread across the network.
The worms are best known for their ability of spreading far and wide over the internet in a relative short amount of time.

### Trojans 
 
 These are the piece of malicious software that is disguised as a piece of harmless or desirable software. It disguise themself in form of useful piece of software.

Remote Access Trojan (RAT) : These ae widely used by modern attacker because it provides the attacker with remote control of victim machine.

Trojan are commonly used today by attacker to exploit a vulnerability in your system and then conduct data exfiltration to steal your sensitive documents, creating backdoors to maintain persistence on your system and other malicious activities.

### Ransomware 

Ransome are the type of malicious software that is designed to block access to a computer system or it's data by encrypting it until a ransom is paid to the attacker. 

To protect against Ransome one can take safety precaution like: 
Always conduct regular backups.
Install software update regularly.
Provide security awareness training to your users.
 Implement Multi-Factor Authentication (MFA).

What should you do if you find yourself or your organization as the victim of a ransomware attack :
- Never Pay the ransom  : paying the ransom doesn't actually guarantee that you will  ever get your data back. 
- If you suspect ransomware has infect your machine you should disconnect it from the network. 
- Notify the authorities.
- Restore your data and system form known good backups.
### Zombies and Botnets

Botnet: network of compromised computer or device that is part of s botnet.

Zombie : It is a name of a compromised computer or devices that is part of a botnet.  Used to perform task using remote commands form the attacker without the user's knowledge.

Command and Control Node : Computer responsible for managing and coordinating the activities of other nodes or devices within a network.

Botnets are used :
- As pivot points
- disguise the real attacker
- to host illegal activities
- To spam others by sending out phishing campaigns and other malware
The most common use for botnets is to conduct a DDoS (Distributed Denial of Service) attack. 
Most common use for a botnet is to conduct a DDoS (Distributed Denial-of-Service) attack        Distributed Denial-of-Service (DDoS) Attack : Occurs when many machines target a single victim and attack them at the exact same time 
Botnets are used by attackers to combine processing power to break through different types of encryption schemes. Attackers usually only use about 20-25% of any zombie’s power.

### Rootkits 
Rootkit: These are the program that are designed to gain administrative level control over a given computer without being detected. 

Account with the highest level of permission is called the administrative account. These  types of account allows the person to install program delete program, open port, shut port, and do whatever it is they want to do in that system. In Unix, Linux, MacOS computer these type of administrative account is called root account. 
 
A computer have different rings of permission throughout the system.
Ring 3 (Outermost Ring) : These are the user level permission are used.
Ring 0 (Innermost or highest Permission Levels) : Operating in this ring 0 is called "Kernel Mode". 

Kernel Mode : It allows a system to control access to thing like device drivers, your sound card, your video display or monitor, and other similar things.

If you login as the administrator or root user on a system, you have root permission and you will be operating at Ring 1 of the operating system. The closer the malicious code is to the kernel, the more permissions it will have and more damage it can cause on the system.

When the Rootkit is installed on a system, it tries to move from ring 1 to ring 0 so that it can hide from other function of the operating system to avoid detection.

One Technique used by the rootkit to gain this deeper level of access is a DLL injection

DLL injection: This technique used to run arbitrary code within the address space of another process by forcing it to load a dynamic-link library.

Dynamic Link Library (DLL) : It is a collection of codes and data that can be used by multiple programs simultaneously to allow for code reuse amd moudulation in software development.

Shim : This piece of software code that is placed between two components and that intercept the calls between component and can be used to redirect them.

Rootkits are extremely powerful and are very difficult to detect as the operating system is essentially blind to them.

the best way to detect them it to mount live bootable Linux distribution OS from a external device and scan the the whole internal drive. always use high quality antimalware and scanning software as these are very hard to detect.


### Back Door  and Logic Bombs

**Backdoor** : These were originally placed in the computer program to bypass the normal security and authentication functions. These were put into the system by designer and programmers during the development process for easier access. 
Modern Remote Access Trojan (RAT) act just like the backdoor in todays network i.e. they maintain persistent access to that system  like using a backdoor. These are placed by the Malicious threat actor.

**Easter Egg** : These are the hidden features or novelty within a program that is typically inserted by the software developer as an inside joke. These codes often have significant vulnerabilities that can hamper the security.

Logic Bombs : These are the malicious code that's inserted into the program, these malicious code will only execute when certain conditions have been met.


### Keylogger

Keylogger: Keylogger is a piece of software or hardware that records every single keystrokes that is made on the computer or mobile device.

Keylogger are of two types:
1) Software Keylogger: It is a malicious program that gets installed on the system by an attacker. These are often bundled with other software or are delivered through social engineering attacks like phishing or pretexting attacks. 
2) Hardware Keylogger: These are the physical devices that need to be plugged in computer in order to record the data. These will resemble a USB drive or they can be embedded within the keyboard itself.

To protect against these keylogger are :

-Perform regular updates and patches.
-Rely on quality antivirus and antimalware solution.
-conduct phishing awareness training for the end user.
-implement multi factor authentication system
-Perform physical check of your desktop, laptop, and servers

Spyware and Bloatware

Spyware: These are the malicious software that is designed to gather and send information about a user or organization without it's knowledge. Spyware can get installed on a system in several different ways:

Bundled with other software
Installed through a malicious website
Installed when user clicks on a deceptive pop-up advertisement.

To protect against these spyware one should only use reputable antivirus and anti-virus tools that regularly gets updated and remove any potential threats.

Bloatware: Any software that comes pre installed on a new computer or smartphone that you as a user do not requested, want or need. Other examples of bloatware are things like unnecessary toolbars or application that promote certain services.
Bloatware isn't malicious but it can:
- Waste your storage space
- slow down the performance of your devices
- Introduce security vulnerabilities into your systems


**<font color="#ffff00"> Remember anytime a piece of software is installed, that is one more potential threat vector for an attacker to exploit if you don’t properly update that application </font>

To remove bloatware, you can either do the following 

- Do a manual removal process.
- Use bloatware removal tools to uninstall the unwanted applications.
- Perform a clean operating system installation.

Malware Attack Techniques
Specific method by which malware code penetrates and infects a targeted system
Some malware focuses on infecting the system’s memory to leverage remote procedure calls over the organization’s network. 
Most modern malware uses fileless techniques to avoid detection by signature-based security software. Fileless Malware is used to create a process in the system memory without relying on the local file system of the infected host
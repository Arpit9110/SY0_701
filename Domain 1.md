# CIA Triad : Confidentiality, Integrity and Availability.

# Confidentiality:
This refers to the process by which data is protected form Unauthorizes user & it is only visible to authorized and authentic user. It ensures access disclosure to authentic user only.

Importance of confidentiality:-

 - Protect personal privacy .
 - Maintain a business advantage.
 - Achieve regulatory compliance.

#### Basic methods to add in on confidentiality.

- Encryption: Making plain text to into a indistinguishable data that will only be decrypted by decryption key.

- Access control :Process of restricting the access to the data so that only Authorised person can access the data by using methods like pin, password, permission.  

- Data Masking : In this process of modifying sensitive data in such a way that it is of no use to unauthorised user but still be usable to authorised user.  Ex.. Hiding the  first 11-12 number showing the last 4-5 digit of 16 digit numbers of the credit card to confirm the card number to the end user while hiding the rest so that only enough data is revealed that needed to be shown.

- Physical security measure: It concerns with physical security like locking the drawer with confidential document, putting security cameras, biometric gate locks, Security guards, access control to the server rooms and documents room etc.

- Training and awareness: This aims to focus on the awareness of the CIA model and specifically to the confidentiality of the data. How to handle confidential data, how to manage it and work with it.

The most common way to ensure the confidentiality is to implement the ENCRYPTION which prevent most of the security concerns related to the confidentiality.

Confidentiality is generally associated to ENCRYPTION

# Integrity: 
This refers to the protecting the originality of the data or the information. It refers to protection against alteration by unauthorized personals. It ensure that the data is accurate, un-altered and reliable.
It verifies the accuracy and trustworthiness of the data, when it is transferred, stored and displayed .It ensures that the original data is unchanged until the authorised user do it intentionally.

#### Three main importance of data integrity:

- Ensure Data Accuracy. : This is most important as in scenarios like financial transaction or medical records the accuracy of data matters the most.

- Maintain Trust. : It is about maintaining trust with end users and with the systems and network. According to the business point of view the user trust in the system is most important like in bank is a zero at the end of the amount in the account is removed the trust of that user will decline in the bank and the user will remove it's business from that bank.

- Ensure System Operability. : It the data get corrupted then it can crash the software of make it unresponsive. This can lead to system failure and system downtime. It will affect the business operation which will lead to financial loss. 

## Five method to implement integrity are:

- Hashing: Hashing is the process of creating a digest that will of fixed size for any file. It's value is unique for each  file and will change even if a blank space is added to the file. It is very helpful in detecting the alteration in the data.

- Digital signatures: It usages both encryption and hashing. In this a hash is generate for the file then this file is embedded with that hash. But the hash is fist encrypted with the private key of the client to maintain the secrecy of the file. When the file is received and the hash obtained from the digital signature is compared with the one freshly calculated hash is the matched for the integrity check.

- Checksum: This process involves calculating a check sum using mathematical process and sending it along the data to the client, the client then receives the data and compare the received checksum with the freshly calculated checksum for integrity check.

- Access Control: It ensures that only authorized users will be able to alter the data. It decreases the chance of getting the data altering to a minimum.

- Regular audits. It involves systematically reviewing logs and operations to ensure that only authorized changes have been made and any discrepancies are addressed.

Generally Integrity is associated with HASHING as for the Integrity implementation HASHING is used to authenticate the data.

# Availability: 
It refers to data being available to use for user when intended. It concerns with the availability of data in any scenario.
### Importance of Availability:-

- Ensuring Business Continuity: As downtime means the business is not able to generate revenue as the main application is not working, thus loosing revenue as well as customer and their trust. Downtime can arise due to many factors at play like cyber attack, data corruption, Network loss, server down due to excessive load etc.

- Maintaining Customer Trust: 

- Upholding an Organization's Reputation:

Redundancy is used in the network and software design to enhance the availability of the system.

### Redundancy 
It refers to the duplication of critical software process, critical component, critical functions with objective of improving/enhancing it's reliability. It's like having a backup server which take over as soon as main system fails.

### Types of redundancy:-

- Server redundancy : It means to have a backup server with load balancer or in failover configuration to provide continuous availability to access to the software.
 
- Data redundancy : It means to store data in different Raid formation OR in combination of remote and physical server to provide better backup and availability in case of data failure, disaster, Cyber attack, Disk Failure etc.

- Network redundancy  : It means to create enough connection so that even if a link goes down it still could be routed using other paths.

- Power redundancy : It Means to have a alternate source of backup power as the main power source goes down. It also require the backup power to last for couple of hours until the main power source is back online.


## <font color="#c00000">Availability is often related to Redundancy.</font>
 
 
 #### <font color="#ffff00">These are the CIA triads by now a days there are 2 more factors</font>

## Non-Repudiation: 
It guarantee that a specific action event has take place and cannot be denied by the both the parties involved. It can be achieved by logging every action, process by users as well as the process initiating any process or features.

## Authentication:
It refers to the process of verifying the identity of a user or a system.

# " CIA triad is now a days transformed to:-  CIANA  by adding non-repudiation and Authentication making it a security polygon."


## Triple A (AAA) of security: Authentication, Authorization, Accounting.

### Authentication: 
It is a security measure that ensure the identity of a individual  or entities about  who they claim to be during starting or accessing a process, data feature.

It can be done by many ways:

### Something User knows ( Knowledge Based ).
  Like Password, Username, Pin code.

### Something User have ( Possession Based ).
  Like security key , key card, RFID card, ID card, OTP.

### Something User is ( Biometric Based ).
  Like Finger-print, Iris scan, Retina scan.

### Something User do ( Action Based ).
  Like Authentication at a particular days of a week like not available on Saturday, Sunday,
       Authentication is performed only after logging in organization private network.

### Something where a user is ( Location Based ).
  Like Authentication only when user is in organization's office geo-location.

Multifactor Authentication:-> It refers to using two or more factor of authentication to get identity so that  authentication process of a user gets initiated.

### Authorization: 
it is the Process to grant the permission and privilege to the user whose authentication process is Successfully finished  and is authenticated.

There are may ways for deciding the permission and privileges. Role Based, Group Based, Action Based, etc.

### Accounting: 
It is process of tracking user activity and the process running in the background. It also track the user clicks, Resources usages, and every process user does, starts, stops. It is generally done for audit trials, security audit, Forensics check and billing purpose.


Security Controls-> These are the method , technique and mechanisms put in place to mitigate risk and protect the CIA Trials of Information System and Data.

##4 Broad categories of Security Control.

### Technical Control 
It involves the hardware and software component that protect a system against cyberattacks. Example Firewall(both physical and software), IDS(Intrusion Detection System), IPS (Intrusion prevention system) etc.

### Managerial Controls
It is also referred to as administrative controls. It involves strategic planning and governance side of security.

### Operational Controls
The process and measure that are designed to protect data and information on day-to-day basis. It more like daily measures takes to protect the data from malicious actors. It governs Internal process and human actions.

### Physical Controls
It concerns with the physical aspect of the security like physical access to the server, unauthorized access to the physical hardware, Vandalism of the server, fire protection, Disaster protection, Power outrage etc. This can be done by allotting security guards, implementing access control, Fire safety equipment, Having Boundaries and reinforcing it with barb-wires, implementing Earthquake protection measures.

## 6 Basic Types of Security Control

### Preventive Controls.
Proactive measure implemented to throw away the potential security threats or breaches.

### Deterrent controls.
Discourage potential attackers by making the effort seen less appealing and more challenging. 

### Detective controls.
Monitor and altering  organizations to malicious activities as they are happening or shortly thereafter. 

### Corrective Controls.
Mitigate any potential damage, error, corruption and restoring a system to normal  state.

### Compensating Controls.
Alternative measures that are implemented when primary security control are not feasible or effective.

### Directive controls.
These are guide, information and mandatory actions. These are often rooted in policy are documentation and det the standards for behaviour within in an organization.

##### Zero trust:- It is the process that demands verification for every use or transaction within the trusted network regardless of it's privileges and permission. It sate that do not trust any user and treat every user as an unauthorized personal until verified it's identity. 

## Zero trust architecture required 2 different plane for its implementation:-

## Control Plane: 
It refers to the overwatching framework and set of components responsible for defining, managing and enforcing the policies related to user and system access within an organization.

### Key element for control plane are:

#### Adoptive identity:

Relies on real time validation that takes into account user's behaviour, device, location and more.

#### Threat Scope Reduction:

Limit the users access to only what they need for their work task because this reduces the network's potential attack surface. Focused on minimizing the "blast radius" that could occur in the event of a breach.

#### Policy Driven Access Control:

Entails developing, managing and enforcing user access policies based on their roles and responsibilities.

#### Secured Zone:

Isolate environments within a network that are designed to house sensitive data.


## Data plane: 
It ensures that the policies are properly implemented and are being executed in a right way.

### Key components of Data plane are:

#### Subject/System:

refers to the individual or an entity that is trying to gain access of the system.

#### Policy Engine:

These the engine or the process that cross reference the access request with it's predefined policies.

#### Policy Administrator:

They are the people that use to establish and manage the access policies in the organization or the system.

#### Policy Enforcement Point:

This is the part of the system that execute weather  to grant or deny access to the system.

# Threat and Vulnerabilities

## Threat

Anything that could Cause harm, Create loss, Damage or compromise our information technology systems is termed as threat. 
### These threat can arise from various sources like:

- Natural Disaster. 
- Cyber Attacks.
- Data Integrity breach.
- Disclosure of sensitive data or confidential information.

# Vulnerabilities
	
Any weakness or flaw in the system that was left in the system either by design or logic is refered to as Vulnerabilities. These can arise due implementation error or implemented in misconfigured form.
These vulnerabilities can be used by malicious actors to gain acess to the sysem, data, network, control over hardware interface etc. Essentially these vulnerability are used to hack into the system.
#### These also comes from some internal factors like:-

- software bugs
- Misconfigured Software
- Improperly protected network devices
- Missing Security patches
- Lack of physical security

### <font color="#ffff00"> Where threats and vulnerabilities intersect , That is where the risk to your enterprise system and networks lies.</font>
### <font color="#ffff00"> If you have a threat, but there is no attached/matching vulnerability  to it , Then you have no risk and vice versa.</font>
### <font color="#ffff00"> The same holds true that if you have a vulnerability but there's no threat against it then there would be no risk.</font>

# Risk

This measure is the combination of the likelihood that a threat exploits a vulnerability and the scale of harmful consequences.

Risk = (Probability that a threat occurs) * (Cost to the asset owner)

## Risk Management 
Finding different ways to minimize the likelihood of an certain outcome  and achieve the desire outcome.

### Gap Analysis

It is the process of evaluating the differences between an organization's current performance and its desired performance. Conducting a gap analysis can be a valuable tool for organizations looking to improve their operations, process, performance or overall security posture.
#### There are several steps involved in conducting a gap analysis:-
- Define the scope of the analysis.
- Gather data on the current state of the organization.
- Analyse the data to identify any areas where the organization's current performance fall short of it's desired performance.
- Develop a plan to bridge the gap.

## 2 Basic type of Gap Analysis

#### Technical Gap Analysis

Involves evaluating an organization's current technical infrastructure. it aims to identify any areas where it fall short of this technical capabilities required to fully utilize their security solutions.

#### Business Gap Analysis

Involves evaluating an organization's current business processes. It also identifies any areas where they fall short of the capabilities required to fully utilize cloud-based solutions.

#### Plan of Action and Milestone (POA&M)

It outlines the specific measures to address each vulnerability and allocates resources for it also. It also set up timelines for each remediation task that is needed.


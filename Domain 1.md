# CIA Triad : Confidentiality, Integrity and Availability.

## Confidentiality:
This refers to the process by which data is protected form Unauthorizes user & it is only visible to authorized and authentic user. It ensures access disclosure to authentic user only.

## Integrity: 
This refers to the protecting the originality of the data or the information. It refers to protection against alteration by unauthorized personals. It ensure that the data is accurate, un-altered and reliable.

## Availability: 
It refers to data being available to use for user when intended. It concerns with the availability of data in any scenario.

- These are the CIA triads by now a days there are 2 more factors:

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
Key element for control plane are:

### Adoptive identity:

Relies on real time validation that takes into account user's behaviour, device, location and more.

# Threat Scope Reduction:

Limit the users access to only what they need for their work task because this reduces the network's potential attack surface. Focused on minimizing the "blast radius" that could occur in the event of a breach.

# Policy Driven Access Control:

Entails developing, managing and enforcing user access policies based on their roles and responsibilities.

# Secured Zone:

Isolate environments within a network that are designed to house sensitive data.


## Data plane: 
It ensures that the policies are properly implemented and are being executed in a right way.

Key components of Data plane are:

## Subject/System:

refers to the individual or an entity that is trying to gain access of the system.

## Policy Engine:

These the engine or the process that cross reference the access request with it's predefined policies.

## Policy Administrator:

They are the people that use to establish and manage the access policies in the organization or the system.

## Policy Enforcement Point:

This is the part of the system that execute weather  to grant or deny access to the system.

## Threat and Vulnerabilities

#### Threat

Anything that could cause harm, create loos, Damage or compromise our information technology systems is termed as threat. 
These threat can arise from various sources like:

Natural Disaster. 
Cyber Attacks.
Data Integrity breach.
Disclosure of sensitive data or confidential information.

## Vulnerabilities

Any weakness or flaw in the system that was left in the system either by design or logic is referred to as Vulnerabilities. These vulnerabilities can be used by malicious actors to gain access to the system, data, network, control over hardware interface etc. Essentially these vulnerability are used to hack into the system.


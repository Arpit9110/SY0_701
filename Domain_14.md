
# Security Architecture

### On-premise versus the Cloud

Cloud Computing
 
 It is the delivery of computing services over the internet, including servers, storage, database, networking, software, analytics and intelligence.
 It's advantages are:
  - faster Innovation
  - Flexible resources
  - Economies of scale
  
Responsibility Matrix
 It outlines the division of responsibilities between the cloud service provider and the customer.
 
Third-Party Vendors
 These are the providers that specialized in services to enhance functionality, security and efficiency of cloud solutions.
 
Hybrid Solutions
 This solution combined on-premise, private cloud, and public cloud services, allowing workload flexibility. 
 It's considerations includes: 
   - Sensitive data is protected.
   - Regulatory requirement are met.
   - System can communicate with each other.
   - The solution is cost-effectiveness.

On-Premise solutions
 These includes Computing infrastructure physically located on-site at a business.
 
Key Considerations in cloud Computing

 - Availability: System's ability to be accessed when needed
 
 - Resilience: System's ability to recover from failures.
 
 - Cost: Consider both upfront and long-term costs.
 - Responsiveness: Speed at which the system can adapt to demand.
 
 - Scalability: System's ability to handle increased workloads.
 
 - Ease of Deployment: Cloud services are easier to set up than on-premise solutions.
 
 - Risk Transference: Some risks are transferred to the provider, but mostly customers are responsible for security.
 
 - Ease of recovery: Cloud services offer easy data recovery and backup solutions.
 
 - Patch Availability: Providers release patches for vulnerabilities automatically.
 
 - Inability to patch: Compatibility issues or lack of control can hinder patching.
 
 - Power: Cloud provider manages infrastructure, including power supply. The 

 - Compute: Refers to computational resources, including CPUs, memory, and storage, as cloud providers offer various compute options to suit different needs.
 
 
Remember
 - Cloud computing offers flexibility, scalability, and cost-effectiveness.
 
 - On-premise solutions provide control and security but can be expensive and challenging to maintain.
 
 - Hybrid solutions offer flexibility and control but require considerations of security, compliance, interoperability, and cost.
 
 

### Cloud Security

Shared Physical Server Vulnerabilities

 In cloud environments, multiple users share the same physical server. It leads to compromisation of data , as data from one user can potentially impact others on the same server.
 
 Mitigation includes implementation of strong isolation mechanisms such as hypervisor protection, secure multi-tenancy. alos by performing regular vulnerability scanning, and patching  security gaps.
 
Inadequate Virtual Environment Security

 Virtualization is essential in cloud computing and inadequate security in the virtual environment can lead to unauthorized access and data breaches.

Mitigation of this includes:
 - Use secure VM templates
 - Regularly update and patch VMs
 - Monitor for unusual activities
 - Employ network segmentation to isolate VMs
 
User Access Management

 Weak user access management can result in unauthorized access to sensitive
data and systems. 
 To mitigate this problem includes:
   - Enforce strong password policies
   - Implement multi-factor authentication
   - Limit user permissions (Principle of Least Privilege)
   - Monitor user activities for suspicious behavior

Lack of Up-To-Date Security Measures

 Cloud environments are dynamic and require up-to-date security measures and lack of up-to-date security measure, as failure to update can leave systems vulnerable to new threats.
 
 Mitigation to this problem includes:
  - Regularly update and patch software and systems
  - Review and update security policies
  - Stay informed about the latest threats and best practices
  
Single Point of Failure
 
 Cloud services relying on specific resources or processes can lead to system-wide outages if they fail. 
  It's Mitigation includes: 
   - Implement redundancy and failover procedures
   - Use multiple servers, data centers, or cloud providers
   - Regularly test failover procedures
   
Weak Authentication and Encryption Practices

 Weak authentication and encryption can expose cloud system and data, this can relust to unsuthorisedd access and data leaks.
 The mitigation of this problem:
   - Use multi-factor authentication.
   - Strong encryption algorithms.
   - Secure key management parctices.

Unclear Policies
 
 Unclear security policies can lead to confusion and inconsistencies in implementing security measures
  The mitigation includes:
   - Develop clear and comprehensive security policies covering data handling, access control, incident response, and more. 

   - Regularly review and update policies and provide effective communication and training.


Data Remnants
 Data Remnants
  Data remnants is the residual data left behind after deletion or erasure processes. In cloud environment, data may not be completely removed, posing a security risk and may lead to data leak.
  
 The mitigation involves:
   - Implement secure data deletion procedures.
   - Use secure deletion methods.
   - Manage backups securely.
   - Verify data removal after deletion

Remember: The cloud security is always a shared responsibility.


### Virtulization and Containerization

 Virtualization
  It means to emulation of servers, each server with it's own OS within a virtual machine.
   
 Containerization
  It is a lightweight alternative, this technoloy encapsulate app with their OS environment.
  Key Benefits are:
   - Efficiency and Speed
   - Portability
   - Scalability 
   - Isolation
   - Consistency
    
 Hypevisors
 
  There are two types of hypervisors namely :
  
  Type 1 (Bare Metal): In this the hypervisor runs directly on Hardware eg. Hyper-V, XenServer, ESXi.
  
  Type 2 (Hosted): In thid the hypervisor operates within a standard OS eg. VirtualBox, VMware.
  
 
 Virtualization Vulnerabilities
 
  Virtual Machine (VM) Escape : Attackers break out of isolated VMs to access the hypervisor.
  
  Privilege Elevation: Unauthorized elevation to higher-level users.
  
  Live VM Migration: Attacker captures unencrypted data between servers.
  
  Resource Reuse: Improper clearing of resources may expose sensitive data.
  
 Containerization Technologies
  Docker, kubernetes, Red Hat, OpenShift are popular containerization plateforms. These are the application that revolutized the deployment in cloud environment.
  
 Securing Virtual Machines
  - Regularly update OS, applications, and apply security patches
  - Install antivirus solutions and software firewalls
  - Use strong passwords and implement security policies
  - Secure the hypervisor with manufacturer-released patches
  - Limit VM connections to physical machines and isolate infected VMs
  - Distribute VMs among multiple servers to prevent resource exhaustion
  - Monitor VMs to prevent "Virtualization Sprawl”
  - Enable encryption of VM files for data safety and confidentiality
  
Serverless
 What is Serverless?
  Serverless computing doesn't mean no servers; it means it shifts server management away from developers. It Relies on cloud service providers to handle server management, databases, and some application logic. In this model developers write and deploy individual functions triggered by events. It is called a Function as a service (FaaS) Model.
  
 Benefits of Serverless
 
   Reduced operational costs: Pay only for compute time used, no charges when code is idle. 
   
   Automatic scaling: Cloud provider scales resources based on workload, ensuring optimal capacity.
   
   Focus on core product: Developers can concentrate on application functionality, not server management.
   
   Faster time to market: Reduced infrastructure concerns speed up application development.
   
   
 Challenges and Risk
 
  Vendor Lock-in: Reliance on proprietary interfaces limits flexibility and may increase costs.
  
  Immaturity of best Practices: Serverless is a relatively new field, and best practices are still evolving.
  
 
 Not a one-size-fits-all solution
  
  Consider the specific needs and requirements of your application; serverless introduces challenges like Vendor Lock-in and service provider dependencies.
  



--------------------------------------------------------------------------
### Microservices

Microservices
This architectural style for breaking down large application into small, independent services. Each of the microservice runs a unique process and communicates through a well defined, lightweight mechanism. In contrast with traditional monolithic architecture where all components are inter connected, here each service in the microservice architecture is self-contained and able to run independently.

Advantages of microservices

 - Scalibility: In this architecture the services can be scaled independently based on demand.
  
 - Flexibility: Microservices can use different technologies and be managed by different teams.

 - Resilience: Isolation reduces the risk of system-wide failures which in return increases resilience.
 
 - Faster Deployment and updates: Independent deployment and updates allow for agility and reduced deployment risk.
  
Challenges of Microservices

 Complexity: Managing multiple services involves inter-service communication, data consistency, and distributed system testing.

 Data Management: Each microservice can have its own database, leading to data consistency challenges. 
 
 Network Latency: Increased inter-service communication can result in network latency and slower response times.
 
 Security: The distributed nature of microservices increases the attack surface, requiring robust security measures.
 
### Network Infrastructure

Network Infrastructure
 
 It is the backbone of modern organizations. It comprises of hardware, software, ervices, and facilities for network support and management. 

Physical separation
 
 This is often refferred to as "Air Gapping". It isolates a system by physically disconnecting it for all networks. Physical seperation is one of the most secure method of security, but it is still vulnerable to sophisticated attacks. 
 
Logical Separation
 This establishes boundaies within a network to restrict acces to a certain areas. It is implemented by using Firewalls, VLANs, and network devices.
 
Comparison
 Physical Seperation (Air Gappping): It is highly secure as it provides complete isolation.
 
 Logical Sepration: It is more flexible and eaiser to implement. It is less secure if not configured properly.
 
 
### Software-defined Network (SDN)

Software-defined Network
 Software-Defined Networking (SDN) is a transformative approach to network management that decouples the network control plane from the data forwarding plane. This separation allows for more dynamic and programmable network configurations, making networks more flexible, efficient, and easier to manage. This management is done with a centrallized server that decides how data moves through the network.
 
 
SDN Architecture
 Three Distinct Planes are:
  - Data Plane (Forwarding Plane): This plane is responsible for handling data packets. This also makes decisions based on protocols like IP and Ethernet. It is mainly concerned with sending and receiving data.
 
  - Control Plane: This a centralized decision-maker in SDN. It dictates traffic flow across the entire network and it replaces traditional, distributed router control planes. This result in increases in network manageability and flexibility.
  
  - Application Plane: This plane Hosts all network applications that interact with the SDN controller. The applications instruct the controller on network management. The controller manipulates the network based on these instructions.

### Infrastructure as Code (IaC)

Infracture as Coad (IaC)
 It ia a mordern approcah to It Infrastructure management. It automates the provisioning and management through code. This is primarly used in DevOps and with cloud computing.
 
IaC Method
 In this the developers and ops teams manages infrastructure through code. These codes files are versioned, tested and audited. High level languages like YAML, JASON or domain specific languages are used e.g. HCL.  Idempotence methods are used to ensure the identical environments. (Idempotence refers to a function or a operation that can be repeated without changing the outcome.)
 
Benefits of IaC

 - Speed and efficiency
 - Consistency and standardization
 - scalability
 - cost Savings
 - Auditability and compliance
 
Challenges in IaC:
 - Learning Curve: It means to learn new skill and mindset that is requires. In this infrastructure the teams learn to write, test and maintain infrastructure code.
 
 - Complexity: Infrastructure code can become complex due to many management components. It mitigates with modularization and documentation
 
 - Security Risk: In this there is always a chance of sensitive data exposure in code files which can be caused due to insecure configuration.
 
### Centralizes vs Decentralizes Architectures

Centralized architecture
 In this all the computing functions are managed from a single location or authority. I this architecture the data and applications is stored in one location and is accessed via a network.

It's components includes:
  - central server
  - Mainframe
  - Data Center
  
It's benifits includes
 
  - Efficiency and control: centralization provides high resource control and efficient resource allocation as it have status of whole infrasturcture.
  
  - Consistency: This ensures uniform and accurate data across the organization
  
  - Cost-effective: It reduces maintenance and infrastructure costs 
 
It Risk are:
 - Single point failure: Server failure can disrupt the entire network
 
 - Scalability Issues: The centralized architecture struggles to handle growth, leading to performance problems.
 
 - Security Risk: These are attractive targets for cybercriminals, as compromising a central server risks whole data and app security.
 
 
Decentralized Architecture

In this architecture the computing functions distributed across multiple systems or locations. There is No single point of control, each node operates independently. 

It's benifits are:
 - Resilience: It can continue functioning despite individual node failures.
 
 - Scalability: It can easily scales with organization growth by adding new nodes.
 
 - Flexibility: It supports remote work and distributed teams.
 
It's Risk Includes:

 - Security Risk: It is vulnerable to security threats and especially in remote work scenarios.
 
 - Management Challenges: Due to it's decentralize location the management becomes complex as it need coordinating multiple nodes.
 
 - Data Inconsistency: There is always a Potential of issues with data consistency and synchronization.
 
Consideration for Choosing Architecture

 Choice depends on the organization's specific needs and context as:
   
   - Centralized systems is best for data accuracy and resource management priorities.
 
   - Decentralized systems is best for Resilience, flexibility, and rapid scaling needs.
 
 
### Internet Of Things (IoT)

Internet Of Things (IoT)

 It is a network of physical devices with sensors, software, and connectivity. It enables data exchange among connected objects.
 
Hub/Control System
 It is central component connecting IoT devices. It collects, processes, analyzes data, and sends commands. It can either be a physical device or software platform.
 
Smart Devices
 It is a type of device that detect changes in environment, convert into data. It measure various parameters like temperature, motion etc. It enable interaction and autonomous decisions in smart devices.
 
IoT Risk
 
 Weak Default setting: It is a common security risk. Default usernames/passwords are easy targets for hackers. The users must change defaults upon installation is essential.
 
 Pooerly Configured Network Services: Devices may have vulnerabilities due to open ports, unencrypted communications. The unnecessary services can increase attack surface. Keeping IoT devices on a separate network is recommended.
 
### ICS and SCADA

Industrial Control Systems (ICS)

 These are the systems used to monitor and control industrial processes, found in various industries like electrical water, oil, gas and data. 

 Distributed Control System (DCS): It is used in control production systems within a single location.

 Progammable logic Controllers (PLCs): It is used to control specific processes such as assembly lines and factories.

Supervisory Control and Data Acquisition (SCADA) systems

 These are the type of ICS designed for monitoring and controlling geographically dispersed
industrial processes. 
 Common in industries like:
  - Electric power generation, transmission, and distribution systems.
  - Water treatment and distribution systems.
  - Oil and gas pipeline monitoring and control systems.
  
Risk and Vulnerabilities
  
 - Unauthorized Access: Unauthorized individuals can manipulate system operations without
proper protection.

 - Malware Attacks: Vulnerable to disruptive malware attacks.
  
 - Lack of Updates: Running outdated software with unpatched vulnerabilities.
  
 - Physical Threats: Susceptible to damage to hardware or infrastructure.
  
Securing ICS and SCADA Systems
 - Implementing Strong Access Controls: It refers to setting strong passwords, two-factor authentication. It also means to have limited access to authorized personnel only.
 
 - Regularly Update and Patch Systems: Keep systems updated to protect against known vulnerabilities.
 
 - Use Firewall and Intrusion Detection Systems: Detect and prevent unauthorized access.
 
 - Conduct Regular Security Audits: Identify and address potential vulnerabilities through routine assessments.
 
 - Employee Training: Train employees on security awareness and response to potential threats.
 
 
### Embedded Systems

Embedded Systems

 These are the specialized computing components designed for dedicated functions within larger devices. They integrate hardware and mechanical elements and are essential for various
daily-use devices.

Real-Time Operating System (RTOS)
 
 These are designed for real-time applications that process data without significant delays. Critical for time-sensitive applications like flight navigation and medical equipment. 
 

Risks and Vulnerabilities in Embedded Systems
 
 - Hardware Failure: Prone to failure in harsh environments.
 
 - Software Bugs: Can cause system malfunctions and safety risks.
 
 - Security Vulnerabilities: Vulnerable to cyber-attacks and unauthorized access.
 
 - Outdated System: Aging software and hardware can be more susceptible to attacks.
 

Key Security Strategies for Embedded System

 - Network Segmentation: Divide the network into segments to limit potential damage in case of a breach.
 
 - Wrappers (e.g., IPSec): Protect data during transfer by hiding data interception points.
 
 - Firmware Code Control: Manage low-level software to maintain system integrity.
 
 - Challenges in Patching: Updates face operational constraints; OTA updates demand meticulous
planning and security measures. It also includes Over-the-Air (OTA) Updates which means Patches are delivered and installed remotely.

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
   - Sensitive data iss protected.
   - Regulatory requirement are met.
   - System can communicate with each other.
   - The solution is cost-effectiveness.

On-Premise solutions
 These includes Computing infrastructure physically located on-site at abusiness.
 
Key Considerations in cloud Computing

 - Availability: System's ability to be accessed when needed
 
 - Resilience: System's ability to recover from failures.
 
 - Cost: Consider both upfront and long-term costs.
 - Responsiveness: Speed at which the system can adapt to demand.
 
 - Scalability: System's ability to handle increased workloads.
 
 - Ease of Deployment: Cloud services are easier to set up than on-premise solutions.
 
 - Risk Transference: Some risks are transferred to the provider, but mostlty customers are responsible for security.
 
 - Ease of recovery: Cloud services offer easy data recovery and backup solutions.
 
 - Patch Avalibility: Providers release patches for vulnerabilities automatically.
 
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
  
  
### Microservices

Microservices
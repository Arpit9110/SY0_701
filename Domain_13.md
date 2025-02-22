# Cyber Resilience and Redundancy

### High Availability

High Availability

This aims to keeps services continuously available by minimizing downtime. It is achieved through load balancing, clustering, redundancy, and multi-cloud strategies.

Uptime and availability Standards

Uptime: This the time a system is online typically expressed as a percentage.

Five Nines: This refers to 99.999% uptime, allowing about 5 minutes of downtime per year.

Six Nines: This refers to 99.9999% of uptime, it allows only 31 seconds of downtime per year.

Load Balancing

This is the distribution of workload across multiple resource. It helps in optimization of resource use, throughput, and response time. It prevents overloading of any single resource. It always directs the incoming request to the most capable server available.

Clustering

This process uses multiple computers, storage devices, and network connections as a single system. It provides a high availability, reliability, and stability. It ensures continuity of service even in case of hardware failure. It can be combines with load balancing methods for robust solutions.

Redundancy

It involves duplicating critical component to increase system reliability. It also helps in preventing single point failure in the system. The redundancy can be applied to any system by adding multiple of this system:

- Power

- Network connections

- Servers

- Software Services

- service provider

Multi-Cloud Approach

This approach distributes data, applications, and services across multiple cloud providers. It mitigates the risk of a single point of failure. It offers flexibility for cost optimization and aids in avoiding vendor lock-in. It requires proper data management, unified threat management, and consistent policy enforcement for security and compliance.

Strategic Planning

it is about designing a robust system architecture to achieve high availability. It utilizes load balancing, clustering, redundancy, and multi-cloud approaches. It is a proactive method that reduce the risk of service disruption and downtime cost. It safeguards the organizational continuity and reliability in a competitive environment.

### Data Redundancy

RAID overview

Raid (Redundancy Array of interdependent Disk) is a method which combines multiple physical storage devices unto a single logical storage device recognized by the operating system to provide data redundancy. RAIDs are essential for ensuring data redundancy, availability, and performance in enterprise networks. The choice of RAID type depends on specific requirements for performance and fault tolerance.

RAID 0

 In this method data is striped across multiple disks. It is used for improved performance but offer no data redundancy. By using multiple drives one can increase read and write speeds. It is suitable for scenarios where performances are essential, and data redundancy is not a concern.

RAID 1

 It provides redundancy by mirroring data identically on two storage devices. It ensures data integrity and availability. It is suitable for critical applications and maintains a complete copy of data on both devices. Only one storage device can fail without data loss or downtime.

RAID 5

 It utilizes striping with parity across at least three storage devices. It offers fault tolerance by distributing data and parity. It can continue operations if one storage device fails. Data reconstruction is possible but result in slower access speeds.

RAID 6

 It is similar to RAID 5 but includes double parity data. It requires at least four storage devices. It can withstand the failure of two storage devices without data loss.

RAID 10

 It combines RAID 1(Mirroring) and RAID 0 (Striping). It offers high performance, fault tolerance and data redundancy. It also requires an even number of storage devices, within a minimum of four.

RAID Resilience Categories

 Failure-resistant: Resists hardware malfunctions through redundancy (e.g., RAID 1)

 Fault-tolerance: It allows continued operation and quick data rebuild in case of failure e.g. RAID 1, RAID 5, RAID 6, RAID 10.

 Disaster-tolerance: Safeguards against catastrophic event by maintaining data in independent zones e.g. RAID 1, RAID 10.

### Capacity Planning

Capacity Planning

 In includes critical strategic planning effort for organizations. It ensures an organization is prepared to meet future demands in a cost-effective manner.

For Main Aspect of Capacity Planning

 People: In this the current personnel skills and capacity are Analysed and the future personnel needs for hiring, training, or downsizing is forecasted. By this the organizations ensure the right number of people with the right skills for strategic objectives. For example, Hiring seasonal employees for holiday retail demand.

 Technology: It is done by assessing the current technology resources and their usage. By predict future technology demands, by considering these forecast scalability and potential investments are done in new technology. For example: Ensuring an e-commerce platform can handle traffic spikes.

 Infrastructure: In this planning for physical spaces and utilities to support operations. It also includes office spaces, data centres, and more. It is done to optimize space and power consumption. For example: Data centre capacity planning for server installations.

 Processes: In this planning the business process is optimized for varying demand levels. It is done to streamline the workflows, improve efficiently and consider outsourcing. For Example: Automating employee onboarding to handle high demand.

### Powering Data Centre

Key terms

 Surges: Sudden, small increases in voltage beyond the standard level (e.g., 120V

in the US).

 Spikes: Short-lived voltage increases, often caused by short circuits, tripped

breakers, or lightning.

 Sags: Brief decreases in voltage, usually not severe enough to cause system

shutdown.

 Undervoltage Events (Brownouts): Prolonged reduction in voltage, leading to system shutdown.

 Power Loss Events (Blackouts): Complete loss of power for a period, potentially causing data loss and damage.

Power Protection Components

 Line Conditioners: It stabilizes voltage supply and filter out fluctuations. This mitigates surges, sags, and undervoltage events. It also prevents unexpected system behaviour and hardware degradation. It Not suitable for scenario in which there is a significant undervoltage events or complete power failures.

 Uninterruptible Power Supplies (UPS): It provide emergency power during power source failures. It offers line conditioning functions. It includes battery backup to maintain power during short-duration failures. This typically supply 15 to 60 minutes of power during a complete power failure.

 Generators: This method Convert mechanical energy into electrical energy for use in an external circuit through the process of electromagnetic induction. These backup generators supply power during power grid outages.

 Different Types of Generators are:

 - Portable gas-engine generators

 - Permanently installed generators

 - Battery-inverter generators

 Power Distribution Centre (PDC): It is the Central hub for power reception and distribution. It includes circuit protection, monitoring, and load balancing. It integrates with UPS and backup generators for seamless transitions during power events.

 Considerations for Data Centres

  - Large data centres use rack-mounted UPS for server protection

  - UPS provides line conditioning and battery backup for 10-15 minutes

  - Power distribution units manage load balancing and line conditioning

  - Backup generators are crucial for extended power outages but require startup

time.

  - Building data centres with redundancy and protections tailored to use cases and

budgets.

### Data Backup

Data Backup: This is the method of creating duplicate copies of digital information to protect against data loss, corruption, or unavailability. It safeguards data from accidental deletion or system failures.

Onsite and Offsite Backup

  Onsite Backup: Sorting data in the same physical location as the original data.

  Offsite Backup: Storing data copies in a geographically separate location.

  Importance: Onsite backups are convenient but vulnerable to disasters, whereas offsite backups protect against physical disasters.

Backup Frequency

  Determining factor of backup frequency is the organization’s RPO. RPO ensures that the backup plan will maintain the amount of data required to keep any data loss under the organization’s RPO threshold.

  Considerations for backup frequency:

   - Data change rate

   - Resource allocation

   - Organizational needs

Encryption

  It is fundamental safeguard that protects the backup data from unauthorized access and potential breach, by jumbling out the or removing the and replacing them with the help of a key.

   - Data-at-rest Encryption: Encrypting data as it is written to storage

   - Data-in-transit Encryption: Protecting data during transmission

   - Importance: Safeguarding backup data from unauthorized access and breaches

Snapshots: It is a Point-in-time copies capturing a consistent state. It Records only changes since the previous snapshot, reducing storage requirements. Use case: Valuable for systems where data consistency is critical, like databases and file servers.

Data Recovery

  Several key steps in the data recovery process:

   - Selection of the right backup

   - Initiating the recovery process

   - Data validation

   - Testing and validation

   - Documentation and reporting

   - Notification

  Importance of data recovery is about regaining access to data in case of loss or system failure; a well-defined and tested recovery plan is essential.

Replication

It the real-time or near-real-time data copying to maintain data continuity.

Benefits of replication are:

  - Ensures seamless data continuity

  - Suitable for high-availability environments

Journaling

It is about maintaining a detailed record of data changes over time.

Its benefits include:

   - Enables granular data recovery

   - Maintains an audit trail

   - Ensures data integrity and compliance

Consideration to undertake is the: Data tracking granularity, size, retention policies, and security.

### Continuity of Operations Plan

continuity of Operations Plan (COOP)

 This plan ensures that an organization's ability to recovery form disruptive events or a disaster. It requires detailed planning and forethought.

 Key terms

  Business Continuity planning (BC Plan)

   This plan and process is created for responding to disruptive events. It addresses a wide range of threat and disruptive incidents. It also involves preventative actions and recovery steps. It covers both technical and non-technical disruption.

  Disaster Recovery Plan (DRP)

   This plan and process focuses on disaster response. It is a subset of BC plan which focuses on faster recovery after disaster. It addresses the specific like hurricanes, fires, or floods.

 Strategies for Business Continuity

  - Always consider alternative location for critical infrastructure.

  - Distribute staff across multiple geographic regions.

  - use cloud services to maintain operation during disaster.

 Role of senior Management

  - Senior Managers are responsible for developing the BC plan.

  - They define the goals for BC and DR efforts.

  - They a business continuity coordination to lead the business continuity committee.

 Business Continuity Committee

  This committee comprises of representatives from various departments (IT, Legal, security). This committee determines recovery priority for different events. They also identifies and prioritizes systems, critical for business continuity.

 Defining Scope

  The senior management decides the plan's scope based on risk appetite and tolerance. The scope can be broken by business function or by geographical areas. All components must be coherent and compatible for crisis situations.

### Redundant Site Considerations

Redundant Site

These are the backup location or facility that can take over essential functions and operations in case the primary site experiences a failure or disruption.

Type of Continuity Locations

  - Hot Sites: These are the up and running site working continuously. This enables a quick switchover, but it requires duplicating all Infrastructure and data. It is very expensive to create and maintain but provides instant availability.

  - Warm Sites: These are not the fully equipped and setup sites but is fundamentally in place. It needs a few days to setup but it is cheaper to operate and maintain. It is slight slower than Hot Sites.

  - Cold Sites: These are the sites that have more fewer facilities than the warn site, might be just a empty building. It need 1-2 months to setup. It is cost-effective but adds more recovery time.

  - Mobile Sites: This can be hot, warm or cold. It utilizes portable units like trailers or tents. It offers flexibility and quick deployment. Ex military DjC2

 Platform Diversity

 It is critical for effective virtual redundant sites. It helps in diversify operating systems, network equipment, and cloud platforms. It reduces the risk of a single point of failure. It ensures resilience and adaptability in case of disruptions.

 Virtual Sites

 These are the sites that leverage the cloud-based environment for redundancy. This offers scalability, cost-effectiveness, and easy maintenance.

 This is also of different type:

   - Virtual Hot Site: Fully replicated and instantly accessible in the cloud

   - Virtual Warm Site: Involves scaling up resources when needed

   - Virtual cold Site: Minimizes ongoing costs by activating resources only during disasters

Geographic Dispersion

It involves spreading resources across different locations for higher redundancy. It mitigates the risk of localized outages and enhances disaster recovery capability.

Consideration for redundant Site selection

 - Think about technology stack, people's workspace, and long-term support

 - Determine which type of redundant site suits your organization's needs

- Ensure continuity of essential functions and services in the event of disruptions

### Resilience and Recovery Testing

Resilience Testing

This assess system's ability to withstand and adapt to disruptive events. It ensures the system can recover from unforeseen incidents. These testing is conducted through tabletop exercise, failover tests, simulations and parallel processing. It helps in preparing for events like power loss, natural disasters, ransomware attacks, and data breaches.

Recovery Testing

This testing evaluates the system's capacity to restore normal operation after a disruptive event. It involves executing planned recovery actions. It is performed through failover tests, simulations, and parallel processing. It ensures that planned recovery procedures work effectively in real-world scenarios=.

Tabletop Exercises

In this scenario-based discussion done among key stakeholders. They identify the gaps and seams in response plan. They promote team-building among stakeholders. In this test there is no deployment of actual resources.

Failover Tests

 It is a controlled experiment for transitioning from primary to backup components. It ensures uninterrupted functionality during disasters. It requires more resources and time. This validates the effectiveness of disaster recovery plans. It can also identify and rectify issues in the failover process.

Simulations

 It is a computer-generated representation of a real-world scenario. It allows for a hands-on response actions in a virtual environment. It helps in assessing incident responders and system administrators in real-time. This helps in evaluating reactions and staff performance, it also gives key insight in the feedback for learning and improvement.

Parallel Processing

This helps in replicating data and system processes onto a secondary system. It helps in running primary and secondary system concurrently. It tests reliability and stability of the secondary setup. It ensures no disruption to day-to-day operations. It helps in assessing the system's ability to handle multiple failure scenarios simultaneously.

 The use of parallel processing helps in

  - Resilience Testing: This Test the ability of the system to handle multiple failure scenarios 

  - Recovery Testing: This test the efficiency of the system to recover from multiple point of failure.
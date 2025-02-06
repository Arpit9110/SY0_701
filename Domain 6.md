### Data Protection

#### Data Classification 

  Data Classification : it is based on the value of the organization and the sensitivity of the information, determined by the data owner.
  
  Sensitive Data : Information that if accessed by unauthorised persons, can result in the loss of security or competitive advantage for a company. Over classifying the data leads to protecting all data at a high level.
  
Importance of Data classification : 
- It helps to allocate appropriate protection resources.
- Prevents over-classification to avoid excessive costs.
- Requires proper policies to identify and classify data accurately.
  
Commercial business Classification levels
 - Public : No impact if released, It often publicly accessible data 
 - Sensitive : Minimal impact if released, e.g. financial data.
 - Private : Contain internal personal or salary information.
 - Confidential : These are the trade secrets, intellectual property, source code, etc.
 - Critical : Extremely valuable and restricted information.
 
Government Classification Levels
 - Unclassified : Generally releasable to the public.
 - Sensitive but unclassified : It includes medical records, personal files, etc.
 - Confidential : It contains could affect the government.
 - Secret : Holds data like military deployment plans, defective postures.
 - Top Secret : It is of the  highest level of secrecy. It includes things like highly sensitive national security information, military installations and nuclear weapons coordinates etc.


Legal Requirements: Depending on the type of organizatio they are legaly obliged to mantain specific data for a fixed period of time.


Documentation : Organizational policies should clearly outline data classification, retention, and disposal requirement.


<font color="#ffff00">Note: Understanding data classification and their proper handling is vital for protecting sensitive information and complying with relevant regulation.</font>


  
#### Data Ownership 
 
 Data Ownership :  Process of identifying the individual responsible for maintaining confidentiality, integrity, availability, and privacy of information assets.
 
 Data Owner : A senior executive for labeling information assets and ensuring they are protected with appropiate controls.
 
 Data Controller : Entity responsible for determining data storage, collection, and usage purpose and method, as well as ensuring the leaglity of thses process.
 
 Data Processor : A group or individual hired by the datacontroller to assist with task like data collection and processing. 
 
 Data Steward : Focuses on data quality and metadata, ensuring data is appropiately labeled and classified, often working under the data owner.
 
 Data Custodian : Responsible for managing the system on which data assets are stored, including enforcing access control, encryption and backup measure.
 
 Privacy Officer : They Oversees privacy related data, such as personally identifiable information (PII), sensitive personal information (SPI), or protected health information (PHI), and ensuring compliance with legal and regulatory frameworks.
 
 Data Ownership Responsibility : The It department (CIO ot IT personel) should not be the data owner, data owner shpuld be an individual from the business side who understand the data's content and can make informed decisions about classification.
 
 Slection of Data Owners :  Data owner should be designated within their department based on their knowledge of tha data and it's significance within the organization.
 
 NOTE: Proper data ownership is essential for maintaining data security, compliance, and effective data management within an organization. Different roles contribute to safeguarding and managing data appropriately.
 
 
 #### Data States
 
 Data at Rest : This the data that is stored in the database, file system, or a storage system, not actively moving or being used.
 
 Encryption Methods : 
  Full Disk Encryption (FDE) : Encrypts the entire Hard drive.
  Partation Encryption: Encrypts specific partations, leaving others unencrypted.
  File Encryption: Encrypts individual files.
  Volume Encryption: Encrypts data stored in a database at column, row, or table levels.
  Record Encryption: Encrypt specific fields within a database record.
  
 Data in Transit(Data in motion): Data in transit is basically the data actively moving from one location to another, vulnerable to interception.
  Transport Encryption Methods are:
  
- SSL (secure Sockets Layer) and TLS (Transport layer security): Secure communication over network, widely used in web browsing and email.

- VPN (Virtual Private network): Creates secure connection over less secure network like the Internet.

- IPSEC (Internet protocol security): Secures IP communications by authenticating and encrypting IP packets.

 Data in Use: In this the data is actively being used and undergoes many process like data being created, retrieved, updated, or deleted.
 Protection measure:  
 - Encryption at the application Level: Encrypt data during processing.
 - Access control: Restrict access to data during processing.
 - Secure Enclaves: Isolate environment for processing sensitive data.
 - Mechanism like INTEL Software guard: Encrypt data in memory to prevent unauthorised access
   
<font color="#ffff00">Note: Understanding the three data state (Data at rest, Data in transit, Data in Use) and implementing appropriate security measure for each is essential for comprehensive data protection.</font>






#### Data Types: 

Regulated Data: This is the data controlled by laws, regulatio, or company standards. 
Compliance requirements for this type of data can be : 
GDPR General Data Protection Regulation.
HIPPA Health insuarance portability and accountability Act.

PII (Personal Identification Information) : Information used to identify an individual (eg : name, Social security number, Address, etc). Thses types of information is often targeted by cybercriminal and are protected by Privacy law.

PHI (persona Health Information) : Information ablut health status, healthcare provision, or payment linked to a specific individual. Thses types of data is protected by HIPPA.

Trade Secrets : Confidential business information giving a comnpetitive edge(e.g manufacturing process, making strategies, porpriety software.) These data are legally protected and unauthorised disclosure of these data result in penalties.

Intellectual Property (IP): These data includes things like inventions, literary works, designs , research papers etc. These type of data are protected by patent, copyrights, trademarks to encourage innovation without frear of it getting stolen with repercrutions. Unauthorised use can lead to legal action.

Legal Information: These are the data related to legal procedding, contracts, regulatory compliance, etc. These require high level of protection for client confidentiality and legal privilege.

Finanacial Information: Data related to financial transaction e.g. salse record, tax document, bank satatements. These re targeted by crybercriminals form fraud and identity theft.Thses data are subjected to PCI DSS (Payment card industry Data Security Standards).

Human  Redable Data: Understand directly by humans eg text document , steadsheet, word file etc.

Non Human redabe Data : These data requires machine or software to be decoded or interpreted. thses data are generally in binary code, machine language. These contains sensitive information and requires protection.


#### Data Sovereignty 

 Data Sovereignty : Digital information subjected to laws of the country where it's located. It recently gained huge importance due highly global data storage and cloud computing solutions.
 
 GDPR (General data protection Regulation) : Protects the EU's citizens data with EUand EEA boarders. This compliance is required regardless of data location. Non-compliance leads to significant fines.
 
 
 Data Sovereignty Laws(e.g. China Russia): Require data storage and processing within nation borders. It is a huge challange for multinational companies and cloud services. 
   
 Access Restrictions: cloud services msy restrict access for multiple geogrphic loaction due to data protection laws and data sovereignty of that particular geographical location.
 
 Data sovereignty and geographical considerations pose complex challenges, but
organizations can navigate them successfully with planning, legal guidance, and strategic
technology use, ensuring compliance and data protection



#### Securing Data 

Geofencing Restrictions: 

Encryption:

Hashing:

Masking:

Tokenization:

Obfuscation:

Segmentation:

Permission Restriction
 
 Data Loss Prevention (DLP)
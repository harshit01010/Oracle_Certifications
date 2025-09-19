# Skill Checks
##  OCI Introduction

1. Which statement about OCl is NOT true?
- [ ] An OCI region is a localized geographic area.
- [ ] An availability domain is one or more data centers located within a region.
- [ ] Availability domains do not share infrastructure, such as power, cooling, or network, within a region.
- [x] A single fault domain can be associated with multiple availability domains within a region.

> A fault domain is a subdivision of an availability domain. Each availability domain contains three fault domains. Fault domains let you distribute your instances so that they are not on the same physical hardware within a single availability domain. A fault domain cannot be associated with multiple availability domains.


2. Which statement about regions and availability domains is true?
- [ ] All OCI regions have a single availability domain.
- [x] An OCI region has one or more availability domains.
- [ ] All OCI regions have three availability domains.
- [ ] Fault domains provide protection against failures across regions.

> An OCI region is composed of one or more isolated, interconnected availability domains. Each availability domain is a separate physical location within a region. The number of availability domains per region may vary; some OCI regions have three availability domains, while some others have a single availability domain.


3. You have subscribed to an OCl region that has one availability domain. You want to deploy a highly available application with two servers and a 2-node database. How would you place the components to maintain the high availability of the application?
- [x] Place one server and a DB node in one fault domain, and the second server and DB node in another fault domain.
- [ ] High availability is not possible as there is only one availability domain in the region.
- [ ] Place all the components in the same fault domain.
- [ ] Place the servers in one fault domain and the database nodes in another fault domain.

> In this scenario, distributing the servers and database nodes across different fault domains within the same availability domain would provide protection against the failure of a single fault domain. If one fault domain experiences a failure, the other would remain unaffected, ensuring the high availability of the application.

4. Which Oracle Cloud Infrastructure service is NOT intended for a multicloud solution?
- [ ] Oracle Interconnect for Azure
- [x] Oracle Roving Edge Infrastructure
- [ ] Oracle Database Service for Azure
- [ ] Oracle MySQL Heatwave on AWS

> Oracle Roving Edge Infrastructure is a service that provides a portable, ruggedized device running a subset of OCI services, designed for deployment in the field outside of a traditional data center. It is not a service specifically designed for multicloud deployment. On the other hand, services like Oracle Database Service for Azure and Oracle Interconnect for Azure are designed to allow Oracle Cloud Infrastructure to interoperate with Azure, indicating a multicloud approach. Oracle MySQL HeatWave is an analytics service for MySQL Database service that runs on AWS but the account management and billing and metering are done through OCI.


5. Which capability can be used to protect against failures within an OCI availability domain?
- [ ] Load Balancer
- [ ] Compartments
- [x] Fault Domain
- [ ] Regions

> Fault domains provide a capability to protect your applications and instances from unexpected hardware failures or network outages within an availability domain. They provide anti-affinity: Each fault domain runs on its own set of physical hardware, so a failure that impacts one fault domain does not affect instances in other fault domains.


<br />
<br />


## Identity and Access Management (IAM)

1. How is a resource in OCl identified?
- [x] With OCID
- [ ] With Tenancy ID
- [ ] With Compartment Name
- [ ] With Username

> Each resource in OCI is assigned a unique Oracle Cloud Identifier (OCID), which is used to identify the resource.


2. Which statement about OCI compartments is NOT true?
- [ ] A compartment is a logical collection of related resources.
- [x] It is a best practice to create all your resources in the root compartment.
- [ ] Compartments can be nested.
- [ ] Compartments help to isolate and control access to resources.

> It is not a best practice to create all resources in the root compartment. Compartments are used to organize and isolate resources to provide a finer level of access control.


3. Which Identity and Access Management component helps to organize multiple users into a team?
- [ ] Compartments
- [x] Groups
- [ ] Dynamic Groups
- [ ] Policies

> In OCI IAM, groups are used to group users that serve a common purpose or belong to the same team. This allows policies to be applied at the group level, rather than individually.


4. Which is NOT a component of OCI Identity and Access Management?
- [ ] Federation
- [ ] Policies
- [x] Network Security Group
- [ ] Principals

> The Network Security Group is a component of OCI Networking, not IAM. IAM in OCI consists of Principals, Policies, Federation, and a few other components.


5. Which statement about OCI Identity and Access Management is true?
- [ ] It is used to protect information on devices.
- [ ] It enables authentication for devices only
- [ ] It enables authorization for on-premises users only
- [x] It enables you to control access for a group of users.    

> OCI Identity and Access Management (IAM) service allows you to control who has access to your cloud resources. It can be used to group users and specify their permissions to provide controlled access to resources.

<br />
<br />


## Networking


1. Which component is NOT created by default with the creation of a Virtual Cloud Network?
- [ ] Default Route Table
- [ ] Default Security List
- [x] Default Local Peering Gateway
- [ ] Default DHCP Options

> When you create a VCN, a default route table, security list, and DHCP options are created automatically, but a Local Peering Gateway (LPG) is not created by default. LPGs are used to connect two VCNs in the same region.   

2. Which statement about Virtual Cloud Network (VCN) peering between two VCNs is NOT valid?
- [ ] Peered VCNs cannot have overlapping CIDRs.
- [ ] Peered VCNs can exist in the same OCI region.
- [x] A VCN peering connection is a VPN-based connection.
- [ ] Peered VCNs can exist in different OCI regions.

> VCN peering is not a VPN-based connection; instead, it is a networking connection between two VCNs that enables traffic routing between the VCNs using private IP addresses. Peer VCNs must not have overlapping CIDRs. VCNs can be peered in the same region or different regions through a DRG.

3. Which OSI layer traffic is supported by the OCI Network Load Balancer?
- [ ] Layer 5 (session)
- [ ] Layer 7 (application)
- [x] Layer 4 (transport)
- [ ] Layer 2 (data link)

> OCI Network Load Balancer operates at layer 4 (transport layer) of the OSI model. It distributes traffic among instances within its backend set based on TCP or UDP protocols.

4. Which statement about a Virtual Cloud Network (VCN) is true?
- [ ] A VCN can be used with only one instance.
- [x] A VCN can reside only in a single region but can span multiple availability domains.
- [ ] A VCN can have only one public subnet and more than one private subnet.
- [ ] A VCN can span OCI regions.

> A VCN is a virtual, private network that you set up in Oracle data centers in a single OCI region. It resembles a traditional network, with firewall rules and specific types of communication gateways that you can choose to use. A VCN spans all the availability domains in the region.


5. Which VCN component blocks inbound traffic, but enables outbound traffic to the internet?
- [ ] Dynamic Routing Gateway
- [x] NAT Gateway
- [ ] Service Gateway
- [ ] Internet Gateway

> A NAT Gateway in a VCN enables instances in a private subnet to initiate connections to the internet but prevents unsolicited inbound connections from the internet.

<br />
<br />


## Compute


1. Which two parameters can be customized when creating a flexible shape compute instance?
- [x] Amount of memory
- [ ] Number of virtual NICs
- [x] Number of OCPUs
- [ ] Number of physical NICs

> When creating a flexible shape compute instance in OCI, users can customize the number of Oracle Cloud Processor Units (OCPUs) and the amount of memory allocated to the instance. The number of virtual NICs and physical NICs are not customizable parameters for flexible shape compute instances.


2. What is the primary purpose of Oracle Cloud Infrastructure Functions?
- [ ] To store and manage files
- [ ] To provide a managed database service
- [x] To execute code in response to events or HTTP requests
- [ ] To deploy and manage virtual machines

> The primary purpose of OCI Functions is to execute code in response to events or HTTP requests. Functions provide a serverless computing platform that allows developers to build, deploy, and run applications without the need to manage the underlying infrastructure.


3. Which type of storage is associated with instances in the OCI Compute service?
- [ ] File Storage
- [x] Block Storage
- [ ] Archive Storage
- [ ] Object Storage

> Block storage is the type of storage associated with instances in the OCI Compute service. It provides low-latency, high-performance storage volumes that can be attached to instances to store data and applications.


4. Which statement about the working of autoscaling in an instance pool is true?
- [x] It automatically provisions and removes instances in an instance pool.
- [ ] It can perform only metric-based autoscaling.
- [ ] It can perform only schedule-based autoscaling.
- [ ] It automatically changes the shape of the compute instance to increase the number of OCPU count and memory.

> Autoscaling in an instance pool within the OCI Compute service automatically provisions and removes instances based on specific conditions or schedules. It does not change the shape of the compute instance, nor is it limited to only metric-based or schedule-based autoscaling. Instead, autoscaling can be driven by both metric-based and schedule-based policies, offering a more dynamic and flexible scaling solution.


5. Which processor type is NOT available for the OCI Compute service?
- [ ] Intel
- [ ] Ampere
- [ ] AMD
- [x] Snapdragon

> The OCI Compute service offers instances powered by various processor types, including AMD, Intel, and Ampere. However, Snapdragon, which is a processor type commonly used in mobile devices, is not available for OCI Compute.

<br />
<br />



## Storage

1. You have created an Object Storage bucket of Archive tier. Which statement is NOT valid for the Archive Storage tier?
- [ ] The minimum duration to store objects is 90 days.
- [ ] The default time available to download an object after restoration is 24 hours.
- [x] The Archive storage bucket can be upgraded to Standard storage.
- [ ] From the time a restore request is made, it takes at most an hour to read the data.

> An existing standard Object Storage bucket cannot be downgraded to the Archive Storage tier and an Archive Storage bucket cannot be upgraded to the standard Object Storage tier. Other statements are correct. The minimum duration to store objects in the Archive tier is 90 days. Objects in the Archive Storage tier cannot be accessed directly. Instead, you need to restore the object to the Standard tier before reading it. From the time a restore request is made, it takes at most an hour to read the data. You can specify a duration time from 1 to 240 hours that the restored data is accessible for download on the Object Storage tier. If you do not explicitly set a duration time, data is available for download for 24 hours by default.


2. In the Oracle Cloud Infrastructure Object Storage Service, what is the primary purpose of a pre-authenticated request URL?
- [x] To provide temporary and secure access to a specific object
- [ ] To track and monitor object access and usage
- [ ] To enable public read access to a specific object
- [ ] To enable automatic transition of objects between storage tiers

> A pre-authenticated request URL is a feature in the OCI Object Storage service that provides temporary and secure access to a specific object. It enables users to generate a unique URL with a predefined expiration time, allowing external users to access the object without requiring authentication or authorization through OCI Identity and Access Management.


3. You have an extremely high performance database workload that requires at least 90 IOPS/GB and 90,000 IOPS per volume. Which OCI Block Volume performance level can be used to meet this requirement?
- [x] Ultra High Performance
- [ ] Balanced
- [ ] Higher Performance
- [ ] Lower Cost


> The Ultra High Performance tier in OCI Block Volume service can provide up to 225 IOPS/GB, to a maximum of 300,000 IOPS per volume. The Ultra High Performance level is recommended for workloads with the highest I/O requirements, requiring the best possible performance, such as large databases. Other tiers such as Balanced, Higher Performance, and Lower Cost cannot deliver this level of performance.


4. You want to store the backup of a database in cloud storage for an extended period at the lowest storage cost. Which object storage tier would you use for storing these backup files?
- [x] Archive
- [ ] Premium
- [ ] Standard
- [ ] Infrequent Access

> Archive tier is designed for storing data that is rarely accessed and requires long retention periods. It provides a low-cost storage solution for retaining data that is seldom retrieved. It is ideal for use cases such as long-term data retention and archival, including database backups.


5. What feature of the Oracle Cloud Infrastructure Block Volume service ensures data durability and protection against hardware failures?
- [x] Replication
- [ ] Encryption
- [ ] Deduplication
- [ ] Compression

> The OCI Block Volume service uses replication to ensure data durability and protection against hardware failures. Data is automatically replicated across multiple storage devices within the same availability domain, which helps maintain data integrity and availability in case of hardware issues.


<br />
<br />


## Security

1. Which of the following is NOT a component of the Oracle Cloud Infrastructure Vault service?
- [x] Database backup
- [ ] Secret
- [ ] Master encryption key
- [ ] Vault

> OCI Vault is composed of various components including master encryption keys, secrets, and vaults. A vault in OCI is a logical entity where you can centrally manage and store your encryption keys and secrets. A secret is a resource that helps manage credentials needed to access OCI resources. A master encryption key is a key that OCI uses to encrypt the encryption keys that you create in the vault (these are customer managed). Database backup is not a component of OCI Vault; it is a functionality associated with the OCI Database service.

2. In the OCl shared security responsibility model, who is responsible for securing the underlying cloud infrastructure?
- [ ] Third-party vendors
- [x] Oracle
- [ ] Government agencies
- [ ] The customer

> In the OCI shared security responsibility model, Oracle is responsible for securing the underlying cloud infrastructure. This includes securing the physical data centers, network infrastructure, and hardware that support the cloud services, ensuring a secure and reliable environment for customers to deploy their applications and store data.

3. What is the primary purpose of the Oracle Cloud Infrastructure Vault service?
- [ ] To enforce security best practices in designated compartments
- [ ] To detect, assess, and remediate security risks in your cloud infrastructure
- [ ] To provide security recommendations and insights for your cloud infrastructure
- [x] To store and manage encryption keys and secrets

> The primary purpose of the OCI Vault service is to store and manage encryption keys and secrets. The Vault service helps you to securely store, manage, and control access to encryption keys, secrets, and certificates, ensuring the protection of sensitive data.


4. What is the main advantage of using OCI Security Zones when deploying resources in your cloud environment?
- [x] Ensuring adherence to security best practices and policies
- [ ] Automatic resource scaling
- [ ] Load balancing across multiple instances
- [ ] Streamlining application deployment

> The main advantage of using OCI Security Zones when deploying resources in your cloud environment is to ensure adherence to security best practices and policies. Security Zones help maintain a strong security posture by automatically enforcing predefined security policies within designated compartments, preventing the creation of non-compliant resources.


5. Which option is NOT a component of Oracle Cloud Guard?
- [ ] Detectors
- [x] Targets
- [ ] Responders
- [ ] Problems

> Oracle Cloud Guard has three main components – detectors, problems, and responders. Detectors continuously monitor your infrastructure, looking for potential issues. Problems are the security risks and issues that detectors identify. Responders are the automatic or manual actions taken to address the identified problems. Targets are not a component of Oracle Cloud Guard.

<br />
<br />

## Governance and Administration


1. Which type of traffic is charged under data transfer costs in Oracle Cloud Infrastructure?
- [ ] Ingress and egress are charged between instances in different availability domains.
- [ ] Egress and ingress are both charged to and from the internet.
- [ ] Ingress is charged between two availability domains.
- [x] Egress to the internet is charged.

> In OCI, ingress data transfer (data coming into OCI from the internet) is typically free. However, egress data transfer (data going out from OCI to the internet) is chargeable after the first 10 TB/month, depending on the specific region and destination.


2. Which is NOT a factor that influences pricing in Oracle Cloud Infrastructure?
- [x] Choice of OCI region
- [ ] Services consumed
- [ ] Type of resource
- [ ] Data transfer

> OCI maintains the same pricing across all regions, so the choice of OCI region does not directly influence pricing. The primary factors that influence pricing in OCI include data transfer costs, the specific services consumed, and the specific type of resource utilized.


3. Which is NOT a supported Oracle Cloud Infrastructure pricing model?
- [x] Sovereign subscriptions
- [ ] Oracle Universal Credits
- [ ] Bring Your Own License (BYOL)
- [ ] Pay As You Go

> The supported pricing models in OCI include Pay As You Go, Oracle Universal Credits, and Bring Your Own License (BYOL). Sovereign subscriptions is not a known pricing model in OCI.


4. In Oracle Cloud Infrastructure, what can you set up to receive notifications when budget thresholds are reached?
- [ ] Push notifications
- [ ] SMS notifications
- [x] Email alerts
- [ ] Pager alerts

> In Oracle Cloud Infrastructure, you can set up email alerts to receive notifications when budget thresholds are reached. These alerts help customers stay informed about their spending and take appropriate actions to manage their costs.


5. In Oracle Cloud Infrastructure, what is the key difference between service limits and compartment quotas?
- [ ] Service limits are user-defined for compartments, while compartment quotas are set by Oracle for a tenancy or region.
- [ ] Both are set and can be modified only by Oracle.
- [x] Service limits are set by Oracle for a tenancy or region, while compartment quotas are user-defined for specific compartments.
- [ ] Both apply only to specific compartments and can be modified only by the user.

> Service limits are the upper bounds placed by Oracle on the number of resources you can create in a region or tenancy, while compartment quotas are the upper bounds defined by the users for resource usage within specific compartments. The distinction is that service limits are set by Oracle and apply to a tenancy in a region, while compartment quotas are set by the users and apply to specific compartments.

<br/>


***

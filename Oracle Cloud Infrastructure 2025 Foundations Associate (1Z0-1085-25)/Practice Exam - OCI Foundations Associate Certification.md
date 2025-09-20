# OCI Foundations Associate Certification
## __*Practice Exam*__: OCI Foundations Associate Certification


1. Which Oracle Cloud Infrastructure service is designed to protect your web applications from various types of malicious attacks, such as SQL
injection and cross-site scripting?
- [ ] Security Zones
- [x] Web Application Firewall (WAF)
- [ ] Cloud Guard
- [ ] Vault Service

> Oracle Cloud Infrastructure Web Application Firewall (WAF) is designed to protect your web applications from various types of malicious attacks, such as SQL injection and cross-site scripting. WAF inspects incoming web traffic and filters out any requests that match predefined security rules, ensuring the security and availability of your web applications. 

2. Which type of Oracle Cloud Infrastructure networking gateway allows access to Oracle services within the same region without traversing the
public internet?
- [ ] NAT Gateway
- [ ] Dynamic Routing Gateway
- [ ] Internet Gateway
- [x] Service Gateway

> A Service Gateway in Oracle Cloud Infrastructure networking service enables access to Oracle services within the same region without the traffic going through the public internet. This provides a more secure and reliable connection for accessing Oracle services like Object Storage, Autonomous Database, and others. 

3. In Oracle Cloud Infrastructure, what is the main difference between a Load Balancer and a Network Load Balancer?
- [ ] A Load Balancer supports only IPv4 addresses, whereas a Network Load Balancer supports both IPv4 and IPv6 addresses.
- [x] A Load Balancer works at the application layer (layer 7), whereas a Network Load Balancer works at the transport layer (layer 4).
- [ ] A Load Balancer is used for private networks, whereas a Network Load Balancer is used for public networks.
- [ ] A Load Balancer works at the transport layer (layer 4), whereas a Network Load Balancer works at the application layer (layer 7).

> The main difference between a Load Balancer and a Network Load Balancer in Oracle Cloud Infrastructure is that a Load Balancer works at the application layer (layer 7) and can handle application-specific traffic, while a Network Load Balancer works at the transport layer (layer 4) and can handle any type of TCP or UDP traffic. 

4. What is the main benefit of using Oracle Cloud Infrastructure Security Zones for resource management?
- [x] Enforcing best practice security configurations
- [ ] Load balancing across regions
- [ ] Managing IAM policies
- [ ] Reducing network latency

> Oracle Cloud Infrastructure Security Zones help to enforce best practice security configurations for your resources. By using Security Zones, you can ensure that resources are created and managed with security best practices, minimizing potential security risks and improving the overall security posture of your infrastructure.


5. Which attribute can be customized when creating an Oracle Cloud Infrastructure Compute flexible shape instance?
- [x] Number of OCPUs and amount of memory
- [ ] Instance shape and instance size
- [ ] Operating system and disk type
- [ ] Number of physical NICs and number of virtual NICs

> When creating an Oracle Cloud Infrastructure Compute flexible shape instance, users can customize the number of OCPUs and the amount of memory according to their needs. Flexible shapes provide more control over resource allocation and help users optimize costs and performance. 


6. Which is a key characteristic of an Oracle Cloud Infrastructure Block Volume?
- [ ] It is ephemeral and deleted when the associated instance is terminated.
- [ ] It is used to store and manage object data.
- [x] It is automatically replicated within an availability domain for high durability.
- [ ] It is a shared file system designed for high performance.

> OCI Block Volumes are automatically replicated within an availability domain for high durability, ensuring data redundancy and protection against hardware failures. 

7. What does "Auto-Tiering" mean in OCI Object Storage?
- [ ] It disables file versioning when objects go unused.
- [x] It moves data to lower-cost tiers based on access patterns.
- [ ] It automatically renames all objects in a bucket every 30 days.
- [ ] It merges multiple buckets into a single bucket automatically.

> Auto-Tiering uses lifecycle policies to move infrequently accessed data from the Standard tier to a lower-cost storage tier, such as Archive or Infrequent Access. This helps reduce costs by keeping rarely accessed objects in less expensive storage.


8. In the Oracle Cloud Infrastructure Compute service, which feature enables users to migrate running instances between different physical servers?
- [x] Live Migration
- [ ] Instance Migration
- [ ] Instance Evacuation
- [ ] Fault Domain Balancing

> Live Migration is a feature in the Oracle Cloud Infrastructure Compute service that enables users to migrate running instances between different fault domains without any downtime. It allows users to perform maintenance or balance workloads across fault domains while maintaining the availability and performance of their applications. 


9. What is the main advantage of vertical scaling in the Oracle Cloud Infrastructure Compute service?
- [ ] Increased fault tolerance
- [x] Enhanced performance with more OCPUs and memory
- [ ] Improved load balancing
- [ ] Reduced network latency

> Vertical scaling in the Oracle Cloud Infrastructure Compute service refers to the process of increasing the performance of an instance by adding more OCPUs and memory. This allows for improved processing capabilities and resource allocation, resulting in enhanced performance for the compute instance. 


10. What is the primary function of the Auto-Tiering feature in the Oracle Cloud Infrastructure Object Storage service?
- [ ] Eliminating storage fees for all objects
- [ ] Reducing storage costs by automatically moving objects between Standard and Archive tiers
- [ ] Providing real-time usage analytics for all objects in the bucket
- [x] Reducing storage costs by automatically moving objects between Standard and Infrequent Access tiers

> Auto Tiering for Object Storage is a feature that helps you automatically move objects between Standard and Infrequent Access tiers based on their access patterns.


11. Which statement best describes Autoscaling for OCI Compute?
- [ ] Autoscaling forces you to stop all instances before resizing them.
- [ ] Autoscaling requires that you create only one VM in your deployment.
- [ ] Autoscaling supports only scaling down resources, not scaling up.
- [x] Autoscaling automatically adjusts the number of running instances based on defined metrics.

> Dynamic Groups allow OCI Compute instances and other cloud resources to act as principals and receive permissions via IAM policies. This means that Compute instances, Functions, and other resources can have permissions without requiring a specific user to authenticate.


12. In Oracle Cloud Infrastructure, which component of an IAM policy statement defines the user or group the policy applies to?
- [ ] Effect
- [x] Principal
- [ ] Resource
- [ ] Action

> In Oracle Cloud Infrastructure, the "Principal" component of an IAM policy statement defines the user or group the policy applies to. It specifies the groups that the policy statement affects, granting them access to resources and actions defined in the policy statement. 


13. Which is NOT a component of an IAM policy statement in Oracle Cloud Infrastructure?
- [ ] Action Verb
- [x] Encryption
- [ ] Resource-type
- [ ] Location

> An IAM policy statement in Oracle Cloud Infrastructure typically consists of these components: Location (compartment or tenancy), Action Verb (the specific action to be allowed), Resource (the resources the action can be performed on), Principal (group the policy applies to), and a set of optional Conditions. Encryption is not a component of an IAM policy statement; it is a security measure used to protect sensitive data. 


14. In the Oracle Cloud Infrastructure Block Volume service, which feature enables you to increase the size of a block volume without any
downtime?
- [ ] Volume Bursting
- [ ] Volume Elasticity
- [x] Online Resizing
- [ ] Dynamic Volume Resizing

> In the Oracle Cloud Infrastructure Block Volume service, Online Resizing enables you to increase the size of a block volume without any downtime. This feature allows you to scale storage capacity on the fly to accommodate growing data needs or application requirements, ensuring continuous availability and performance. 


15. Which Oracle Cloud Infrastructure (OCI) offering allows you to run cloud services in your own data center while maintaining regulatory
compliance?
- [ ] Oracle Database Service for Azure
- [x] OCI Dedicated Region
- [ ] Oracle Database@Azure
- [ ] MySQL HeatWave Database Service

> OCI Dedicated Region enables customers to deploy an Oracle Cloud region in their own data center.


16. How are compartment quotas applied in Oracle Cloud Infrastructure?
- [ ] On a per-region basis
- [x] On a per-compartment basis
- [ ] On a per-tenancy basis
- [ ] Globally, across all compartments

> In Oracle Cloud Infrastructure, compartment quotas are applied on a per-compartment basis. This allows administrators to set different resource limits for each compartment, ensuring that resource usage aligns with the organization's policies and requirements. 


17. Which security feature prevents users from making risky or non-compliant changes to OCI resources?
- [ ] OCI Load Balancer
- [x] OCI Security Zones
- [ ] OCI Object Storage Lifecycle Policy
- [ ] OCI Cloud Guard


18. Which Oracle Cloud Infrastructure service continuously monitors your cloud resources and configurations to detect, assess, and remediate
security risks?
- [ ] Security Advisor
- [x] Cloud Guard
- [ ] Security Zones
- [ ] Vault Service

> Oracle Cloud Infrastructure Cloud Guard continuously monitors your cloud resources and configurations to detect, assess, and remediate security risks. Cloud Guard helps maintain a strong security posture by identifying and addressing potential security issues before they become critical. 


19. What is the term used to describe the combination of an instance's shape, base image, and metadata in the Oracle Cloud Infrastructure
Compute service?
- [x] Instance Configuration
- [ ] Instance Profile
- [ ] Instance Specification
- [ ] Instance Template

> In the Oracle Cloud Infrastructure Compute service, an Instance Configuration is a predefined configuration that includes the instance's shape, base image, and metadata. It allows users to quickly create new instances with the same configuration, streamlining the deployment process.


20. What is the primary goal of distributing resources across multiple availability domains in Oracle Cloud Infrastructure?
- [ ] To increase storage capacity for a region
- [ ] To reduce latency for users in different geographic locations
- [ ] To segregate resources based on project or department
- [x] To improve fault tolerance and high availability

> The primary goal of distributing resources across multiple availability domains in Oracle Cloud Infrastructure is to improve fault tolerance and high availability. By spreading resources across isolated, fault-tolerant data centers within a region, applications can continue operating even if one availability domain experiences an outage. 


21. What is the primary purpose of setting up budgets in Oracle Cloud Infrastructure?
- [x] To monitor and control spending on OCI services
- [ ] To automatically pause OCI services when spending reaches a certain threshold
- [ ] To allocate resources across compartments
- [ ] To set up billing accounts for OCI customers

> The primary purpose of setting up budgets in Oracle Cloud Infrastructure is to monitor and control spending on OCI services. Budgets allow customers to track their spending and receive alerts when their spending approaches or exceeds the budget limits they have set, enabling them to manage costs effectively. 


22. In Oracle Cloud Infrastructure, which component is responsible for controlling traffic between subnets within a virtual cloud network (VCN)?
- [ ] Network Security Groups
- [ ] Internet Gateways
- [ ] Route Tables
- [x] Security Lists

> In Oracle Cloud Infrastructure, Security Lists are responsible for controlling traffic between subnets within a virtual cloud network (VCN). They define ingress and egress rules to determine the allowed traffic at the subnet level. 


23. Which protocol is used by the Oracle Cloud Infrastructure File Storage service for file access?
- [x] NFS (Network File System)
- [ ] SMB (Server Message Block)
- [ ] FTP (File Transfer Protocol)
- [ ] iSCSI (Internet Small Computer Systems Interface)

> The Oracle Cloud Infrastructure File Storage service uses the Network File System (NFS) protocol for file access. NFS allows clients to access files over a network in a manner that appears as though they are part of the local file system. 


24. Which is NOT a type of OCI Compute instance?
- [x] Nano instances
- [ ] Dedicated Virtual Machine Hosts
- [ ] Virtual Machines (VMs)
- [ ] Bare Metal

> The Oracle Cloud Infrastructure Compute service offers Virtual Machines (VMs), Bare Metal instances, and Dedicated Virtual Machine Hosts. Nano instances is not a type of OCI Compute instance. 

25. Which Oracle Cloud Infrastructure service is not designed for use with multiple cloud providers?
- [ ] Oracle Interconnect for Azure
- [ ] MySQL HeatWave Database Service
- [ ] Oracle Database@Azure
- [x] Oracle Roving Edge Infrastructure

> Oracle Roving Edge Infrastructure is a service designed to host workloads and use cases that operate at the edge, especially the far edge and tactical edge. It is designed to function as an extension of your Oracle Cloud tenancy.


26. What is the primary function of a Route Table in Oracle Cloud Infrastructure Networking Service?
- [x] To define rules to route traffic from subnets to destinations outside the VCN
- [ ] To define rules controlling traffic flow between subnets
- [ ] To provide a private connection between a VCN and an on-premises network
- [ ] To connect a VCN to the public internet

> A Route Table is a component in Oracle Cloud Infrastructure Networking Service that defines rules for packet forwarding to destinations outside the Virtual Cloud Network (VCN). Route Tables have rules to route traffic from subnets to destinations outside the VCN by way of gateways or specially configured instances. 


27. In OCI Networking, what is the role of a Dynamic Routing Gateway (DRG)?
- [x] To provide a path for traffic between a VCN and an on-premises network or another VCN
- [ ] To provide a path for traffic between a VCN and the public internet
- [ ] To distribute incoming traffic to backend resources
- [ ] To enforce security rules on a group of cloud resources

> A Dynamic Routing Gateway (DRG) provides a path for traffic between a VCN and an on-premises network or another VCN in the same or different region. 


28. Why is it important to choose an OCI Region close to your users?
- [ ] To enable automatic resource scaling
- [ ] To reduce the cost of cloud storage
- [ ] To ensure that only one Availability Domain is used
- [x] To minimize latency and improve application performance

> It is important to choose a region close to users to reduce network latency and increase application performance. 


29. Which statement about compartments in Oracle Cloud Infrastructure is NOT true?
- [ ] Compartments can be nested to create a hierarchy.
- [ ] IAM policies can be written to grant access to resources in specific compartments.
- [ ] Compartments are global resources.
- [x] Compartments provide a way to store and manage encryption keys and secrets.

> Compartments in Oracle Cloud Infrastructure are a global resource; they can be nested to create a hierarchy; and IAM policies can be written to grant access to resources in specific compartments. However, storing and managing encryption keys and secrets is a function of the Oracle Cloud Infrastructure Vault service, not compartments. 


30. Which type of load balancing policy is supported by Oracle Cloud Infrastructure Load Balancer?
- [ ] Most connections
- [x] Weighted Round Robin
- [ ] Name Hash
- [ ] Random

> Oracle Cloud Infrastructure Load Balancer supports three types of load balancing algorithms: Round Robin, Least Connections, and IP Hash. The Round Robin algorithm distributes incoming traffic evenly across instances. This algorithm helps ensure efficient distribution of network traffic and maintain the availability and performance of applications. Weighted Round Robin, Weighted Least Connections, and Random are not supported by OCI Load Balancer. 


31. Which is a key difference between Security Lists and Network Security Groups in Oracle Cloud Infrastructure?
- [ ] Security Lists are stateful, whereas Network Security Groups are stateless.
- [ ] Security Lists support only ingress rules, whereas Network Security Groups support both ingress and egress rules.
- [ ] Security Lists encrypt data in transit, whereas Network Security Groups do not.
- [x] Security Lists apply to subnets, whereas Network Security Groups apply to individual instance VNICs.

> The key difference between Security Lists and Network Security Groups in Oracle Cloud Infrastructure is that Security Lists apply to subnets, while Network Security Groups apply to individual instance VNICs. This allows for more granular control of traffic in and out of instances. 


32. What is the function of a Dynamic Group in OCI IAM?
- [ ] A group that enforces two-factor authentication for high-security environments
- [x] A group that allows policies to be assigned to compute instances and other OCI resources, instead of users
- [ ] A group that stores audit logs for IAM security events
- [ ] A group of users that automatically receives administrator privileges

> Dynamic Groups allow OCI Compute instances and other cloud resources to act as principals and receive permissions via IAM policies. This means that Compute instances, Functions, and other resources can have permissions without requiring a specific user to authenticate.


33. In the Oracle Cloud Infrastructure Object Storage service, which storage tier is designed for rarely or seldom accessed data that can be restored
within hours?
- [ ] Standard Storage
- [x] Archive Storage
- [ ] Intelligent Tiering
- [ ] One Zone-Infrequent Access

> Archive Storage is a storage tier in the Oracle Cloud Infrastructure Object Storage service designed for rarely or seldom accessed data that can be restored within hours. It offers the lowest cost per stored gigabyte and is suitable for long-term storage of data that is not needed for immediate access, such as backups or historical data. 


34. Which data transfer type is generally free of charge in Oracle Cloud Infrastructure?
- [ ] Egress data transfer to AWS or GCP
- [ ] Egress data transfer to the Internet
- [ ] Egress data transfer to a different OCI region
- [x] Ingress data transfer

> Ingress data transfer refers to the data transferred into Oracle Cloud Infrastructure from other sources. Generally, ingress data transfer is free of charge, while egress data transfer can have associated costs depending on the destination (to a different cloud provider like AWS or GCP, to a different OCI region, or to the internet). 


35. Which type of scaling is achieved by adding or removing instances within an instance pool in Oracle Cloud Infrastructure Compute?
- [ ] Vertical scaling
- [ ] Diagonal scaling
- [ ] Proportional scaling
- [x] Horizontal scaling

> Horizontal scaling is achieved by adding or removing instances within an instance pool in Oracle Cloud Infrastructure Compute. This type of scaling helps manage workloads and maintain optimal resource utilization by distributing traffic across multiple instances. 


36. Which is a key function of a Route Table in a VCN?
- [x] To direct network traffic to the correct destination
- [ ] To define firewall rules that determine allowed network traffic
- [ ] To store user credentials for access to OCI services
- [ ] To provide encryption services for data at rest in the VCN

> A Route Table in OCI defines how traffic leaving a subnet is routed. You create route rules to send traffic to specific targets, such as an Internet Gateway (for public traffic) or a NAT Gateway (for instances in a private subnet requiring outbound internet access). It does not manage encryption or user credentials; those functions are handled by other services. Firewall rules are set using Security Lists or Network Security Groups, not Route Tables.


37. In the Oracle Cloud Infrastructure shared security responsibility model, who is responsible for securing the customer's data, applications, and
access control?
- [x] The customer
- [ ] Government agencies
- [ ] Oracle
- [ ] Third-party vendors

> In the Oracle Cloud Infrastructure shared security responsibility model, the customer is responsible for securing their data, applications, and access control. This includes implementing appropriate security measures such as encryption, user access control, and monitoring to protect sensitive data and ensure the overall security of their cloud environment. 


38. How does Oracle Cloud Infrastructure's Bring Your Own License (BYOL) feature help customers save
on costs?
- [ ] By offering free software licenses for certain OCI services
- [ ] By bundling software licenses with OCI services at a discounted rate
- [x] By allowing customers to use existing software licenses in OCI
- [ ] By providing discounts on new software licenses purchased for OCI

> Oracle Cloud Infrastructure's Bring Your Own License (BYOL) feature helps customers save on costs by allowing them to use their existing software licenses in OCI. This means customers can leverage their investment in Oracle software licenses when migrating or deploying new applications in OCI, without the need to purchase additional licenses. 


39. What type of storage is associated with instances in the Oracle Cloud Infrastructure Compute service?
- [ ] Infrequent Access Storage
- [x] Block Storage
- [ ] Archive Storage
- [ ] Object Storage

> Block storage is the type of storage associated with instances in the Oracle Cloud Infrastructure Compute service. It provides low-latency, high-performance storage volumes that can be attached to instances to store data and applications. 


40. Which tool in Oracle Cloud Infrastructure allows you to visualize and analyze your cloud usage and spending patterns over time?
- [ ] Usage Reports
- [x] Cost Analysis
- [ ] Quotas
- [ ] Budgets

> The Cost Analysis tool in Oracle Cloud Infrastructure enables users to visualize and analyze their cloud usage and spending patterns over time. This helps users better understand their consumption of resources and services and make informed decisions about cost optimization. 


<br />

___
## Coursera Notes - Week 1

### Module 1: AWS Overview  and Security
**Regions**. 
Regions are geographic locations worldwide where AWS hosts its data centers. Each AWS Region is associated with a geographical name and a Region code. Example: Canada (Central) ca-central-1

**Availability Zones**. 
An Availability Zones(AZ) consists of one or more data centers with redundant power, networking, and connectivity. These data centers operate in discrete facilities with undisclosed locations. They are connected using redundant high-speed and low-latency links. Example: us-east-1a -> an AZ in us-east-1 (Northern Virginia Region).

**Edge Locations**. 
An edge location is a site that Amazon CloudFront uses to store cached copies of your content closer to your customers for faster delivery. Edge locations are an integral component of the AWS infrastructure, supporting the delivery of content and services to end-users worldwide.

A simple way to understand their relationship is:

Region: Where your application lives. 
Availability Zone: How your application stays available. 
Edge Location: How your content reaches users faster. 

**Shared Responsibility Model**. 
##### AWS Responsibilities (Security of the Cloud):  
AWS is responsible for protecting the infrastructure that runs all the services in the AWS Cloud. This includes:
- Physical security of data centers
- Managing hardware, software, and networking components
- Ensuring the security of AWS Regions and Availability Zones

##### Customer Responsibilities (Security in the Cloud):  
Customers are responsible for securing their applications and data in the cloud. This includes:
- Configuring AWS services properly
- Managing access controls
- Protecting data through encryption and backups

##### Root User:  
Root User is the original account created when you set up your AWS account. It has complete access to all AWS services and resources, much like a master key to a house that opens every door. 

##### IAM User:
IAM Users (Identity and Access Management Users) are created within your AWS account to allow others to access AWS resources without giving them full control. Think of IAM Users as individual keys that can be given to family members, each with specific permissions tailored to their needs. 

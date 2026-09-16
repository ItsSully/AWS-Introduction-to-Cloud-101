# AWS Educate – Introduction to AWS
## Module 4: AWS Core Services

### Module Objectives

By the end of this module, I should be able to:

- Define the different types of AWS services
- Identify the main categories of services used as part of a cloud architecture
- Describe each core AWS service, including its use, features and benefits

---

## 1. AWS Core Services

AWS provides a wide range of cloud services that can be combined to build complete applications and IT environments.

AWS services cover areas including:

- Compute
- Storage
- Networking
- Databases
- Security
- Monitoring
- Application integration

This module introduces several core AWS services and explains how they can work together as part of a cloud architecture.

---

## 2. Monolithic Architecture

A **monolithic architecture** is an application where the different components of the application are developed and deployed as a single unit.

For example, an application may contain:

- User interface
- Application logic
- Database functionality

All of these components can be part of one application.

### Advantages

- Simple to develop initially
- Easier to deploy as a single application
- Straightforward architecture for smaller applications

### Disadvantages

- Changes to one part can require redeploying the whole application
- Scaling individual components can be difficult
- A problem in one component can potentially affect the entire application
- Large applications can become difficult to maintain

---

## 3. Microservices Architecture

A **microservices architecture** breaks an application into smaller, independent services.

Each service performs a specific function and can be developed, deployed and scaled independently.

For example:

```text
Application
│
├── User Service
├── Payment Service
├── Authentication Service
├── Product Service
└── Notification Service
```

### Advantages

- Individual services can be scaled independently
- Services can be developed and deployed separately
- Problems can potentially be isolated to individual services
- Different technologies can be used for different services

### Disadvantages

- More complex architecture
- Requires communication between services
- Monitoring and managing multiple services can be more difficult
- Requires careful design of networking and security

### Monolithic vs Microservices

| Monolithic |	Microservices |
|---|---|
| Single application unit |	Multiple independent services |
| Usually simpler initially	| More complex |
| Components are tightly connected	| Components are more independent |
| Scaling can affect the whole application	| Individual services can be scaled |
| Easier to deploy initially	| Services can be deployed independently |

### Advantages

- Individual services can be scaled independently
- Services can be developed and deployed separately
- Problems can potentially be isolated to individual services
- Different technologies can be used for different services

### Disadvantages
- More complex architecture
- Requires communication between services
- Monitoring and managing multiple services can be more difficult
- Requires careful design of networking and security

### Monolithic vs Microservices
| Monolithic	| Microservices |
|---|---|
| Single application unit	| Multiple independent services | 
| Usually simpler initially	| More complex |
| Components are tightly connected	| Components are more independent |
| Scaling can affect the whole application	| Individual services can be scaled |
| Easier to deploy initially	| Services can be deployed independently |

---

## 4. Types of AWS Services

AWS services can be grouped into different categories depending on the function they provide.

Important categories include:

Compute – Provides processing power
Storage – Stores data and files
Networking – Connects and controls communication between resources
Database – Stores and manages structured and unstructured data
Security – Controls access and protects resources
Monitoring – Tracks resources, applications and performance
Application Integration – Allows applications and services to communicate

Different AWS services can be combined to create a complete cloud architecture.

---

## 5. Core Services Architecture

A cloud application can use multiple AWS services together.

For example:
```text
                    Users
                      │
                      ▼
                  Application
                      │
          ┌───────────┴───────────┐
          ▼                       ▼
        EC2                    Lambda
          │                       │
          └───────────┬───────────┘
                      ▼
                  Database
                 ┌────┴────┐
                 ▼         ▼
                RDS     DynamoDB

          ┌─────────────────────┐
          │       S3            │
          │   Object Storage    │
          └─────────────────────┘

          ┌─────────────────────┐
          │    CloudWatch       │
          │     Monitoring      │
          └─────────────────────┘

          ┌─────────────────────┐
          │        IAM          │
          │  Access & Security  │
          └─────────────────────┘
```

The services have different purposes but can work together to build secure, scalable applications.

---

## 6. AWS Identity and Access Management (IAM)

AWS Identity and Access Management (IAM) controls who can access AWS resources and what they are allowed to do.

IAM can be used to manage:

Users
Groups
Roles
Permissions
Policies
Key concept

IAM follows the principle of giving users and systems only the permissions they need.

This is known as the principle of least privilege.

#### Example

A developer may need permission to access a specific S3 bucket but should not automatically have permission to delete an entire AWS account's resources.

### Why IAM is important

IAM helps organisations:

Control access
Protect resources
Manage permissions
Reduce unnecessary privileges
Improve security

IAM = Who can access what, and what can they do?

---

## 7. Amazon DynamoDB

Amazon DynamoDB is a fully managed NoSQL database service.

It is designed to provide fast and predictable performance at scale.

DynamoDB is useful for applications that require:

High performance
Scalability
Low-latency data access
Flexible data structures

Unlike traditional relational databases, DynamoDB uses a NoSQL data model.

### Key idea

DynamoDB = Managed NoSQL database

---

## 8. Amazon Virtual Private Cloud (VPC)

Amazon VPC allows customers to create a logically isolated network within AWS.

A VPC provides control over networking for AWS resources.

It can include:

IP address ranges
Subnets
Route tables
Network connectivity
Security controls

For example, an organisation could create a VPC containing its application servers and databases.

### Key idea

VPC = Your virtual network in AWS

VPCs are important for controlling how AWS resources communicate with each other and with external networks.

---

## 9. Amazon Elastic Compute Cloud (EC2)

Amazon EC2 provides virtual servers in the AWS cloud.

EC2 allows customers to run applications using virtual machines rather than purchasing physical servers.

Customers can configure aspects such as:

Operating system
CPU
Memory
Storage
Networking
Benefits
Flexible computing capacity
Scalable
Multiple instance types
Control over the operating environment
Example

A company could deploy a web application onto an EC2 instance instead of purchasing and maintaining a physical server.

EC2 = Virtual servers in the cloud

---

## 10. AWS Lambda

AWS Lambda is a serverless compute service that runs code in response to events.

With Lambda, developers do not need to manage the underlying servers.

Lambda functions can be triggered by events such as:

Application requests
File uploads
Database events
Scheduled events
Messages from other AWS services
Benefits
No server management
Automatically scales based on demand
Event-driven
Pay for compute usage
Key idea

Lambda = Run code without managing servers

---

## 11. Amazon Simple Notification Service (SNS)

Amazon SNS is a messaging and notification service.

It can send messages or notifications from one system to multiple recipients or services.

SNS can be used for:

Application notifications
Alerts
Messaging
Event-driven architectures
Example

A monitoring system could detect an important event and use SNS to send a notification.

SNS = Messaging and notifications

---

## 12. Amazon CloudWatch

Amazon CloudWatch is a monitoring and observability service.

It can collect and monitor information about AWS resources and applications.

CloudWatch can be used to monitor:

Metrics
Logs
Events
Application performance
Resource activity
Example

CloudWatch could monitor an EC2 instance and provide information about its resource usage.

It can also be used to create alarms when certain conditions occur.

### Key idea

CloudWatch = Monitor AWS resources and applications

---

## 13. Amazon Relational Database Service (RDS)

Amazon RDS is a managed relational database service.

It makes it easier to set up, operate and scale relational databases without managing all of the underlying infrastructure yourself.

Relational databases organise data into structured tables.

RDS can be used for applications that require structured relational data.

Benefits
Managed database infrastructure
Automated administrative tasks
Scalability options
High availability features
Database backups

RDS = Managed relational database

---

## 14. Amazon Simple Storage Service (S3)

Amazon S3 is an object storage service.

It is designed to store and retrieve large amounts of data.

S3 can be used for:

Files
Images
Videos
Backups
Logs
Application data

S3 stores objects inside buckets.

Basic structure

```text
S3
│
└── Bucket
    │
    ├── image.jpg
    ├── report.pdf
    ├── backup.zip
    └── data.csv
```

### Key idea

S3 = Object storage

S3 is highly scalable and is commonly used for storing data that applications need to access.

---

## 15. AWS Core Services – Quick Reference

| Service	| Category	| Main Purpose |
|---|---|---|
| IAM	| Security | Identity and access management |
| DynamoDB |	Database |	NoSQL database |
| VPC |	Networking	| Virtual network |
| EC2 |	Compute |	Virtual servers |
| Lambda	| Compute |	Serverless code execution |
| SNS	| Application Integration	| Messaging and notifications |
| CloudWatch |	Monitoring	| Monitoring, metrics and logs |
| RDS	| Database |	Managed relational database |
| S3	| Storage	| Object storage |

---

## 16. Understanding the Services Together

The core AWS services can be combined to build a complete application.

For example:

VPC provides the application's network environment.
EC2 can run the application's servers.
S3 can store files and application objects.
RDS can store structured relational data.
DynamoDB can store NoSQL data.
IAM controls access to AWS resources.
Lambda can run code in response to events.
SNS can send notifications.
CloudWatch monitors the environment.

This demonstrates that AWS services are designed to work together rather than being used in isolation.

---

## 17. AWS Core Services Demos

This module also includes demonstrations of several core AWS services.

The demonstrations covered:

Amazon S3
Amazon EC2
Amazon VPC
Amazon RDS
AWS IAM
AWS Lambda
Amazon CloudWatch

These demonstrations provide practical exposure to how the services are accessed and used within AWS.

### Key Concepts to Remember
| Concept |	Definition |
|---|---|
| Monolithic Architecture	| Application built and deployed as a single unit |
| Microservices |	Application divided into smaller independent services |
| IAM	| Manages identities, permissions and access |
| DynamoDB |	Managed NoSQL database |
| VPC |	Isolated virtual network in AWS |
| EC2 | Virtual cloud servers |
| Lambda | Serverless code execution |
| SNS	| Messaging and notification service |
| CloudWatch | Monitoring and observability service |
| RDS	| Managed relational database |
| S3	| Object storage service |

---

## AWS Services – Easy Memory Guide
```text
IAM       → Access & permissions
VPC       → Network
EC2       → Virtual server
Lambda    → Serverless code
S3        → Object storage
RDS       → Relational database
DynamoDB  → NoSQL database
SNS       → Notifications
CloudWatch → Monitoring
```
---

## Module 4 Summary

Module 4 introduced several of the core services used to build applications and infrastructure on AWS.

I learned how cloud applications can use different AWS services together, and how monolithic and microservices architectures differ.

The module introduced core AWS services including EC2, Lambda, S3, RDS, DynamoDB, VPC, IAM, SNS and CloudWatch.

Each service has a different role within a cloud architecture:

EC2 and Lambda provide compute
S3 provides object storage
RDS and DynamoDB provide databases
VPC provides networking
IAM provides identity and access management
SNS provides messaging and notifications
CloudWatch provides monitoring

Understanding how these services work individually and how they can be combined is an important foundation for designing and securing AWS environments.


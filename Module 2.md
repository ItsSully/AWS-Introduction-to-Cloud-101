# AWS Educate – Introduction to AWS
## Module 2: Introduction to AWS

### Module Objectives

By the end of this module, I should be able to:

- Discuss the history of AWS cloud computing
- Describe the AWS global infrastructure
- Explain the customer and AWS responsibilities within the shared responsibility model
- Describe the AWS Well-Architected Framework and its pillars
- Understand Total Cost of Ownership (TCO) and AWS billing considerations

---

# 1. AWS Offerings

**Amazon Web Services (AWS)** is a cloud computing platform that provides a wide range of services for different computing requirements.

AWS services cover areas such as:

- Compute
- Storage
- Databases
- Networking
- Security
- Analytics
- Machine Learning
- Application development

AWS provides customers with access to cloud infrastructure without requiring them to build and maintain their own physical data centres.

---

# 2. AWS Benefits

AWS provides several benefits to organisations using cloud computing.

### Flexibility

Organisations can choose the services and resources that meet their specific requirements.

### Scalability

Resources can be increased or decreased as demand changes.

### Global Reach

AWS has infrastructure distributed across multiple geographical locations, allowing organisations to deploy applications closer to their customers.

### Security

AWS provides security features and services to help customers protect their cloud environments.

### Reliability

AWS infrastructure is designed to support highly available and reliable applications.

### Cost Efficiency

Customers can avoid many of the large upfront costs associated with purchasing and maintaining physical infrastructure.

---

# 3. Brief History of AWS

AWS was developed by Amazon as a way of providing scalable technology infrastructure through cloud services.

AWS launched its first major public cloud services in **2006**, initially providing services such as storage and computing infrastructure.

AWS continued expanding its services and infrastructure, becoming one of the major providers of cloud computing services.

Today, AWS provides a large range of cloud services used by organisations around the world.

---

# 4. AWS is a Leader in Cloud Computing

AWS is one of the major providers in the global cloud computing industry.

Its large range of services allows organisations to build and operate many different types of applications and infrastructure without having to maintain their own physical data centres.

AWS is used by:

- Start-ups
- Universities
- Governments
- Large enterprises
- Developers
- Small businesses

AWS provides services that can support everything from small applications to large-scale enterprise systems.

---

# 5. AWS Global Infrastructure

AWS operates a global infrastructure designed to provide reliable and highly available cloud services.

The infrastructure is organised into several key components:

- **Regions**
- **Availability Zones (AZs)**
- **Edge Locations**

These components allow AWS customers to deploy resources across different geographical locations.

---

# 6. Regions, Availability Zones and Edge Locations

## AWS Regions

An **AWS Region** is a separate geographical area containing AWS infrastructure.

Examples include regions in:

- Europe
- North America
- Asia Pacific
- South America

When deploying AWS resources, customers can select the Region where their resources will operate.

### Why choose a specific Region?

Choosing an appropriate Region can help with:

- Reducing latency
- Meeting data residency requirements
- Regulatory requirements
- Disaster recovery
- Availability

---

## Availability Zones (AZs)

An **Availability Zone** is one or more discrete data centres within an AWS Region.

Each Region contains multiple Availability Zones.

Availability Zones are designed to be sufficiently separated from each other to reduce the impact of failures while remaining connected through AWS networking.

### Key idea

> **Region = Geographical area**  
> **Availability Zone = Isolated infrastructure location within a Region**

Using multiple Availability Zones can improve application availability and resilience.

---

## Edge Locations

**Edge Locations** are locations used by AWS services to deliver content and applications closer to end users.

They help reduce latency by allowing content to be delivered from locations geographically closer to users.

### Key idea

> **Edge Location = Brings content/services closer to users**

---

# 7. Map of AWS Regions

AWS has Regions distributed around the world.

This global infrastructure allows organisations to choose where their applications and data are hosted.

When selecting a Region, organisations should consider factors such as:

- User location
- Network latency
- Legal and regulatory requirements
- Service availability
- Cost
- Disaster recovery requirements

---

# 8. Planning for Failure

Cloud environments should be designed with the assumption that failures can occur.

A well-designed AWS environment should avoid relying on a single point of failure.

For example, an application could be deployed across multiple Availability Zones.

If one Availability Zone experiences a problem, the application may continue operating using resources in another Availability Zone.

### Key principle

> **Design systems to continue operating even when individual components fail.**

This is an important concept for building highly available and resilient systems.

---

# 9. Example of AWS Regions

A company operating internationally may choose different AWS Regions based on where its users are located.

For example:

- A UK-based application could use a European Region.
- A US-based application could use a North American Region.
- A global application could deploy resources across multiple Regions.

The appropriate Region depends on the application's requirements.

---

# 10. Benefits of AWS Global Infrastructure

AWS's global infrastructure provides several advantages.

### Lower Latency

Applications can be deployed closer to users, reducing the distance data needs to travel.

### High Availability

Applications can use multiple Availability Zones to reduce the impact of infrastructure failures.

### Disaster Recovery

Resources can be distributed across different locations to help protect against regional failures.

### Global Expansion

Organisations can deploy applications in different geographical locations as they expand.

### Data Residency

Organisations can select Regions based on legal, regulatory and data-location requirements.

---

# 11. AWS Shared Responsibility

AWS uses a **Shared Responsibility Model** for cloud security.

This means that security responsibilities are divided between:

- **AWS**
- **The customer**

AWS is responsible for security **of the cloud**, while customers are responsible for security **in the cloud**.

---

# 12. Shared Responsibility Model

## AWS Responsibilities

AWS is responsible for protecting the underlying infrastructure that runs AWS services.

This includes areas such as:

- Physical data centres
- Physical hardware
- Networking infrastructure
- Facilities
- Infrastructure that supports AWS services

AWS is responsible for ensuring that the underlying cloud infrastructure is secure.

---

## Customer Responsibilities

Customers are responsible for securing what they put into the AWS environment.

Depending on the services being used, this can include:

- Customer data
- Operating systems
- Applications
- Access controls
- Identity and permissions
- Network configuration
- Security settings

The exact customer responsibility depends on the AWS service being used.

### Key idea

> **AWS = Security OF the cloud**  
> **Customer = Security IN the cloud**

---

# 13. AWS Well-Architected Framework

The **AWS Well-Architected Framework** provides guidance for designing and operating secure, reliable, efficient and cost-effective cloud workloads.

It is based around several key principles called **pillars**.

The six pillars are:

1. Operational Excellence
2. Security
3. Reliability
4. Performance Efficiency
5. Cost Optimization
6. Sustainability

---

## 13.1 Operational Excellence

Focuses on operating and monitoring systems effectively.

Important areas include:

- Monitoring
- Automation
- Continuous improvement
- Responding to events
- Improving operational processes

### Goal

> Run and improve systems effectively.

---

## 13.2 Security

Focuses on protecting systems, data and infrastructure.

Important areas include:

- Identity and access management
- Access control
- Data protection
- Detection
- Incident response

### Goal

> Protect information and systems from threats.

---

## 13.3 Reliability

Focuses on ensuring workloads perform correctly and recover from failures.

Important areas include:

- Fault tolerance
- Recovery
- High availability
- Monitoring
- Disaster recovery

### Goal

> Keep systems operating and recover quickly from failures.

---

## 13.4 Performance Efficiency

Focuses on using computing resources efficiently.

This includes selecting appropriate resources and adapting them as requirements change.

### Goal

> Use resources efficiently while maintaining the required performance.

---

## 13.5 Cost Optimization

Focuses on avoiding unnecessary cloud expenditure.

This includes:

- Monitoring usage
- Selecting appropriate resources
- Eliminating unnecessary resources
- Understanding pricing
- Optimising workloads

### Goal

> Get the required business value while avoiding unnecessary costs.

---

## 13.6 Sustainability

Focuses on reducing the environmental impact of cloud workloads.

This includes using resources efficiently and avoiding unnecessary consumption.

### Goal

> Reduce the environmental impact of running cloud workloads.

---

# 14. Costs & Billing

Cloud computing introduces different ways of paying for computing resources.

AWS generally allows customers to pay based on their usage of services.

Important billing considerations include:

- Which AWS services are being used
- How much each service is being used
- Where resources are deployed
- Storage usage
- Data transfer
- Computing usage

Customers should monitor their AWS usage to avoid unexpected costs.

---

# 15. Total Cost of Ownership (TCO)

**Total Cost of Ownership (TCO)** is the overall cost of acquiring, operating and maintaining a technology solution.

When comparing traditional infrastructure with cloud infrastructure, organisations should consider more than just the purchase price of hardware.

Traditional infrastructure can involve costs such as:

- Servers
- Storage
- Networking equipment
- Data centre space
- Electricity
- Cooling
- Hardware maintenance
- IT staff
- Hardware replacement

Cloud computing can change these costs because much of the underlying infrastructure is managed by the cloud provider.

### Key idea

> **TCO = The overall cost of owning and operating a solution.**

---

# 16. AWS Pricing Calculator

The **AWS Pricing Calculator** can be used to estimate the potential cost of AWS services.

It allows customers to estimate costs based on factors such as:

- Services being used
- Number of resources
- Usage levels
- Region
- Storage
- Computing requirements

This can help organisations plan and compare potential AWS deployments before implementing them.

---

# 17. AWS Pricing Models

AWS provides different pricing options depending on the service and usage requirements.

Common pricing approaches include:

### Pay-as-you-go

Customers pay for the resources they actually use.

### Reserved/Savings Options

Customers can receive lower costs by committing to certain levels of usage or capacity for a specified period, depending on the service.

### Spot Pricing

Certain AWS compute capacity can be purchased at discounted prices when available, making it useful for workloads that can tolerate interruptions.

---

# 18. AWS Free Tier

The **AWS Free Tier** allows customers to use certain AWS services within specified usage limits without being charged for those eligible amounts.

Free Tier eligibility and limits depend on the specific AWS service and account conditions.

> Always check the current AWS Free Tier terms before using services, as limits and eligibility can change.

---

# 19. AWS Billing Dashboard

The AWS Billing Dashboard provides information about AWS account costs and usage.

It can be used to:

- View current charges
- Review usage
- Monitor spending
- Understand costs
- Manage billing information

Monitoring billing is important when working with cloud environments.

---

# 20. Billing Examples

AWS costs depend on the services and resources being used.

For example, an organisation's bill could be affected by:

- Amount of compute time
- Amount of storage used
- Number of requests
- Data transferred
- Region selected
- Resources running continuously

Therefore, cloud costs should be monitored and managed as part of operating an AWS environment.

---

# Key Concepts to Remember

| Concept | Definition |
|---|---|
| **AWS Region** | Geographical area containing AWS infrastructure |
| **Availability Zone** | Isolated infrastructure location within an AWS Region |
| **Edge Location** | Location used to deliver content closer to users |
| **Shared Responsibility Model** | AWS and the customer share security responsibilities |
| **AWS Responsibility** | Security of the underlying cloud infrastructure |
| **Customer Responsibility** | Security of resources and data within the cloud |
| **Well-Architected Framework** | Guidance for designing effective cloud workloads |
| **TCO** | Total Cost of Ownership |
| **AWS Pricing Calculator** | Tool for estimating AWS costs |
| **Free Tier** | Eligible AWS usage available within specified limits |
| **Billing Dashboard** | Tool for monitoring AWS costs and usage |

---

# Well-Architected Framework – Quick Reference

| Pillar | Main Focus |
|---|---|
| **Operational Excellence** | Operating and improving systems |
| **Security** | Protecting systems and data |
| **Reliability** | Recovering from failures and maintaining availability |
| **Performance Efficiency** | Using resources efficiently |
| **Cost Optimization** | Managing and reducing unnecessary costs |
| **Sustainability** | Reducing environmental impact |

---

# AWS Global Infrastructure – Quick Reference

```text
AWS Global Infrastructure
│
├── Regions
│   └── Geographical areas
│
├── Availability Zones
│   └── Isolated infrastructure locations within Regions
│
└── Edge Locations
    └── Locations that help deliver content closer to users
```
---

Module 2 Summary

Module 2 introduced the fundamentals of Amazon Web Services (AWS), including its history, global infrastructure and major benefits.

I learned how AWS Regions, Availability Zones and Edge Locations work together to provide a global and resilient cloud infrastructure.

The module also introduced the AWS Shared Responsibility Model, which explains how security responsibilities are divided between AWS and the customer.

The AWS Well-Architected Framework provides six pillars for designing effective cloud workloads:

Operational Excellence
Security
Reliability
Performance Efficiency
Cost Optimization
Sustainability

Finally, the module covered cloud costs, Total Cost of Ownership (TCO), AWS pricing, the AWS Pricing Calculator, Free Tier and billing.

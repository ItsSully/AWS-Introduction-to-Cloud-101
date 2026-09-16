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





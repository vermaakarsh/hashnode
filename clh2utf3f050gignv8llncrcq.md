---
title: "Deep Dive into Architecture Patterns, Part 1"
seoDescription: "Guide to architecture patterns for software systems, covering functional and non-functional requirements for optimal selection"
datePublished: Sun Apr 30 2023 03:30:39 GMT+0000 (Coordinated Universal Time)
cuid: clh2utf3f050gignv8llncrcq
slug: deep-dive-into-architecture-patterns-part-1
canonical: https://www.cafeio.xyz/deep-dive-into-architecture-patterns-part-1/
cover: https://cdn.hashnode.com/res/hashnode/image/stock/unsplash/SQ9GJ6vkuOM/upload/a4e632d5edb646df48ff96f411215bdb.jpeg
tags: software-architecture, system-design

---

> Deep Dive into Architecture Patterns. This Post is focused on understanding requirements (Functional and Non-Functional)

Architecture patterns are general, reusable solutions to recurring design problems at the system level. They provide a blueprint for organising and structuring software systems and their components, such as modules, layers, and services. Architecture patterns provide guidance on how to design and implement software systems with specific characteristics and qualities, such as scalability, performance, security, and maintainability.

In the previous post \[Architecture Patterns,\] we looked at patterns from a bird's-eye view. Patterns, however, are the heart and soul of Architecture and warrant a much deeper conversation. In the upcoming parts (still discovering how many to write) I intend to talk about patterns in more depth.

In this post, I will talk about System requirement that lead to the right pattern selection.

## Factors Influencing Architectural Pattern Choice

There could be a variety of factors influencing the choice of patterns. Some of the more obvious ones are listed below.

1. **Functional Requirements :** Functional requirements describe what the system should do, such as the features it must provide and the tasks it must perform. The functional requirements of a system can help determine the appropriate architecture pattern. For example, if the system needs to support multiple user interfaces, a layered architecture pattern may be appropriate, as it provides a clear separation between the presentation layer and the business logic layer. On the other hand, if the system needs to support complex business workflows and data processing, a workflow-driven architecture pattern may be more suitable.
    
2. **Technology Stack:** The technology stack used in the system can influence the choice of architecture pattern. For example, if the system is built using a specific programming language or framework, there may be architecture patterns that are better suited to that technology stack.
    
3. **Domain Complexity:** The complexity of the domain that the system is intended to model can help determine the appropriate architecture pattern. For example, if the domain is complex and involves many interacting components, a domain-driven design (DDD) architecture pattern may be appropriate.
    
4. **Non-functional Requirements:** Non-functional requirements such as performance, security, and maintainability can also influence the choice of architecture pattern. For example, if the system needs to be highly secure, a layered architecture pattern may be appropriate.
    

Beyond this, I have found the following to be also a contributing factor :

* Team’s Capability (One of the Underdog in the selection)
    
* COTS products and Vendor-driven environments (Influence Security and compliance heavily)
    
* Existing IT Landscape (Data Center Setups can potentially challenge some modern patterns which are better suited to cloud)
    
* Pricing and Time To Market
    

## Functional Requirements

Functional requirements are a crucial element in the development of software systems. They define what a system should do, including its features and functionality. When it comes to designing the software architecture, functional requirements have a significant impact on the selection of appropriate architecture patterns.

(img)

Functional requirements can determine the appropriate architecture pattern by providing insights into the system's features and capabilities.

* For example, if the system needs to handle complex business workflows and data processing, a workflow-driven architecture pattern may be more suitable. This pattern provides a visual representation of the workflow and ensures that the business logic is decoupled from the presentation layer.
    
* Similarly, if the system needs to support multiple user interfaces, a layered architecture pattern may be appropriate. This pattern separates the system into different layers, each with a specific responsibility, making it easier to maintain and scale the system.
    
* Another example of how functional requirements can impact architecture patterns is in the case of real-time systems. Real-time systems have stringent timing requirements and require an architecture pattern that can provide predictable and reliable performance. In this case, a microservices architecture pattern may be more suitable, as it enables the system to be broken down into smaller, independent services that can be scaled and deployed separately.
    

In conclusion, functional requirements have a significant impact on the selection of appropriate architecture patterns. The selection of an architecture pattern must meet the functional requirements of the system and ensure that it is scalable, maintainable, and extensible. Therefore, it is crucial to carefully analyse the system's functional requirements before selecting an appropriate architecture pattern.

## Non – Functional requirements

Non-functional requirements define the performance, security, reliability, and other quality attributes that a software system must meet. Non-functional requirements are important because they determine how well the system performs its tasks and how easy it is to use and maintain.

(img)

* One example of how non-functional requirements impact architecture patterns is in the case of performance. If a system has high-performance requirements, such as low latency or high throughput, then an appropriate architecture pattern must be selected. In this case, a distributed architecture pattern, such as a microservices architecture or a service-oriented architecture, may be more suitable, as it provides scalability and fault tolerance.
    
* Similarly, if a system needs to be highly secure, a layered architecture pattern with a clear separation of concerns may be more appropriate. This pattern separates the system into different layers, each with a specific responsibility, making it easier to secure and maintain.
    
* Another example of how non-functional requirements can influence architecture patterns is in the case of scalability. If a system needs to handle a large volume of data or traffic, then an appropriate architecture pattern must be selected. In this case, a distributed architecture pattern such as a microservices' architecture may be more suitable, as it enables the system to be broken down into smaller, independent services that can be scaled and deployed separately.
    

### Types of NFRs

In general, NFRs are quality attributes of the system and are usually the “ity” requirements. Some of them are mentioned before.

1. **Performance**: This refers to how the system responds to a specific workload or user load. Performance requirements can include response time, throughput, and resource utilization.
    
2. **Scalability**: This refers to the system's ability to handle an increasing amount of work or users without affecting its performance. Scalability requirements can include horizontal scalability, vertical scalability, and load balancing.
    
3. **Reliability**: This refers to the system's ability to function correctly and without failure over time. Reliability requirements can include fault tolerance, disaster recovery, and backup and recovery.
    
4. **Security**: This refers to the system's ability to protect against unauthorised access, data theft, and other security threats. Security requirements can include authentication, access control, encryption, and compliance with industry standards.
    
5. **Usability**: This refers to how easy the system is to use and how well it meets user needs. Usability requirements can include accessibility, responsiveness, and user interface design.
    
6. **Maintainability**: This refers to how easy it is to maintain and update the system over time. Maintainability requirements can include modularity, documentation, and code quality.
    
7. **Interoperability**: This refers to the system's ability to interact with other systems and applications. Interoperability requirements can include support for industry standards and protocols, data exchange formats, and integration with third-party systems.
    
8. **Compatibility**: This refers to the system's ability to work with different hardware, software, and network environments. Compatibility requirements can include support for different operating systems, browsers, databases, and other software components.
    
9. **Availability**: This refers to the system's ability to be accessible and operational when required. Availability requirements can include uptime, downtime, and recovery time objectives.
    
10. **Capacity**: This refers to the system's ability to handle a specific volume of data or transactions. Capacity requirements can include data storage, processing power, and network bandwidth.
    
11. **Compliance**: This refers to the system's ability to meet legal, regulatory, and industry standards. Compliance requirements can include data privacy, security regulations, accessibility standards, and industry-specific regulations.
    
12. **Performance efficiency**: This refers to the system's ability to achieve performance objectives with minimal resource consumption. Performance efficiency requirements can include energy efficiency, resource utilization, and optimization of memory and processing power.
    
13. **Testability**: This refers to how easy it is to test the system and validate its functionality. Testability requirements can include support for automated testing, test data management, and traceability of test results.
    

The list can be further extended, but this is a good starting point for evaluation of NFRs.

### How to Prioritise NFRs?

Prioritising non-functional requirements (NFRs) is critical to the success of software development projects. Here are some common prioritisation techniques for NFRs:

1. **MoSCoW method**: This technique involves dividing NFRs into four categories: Must have, Should have, Could have, and Won't have. The must-have requirements are the most critical, while the won't-have requirements are the least important.
    
2. **Cost-benefit analysis**: This technique involves assessing the cost of implementing an NFR against its benefits. NFRs with the highest benefits and lowest costs are given a higher priority.
    
3. **Risk-based prioritisation**: This technique involves identifying the potential risks associated with each NFR and prioritizing them based on their impact on the system's performance, reliability, and security.
    
4. **User-based prioritisation**: This technique involves prioritizing NFRs based on user needs and preferences. User feedback and surveys can help identify the most critical NFRs from a user's perspective.
    
5. **Impact mapping**: This technique involves mapping NFRs to the system's goals and objectives. NFRs that have a more significant impact on achieving the system's goals are given a higher priority.
    
6. **Kano model**: This technique involves categorising NFRs into three categories: must-haves, performance, and delighters. Must-haves are essential requirements, performance requirements are expected by users, and delighters are features that exceed user expectations.
    
7. **Planning poker**: This technique involves a collaborative effort where development team members discuss and estimate the priority of each NFR. This technique can help achieve consensus and ensure that.
    

In conclusion, prioritisation of NFRs is a critical activity in software development. By using techniques such as MoSCoW, AHP, Cost-Benefit Analysis, Risk-Based Prioritisation, Agile Prioritisation, and Kano Model, software developers can ensure that the most critical requirements are met, and resources are allocated effectively to achieve the desired system performance, reliability, and user satisfaction.

## Summary

"Deep Dive into Architecture Patterns, Part 1" is a comprehensive guide that delves into the world of architecture patterns. Architecture patterns provide reusable solutions to common design problems, serving as a blueprint for structuring and organising software systems and their components. The post emphasises understanding the functional and non-functional requirements when selecting the appropriate architecture pattern for a system.

Functional requirements define what the system should do, such as the features it must provide and the tasks it must perform. These requirements can help determine the appropriate architecture pattern. For example, a workflow-driven architecture pattern is more suitable for systems that handle complex business workflows and data processing. On the other hand, a layered architecture pattern may be more appropriate for systems that support multiple user interfaces.

Non-functional requirements, such as performance, security, reliability, and scalability, determine how well the system performs its tasks and how easy it is to use and maintain. A distributed architecture pattern, such as a microservices' architecture, may be more suitable for systems that require high-performance and scalability. A layered architecture pattern with a clear separation of concerns may be more appropriate for highly secure systems. The post also discusses the types of NFRs, such as performance, security, and maintainability.

The post concludes that selecting the appropriate architecture pattern requires careful analysis of the system's functional and non-functional requirements to ensure that it is scalable, maintainable, and extensible. Other factors such as technology stack, domain complexity, and team capability can also influence the pattern selection. This informative guide is a must-read for developers, architects, and software engineers who are keen to learn more about architecture patterns and their impact on software design.

## References

* \[[https://akfpartners.com/growth-blog/the-problem-with-non-functional-requirements](https://akfpartners.com/growth-blog/the-problem-with-non-functional-requirements)\]
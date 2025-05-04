# Software Requirements Specification
## For Student Club Management System with Budget and Venue Integration

Version 0.1  
Prepared by   
Teow Wei Ting  
Eng Zi Ying  
See Jie Sheng  
Sua Wei Khong  
<organization>  
<date created>  

Table of Contents
=================
* [Revision History](#revision-history)
* 1 [Introduction](#1-introduction)
  * 1.1 [Document Purpose](#11-document-purpose)
  * 1.2 [Product Scope](#12-product-scope)
  * 1.3 [Product overview](#13-product-overview)
    * 1.3.1 [Product Perspective](#131-product-perspective)
    * 1.3.2 [Product Functions](#132-product-functions)
    * 1.3.3 [User Characteristics](#133-user-characteristics)
    * 1.3.4 [Limitations](#134-limitations)
  * 1.4 [Definitions](#14-definitions)
* 2 [References](#2-references)
  * 2.1 [Product Perspective](#21-product-perspective)
  * 2.2 [Product Functions](#22-product-functions)
  * 2.3 [Product Constraints](#23-product-constraints)
  * 2.4 [User Characteristics](#24-user-characteristics)
  * 2.5 [Assumptions and Dependencies](#25-assumptions-and-dependencies)
  * 2.6 [Apportioning of Requirements](#26-apportioning-of-requirements)
* 3 [Requirements](#3-requirements)
  * 3.1 [Product Functions](#31-product-functions)
    * 3.1.1 [User Interfaces](#311-user-interfaces)
    * 3.1.2 [Hardware Interfaces](#312-hardware-interfaces)
    * 3.1.3 [Software Interfaces](#313-software-interfaces)
  * 3.2 [Performance Requirements](#32-performance-requirements)
  * 3.3 [Usability Requirements](#33-usability-requirements)
    * 3.3.1 [Performance](#331-performance)
    * 3.3.2 [Security](#332-security)
    * 3.3.3 [Reliability](#333-reliability)
    * 3.3.4 [Availability](#334-availability)
  * 3.4 [Interface Requirements](#34-interface-requirements)
  * 3.5 [Logical Datacse Requirements](#35-logical-database-requirements)
    * 3.5.1 [Installation](#351-installation)
    * 3.5.2 [Distribution](#352-distribution)
    * 3.5.3 [Maintainability](#353-maintainability)
    * 3.5.4 [Reusability](#354-reusability)
    * 3.5.5 [Portability](#355-portability)
    * 3.5.6 [Cost](#356-cost)
    * 3.5.7 [Deadline](#357-deadline)
    * 3.5.8 [Proof of Concept](#358-proof-of-concept)
   * 3.6 [Design Constraints](#36-design-constraints)
   * 3.7 [Software System Attributes](#37-software-system-attributes)
* 4 [Verification](#4-verification)
* 5 [Appendixes](#5-appendixes)

## Revision History
| Name | Date    | Reason For Changes  | Version   |
| ---- | ------- | ------------------- | --------- |
|      |         |                     |           |
|      |         |                     |           |
|      |         |                     |           |

## 1. Introduction
> This section should provide an overview of the entire document

### 1.1 Document Purpose
Describe the purpose of the SRS and its intended audience.

### 1.2 Product Scope
Identify the product whose software requirements are specified in this document, including the revision or release number. Explain what the product that is covered by this SRS will do, particularly if this SRS describes only part of the system or a single subsystem. Provide a short description of the software being specified and its purpose, including relevant benefits, objectives, and goals. Relate the software to corporate goals or business strategies. If a separate vision and scope document is available, refer to it rather than duplicating its contents here.

### 1.3 Product Overview
#### 1.3.4 Limitations
1. Scope of Features: The system gives priority to essential features including user identification, club management, event scheduling, and budget approval workflows because of its short development period—one academic semester. Intelligent budget optimization tools, machine learning for event recommendations, and comprehensive analytics dashboards are examples of advanced technologies that have been left out. Although this choice guarantees on-time delivery, it restricts future-proofing and intelligent capabilities.

2. Budget Constraints: The development is limited to open-source and free tools like Bootstrap/Tailwind CSS, Django, and PostgreSQL.  Funding is not available for enterprise services, premium plugins, or commercial APIs.  Options like premium alerting systems, powerful cloud services, or complex calendar integrations are thus not available.  This could restrict performance improvements, scalability, and some user conveniences.

User Base Access: The application only supports authenticated users from the university domain. Students, club directors and administrators are all included in this. Even if they participate in club activities, guest users, alumni, and outside collaborators are unable to use the portal. This restricts collaborations and community outreach that could improve club involvement.

Internet Dependency: Since the program is web-based and hosted on-campus or on a cloud server, users need to have a steady and reliable internet connection. As a result, tasks like creating an event, submitting a budget, or editing a profile cannot be completed without an offline connection. This might be problematic in isolated locations or when there are network failures.

Mobile Limitations: Even though the system has responsive design support for mobile use on tablets and smartphones, it is not a native smartphone application. Its performance might be slower, and the loading process could be slower compared to the totally optimized smartphone applications. Further, mobile-related features like native calendar syncing, push notifications, or biometric login are unsupported.

Technical Integration: All integrations must comply with university IT policy and security procedures. For example, Single Sign-On (SSO) integration must integrate via OAuth2 or LDAP, and external APIs like Google Calendar must comply with campus data governance. That constrains integration flexibility with third-party applications and will prevent or delay some features when APIs do not fit institution criteria.

Resource Availability: The project is largely sustained and created by student, who may possess varying availability and technical abilities. This can cause delayed fixes of bugs, decreased testing coverage, and uneven development cycles. Feature requests or enhancements may be postponed due to school responsibilities.

Hosting Environment: The deployment must take place on Linux-based servers from the institution or authorized cloud infrastructure.  This limits the use of some server technologies (like Windows hosting) and the potential for deployment automation.  Creating environments with restricted access or compliance requirements can also present administrative challenges for developers.

#### 1.3.4 Definitions
| **Term**                  | **Definition**                                                                                                                                       |
|---------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Application**           | The web-based Club and Event Management System designed to support university students and staff in organizing, managing, and approving club events. |
| **User**                  | Any individual interacting with the system, including students, club leaders, faculty advisors, and administrators.                                 |
| **Club Leader**           | A student with administrative rights over a club, responsible for event planning, budget submission, and activity management.                        |
| **Administrator**         | A university staff user with full access to manage clubs, events, budgets, and system-wide settings.                                                 |
| **Event Proposal**        | A structured digital request submitted by a club leader to organize an event, including logistics and financial needs.                              |
| **Budget Approval Workflow** | A step-by-step process for reviewing and approving club-submitted budgets before funds are allocated.                                                 |
| **Single Sign-On (SSO)**  | A secure login method allowing users to access the system using existing university credentials.                                                     |
| **Dashboard**             | The main interface displaying a summary of club activities, pending tasks, and budget status for the user.                                           |
| **Responsive Design**     | UI/UX design approach ensuring the application functions well on desktops, tablets, and smartphones.                                                 |
| **Django**                | A high-level, open-source Python web framework used to build the backend of the application.                                                         |
| **PostgreSQL**            | An open-source relational database management system used to store and retrieve the application's data.                                              |
| **API (Application Programming Interface)** | A set of protocols that allow software components to communicate, such as with Google Calendar or email notifications.                      |
| **Open Source**           | Software with publicly accessible code that can be freely used, modified, and distributed.                                                           |
| **Authentication**        | The process of verifying a user’s identity through credentials like usernames and passwords.                                                         |
| **Authorization**         | The process of granting a user specific system permissions based on their role (e.g., student, advisor, admin).                                     |
| **Hosting Server**        | The server environment where the system is deployed, typically a Linux-based or cloud infrastructure approved by the university.                     |

### 1.4 References
List any other documents or Web addresses to which this SRS refers. These may include user interface style guides, contracts, standards, system requirements specifications, use case documents, or a vision and scope document. Provide enough information so that the reader could access a copy of each reference, including title, author, version number, date, and source or location.

### 1.5 Document Overview
Describe what the rest of the document contains and how it is organized.

## 2. Product Overview
> This section should describe the general factors that affect the product and its requirements. This section does not state specific requirements. Instead, it provides a background for those requirements, which are defined in detail in Section 3, and makes them easier to understand.

### 2.1 Product Perspective
Describe the context and origin of the product being specified in this SRS. For example, state whether this product is a follow-on member of a product family, a replacement for certain existing systems, or a new, self-contained product. If the SRS defines a component of a larger system, relate the requirements of the larger system to the functionality of this software and identify interfaces between the two. A simple diagram that shows the major components of the overall system, subsystem interconnections, and external interfaces can be helpful.

### 2.2 Product Functions
Summarize the major functions the product must perform or must let the user perform. Details will be provided in Section 3, so only a high level summary (such as a bullet list) is needed here. Organize the functions to make them understandable to any reader of the SRS. A picture of the major groups of related requirements and how they relate, such as a top level data flow diagram or object class diagram, is often effective.

### 2.3 Product Constraints
This subsection should provide a general description of any other items that will limit the developer’s options. These may include:  

* Interfaces to users, other applications or hardware.  
* Quality of service constraints.  
* Standards compliance.  
* Constraints around design or implementation.

### 2.4 User Characteristics
Identify the various user classes that you anticipate will use this product. User classes may be differentiated based on frequency of use, subset of product functions used, technical expertise, security or privilege levels, educational level, or experience. Describe the pertinent characteristics of each user class. Certain requirements may pertain only to certain user classes. Distinguish the most important user classes for this product from those who are less important to satisfy.

### 2.5 Assumptions and Dependencies
List any assumed factors (as opposed to known facts) that could affect the requirements stated in the SRS. These could include third-party or commercial components that you plan to use, issues around the development or operating environment, or constraints. The project could be affected if these assumptions are incorrect, are not shared, or change. Also identify any dependencies the project has on external factors, such as software components that you intend to reuse from another project, unless they are already documented elsewhere (for example, in the vision and scope document or the project plan).

### 2.6 Apportioning of Requirements
Apportion the software requirements to software elements. For requirements that will require implementation over multiple software elements, or when allocation to a software element is initially undefined, this should be so stated. A cross reference table by function and software element should be used to summarize the apportioning.

Identify requirements that may be delayed until future versions of the system (e.g., blocks and/or increments).

## 3. Requirements
> This section specifies the software product's requirements. Specify all of the software requirements to a level of detail sufficient to enable designers to design a software system to satisfy those requirements, and to enable testers to test that the software system satisfies those requirements.

> The specific requirements should:
* Be uniquely identifiable.
* State the subject of the requirement (e.g., system, software, etc.) and what shall be done.
* Optionally state the conditions and constraints, if any.
* Describe every input (stimulus) into the software system, every output (response) from the software system, and all functions performed by the software system in response to an input or in support of an output.
* Be verifiable (e.g., the requirement realization can be proven to the customer's satisfaction)
* Conform to agreed upon syntax, keywords, and terms.

### 3.1 External Interfaces
> This subsection defines all the inputs into and outputs requirements of the software system. Each interface defined may include the following content:
* Name of item
* Source of input or destination of output
* Valid range, accuracy, and/or tolerance
* Units of measure
* Timing
* Relationships to other inputs/outputs
* Screen formats/organization
* Window formats/organization
* Data formats
* Command formats
* End messages

#### 3.1.1 User interfaces
Define the software components for which a user interface is needed. Describe the logical characteristics of each interface between the software product and the users. This may include sample screen images, any GUI standards or product family style guides that are to be followed, screen layout constraints, standard buttons and functions (e.g., help) that will appear on every screen, keyboard shortcuts, error message display standards, and so on. Details of the user interface design should be documented in a separate user interface specification.

Could be further divided into Usability and Convenience requirements.

#### 3.1.2 Hardware interfaces
Describe the logical and physical characteristics of each interface between the software product and the hardware components of the system. This may include the supported device types, the nature of the data and control interactions between the software and the hardware, and communication protocols to be used.

#### 3.1.3 Software interfaces
Describe the connections between this product and other specific software components (name and version), including databases, operating systems, tools, libraries, and integrated commercial components. Identify the data items or messages coming into the system and going out and describe the purpose of each. Describe the services needed and the nature of communications. Refer to documents that describe detailed application programming interface protocols. Identify data that will be shared across software components. If the data sharing mechanism must be implemented in a specific way (for example, use of a global data area in a multitasking operating system), specify this as an implementation constraint.

### 3.2 Functional
> This section specifies the requirements of functional effects that the software-to-be is to have on its environment.

### 3.3 Quality of Service
> This section states additional, quality-related property requirements that the functional effects of the software should present.

#### 3.3.1 Performance
If there are performance requirements for the product under various circumstances, state them here and explain their rationale, to help the developers understand the intent and make suitable design choices. Specify the timing relationships for real time systems. Make such requirements as specific as possible. You may need to state performance requirements for individual functional requirements or features.

#### 3.3.2 Security
Specify any requirements regarding security or privacy issues surrounding use of the product or protection of the data used or created by the product. Define any user identity authentication requirements. Refer to any external policies or regulations containing security issues that affect the product. Define any security or privacy certifications that must be satisfied.

#### 3.3.3 Reliability
Specify the factors required to establish the required reliability of the software system at time of delivery.

#### 3.3.4 Availability
Specify the factors required to guarantee a defined availability level for the entire system such as checkpoint, recovery, and restart.

### 3.4 Compliance
Specify the requirements derived from existing standards or regulations, including:  
* Report format
* Data naming
* Accounting procedures
* Audit tracing

For example, this could specify the requirement for software to trace processing activity. Such traces are needed for some applications to meet minimum regulatory or financial standards. An audit trace requirement may, for example, state that all changes to a payroll database shall be recorded in a trace file with before and after values.

### 3.5 Design and Implementation

#### 3.5.1 Installation
Constraints to ensure that the software-to-be will run smoothly on the target implementation platform.

#### 3.5.2 Distribution
Constraints on software components to fit the geographically distributed structure of the host organization, the distribution of data to be processed, or the distribution of devices to be controlled.

#### 3.5.3 Maintainability
Specify attributes of software that relate to the ease of maintenance of the software itself. These may include requirements for certain modularity, interfaces, or complexity limitation. Requirements should not be placed here just because they are thought to be good design practices.

#### 3.5.4 Reusability
<!-- TODO: come up with a description -->

#### 3.5.5 Portability
Specify attributes of software that relate to the ease of porting the software to other host machines and/or operating systems.

#### 3.5.6 Cost
Specify monetary cost of the software product.

#### 3.5.7 Deadline
Specify schedule for delivery of the software product.

#### 3.5.8 Proof of Concept
<!-- TODO: come up with a description -->

## 4. Verification
> This section provides the verification approaches and methods planned to qualify the software. The information items for verification are recommended to be given in a parallel manner with the requirement items in Section 3. The purpose of the verification process is to provide objective evidence that a system or system element fulfills its specified requirements and characteristics.

<!-- TODO: give more guidance, similar to section 3 -->
<!-- ieee 15288:2015 -->

## 5. Appendixes

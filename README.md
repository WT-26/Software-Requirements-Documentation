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
     * 3.1.1 [Register User](#311-register-user)
     * 3.1.2 [Login User](#312-login-user)
     * 3.1.3 [Log out User](#313-log-out-user)
     * 3.1.4 [Reset Password](#314-reset-password)
     * 3.1.5 [Update Profile](#315-update-profile)
     * 3.1.6 [Change Role](#316-change-role)
     * 3.1.7 [Request Create Club](#317-request-create-club)
     * 3.1.8 [Club Approval](#318-club-approval)
     * 3.1.9 [Create Club](#319-create-club)
     * 3.1.19 [Approve Event](#3119-approve-event)
     * 3.1.20 [Request Venue](#3120-request-venue)
     * 3.1.21 [Approve Venue Request](#3121-approve-venue-request)
     * 3.1.22 [View Calendar](#3122-view-calendar)
     * 3.1.23 [Submit Budget Request](#3123-submit-budget-request)
     * 3.1.24 [Approve Budget](#3124-approve-budget)
     * 3.1.25 [View Club Budget](#3125-view-club-budget)
     * 3.1.26 [Generate Financial Report](#3126-generate-financial-report)
     * 3.1.27 [Send Announcement](#3127-send-announcement)
     * 3.1.28 [Notify User](#3128-notify-user)
     * 3.1.29 [View All Clubs](#3129-view-all-user)
     * 3.1.30 [Generate System Report](#3130-generate-system-report)
     * 3.1.31 [Search Clubs](#3131-search-clubs)
     * 3.1.32 [Filter Events](#3132-filter-events)
     * 3.1.33 [Sort Budget Requests](#3133-sort-budget-requests)
     * 3.1.34 [Log Activity](#3134-log-activity)
     * 3.1.35 [View Audit Log](#3135-view-audit-log)
     * 3.1.36 [Set Permissions](#3136-set-permissions)
  * 3.2 [Performance Requirements](#32-performance-requirements)
  * 3.3 [Usability Requirements](#33-usability-requirements)
    * 3.3.1 [Performance](#331-performance)
    * 3.3.2 [Security](#332-security)
    * 3.3.3 [Reliability](#333-reliability)
    * 3.3.4 [Availability](#334-availability)
  * 3.4 [Interface Requirements](#34-interface-requirements)
    * 3.4.1 [User Interfaces](#341-user-interfaces)
    * 3.4.2 [Hardware Interfaces](#342-hardware-interfaces)
    * 3.4.3 [Software Interfaces](#343-software-interfaces)
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
The purpose of the "Student Club Management System with Budget and Venue Integration" is to provide a comprehensive digital solution that centralizes and simplifies the management of student clubs within the university. The goal of this system is to solve common problems that student organisations face, like inadequate communication, manual membership and financial tracking, and trouble organising event logistics and venue reservations. The software integrates with current university financial systems and space reservation tools, allowing clubs to manage their budgets, submit funding requests, and reserve spaces with minimal administrative friction. Along with offering a user-friendly interface for students to take part in club activities, attend events, and stay informed, it also promotes transparency in financial management and decision-making processes. Lastly, the system aims to promote a more active and organised student life environment, lessen administrative burdens for university staff and student leaders, and support the development and success of student-driven projects. 

### 1.2 Product Scope
This Software Requirements Specification (SRS) document defines the software requirements for the Student Club Management System with Budget and Venue Integration, Release 1.0. The system is a centralized web-based platform designed to support and streamline the operations of student clubs within a university setting. It focuses on automating and integrating core club management functions, including member registration, event planning, budget tracking, fund requests, and venue reservations.

The program will enable club leaders to organise club activities efficiently, submit and monitor budget requests in conjunction with the university's financial system, and schedule event spaces via connectivity with the campus venue booking system.  Additionally, it provides members with access to club events and information, encouraging more active participation. While this SRS describes the entire system, future updates could include improved analytics, mobile support, and greater integration capabilities.

The system's primary goals are to eliminate manual administrative work, improve operational transparency, and encourage student participation. This software supports institutional objectives to update student services and increase co-curricular involvement by integrating with the university's overall aims of digital transformation, operational efficiency, and improved student experience.

### 1.3 Product Overview
#### 1.3.2 Product Functions

The following table features an overview of the list of features in the system along with a brief description, categorized by accessible actors.

| **Function ID** | **Function Name**            | **Description**                                                  | **Accessible Actor(s)**                |
|------------------|-------------------------------|------------------------------------------------------------------|----------------------------------------|
| F-001            | User Registration             | Allows users (e.g., students) to register an account             | Student                                |
| F-002            | User Login                    | Authenticates user credentials to access the system              | All users                              |
| F-003            | User Logout                   | Ends the current user session                                    | All users                              |
| F-004            | Password Reset                | Sends reset link and allows users to update password             | All users                              |
| F-005            | Edit Profile                  | Users can update their profile information                       | All users                              |
| F-006            | Role Management               | Allows admins to promote or demote user roles                    | System Admin                           |
| F-007            | Request Club Creation         | Submit a request to form a new club                              | Student                                |
| F-008            | Approve Club Request          | Review and approve club creation requests                        | System Admin                           |
| F-009            | Create Club                   | Create a new club in the system                                  | System Admin                           |
| F-010            | Update Club Details           | Edit information about an existing club                          | President                              |
| F-011            | Delete Club                   | Remove an existing club from the system                          | System Admin                           |
| F-012            | Request Club Membership       | Submit request to join a club                                    | Student                                |
| F-013            | Approve Membership            | Approve membership requests for a club                           | President, System Admin                |
| F-014            | Remove Club Member            | Remove a student from the club                                   | President                              |
| F-015            | View Clubs                    | List and filter clubs based on criteria                          | Student                                |
| F-016            | Propose Event                 | Submit a proposal to organize an event                           | President                              |
| F-017            | Update Event Details          | Modify information about a scheduled event                       | President, Committee                   |
| F-018            | Cancel Event                  | Cancel a planned or ongoing event                                | President                              |
| F-019            | Approve Event                 | Approve or reject proposed events                                | Event Admin                            |
| F-020            | Request Venue Booking         | Submit request for venue use                                     | President                              |
| F-021            | Approve Venue Booking         | Review and approve venue booking requests                        | Event Admin                            |
| F-022            | View Event Calendar           | Browse upcoming and scheduled events                             | All users                              |
| F-023            | Submit Budget Proposal        | Propose a budget for an event or club activity                   | President                              |
| F-024            | Approve Budget Proposal       | Review and approve or reject budget requests                     | Event Admin                            |
| F-025            | View Club Budget              | Monitor club budget, usage history, and balances                 | President, Event Admin                 |
| F-026            | Generate Financial Report     | Produce detailed budget reports in PDF/CSV format                | President, Member, Event Admin         |
| F-027            | Send Announcement             | Notify club members with announcements or updates                | President, Committee                   |
| F-028            | System Notification           | Send alerts or notifications within the system                   | System (automated)                     |
| F-029            | View All Clubs                | View a list of all clubs in the system                           | Event Admin, System Admin              |
| F-030            | Generate System Reports       | Create reports on system usage and activities                    | Event Admin, System Admin              |
| F-031            | Search Clubs                  | Search clubs by name, category, or tags                          | All users                              |
| F-032            | Filter Events                 | Filter events by date, venue, or club                            | All users                              |
| F-033            | Sort Budget Requests          | Organize budget requests based on certain criteria               | Event Admin                            |
| F-034            | Record System Activity        | Automatically log important user/system actions                  | System (automated), Admin              |
| F-035            | View Audit Logs               | Review logged system activities                                  | System Admin                           |
| F-036            | Configure Permissions         | Assign or modify access rights for each user role                | System Admin                           |

---

#### 1.3.3 User Characteristics

The general characteristics of the intended groups of users are as follows:

| **User Group**        | **Expected Role in System**                            | **Educational Level**     | **Technical Expertise**             | **Notes on Usability Needs**                       |
|------------------------|---------------------------------------------------------|----------------------------|--------------------------------------|----------------------------------------------------|
| Students               | Register, join clubs, view events, participate          | Undergraduate/Diploma      | Basic (form filling, navigation)     | Needs intuitive UI, simple navigation              |
| Club Presidents        | Manage clubs, create events, send announcements         | Undergraduate               | Moderate (forms, content editing)    | Require dashboard with clear controls              |
| Committee Members      | Assist presidents, help manage events                   | Undergraduate               | Moderate                             | Similar needs as presidents                        |
| Event Administrators   | Approve events/venues, manage finance requests          | Staff/Faculty               | Moderate to Advanced                 | Require admin panels, data filtering               |
| System Administrators  | Manage roles, security, audit, clubs                    | IT Staff/Admin              | Advanced                             | Need access to logs, system configurations         |

#### 1.3.4 Limitations
1. Scope of Features: The system gives priority to essential features including user identification, club management, event scheduling, and budget approval workflows because of its short development period—one academic semester. Intelligent budget optimization tools, machine learning for event recommendations, and comprehensive analytics dashboards are examples of advanced technologies that have been left out. Although this choice guarantees on-time delivery, it restricts future-proofing and intelligent capabilities.

2. Budget Constraints: The development is limited to open-source and free tools like Bootstrap/Tailwind CSS, Django, and PostgreSQL.  Funding is not available for enterprise services, premium plugins, or commercial APIs.  Options like premium alerting systems, powerful cloud services, or complex calendar integrations are thus not available.  This could restrict performance improvements, scalability, and some user conveniences.

3. User Base Access: The application only supports authenticated users from the university domain. Students, club directors and administrators are all included in this. Even if they participate in club activities, guest users, alumni, and outside collaborators are unable to use the portal. This restricts collaborations and community outreach that could improve club involvement.

4. Internet Dependency: Since the program is web-based and hosted on-campus or on a cloud server, users need to have a steady and reliable internet connection. As a result, tasks like creating an event, submitting a budget, or editing a profile cannot be completed without an offline connection. This might be problematic in isolated locations or when there are network failures.

5. Mobile Limitations: Even though the system has responsive design support for mobile use on tablets and smartphones, it is not a native smartphone application. Its performance might be slower, and the loading process could be slower compared to the totally optimized smartphone applications. Further, mobile-related features like native calendar syncing, push notifications, or biometric login are unsupported.

6. Technical Integration: All integrations must comply with university IT policy and security procedures. For example, Single Sign-On (SSO) integration must integrate via OAuth2 or LDAP, and external APIs like Google Calendar must comply with campus data governance. That constrains integration flexibility with third-party applications and will prevent or delay some features when APIs do not fit institution criteria.

7. Resource Availability: The project is largely sustained and created by student, who may possess varying availability and technical abilities. This can cause delayed fixes of bugs, decreased testing coverage, and uneven development cycles. Feature requests or enhancements may be postponed due to school responsibilities.

8. Hosting Environment: The deployment must take place on Linux-based servers from the institution or authorized cloud infrastructure.  This limits the use of some server technologies (like Windows hosting) and the potential for deployment automation.  Creating environments with restricted access or compliance requirements can also present administrative challenges for developers.

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
1. Chenjeri, A., Sai, Satya, T., Santhan Mourya, K., Murali, K., Muddada, & Student. (2024). Issue 3 www.jetir.org (ISSN-2349-5162). JETIR2403033 Journal of Emerging Technologies and Innovative Research, 11.
2. Et. al., A. A. A. (2021). Design Architecture Of An Integrated Student Activities Management System For Higher Education. Turkish Journal of Computer and Mathematics Education (TURCOMAT), 12(5), 1676–1683. https://doi.org/10.17762/turcomat.v12i5.2158
3. Hariprasad, M., Neha N, Dey, N., Pratiba D, & Ramakanth Kumar P. (2023). College Club Activity Management System. https://doi.org/10.1109/csitss60515.2023.10334208
4. Khatri, I. A., Ghonge, M., Mirajkar, R., Shinde, S., Hon, R., & Yenkikar, A. (2024). Enhancing Campus Engagement with A Secure and Comprehensive Platform for Club Management and Student Participation. 2024 IEEE International Conference on Blockchain and Distributed Systems Security (ICBDS), 1–6. https://doi.org/10.1109/icbds61829.2024.10837416
5. Mukthashree, B., Chinmayee K G, Manjuprasad, B., & Student. (n.d.). Campus Club Management System Application.

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

### 3.1.19 Approve Event

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-EVENT-04                                                                      |
| **Feature**         | Approve Event                                                                |
| **Purpose**         | To allow event administrators to review and approve club event proposals.   |
| **Actors**          | Event Admin                                                                  |
| **Precondition**    | Admin is logged in and event is in a "Pending Approval" status.              |
| **Postcondition**   | Event is marked as approved and scheduled in the system.                     |
| **Main Flow**       | 1. Admin logs in.<br>2. Navigates to event approvals.<br>3. Selects event.<br>4. Reviews details.<br>5. Clicks "Approve".<br>6. System updates status. |
| **Alternate Scenario** | If event details are incomplete, the admin may reject or request revision. |

---

### 3.1.20 Request Venue Booking

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-EVENT-05                                                                     |
| **Feature**         | Request Venue Booking                                                        |
| **Purpose**         | To allow club presidents to request available venues for events.             |
| **Actors**          | President                                                                    |
| **Precondition**    | Event must be created; president must be authenticated.                      |
| **Postcondition**   | Venue booking request is submitted and pending admin approval.               |
| **Main Flow**       | 1. President logs in.<br>2. Selects an event.<br>3. Chooses venue and timeslot.<br>4. Submits request.<br>5. System logs request. |
| **Alternate Scenario** | If the venue is unavailable, the system shows a conflict warning.          |

---

### 3.1.21 Approve Venue Request

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-EVENT-06                                                                     |
| **Feature**         | Approve Venue Request                                                        |
| **Purpose**         | To enable event admins to approve or reject venue booking requests.          |
| **Actors**          | Event Admin                                                                  |
| **Precondition**    | Venue request exists and admin is logged in.                                 |
| **Postcondition**   | Booking status is updated and the venue is reserved.                         |
| **Main Flow**       | 1. Admin logs in.<br>2. Views pending venue requests.<br>3. Reviews request.<br>4. Clicks "Approve".<br>5. System updates status. |
| **Alternate Scenario** | If schedule conflict exists, admin rejects with comments.                 |

---

### 3.1.22 View Event Calendar

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-EVENT-07                                                                 |
| **Feature**         | View Event Calendar                                                          |
| **Purpose**         | To allow users to browse upcoming events on campus or by club.               |
| **Actors**          | Student, President, Committee                                                |
| **Precondition**    | User is logged in.                                                           |
| **Postcondition**   | Events are displayed in calendar format.                                     |
| **Main Flow**       | 1. User logs in.<br>2. Navigates to event calendar.<br>3. Optionally filters by club/date.<br>4. Views events. |
| **Alternate Scenario** | If no events are available, display "No events scheduled".               |

---

### 3.1.23 Submit Budget Request

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-01                                                                   |
| **Feature**         | Submit Budget Request                                                        |
| **Purpose**         | To allow presidents to request funds for event or club operation.            |
| **Actors**          | President                                                                    |
| **Precondition**    | Club and event must exist, president is authenticated.                      |
| **Postcondition**   | Budget request is submitted for review.                                      |
| **Main Flow**       | 1. President logs in.<br>2. Navigates to finance section.<br>3. Fills in amount and justification.<br>4. Submits form.<br>5. System logs request. |
| **Alternate Scenario** | If required fields are missing, show error and prompt correction.         |

---

### 3.1.24 Approve Budget Request

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-02                                                                      |
| **Feature**         | Approve Budget Request                                                       |
| **Purpose**         | To enable event admins to approve or reject submitted budget requests.       |
| **Actors**          | Event Admin                                                                  |
| **Precondition**    | Budget request is submitted and pending.                                    |
| **Postcondition**   | Budget request is marked approved or rejected with remarks.                  |
| **Main Flow**       | 1. Admin logs in.<br>2. Opens finance dashboard.<br>3. Selects request.<br>4. Reviews.<br>5. Approves or rejects. |
| **Alternate Scenario** | If data is unclear, admin may request clarification from club.           |

---

### 3.1.25 View Club Budget

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-03                                                                     |
| **Feature**         | View Club Budget                                                             |
| **Purpose**         | To allow clubs and admins to monitor financial balance and transaction logs. |
| **Actors**          | President, Event Admin                                                       |
| **Precondition**    | User is authenticated and authorized.                                       |
| **Postcondition**   | Budget data is displayed.                                                    |
| **Main Flow**       | 1. User logs in.<br>2. Navigates to budget section.<br>3. Views summary and breakdown. |
| **Alternate Scenario** | If no data, show “No transactions available”.                            |

---

### 3.1.26 Generate Financial Report

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-04                                                                      |
| **Feature**         | Generate Financial Report                                                    |
| **Purpose**         | To generate downloadable reports of club financial activity.                 |
| **Actors**          | Member, President, Event Admin                                               |
| **Precondition**    | Club exists, user is authorized.                                            |
| **Postcondition**   | Report file (PDF/CSV) is generated and downloadable.                         |
| **Main Flow**       | 1. User logs in.<br>2. Goes to report section.<br>3. Selects club and time period.<br>4. Clicks generate.<br>5. System provides file. |
| **Alternate Scenario** | If no financial data for the period, show a message and skip file generation. |

---

### 3.1.27 Send Club Announcement

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-COMM-01                                                                   |
| **Feature**         | Send Club Announcement                                                       |
| **Purpose**         | To allow club leaders to notify members of updates or events.                |
| **Actors**          | President, Committee                                                         |
| **Precondition**    | User is authorized and part of the club committee.                           |
| **Postcondition**   | Message is delivered to all members via system notification or email.        |
| **Main Flow**       | 1. President/committee logs in.<br>2. Opens communication panel.<br>3. Composes message.<br>4. Sends to club. |
| **Alternate Scenario** | If no members exist, system warns “No recipients available”.              |


### 3.1.28 Notify User
| **Field**          | **Description**                                                                                                                                       |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-COMM-02                                                                                                                                            |
| **Feature**        | Communication & Notifications                                                                                                                         |
| **Purpose**        | To send automated system notifications to specific users when key events occur (e.g., approval, update, rejection).                                  |
| **Actors**         | - System (automated trigger)<br>- System Admin (for monitoring and config)                                                                            |
| **Precondition**   | - User exists in the system<br>- User is active and eligible to receive notifications<br>- System services are operational                            |
| **Postcondition**  | - Notification is stored in the system<br>- User is alerted through UI/email/push depending on configuration                                          |
| **Main Flow**      | 1. System detects event requiring notification<br>2. Calls `notify_user(user_id, message, type)`<br>3. Validates user ID and type<br>4. Logs message<br>5. Sends via configured channel (dashboard/email/push) |
| **Alternate Flow** | - A1: Invalid user ID → Log error, skip notification<br>- A2: Notification service down → Retry or store as unsent<br>- A3: Invalid type → Use default type (e.g., "info") |

### 3.1.29 View All Clubs
| **Field**          | **Description**                                                                                                                                             |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-CLUB-01                                                                                                                                                  |
| **Feature**        | Club Management                                                                                                                                            |
| **Purpose**        | To allow system and event administrators to view a list of all registered clubs in the system.                                                              |
| **Actors**         | - Event Admin<br>- System Admin                                                                                                                             |
| **Precondition**   | - Admin user is authenticated<br>- User has appropriate admin privileges (event or system admin)<br>- Clubs exist in the system                            |
| **Postcondition**  | - List of all clubs is displayed to the admin<br>- Admin can access club details for further actions (edit, review, approve, etc.)                         |
| **Main Flow**      | 1. Admin logs into the system<br>2. Navigates to the club management section<br>3. System calls `view_all_clubs()`<br>4. System retrieves and displays club list |
| **Alternate Flow** | - A1: No clubs are registered → Show message: "No clubs found"<br>- A2: Database error → Show error message and log issue                                   |

### 3.1.30 Generate System Report
## 📊 Use Case: generate_system_report()

| **Field**          | **Description**                                                                                                                                                      |
|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-REPORT-01                                                                                                                                                         |
| **Feature**        | Reporting & Analytics                                                                                                                                                |
| **Purpose**        | To allow admins to generate system-wide reports covering usage statistics, club activity, and budget performance.                                                    |
| **Actors**         | - Event Admin<br>- System Admin                                                                                                                                      |
| **Precondition**   | - Admin is authenticated and authorized<br>- Relevant data (usage logs, club activity, budgets) exist in the system                                                  |
| **Postcondition**  | - A report is generated and displayed or downloaded<br>- May be stored for historical reference                                                                      |
| **Main Flow**      | 1. Admin accesses the report section<br>2. Clicks “Generate Report”<br>3. System compiles data: usage logs, club activities, budget stats<br>4. Report is displayed or exported |
| **Alternate Flow** | - A1: No data available → Show message: “No data to report”<br>- A2: Report generation fails due to server error → Show error message and log the issue              |

### 3.1.31 Search Clubs
| **Field**          | **Description**                                                                                                                                                 |
|--------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-SEARCH-01                                                                                                                                                      |
| **Feature**        | Club Discovery / Search                                                                                                                                         |
| **Purpose**        | To allow all users to search for clubs using keywords that match names, categories, or tags.                                                                    |
| **Actors**         | - All users (guests, students, admins)                                                                                                                           |
| **Precondition**   | - Clubs exist in the system<br>- User has access to the search interface (public or authenticated view)                                                         |
| **Postcondition**  | - A filtered list of clubs matching the keyword is shown<br>- User can view details or take further action (e.g., request to join, view events)                |
| **Main Flow**      | 1. User enters a keyword into the search bar<br>2. System calls `search_clubs(keyword)`<br>3. Matches club name, category, and tags<br>4. Displays results list |
| **Alternate Flow** | - A1: No matches found → Show message: “No clubs found for that keyword”<br>- A2: Search service down → Show error and log issue                                |

### 3.1.32 Filter Events

| **Field**          | **Description**                                                                                                                                                       |
|--------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-SEARCH-02                                                                                                                                                           |
| **Feature**        | Event Discovery / Filtering                                                                                                                                           |
| **Purpose**        | To allow users to filter upcoming events based on selected criteria such as date, venue, or hosting club.                                                             |
| **Actors**         | - All users (guests, students, admins)                                                                                                                                |
| **Precondition**   | - Events are available in the system<br>- User is on the event listing page or has access to filters                                                                  |
| **Postcondition**  | - A filtered list of events is displayed to the user based on chosen criteria                                                                                         |
| **Main Flow**      | 1. User selects filters: date, venue, or club<br>2. System calls `filter_events(date, venue, club)`<br>3. Events matching the criteria are retrieved<br>4. Results are displayed |
| **Alternate Flow** | - A1: No events match criteria → Show message: “No events found”<br>- A2: Filtering input is invalid → Show validation error or fallback to default view              |

### 3.1.33 Sort Budget Requests
| **Field**        | **Details**                                                                 |
|------------------|------------------------------------------------------------------------------|
| **ID**           | UC-SEARCH-03                                                                    |
| **Feature**      | sort_budget_requests(by='date')                                              |
| **Purpose**      | To allow event admins to organize and view budget requests by a chosen field (e.g., date, amount) for easier processing and review. |
| **Actors**       | Event Admin                                                                  |
| **Precondition** | Event admin is authenticated and has access to the budget management dashboard. |
| **Postcondition**| Budget requests are displayed in sorted order according to the specified field (default: date). |
| **Main Flow**    | 1. Event admin logs in.  <br> 2. Navigates to the budget requests section. <br> 3. Chooses a sort parameter (e.g., date). <br> 4. System retrieves and displays sorted requests. |
| **Alternate Scenario** | If no sort parameter is provided, the system defaults to sorting by date. If no budget requests exist, an empty list is shown. |

### 3.1.34 Log Activities
| **Field**         | **Details**                                                                 |
|-------------------|------------------------------------------------------------------------------|
| **ID**            | UC-AUDIT-01                                                                      |
| **Feature**       | log_activity(user_id, action)                                                |
| **Purpose**       | To automatically track and record significant actions performed by users in the system for audit and security purposes. |
| **Actors**        | System (automated), System Admin (viewer)                                    |
| **Precondition**  | A user performs an action that is deemed auditable (e.g., login, budget approval). |
| **Postcondition** | A log entry is stored in the audit trail with the user ID, action details, and timestamp. |
| **Main Flow**     | 1. User performs a key action in the system. <br> 2. System captures user ID and action. <br> 3. System records the activity in the audit log automatically. |
| **Alternate Scenario** | If logging fails due to a system error, the system retries or reports the failure to the system admin. |

### 3.1.35 View Audit Log
| **Field**         | **Details**                                                                 |
|-------------------|------------------------------------------------------------------------------|
| **ID**            | UC-AUDIT-02                                                                     |
| **Feature**       | view_audit_log()                                                             |
| **Purpose**       | To allow system administrators to access and review system activity logs for monitoring, security audits, and issue investigation. |
| **Actors**        | System Admin                                                                 |
| **Precondition**  | Admin is authenticated and has appropriate permissions to access system logs. |
| **Postcondition** | The system displays a list of recorded user activities with details such as user ID, action, and timestamp. |
| **Main Flow**     | 1. Admin logs in to the system. <br> 2. Navigates to the audit log section. <br> 3. System retrieves and displays activity logs. |
| **Alternate Scenario** | If no logs are available, a message is shown indicating “No audit logs found.” If access is unauthorized, an error message is displayed. |

### 3.1.36 Set Permissions
| **Field**         | **Details**                                                                 |
|-------------------|------------------------------------------------------------------------------|
| **ID**            | UC-AUDIT-03                                                                        |
| **Feature**       | set_permissions(role, permissions)                                           |
| **Purpose**       | To allow system administrators to define or update the actions that each user role is authorized to perform within the system. |
| **Actors**        | System Admin                                                                 |
| **Precondition**  | Admin is authenticated and has access to the role management module.         |
| **Postcondition** | Permissions for the specified role are updated and enforced across the system. |
| **Main Flow**     | 1. Admin logs in. <br> 2. Navigates to the role/permission settings. <br> 3. Selects a role. <br> 4. Assigns or updates permissions. <br> 5. System saves the changes. |
| **Alternate Scenario** | If an invalid role is specified, an error message is shown. If no permissions are selected, the system prompts the admin to select at least one. |

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

### 3.4 Interface Requirements

### 3.4.1 External Interfaces
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

#### 3.4.1 User interfaces
Define the software components for which a user interface is needed. Describe the logical characteristics of each interface between the software product and the users. This may include sample screen images, any GUI standards or product family style guides that are to be followed, screen layout constraints, standard buttons and functions (e.g., help) that will appear on every screen, keyboard shortcuts, error message display standards, and so on. Details of the user interface design should be documented in a separate user interface specification.

Could be further divided into Usability and Convenience requirements.

#### 3.4.2 Hardware interfaces
Describe the logical and physical characteristics of each interface between the software product and the hardware components of the system. This may include the supported device types, the nature of the data and control interactions between the software and the hardware, and communication protocols to be used.

#### 3.4.3 Software interfaces
Describe the connections between this product and other specific software components (name and version), including databases, operating systems, tools, libraries, and integrated commercial components. Identify the data items or messages coming into the system and going out and describe the purpose of each. Describe the services needed and the nature of communications. Refer to documents that describe detailed application programming interface protocols. Identify data that will be shared across software components. If the data sharing mechanism must be implemented in a specific way (for example, use of a global data area in a multitasking operating system), specify this as an implementation constraint.

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

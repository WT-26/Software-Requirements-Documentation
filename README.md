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
  * 1.1 [Purpose](#11-purpose)
  * 1.2 [Scope](#12-scope)
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
     * 3.1.5 [View Profile](#315-view-profile)
     * 3.1.6 [Update Profile](#316-update-profile)
     * 3.1.7 [Request Create Club](#317-request-create-club)
     * 3.1.8 [Club Approval](#318-club-approval)
     * 3.1.9 
     * 3.1.19 [Approve Event Request](#3119-approve-event-request)
     * 3.1.20 [Request Venue Booking](#3120-request-venue-booking)
     * 3.1.21 [Approve Venue Request](#3121-approve-venue-request)
     * 3.1.22 [View Event Calendar](#3122-view-event-calendar)
     * 3.1.23 [Submit Budget Proposal](#3123-submit-budget-proposal)
     * 3.1.24 [Approve Budget Proposal](#3124-approve-budget-proposal)
     * 3.1.25 [View Club Budget](#3125-view-club-budget)
     * 3.1.26 [Generate Financial Report](#3126-generate-financial-report)
     * 3.1.27 [View Financial Report](#3127-view-financial-report)
     * 3.1.28 [Send club Announcement](#3128-send-club-announcement)
     * 3.1.29 [Notify User](#3129-notify-user)
     * 3.1.30 [View All Club](#3130-view-all-user)
     * 3.1.31 [Search Club](#3131-search-club)
     * 3.1.32 [Filter Event](#3132-filter-event)
     * 3.1.33 [Filter Budget Request](#3133-filter-budget-request)
     * 3.1.34 [Log Activity](#3134-log-activity)
     * 3.1.35 [View Audit Log](#3135-view-audit-log)
     * 3.1.36 [Set Permission](#3136-set-permission)
     * 3.1.37 [Generate Venue Status](#3137-generate-venue-status).
     * 3.1.38 [View Venue Status](#3138-view-venue-status).
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
     * 3.6.1 [External Standards and Regulatory Requirements](#361-external-standards-and-regulatory-requirements)
     * 3.6.2 [Project Limitations](#362-project-limitations).
     * 3.6.3 [Technical Constraints](#363-technical-constraints).
     * 3.6.4 [Platform Constraints](#364-platform-constraints).
     * 3.6.5 [Environmental Constraints](#365-environmental-constraints).
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

### 1.1 Purpose
The purpose of the "Student Club Management System with Budget and Venue Integration" is to provide a comprehensive digital solution that centralizes and simplifies the management of student clubs within the university. The goal of this system is to solve common problems that student organisations face, like inadequate communication, manual membership and financial tracking, and trouble organising event logistics and venue reservations. The software integrates with current university financial systems and space reservation tools, allowing clubs to manage their budgets, submit funding requests, and reserve spaces with minimal administrative friction. Along with offering a user-friendly interface for students to take part in club activities, attend events, and stay informed, it also promotes transparency in financial management and decision-making processes. Lastly, the system aims to promote a more active and organised student life environment, lessen administrative burdens for university staff and student leaders, and support the development and success of student-driven projects. 

### 1.2 Scope
This Software Requirements Specification (SRS) document defines the software requirements for the Student Club Management System with Budget and Venue Integration, Release 1.0. The system is a centralized web-based platform designed to support and streamline the operations of student clubs within a university setting. It focuses on automating and integrating core club management functions, including member registration, event planning, budget tracking, fund requests, and venue reservations.

The program will enable club leaders to organise club activities efficiently, submit and monitor budget requests in conjunction with the university's financial system, and schedule event spaces via connectivity with the campus venue booking system.  Additionally, it provides members with access to club events and information, encouraging more active participation. While this SRS describes the entire system, future updates could include improved analytics, mobile support, and greater integration capabilities.

The system's primary goals are to eliminate manual administrative work, improve operational transparency, and encourage student participation. This software supports institutional objectives to update student services and increase co-curricular involvement by integrating with the university's overall aims of digital transformation, operational efficiency, and improved student experience.

### 1.3 Product Overview

#### 1.3.1 Product Perspective
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

### 1.4 Definitions
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

## 2 References
1. Chenjeri, A., Sai, Satya, T., Santhan Mourya, K., Murali, K., Muddada, & Student. (2024). Issue 3 www.jetir.org (ISSN-2349-5162). JETIR2403033 Journal of Emerging Technologies and Innovative Research, 11.
2. Et. al., A. A. A. (2021). Design Architecture Of An Integrated Student Activities Management System For Higher Education. Turkish Journal of Computer and Mathematics Education (TURCOMAT), 12(5), 1676–1683. https://doi.org/10.17762/turcomat.v12i5.2158
3. Hariprasad, M., Neha N, Dey, N., Pratiba D, & Ramakanth Kumar P. (2023). College Club Activity Management System. https://doi.org/10.1109/csitss60515.2023.10334208
4. Khatri, I. A., Ghonge, M., Mirajkar, R., Shinde, S., Hon, R., & Yenkikar, A. (2024). Enhancing Campus Engagement with A Secure and Comprehensive Platform for Club Management and Student Participation. 2024 IEEE International Conference on Blockchain and Distributed Systems Security (ICBDS), 1–6. https://doi.org/10.1109/icbds61829.2024.10837416
5. Mukthashree, B., Chinmayee K G, Manjuprasad, B., & Student. (n.d.). Campus Club Management System Application.

## 3. Requirements
> This section specifies the software product's requirements. Specify all of the software requirements to a level of detail sufficient to enable designers to design a software system to satisfy those requirements, and to enable testers to test that the software system satisfies those requirements.

> The specific requirements should:
* Be uniquely identifiable.
* State the subject of the requirement (e.g., system, software, etc.) and what shall be done.
* Optionally state the conditions and constraints, if any.
* Describe every input (stimulus) into the software system, every output (response) from the software system, and all functions performed by the software system in response to an input or in support of an output.
* Be verifiable (e.g., the requirement realization can be proven to the customer's satisfaction)
* Conform to agreed upon syntax, keywords, and terms.

### 3.1.01 User Registration with Role Selection 

 | **Field**             | **Details**                                                                                                                                                                                                 |
|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**                | UC-USER-01                                                                                                                                                                                                  |
| **Feature**           | User Registration with Role Selection                                                                                                                                                                       |
| **Purpose**           | To register a user and determine their role (Student or President), and ensure appropriate follow-up actions based on the selected role.                                                                    |
| **Actors**            | User (Student/President), Admin, System                                                                                                                                                                     |
| **Precondition**      | - User accesses the registration page.                                                                                                                                                                      |
| **Postcondition**     | - User is registered as Student or President. <br> - Confirmation or notification is sent accordingly.                                                                                                      |
| **Main Flow**         | 1. User accesses the registration page. <br> 2. User fills in details and selects role. <br> 3. If Student is selected: system registers user as Student and sends confirmation. <br> 4. If President is selected: system submits President registration request to Admin. <br> 5. Admin reviews request. <br> 6. If approved, system registers user as President and sends notification. |
| **Alternate Scenario**| - If user selects an invalid role or submits incomplete form, system prompts for correction. <br> - If Admin rejects President request, system does not assign President role; user is notified of rejection. <br> - If confirmation or notification fails, user is registered but unaware until manually informed. |

![Image](https://github.com/user-attachments/assets/8cf05f70-2a53-4944-ba95-d28a41740faa) <br>

*Figure 3.1.01 User Registration with Role Selection* 

---

### 3.1.02 User Login and Role-Based Redirection

| **Field**             | **Details**                                                                                                                                                                                                 |
|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**                | UC-USER-02                                                                                                                                                                                                  |
| **Feature**           | User Login and Role-Based Redirection                                                                                                                                                                       |
| **Purpose**           | To authenticate users and redirect them to the appropriate dashboard based on their role (Student, President, or Admin).                                                                                   |
| **Actors**            | User (Student/President/Admin), System                                                                                                                                                                      |
| **Precondition**      | - User accesses the login page.                                                                                                                                                                             |
| **Postcondition**     | - If login is successful and user role is valid, user is redirected to the correct dashboard. <br> - If invalid, user sees error or is logged out.                                                         |
| **Main Flow**         | 1. User enters username and password. <br> 2. User submits credentials. <br> 3. System checks if credentials are valid. <br> 4. If valid: system retrieves user role. <br> 5. System checks if user role is student, president, or admin. <br> 6. If valid role, system redirects to respective dashboard. |
| **Alternate Scenario**| - If credentials are invalid, show "Invalid Credentials" error message and prompt to try again. <br> - If user role is misconfigured or invalid, show "Invalid user role configuration" and log out user. |

![Image](https://github.com/user-attachments/assets/af42b90b-dfee-413a-84b5-63490e043cd9) <br>

*Figure 3.1.02 User Login and Role-Based Redirection* 

---

### 3.1.03 User Logout Process

| **Field**             | **Details**                                                                                                                                                                                                 |
|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**                | UC-USER-03                                                                                                                                                                                                  |
| **Feature**           | User Logout                                                                                                                                                                                                 |
| **Purpose**           | To log the user out of the system, invalidate the session, clear session data, and redirect them to the login page.                                                                                           |
| **Actors**            | User, System                                                                                                                                                                                                |
| **Precondition**      | - User is logged in.                                                                                                                                                                                         |
| **Postcondition**     | - User session is invalidated. <br> - Session data is cleared. <br> - User is redirected to the login page.                                                                                                 |
| **Main Flow**         | 1. User clicks "Logout" button. <br> 2. System triggers `logout_user()` function. <br> 3. System invalidates the user session. <br> 4. System clears session data. <br> 5. System redirects the user to the login page. |
| **Alternate Scenario**| - If logout fails, show "Logout failed" error message and prompt the user to try again.                                                                                                                      |



*Figure 3.1.03 User Logout Process* 

---

### 3.1.19 Approve Event Request

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-EVENT-04                                                                      |
| **Feature**         | Approve Event                                                                |
| **Purpose**         | To allow event administrator to review and approve club event proposals.   |
| **Actors**          | Admin                                                                 |
| **Precondition**    | Admin is logged in and event is in a "Pending Approval" status.              |
| **Postcondition**   | Event is marked as approved and scheduled in the system.                     |
| **Main Flow**       | 1. Admin logs in.<br>2. Navigates to event approvals.<br>3. View pending event requests <br> 4. Selects event.<br>5. Reviews details.<br>6. Clicks "Approve".<br>7. System updates event status. |
| **Alternate Scenario** | If event details are incomplete, the admin may reject or request revision. |

  ![Image](https://github.com/user-attachments/assets/b4113954-90cf-4078-9a48-76248e21f3d9)<br>
  *Figure 3.1.19 Approve Event Request* 


---

### 3.1.20 Request Venue Booking

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-EVENT-05                                                                     |
| **Feature**         | Request Venue Booking                                                        |
| **Purpose**         | To allow club presidents to request available venues for events.             |
| **Actors**          | President, Campus Space Reservation System (external)                        |
| **Precondition**    | - Event must be created. <br> - President must be authenticated.                      |
| **Postcondition**   | Venue booking request is submitted and pending admin approval.               |
| **Main Flow**       | 1. President logs in.<br>2. Navigate to event management section. <br> 3. Selects an event.<br>4. Select "Request Venue Booking". <br> 5. Chooses venue and timeslot.<br>6. Submits request.<br>7. System logs the request with status "Pending". |
| **Alternate Scenario** | If the venue is already reserved, system notifies unavailability or suggests alternatives.        |

![RequestVenueBooking](https://github.com/user-attachments/assets/d4b7de84-77c9-429c-a0ce-7eb9fcd08265) <br>
*Figure 3.1.20 Request Venue Booking* 

---

### 3.1.21 Approve Venue Request

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-EVENT-06                                                                     |
| **Feature**         | Approve Venue Request                                                        |
| **Purpose**         | To enable admin to approve or reject venue booking requests, and trigger booking in the Campus Space Reservation System.         |
| **Actors**          | 	Admin, Campus Space Reservation System (external)                                                                |
| **Precondition**    | - Admin is logged in. <br> - Event must be created.<br> - Venue request exists with "Pending Approval" status. <br> - Venue status must be viewed.                       |
| **Postcondition**   | 	The booking status is updated in the system and the venue is reserved in the Campus Space Reservation System.                         |
| **Main Flow**       | 1. Admin logs in.<br>2. Navigate to venue approvals. <br> 3. View pending venue requests.<br>4. Select venue request. <br> 5. Review venue request.<br>6. View venue status generated by Campus Space Reservation System (CSRS). <br>7. If the venue is available, Admin clicks "Approve". <br> 8. System reserves venue via CSRS. <br> 9. Booking status in the main system is updated to "Approved & Reserved".
| **Alternate Scenario** | 		If the schedule conflicts during final booking, system returns an error and status is set to rejected or marked for resubmission with a comment.              |

 ![approveVenueRequest](https://github.com/user-attachments/assets/85494f18-59ac-43fc-a9c8-706640a17b68)
<br>
*Figure 3.1.21 Approve Venue Request* 

---

### 3.1.22 View Event Calendar

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-EVENT-07                                                                 |
| **Feature**         | View Event Calendar                                                          |
| **Purpose**         | To allow students to browse upcoming events on campus or by club.               |
| **Actors**          | Student                                              |
| **Precondition**    | Student is logged in.                                                           |
| **Postcondition**   | Events are displayed in calendar format.                                     |
| **Main Flow**       | 1. Student logs in.<br>2. Navigates to event calendar.<br>3. Optionally filters by club/date.<br>4. Display available events. <br> 5. View events |
| **Alternate Scenario** | If no events are available, display "No events scheduled".               |

![viewEventCalendar](https://github.com/user-attachments/assets/efe965e5-cf05-4b4e-88e6-7e8fd00cafe7) <br>
*Figure 3.1.22 View Event Calendar* 


---

### 3.1.23 Submit Budget Proposal

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-01                                                                   |
| **Feature**         | Submit Budget Proposal                                                        |
| **Purpose**         | To allow presidents to request funds for event or club operation.            |
| **Actors**          | President                                                                    |
| **Precondition**    | - Event must be created. <br> - President is authenticated.                      |
| **Postcondition**   | Budget proposal is submitted for review.                                      |
| **Main Flow**       | 1. President logs in.<br>2. Navigates to event management section.<br>3. Selects an event <br> 4. Select "Submit Budget Proposal". <br> 5. Fills in amount and justification.<br>6. Submits proposal.<br>7. System logs request. |
| **Alternate Scenario** | If required fields are missing, show error and prompt correction.         |

![SubmitBudgetProposal](https://github.com/user-attachments/assets/538e6086-9410-46d2-99ce-2feb6bad02ca)
 <br>
*Figure 3.1.23 Submit Budget Proposal* 


---

### 3.1.24 Approve Budget Proposal

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-02                                                                      |
| **Feature**         | Approve Budget Proposal                                                       |
| **Purpose**         | To enable admin to approve or reject submitted budget requests.       |
| **Actors**          | Admin, Financial Management System (external)                                |
| **Precondition**    | - Event must be created. <br> - Budget proposal is submitted and pending approval. <br> - Admin is authenticated and has access to finance dashboard.                                   |
| **Postcondition**   | Budget proposal is marked as approved or rejected. If approved, the details are forwarded to the Financial Management System for allocation and record.                  |
| **Main Flow**       | 1. Admin logs in.<br>2. Navigate to budget approvals.<br>3. Selects request.<br>4. Reviews the details and justification.<br>5. Approves or rejects.<br> 6. If approved, system syncs approval and budget details to the Financial Management System. |
| **Alternate Scenario** | If data is unclear, admin may request clarification from club.           |

![approveBudgetProposal](https://github.com/user-attachments/assets/c5f0e92a-2121-4280-b4db-f21938657389) <br>
*Figure 3.1.24 Approve Budget Proposal* 


---

### 3.1.25 View Club Budget

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-03                                                                     |
| **Feature**         | View Club Budget                                                             |
| **Purpose**         | To allow club member and admin to monitor financial balance and transaction logs. |
| **Actors**          | Member, Admin                                                       |
| **Precondition**    | Member or admin is logged in.                                     |
| **Postcondition**   | Budget data is displayed.                                                    |
| **Main Flow**       | 1. Member or admin logs in.<br>2. Navigates to budget section.<br>3. Views summary and breakdown. |
| **Alternate Scenario** | If no data, show “No transactions available”.                            |

![viewClubBudget](https://github.com/user-attachments/assets/7951b43e-06d0-4965-a967-9521f68520f4) <br>
*Figure 3.1.25 View Club Budget* 


---

### 3.1.26 Generate Financial Report

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-04                                                                      |
| **Feature**         | Generate Financial Report                                                    |
| **Purpose**         | 	To allow the Financial Management System to generate downloadable reports of club financial activity.      |
| **Actors**          | Financial Management System (external)                                               |
| **Precondition**    | Club financial data exists and report generation is requested by an authorized module/user.                                            |
| **Postcondition**   | Report file (PDF/CSV) is generated and downloadable.                         |
| **Main Flow**       | 1. A report generation request is received.<br>2. Financial Management System (FMS) processes the request. <br>3. FMS retrieves relevant club financial data. <br>4. FMS compiles data into selected format (PDF/CSV).<br>5. Report is made available for download. |
| **Alternate Scenario** | 	If no data is available for the selected period, FMS returns an error or "No data found" message.|


![generateFinancialReport](https://github.com/user-attachments/assets/6ae170be-7337-4a01-86d9-9f8ff0ff99e4) <br>
*Figure 3.1.26 Generate Financial Report* 

---

### 3.1.27 View Financial Report

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-BUDGET-05                                                                      |
| **Feature**         | View Financial Report                                                   |
| **Purpose**         | To allow members to view or download previously generated financial reports for their club.     |
| **Actors**          | Member                                              |
| **Precondition**    | - Member is authenticated. <br> - Club financial reports have been generated and stored.   |
| **Postcondition**   | Member views or downloads the selected financial report.                         |
| **Main Flow**       | 1. Member logs in. <br>2. Navigates to the financial reports section. <br>3. Selects club and reporting period. <br>4. Clicks to view or download the report.<br>5. System provides access to the report. |
| **Alternate Scenario** | 	If no report is available for the selected period, the system displays a "No reports found" message.|

![viewFinancialReport](https://github.com/user-attachments/assets/f5f558f5-f97c-4e22-b69f-9985af266d6a) <br>
*Figure 3.1.27 View Financial Report* 


---

### 3.1.28 Send Club Announcement

| **Field**           | **Details**                                                                 |
|---------------------|------------------------------------------------------------------------------|
| **ID**              | UC-COMM-01                                                                   |
| **Feature**         | Send Club Announcement                                                       |
| **Purpose**         | To allow president or committee to notify club members of updates or events. |
| **Actors**          | President, Committee                                                         |
| **Precondition**    | President or committe is logged in.                           |
| **Postcondition**   | Message is delivered to all club members via system notification or email. |
| **Main Flow**       | 1. President/committee logs in.<br>2. Opens communication panel.<br>3. Composes message.<br>4. Sends to club. |
| **Alternate Scenario** | If no members exist, system warns “No recipients available”.              |

---

### 3.1.29 Notify User
| **Field**          | **Description**                                                                                                                                       |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-COMM-02                                                                                                                                            |
| **Feature**        | Communication & Notifications                                                                                                                         |
| **Purpose**        | To send automated system notifications to specific users when key events occur                              |
| **Actors**         | - System (automated trigger)<br>- System Admin (for monitoring and config)                                                                            |
| **Precondition**   | - User exists in the system<br>- User is active and eligible to receive notifications<br>- System services are operational                            |
| **Postcondition**  | - Notification is stored in the system<br>- User is alerted through email depending on configuration                                          |
| **Main Flow**      | 1. System detects event requiring notification<br>2. Calls `notify_user(user_id, message, type)`<br>3. Validates user ID<br>4. Logs message<br>5. Sends via configured channel (dashboard/email/push) |
| **Alternate Flow** | - A1: Invalid user ID → Log error, skip notification<br>- A2: Notification service down → Retry or store as unsent<br>- A3: Invalid type → Use default type (e.g., "info") |

![My Image](Function_28.png)

---

### 3.1.30 View All Club
| **Field**          | **Description**                                                                                                                                             |
|--------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-CLUB-01                                                                                                                                                  |
| **Feature**        | View All Club                                                                                                                                         |
| **Purpose**        | To allow system admin view a list of all registered clubs in the system.                                                              |
| **Actors**         | <br> System Admin                                                                                                                             |
| **Precondition**   | - Admin user is authenticated<br>- User has appropriate admin privileges <br>- Clubs exist in the system                            |
| **Postcondition**  | - List of all clubs is displayed to the admin<br>- Admin can view the club's info                      |
| **Main Flow**      | 1. Admin logs into the system<br>2. Navigates to the club management section<br>3. System calls `view_all_clubs()`<br>4. System retrieves and displays club list |
| **Alternate Flow** | - A1: No clubs are registered → Show message: "No clubs found"<br>- A2: Database error → Show error message and log issue                                   |

---

### 3.1.31 Search Club
| **Field**          | **Description**                                                                                                                                                 |
|--------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-SEARCH-01                                                                                                                                                      |
| **Feature**        | Search Club                                                                                                                                         |
| **Purpose**        | To allow all users to search for clubs using keywords that match names, categories, or tags.                                                                    |
| **Actors**         | - All users such as student and admin                                                                                                                         |
| **Precondition**   | - Clubs exist in the system<br>- User has access to the search interface                                                  |
| **Postcondition**  | - A filtered list of clubs matching the keyword is shown<br>- User can view details or take further action like join club               |
| **Main Flow**      | 1. User enters a keyword into the search bar<br>2. System calls `search_clubs(keyword)`<br>3. Matches club name, category, and tags<br>4. Displays results list |
| **Alternate Flow** | - A1: No matches found → Show message: “No clubs found for that keyword”<br>- A2: Search service down → Show error and log issue                                |

---

### 3.1.32 Filter Event

| **Field**          | **Description**                                                                                                                                                       |
|--------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**             | UC-SEARCH-02                                                                                                                                                           |
| **Feature**        | Filter event                                                                                                                                       |
| **Purpose**        | To allow users to filter upcoming events based on selected criteria such as date, venue, or hosting club.                                                             |
| **Actors**         | - Student                                                                                                                            |
| **Precondition**   | - Events are available in the system<br>- User is on the event listing page or has access to filters                                                                  |
| **Postcondition**  | - A filtered list of events is displayed to the user based on chosen criteria                                                                                         |
| **Main Flow**      | 1. User selects filters: date, venue, or club<br>2. System calls `filter_events(date, venue, club)`<br>3. Events matching the criteria are retrieved<br>4. Results are displayed |
| **Alternate Flow** | - A1: No events match criteria → Show message: “No events found”<br>- A2: Filtering input is invalid → Show validation error or fallback to default view              |

### 3.1.33 Filter Budget Request
| **Field**           | **Details**                                                                                                                                                   |
|---------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**              | UC-FIN-005                                                                                                                                                    |
| **Feature**         | Filter categories of the budget request for the club using price range                                                                                                                 |
| **Purpose**         | Allows admin to efficiently filter and organize budget requests based on specified price ranges for faster decision-making and approval workflows.    |
| **Actors**          | - System Admin                                                                                                                                                   |
| **Precondition**    | The user must be logged in as an Admin and budget requests must exist in the system.                                                                    |
| **Postcondition**   | Budget requests are displayed according to the selected price range, improving readability and enabling focused review.                                       |
| **Main Flow**       | 1. Admin logs into the system. <br> 2. Navigates to the Budget Requests section. <br> 3. Selects "Filter by Price Range". <br> 4. Inputs or selects a range (e.g., $0–$500). <br> 5. System displays only the matching requests. |
| **Alternate Scenario** | - **No Matching Requests**: System shows “No budget requests found within the selected range.” <br> - **Invalid Input**: User is prompted to enter a valid range. |

### 3.1.34 Log Activity
| **Field**         | **Details**                                                                 |
|-------------------|------------------------------------------------------------------------------|
| **ID**            | UC-AUDIT-01                                                                      |
| **Feature**       | Log activity                                                |
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
| **Feature**       | View audit log                                                             |
| **Purpose**       | To allow system administrators to access and review system activity logs for monitoring, security audits, and issue investigation. |
| **Actors**        | - System Admin                                                                 |
| **Precondition**  | Admin is authenticated and has appropriate permissions to access system logs. |
| **Postcondition** | The system displays a list of recorded user activities with details such as user ID, action, and timestamp. |
| **Main Flow**     | 1. Admin logs in to the system. <br> 2. Navigates to the audit log section. <br> 3. System retrieves and displays activity logs. |
| **Alternate Scenario** | If no logs are available, a message is shown indicating “No audit logs found.” If access is unauthorized, an error message is displayed. |

### 3.1.36 Set Permission
| **Field**         | **Details**                                                                 |
|-------------------|------------------------------------------------------------------------------|
| **ID**            | UC-AUDIT-03                                                                        |
| **Feature**       | Set permission                                         |
| **Purpose**       | To allow system administrators to define or update the actions that each user role is authorized to perform within the system. |
| **Actors**        | - System Admin                                                                 |
| **Precondition**  | Admin is authenticated and has access to the role management module.         |
| **Postcondition** | Permissions for the specified role are updated and enforced across the system. |
| **Main Flow**     | 1. Admin logs in. <br> 2. Navigates to the role/permission settings. <br> 3. Selects a role. <br> 4. Assigns or updates permissions. <br> 5. System saves the changes. |
| **Alternate Scenario** | If an invalid role is specified, an error message is shown. If no permissions are selected, the system prompts the admin to select at least one. |

### 3.1.37 Generate Venue Status Report
| **Field**           | **Details**                                                                                                                                                    |
|---------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**              | UC-VEN-004                                                                                                                                                     |
| **Feature**         | Generate Venue Status Report                                                                                                                                       |
| **Purpose**         | Automatically generates the current status of all venues for specificed time slots for Admin review and approval.                             |
| **Actors**          | - <<external>> Campus Space Reservation System                                                                                                             |
| **Precondition**    | The Admin must be logged in, and there must be existing venue requests or bookings in the system. Also, event content is approved.                                                             |
| **Postcondition**   | A list of venue statuses (available, pending, booked) is presented to the Admin, enabling follow-up actions like approval.                                     |
| **Main Flow**       | 1. Admin logs in. <br> 2. Navigates to Venue Management. <br> 3. System sends a request to the Campus Space Reservation System. <br> 4. System receives and generates venue status overview. <br> 5. Admin reviews the venue statuses. |
| **Alternate Scenario** | - **No Data**: If no venue data is returned, the system shows: "No venue information available." <br> - **System Failure**: If external API fails, an error message is displayed. |

### 3.1.38 View Venue Status
| **Field**           | **Details**                                                                                                                                                    |
|---------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **ID**              | UC-VEN-005                                                                                                                                                     |
| **Feature**         | View Venue Status                                                                                                                         |
| **Purpose**         | Allows the Admin to view real-time venue availability before making decisions.                                                  |
| **Actors**          | - Admin                                                                                                             |
| **Precondition**    | - Admin must be logged in. <br> - Venue booking requests must exist. <br> - Venue status report is available                 |
| **Postcondition**   | Admin sees updated venue availability |
| **Main Flow**       | 1. Admin logs in. <br> 2. Navigates to Venue Status section. <br> 3. Selects a request to review. <br> 4. Select date and timeslots. <br> 5. View generated status report. |
| **Alternate Scenario** | - **No data found**: System sshows "No data available" message. |

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

## 3.6 Design Constraints
### 3.6.1 External Standards and Regulatory Requirements
a) Data Privacy and Security:
- FERPA Compliance: The platform must comply with the Family Educational Rights and Privacy Act to protect students' educational and activity records.

- University Data Governance: The system must follow internal policies regarding the collection, storage, retention, and access of student data.

- Role-Based Access: Data visibility must be restricted according to user roles (e.g., students, club presidents, admins).

- Audit Logging: All access to sensitive personal data must be logged for accountability and review.

b) Security Standards:
- OWASP Top 10 Compliance: The system must be protected against common vulnerabilities such as SQL injection, XSS, CSRF, and broken authentication.

- HTTPS Protocol: All data exchanges between clients and servers must be encrypted using HTTPS with valid SSL/TLS certificates.

- Secure Coding Practices: Input validation, session management, and secure authentication mechanisms must be implemented to reduce risk.

- HSTS Enforcement: HTTP Strict Transport Security headers should be used to ensure all communication is securely routed.

c) Accessibility Standards:
- WCAG 2.1 Level AA Compliance: The platform must be accessible to users with disabilities by adhering to Web Content Accessibility Guidelines.

- Keyboard Navigation: All interactive elements must be operable without a mouse.

- Screen Reader Support: Pages must use semantic HTML and ARIA roles for compatibility with assistive technologies.

- Responsive Design: The interface must adapt fluidly to different screen sizes and orientations.

### 3.6.2 Project Limitations
a) Time Constraint
- The platform must be completed within one academic semester (approximately 4–5 months).

- Due to limited time, complex features such as analytics, AI, or predictive dashboards are not in scope.

b) Budget Constraint
- The project must utilize free and open-source tools and platforms.
- No commercial licensing or paid APIs are allowed due to limited funding.

c) Resource Availability
- The development team is likely composed of students or part-time contributors with varying skill levels.
- Testing feedback from real stakeholders (students, admins) may be limited due to academic scheduling.

d) Stakeholder Input
- Availability for feedback and user testing from actual stakeholders (e.g., student club members, event approvers, venue managers) may be constrained due to conflicting academic and administrative responsibilities.

### 3.6.3 Technical Constraints
a) Technology Stack
- The backend must use the Django (Python) framework as per university guidelines.

- Frontend technologies must be lightweight and compatible with Django templates.

b) Database Technology
- Only PostgreSQL and SQLite are approved for database implementation due to internal IT restrictions.

c) Integration Requirement
- The system must integrate with the university’s Single Sign-On (SSO) solution via OAuth2 or LDAP for secure user authentication.

d) API Usage
- Any integration with third-party APIs (e.g., Google Calendar, email services) must adhere to the university’s data privacy and security policies.

### 3.6.4 Platform Constraints
a) Hosting Environment
- The platform must be deployable on the university’s Linux-based infrastructure (on-premise or cloud-hosted), limiting the operating system and server stack configurations.

b) Client Compatibility
- The system must be accessible through all major modern browsers, including Google Chrome, Mozilla Firefox, Apple Safari, and Microsoft Edge, without relying on any browser-specific features.

c) Mobile Access
- A fully native mobile application is not in scope. The platform must use responsive web design to ensure usability across smartphones and tablets.

d) Access Restrictions
- Access to the system must be restricted to authenticated university members (students, faculty, staff), with features and permissions tailored to their assigned roles.

### 3.6.5 Environmental Constraints
a) Network Dependency:
- The platform will require reliable internet access to function; offline features are not a requirement.

b) Data Privacy Compliance:
- Data handling must align with FERPA and university-specific privacy policies, including data retention and access control rules.

c) User Access Context:
- The system must perform reliably across both on-campus and remote environments, accounting for variable network speeds and firewall conditions.

d) Maintenance Scheduling:
- System updates must be planned during non-peak hours (e.g., evenings or weekends) to avoid disrupting ongoing student or administrative activities.

## 3.7 Software System Attributes
### i. Scalability
a. Horizontal Growth Support
- The system must be designed to support an increasing number of users, clubs, events, and transactions without requiring major architectural changes.

b. Load Distribution
- System components such as authentication, event scheduling, and budget management should be independently scalable to handle peak load periods (e.g., club registration weeks).

c. API and Data Scalability
- APIs and database queries must be optimized to prevent bottlenecks during high-volume interactions such as bulk approvals or calendar views.

### ii. Responsiveness
a. Fast User Interaction
- UI elements should respond within 500 milliseconds for most actions like button clicks, tab navigation, and form validation.

b. Page Load Performance
- All primary pages (dashboard, event list, profile) must load within 3 seconds under standard conditions.

c. Lightweight Frontend
- The frontend should minimize resource usage using lazy loading, AJAX updates, and asynchronous form submissions.

### iii. Security
a. Session Management
- Sessions must expire after inactivity and use secure session tokens. Re-authentication should be required for critical actions.

b. Role Isolation
- The system must strictly separate user roles (student, committee, admin) to prevent privilege escalation.

c. Secure Data Transactions
- Budget submissions, event approvals, and user profile edits must be protected with input sanitization and transaction validation.

### iv. Usability
a. Intuitive Navigation
- The UI must support easy navigation with clear labels, minimal clicks to reach key features, and consistent layout across pages.

b. Accessible Form Design
- All forms must include helper text, real-time validation feedback, and tooltips to improve user experience.

c. Feedback and Notifications
- Users must receive real-time system feedback (e.g., success/error messages) and relevant in-app/email notifications.

### v. Interoperability
a. External System Integration
- The system must support API-based integration with existing university systems such as financial software, facility booking tools, or attendance tracking.

b. Open Standards Compliance
- Data exchange should use standard formats (e.g., JSON, CSV) and RESTful APIs for compatibility with third-party tools.

c. Calendar and Email Integration
- Seamless syncing with services like Google Calendar, Outlook, and campus email systems is required to coordinate events and notify users.


## 4. Verification
### Requirements Verification
To make sure the Software Requirements Specification (SRS) is accurate, comprehensive, and in line with stakeholder expectations, a rigorous requirements verification procedure will be conducted before the design phase begins.  Software developers, QA engineers, administrative stakeholders, and student reps are all involved in this evaluation process.  Clarity, testability, consistency, and traceability will all be assessed for both functional and non-functional requirements.  Every requirement will have matching test cases and design components if a Requirement Traceability Matrix (RTM) is used.  The project must be cleared of any ambiguous, contradictory, or unnecessary requirements found during this stage before moving on to design.

All comments and modifications brought about by requirement evaluations will be officially recorded in order to maintain accountability and openness.  To record requirements-related issues, assign action items, and monitor their resolution, issue-tracking platforms like GitHub Issues, Trello, or JIRA might be utilized.  Stakeholder input will be documented during meetings and included into the revised SRS via an iterative review procedure.  A collaborative and traceable development workflow will be facilitated by version control of the requirements document, which will enable all stakeholders to view past changes.  This methodical feedback loop guarantees that the validated requirements provide a solid basis for all subsequent development operations.

### Design Verification
The design verification process's goal is to verify that the system architecture and component-level designs satisfy industry standards for modularity, scalability, and maintainability as well as the validated requirements.  The product team, which consists of developers, software architects, and quality assurance staff, will carry out formal reviews.  To guarantee logical coherence and efficient modular separation, design documentation including UML class diagrams, ER diagrams, and data flow diagrams will be examined throughout these evaluations.  The focus will be on confirming that the system design accurately models important operations, including role-based access control, event registration, and budget approval.

Before proceeding with the technical implementation, stakeholders will validate design prototypes, such as low-fidelity wireframes and workflow mockups.  The user interface and system interactions will be improved based on input gathered during these sessions.  All review results, including requests for clarification or changes, will be recorded in shared documentation and followed through on.  The design is kept in line with project limitations, technical viability, and stakeholder needs thanks to the iterative review process.  In the end, the validated design needs to function as an understandable and practical development roadmap.

### Code Verification
The code will undergo human code reviews and static code analysis throughout the development stage.  To automatically find any problems like code smells, formatting errors, and security flaws, static analysis tools like Pylint, ESLint, or SonarQube will be used.  Platforms such as GitHub will be used to conduct peer code reviews concurrently. Before code is merged into the main branch, developers must examine and approve each other's contributions.  Code verification will guarantee that the codebase is maintainable, that the system architecture is followed, and that project coding standards are followed.  Integration must come after all important issues have been resolved.

### Unit Testing
To confirm the accuracy of each component separately, unit testing will be done.  Using frameworks like Pytest or the integrated test runner in Django, developers will create automated test cases.  Core features like club formation, event registration, budget submission, and login authentication will be the focus of these testing.  Where required, mocking will be utilized to separate components.  Before code is deemed stable for integration testing, all tests must pass and a minimum of 80% code coverage will be the goal.

### Integration Testing
The proper operation of associated components will be confirmed by integration testing.  For instance, it will confirm that students may sign up for events after registering and joining a club, and that these interactions result in the proper permissions and notifications.  Tools like Selenium, Postman, or Pytest with Django's LiveServer will be used for testing.  This guarantees that business rules are appropriately enforced across components, data flows between modules, and APIs operate as intended.

### Regression Testing
Using testing frameworks compatible with Django, like Pytest or Django's TestCase, automated regression test suites will be created to ensure consistency and dependability between releases.  These test suites will cover a variety of important use scenarios, such as workflows with different user roles (e.g., a committee member revising a request after it has been submitted by a student and approved by an administrator).  As a defense against regressions brought about by code changes, the tests will run automatically prior to each deployment or merging into the main development branch.

The test library will be able to develop with the system since all regression test cases will be version-controlled using the same Git repository as the application code.  When a test fails, developers will receive feedback right away, and they have to fix the problems before releasing the product.  The regression suite will expand over time to incorporate new capabilities, guaranteeing continuous protection and coverage of the system's essential operations.  In addition to lowering post-deployment problems and enhancing long-term maintainability, this proactive approach to regression testing will greatly increase system stability.

### System Testing
In a controlled staging environment, system testing will verify that the complete system satisfies the validated functional and non-functional requirements.  This covers all of the main user roles (students, club leaders, event administrators, and system administrators) carrying out standard tasks including budget requests, club approval, and event planning.  Error handling, edge cases, and boundary conditions will all be extensively examined.  The QA team will be in charge of carrying out thorough test cases and documenting any errors so they can be fixed.

### Non-Functional Testing
Additionally, the system will be put through a rigorous non-functional testing process to assess its compatibility, security, performance, and usability.  The system's ability to support 500 users at once while keeping response times under three seconds will be tested through performance testing.  Security testing will guarantee that data is safely stored and communicated and validate protection against typical threats like SQL injection, CSRF, and XSS.  In order to verify accessibility, logical navigation, and ease of use, usability testing will entail assessing the interface from the viewpoints of administrators and students.  Testing for compatibility will guarantee that the system operates correctly on all supported platforms, including PCs, tablets, and smartphones, as well as on all supported browsers (Chrome, Firefox, Safari, and Edge).

### User Acceptance Testing (UAT)
The system will undergo User Acceptance Testing (UAT) to confirm that it meets the expectations and real-world requirements of its target users.  The testing method will involve a carefully chosen group of student users, club representatives, event coordinators, and administrative personnel.  Through realistic tasks including club creation, budget proposal submission and approval, event scheduling, and announcement viewing, these users will engage with the system in a staging or UAT environment.  Verifying that the system supports their daily operations, is user-friendly, and operates dependably under normal circumstances is the aim.  In order to replicate independent usage, UAT scenarios will be prepared and testers will be led through the procedure with little help.

Following every UAT session, comprehensive input will be gathered via surveys, structured interviews, or methods for reporting issues.  The QA team and product managers will examine this input to find any lingering bugs, functional gaps, or usability problems.  Before the system is deployed in production, all important problems must be fixed.  The majority of test participants must formally approve the system before it can proceed, and acceptance criteria will be established in cooperation with stakeholders.  The last test to determine whether the system is prepared for live use in an actual university setting is this last stage of verification.

### Deployment Verification
The system will go through smoke testing after it is deployed to the production environment to ensure that essential features like user login, event registration, club listing, and administrative dashboards work as intended.  To guarantee system stability, the QA and DevOps teams will do this testing as soon as the system is deployed.  Real-time tracking of system problems and uptime will also be done with monitoring tools.  The platform's stability, usability, and readiness for the larger university community to access are the main objectives.




## 5. Appendixes

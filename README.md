# LocalConnect Platform

## Table of Contents
1. [Introduction](#introduction)
   - [Purpose](#purpose)
   - [Scope](#scope)
   - [Overview](#overview)
2. [Overall Description](#overall-description)
   - [Product Perspective](#product-perspective)
   - [Product Features](#product-features)
   - [User Classes and Characteristics](#user-classes-and-characteristics)
   - [Operating Environment](#operating-environment)
   - [Design and Implementation Constraints](#design-and-implementation-constraints)
3. [Functional Requirements](#functional-requirements)
   - [User Authentication](#user-authentication)
   - [Product Search and Selection](#product-search-and-selection)
   - [Seller Management](#seller-management)
   - [Reservation System for Service Providers](#reservation-system-for-service-providers)
   - [Skills Marketplace](#skills-marketplace)
4. [Non-Functional Requirements](#non-functional-requirements)
   - [Performance Requirements](#performance-requirements)
   - [Security Requirements](#security-requirements)
   - [Usability Requirements](#usability-requirements)
   - [Reliability Requirements](#reliability-requirements)
   - [Compatibility Requirements](#compatibility-requirements)
   - [Maintainability Requirements](#maintainability-requirements)
   - [Regulatory Compliance](#regulatory-compliance)
5. [System Architecture](#system-architecture)
   - [APIs and Interfaces](#apis-and-interfaces)
   - [Hardware Interfaces](#hardware-interfaces)
   - [Software Interfaces](#software-interfaces)
   - [Communication Interfaces](#communication-interfaces)

## Introduction

### Purpose
LocalConnect is a versatile platform connecting users with nearby sellers, reservation Service Providers, and service providers, aiming to enhance the local user experience through tailored functionalities.

### Scope
The system provides functionalities such as user access and registration, seller accounts, reservation Service Providers accounts, and a service providers. It caters to regular users, sellers, service providers, and skilled individuals.

### Overview
LocalConnect operates as an independent .NET Angular website with a SQL Server database, seamlessly connecting users through dedicated interfaces and interfacing with external systems for data enrichment.

## Overall Description

### Product Features

#### 1. User Access and Registration
- Tailored Account Creation to Meet Individual Needs

#### 2. Looking for service in a specific area or specific account 
- Users can specify their current location or preferred area, enabling a targeted search for local sellers, Reservation Service Providers, and Service Providers.

#### 3. Seller Accounts
- Sellers manage e-commerce and cashier functions through dedicated accounts.

#### 4. Reservation System
- Reservation service providers manage reservations from their accounts.
- Real-time updates and conflict prevention.

#### 5. Service Providers
- Individuals showcase skills and they can accept users' requests and chat with them or refuse.

### User Classes and Characteristics

#### 1. Regular Users
- Consumers seeking local products and services.

#### 2. Sellers
- They can show their product and update it frequently 

#### 3. Reservation System
- Providers manage reservations and availability

#### 4. Service Providers
- Showcase skills and services through their profiles and respond to service requests.

### Operating Environment

- The .NET Angular website operates on standard PCs, tablets, and smartphones.
- Cross-platform accessibility supported, with compatibility on major web browsers (Chrome, Firefox, Safari, Edge).
- A stable internet connection is vital for optimal performance, real-time updates, and communication.

### Design and Implementation Constraints

- .NET framework on the backend, Angular on the frontend, and SQL Server as the relational database.
- Minimum hardware requirements: 2GB RAM, dual-core processor.

## Functional Requirements

### 1. User Authentication

#### 1.1 Description
- Users securely create accounts, log in, and manage profiles.
- Authentication mechanisms implemented for security and privacy.

### 2. Product Search and Selection

#### 2.1 Description
- Users search for products or services through the Angular frontend.
- SQL Server database facilitates efficient retrieval of information.

### 3. Seller Management

#### 3.1 Description
- Sellers create and manage accounts through Angular interfaces.
- .NET backend and SQL Server database facilitate account management.

### 4. Reservation System for Service Providers

#### 4.1 Description
- Service providers create accounts with reservation systems.
- .NET backend and SQL Server database manage reservations and prevent conflicts.

### 5. Skills Marketplace

#### 5.1 Description
- Individuals with skills create profiles using Angular interfaces.
- .NET backend and SQL Server database manage skill profiles and facilitate communication.

### Dependencies
- Dependent on .NET backend, Angular interfaces, and SQL Server database.

### Assumptions and Preconditions
- Requires a stable internet connection for real-time updates, with the flexibility for sellers to postpone data updates for a specified period, up to one day, due to internet availability constraints.
- Assumes accurate information for user accounts.

## Non-Functional Requirements

### 1. Performance Requirements

#### 1.1 Response Time
- System response within 2 seconds for user actions.
- Prompt processing of search queries, transactions, and reservation confirmations.

#### 1.2 Scalability
- Support for up to 10,000 simultaneous users without significant performance degradation.
- Efficient scaling of database queries and transaction handling.

### 2. Security Requirements

#### 2.1 User Authentication
- Secure hashing and storage of user passwords in the SQL Server database.

#### 2.3 Access Control
- Role-based access control (RBAC) to restrict unauthorized access to sensitive functionalities.

### 3. Usability Requirements

#### 3.1 User Interface Design
- Intuitive and user-friendly interface following modern design principles.
- Implementation of accessibility features for inclusivity.

#### 3.2 Error Handling
- Provision of informative and user-friendly error messages for invalid inputs or system errors.

### 4. Reliability Requirements

#### 4.1 System Uptime
- Advance communication of scheduled maintenance to users.

#### 4.2 Data Integrity
- SQL Server database ensures integrity, preventing data corruption or loss.

### 5. Compatibility Requirements

#### 5.1 Browser Compatibility
- Angular frontend compatible with major web browsers (Chrome, Firefox, Safari, Edge).

#### 5.2 Device Compatibility
- .NET Angular website responsive and compatible with standard PCs, tablets, and smartphones.

### 6. Maintainability Requirements

#### 6.1 Code Documentation
- Thorough documentation of code for .NET backend and Angular frontend for ease of maintenance and updates.

#### 6.2 Modularity
- System designed with a modular architecture for future enhancements or modifications.

### 7. Regulatory Compliance

#### 7.1 PCI DSS Compliance (if handling payment transactions)
- Compliance with Payment Card Industry Data Security Standard (PCI DSS) for secure payment processing.

## System Architecture

### APIs and Interfaces

- Exposes RESTful APIs for communication between Angular frontend and .NET backend.
- Manages user authentication, product/service listings, reservations, and skills marketplace.

### Hardware Interfaces

#### Standard PCs, Tablets, and Smartphones
- System accessible and functional on devices with varying screen sizes and capabilities.

### Software Interfaces

#### Web Browsers
- Angular frontend compatible with latest versions of popular web browsers (Chrome, Firefox, Safari, Edge).

#### Database Management System
- Interfaces with SQL Server database for efficient storage and retrieval of data.

### Communication Interfaces

#### Internet Connection
- Relies on a stable internet connection for real-time updates, data synchronization, and user interactions.
- Utilizes HTTPS for secure communication between frontend and backend.

#### Email Notifications
- Sends email notifications for account verification, password recovery, and important system updates.

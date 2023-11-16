 # LocalConnect

Welcome to LocalConnect – Your Local Connection to Products, Services, and More!

## Overview
LocalConnect is a versatile platform connecting users with nearby sellers, Reservation Service Providers, and Service Providers. 

## Purpose
LocalConnect aims to enhance the local user experience by providing tailored functionalities. Whether you're a regular user, a seller, a reservation service provider, or a skilled individual, LocalConnect has something for you.

## Features
### 1. User Access and Registration
- Tailored account creation to meet individual needs.
- Customize account settings for a personalized experience.

### 2. Service Search in Specific Areas or Accounts
- Specify your location or preferred area for a targeted search.
- Filter search results based on account types.

### 3. Seller Accounts
- Manage product listings and cashier functions for seamless transactions.

### 4. Reservation System providers
- Efficiently manage reservations with real-time updates.
- Conflict prevention mechanisms for a smooth booking experience.

### 5. Service Providers
- Showcase skills and services through profiles.
- Accept or refuse user requests with real-time chat functionality.

## User Classes and Characteristics
- Regular Users: Discover and explore local products and services.
- Sellers: Showcase products and manage listings.
- Reservation Service Providers: Offer Efficiently manage reservation.
- Service Providers: Showcase skills and services to attract users.

## Operating Environment
- Cross-platform accessibility on PCs, tablets, and smartphones.
- Browser compatibility: Chrome, Firefox, Safari, Edge.
- Stable internet connection for optimal performance.

## Design and Implementation Constraints
- Technology Stack: .NET framework, Angular, SQL Server.
- Minimum Hardware Requirements: 2GB RAM, dual-core processor.



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

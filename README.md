 # LocalConnect

Welcome to LocalConnect – Your Local Connection to Products, Services, and More!

## Overview
LocalConnect is a versatile platform connecting users with nearby Reservation Providers and Service Providers. 

## Purpose
LocalConnect aims to enhance the local user experience by providing tailored functionalities. Whether you're a regular user, a reservation  provider, or a skilled individual, LocalConnect has something for you.

## Features
### 1. User Access and Registration
- Tailored account creation to meet individual needs.
- Customize account settings for a personalized experience.

### 2. Service Search in Specific Areas or Accounts
- Specify your location or preferred area for a targeted search.
- Filter search results based on account types.

### 3. Seamless Service Interaction
-Experience a seamless service interaction by choosing a service provider or reservation. This feature includes an integrated chat functionality for real-time communication and the convenience of secure online payments.

### 4. Reservation System providers
- Efficiently manage reservations with real-time updates.
- Conflict prevention mechanisms for a smooth booking experience.

### 5. Service Providers
- Showcase skills and services through profiles.
- Accept or refuse user requests.

### Portfolio Enhancement:
 -Empower reservation and services providers to showcase their abilities and expertise through a comprehensive and dynamic portfolio feature on LocalConnect.


## User Classes and Characteristics
- Regular Users: Discover and explore local services.
- Reservation Service Providers: Offer Efficiently managed reservations.
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

  
# Functional Requirements

## 1. User Access and Registration

### 1.1 Account Creation:
   - Implement social media authentication (e.g., Google, Facebook) as an alternative registration method, enhancing user convenience.
   - Enable users to create personalized accounts tailored to meet their individual needs.
   - Prioritize data security and privacy in the account creation process.

### 1.2 Tailored Account Settings:
   - Allow users to customize account settings, providing flexibility in managing privacy preferences and notification configurations.

## 2. Service Search in Specific Areas or Accounts

### 2.1 Location-Based Search:
   - Empower users with the ability to specify their current location or preferred area for a precise and targeted service search.
   - Deliver search results for Reservation Providers and Service Providers based on the specified location.

### 2.2 Account-Specific Search:
   - Enable users to filter search results based on specific account types, facilitating a more refined search experience for regular users, reservation providers, or service providers.

## 3. Reservation System

### 3.1 Reservation Management:
   - Provide Reservation Service Providers with efficient tools for managing reservations through their accounts.
   - Ensure real-time updates to maintain accurate availability of information.

### 3.2 Conflict Prevention:
   - Incorporate conflict prevention mechanisms within the system to proactively avoid overlapping reservations, ensuring a seamless booking experience.

## 4. Service Providers

### 4.1 Skills Showcase:
   - Empower Service Providers to present their skills and services through detailed profiles, enriched with comprehensive descriptions and multimedia content.

### 4.2 Request Handling:
   - Enable Service Providers to efficiently manage user requests through real-time chat functionality.
   - Introduce a portfolio feature for Service Providers, allowing them to showcase past work, client testimonials, and certifications, thereby enhancing user confidence.

## 5. Rating and Reviews

### 5.1 Previous Services Rating:
   - Provide users with the opportunity to rate specific aspects of past services, covering various facets such as punctuality, communication, and service quality.
     
### 5.2 Overall Rating:
   - Dynamically calculate an overall rating based on comprehensive evaluations provided in the "Previous Services Rating" section.
   - 
## 6. Real-Time Chat

### 6.1 Instant Interaction:
   - Facilitate direct and real-time communication between users and service providers immediately after the service provider accepts a request, ensuring seamless and efficient collaboration.

## 7. Payment Integration

### 7.1 Secure Online Payments:
   - Implement a robust system that allows users the option to make secure online payments for services.
   - Ensure users can confidently enter their card information, with payment processing occurring only after the service provider accepts the user's request and finalizes the reservation.


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
- Angular frontend is compatible with the latest versions of popular web browsers (Chrome, Firefox, Safari, Edge).

#### Database Management System
- Interfaces with SQL Server database for efficient storage and retrieval of data.

### Communication Interfaces

#### Internet Connection
- Relies on a stable internet connection for real-time updates, data synchronization, and user interactions.
- Utilizes HTTPS for secure communication between the front end and back end.

#### Email Notifications
- Sends email notifications for account verification, password recovery, and important system updates.




____________________________________________________________________________________________________________________________________________________________________


# User Stories

## User Story 1: Register as a Regular User

As a potential user, I want to be able to register as a regular user on the platform so that I can access and utilize various services.

### Acceptance Criteria:

- The registration process should include providing basic information such as name, email, and password.
- Upon successful registration, the user should receive a confirmation email.
- The user should be able to log in with the registered credentials.

## User Story 2: View and Edit My Profile

As a registered user, I want to be able to view and edit my profile information to ensure that it is accurate and up-to-date.

### Acceptance Criteria:

- There should be a user profile section accessible after logging in.
- The user should be able to view their existing profile information.
- The user should be able to edit and update their profile details such as name, contact information, and preferences.

## User Story 3: Determine My Location

As a user, I want the platform to automatically determine my location or allow me to manually input my location to ensure that I receive relevant local services.

### Acceptance Criteria:

- The platform should have a feature to automatically detect the user's location based on device data.
- Alternatively, the user should be able to manually input their location.
- The user's location should be stored and used for providing location-specific services.

## User Story 4: Choose Needed Services and Filter Providers

As a user, I want to be able to choose from a list of services and have the option to filter service providers based on my location.

### Acceptance Criteria:

- The platform should have a list of available services for users to choose from.
- The user should be able to filter service providers based on their determined or manually inputted location.
- The filtered results should display relevant service providers for the selected service in the user's location.

## User Story 5: Reservation Providers, and Service Providers

As a user, depending on the selected service, I want to interact with reservation providers, and service providers in different ways.

### Acceptance Criteria:

### For Reservation Provider:

- View available appointments.
- Search for specific reservation services.
- Choose and request a reservation appointment.

#### For Service Provider:

- View available services.
- Search for specific service providers.
- Choose and send a service request to the selected provider.

## User Story 7: Reservation Provider Operations

As a reservation provider, I want to be able to manage my appointments effectively.

### Acceptance Criteria:

- Log in with reservation provider credentials.
- View a list of appointments.
- Add new free appointments to the list.
- Edit and update details of existing free appointments.

## User Story 8: Service Provider Operations

As a service provider, I want to be able to manage orders and their status.

### Acceptance Criteria:

- Log in with service provider credentials.
- View a list of orders.
- Accept or decline orders based on availability.
- Update the status of orders to keep users informed.

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

## User Access and Registration

- **Sign Up:** As a new user, you can sign up for LocalConnect using your email and password or with [Google/Facebook] account to create a personalized account.

- **Log In:** Existing users can log in quickly and easily using their Google or Facebook accounts.

### Acceptance Criteria:

- The registration process should include providing basic information such as name, email, and password.
- Upon successful registration, the user should receive a confirmation email.
- The user should be able to log in with the registered credentials.

## Password Reset

**User Story: Reset Password**
- As a registered user,
- I want to reset my password if I forget it,
- So that I can regain access to my account.

**Acceptance Criteria:**
- Provide a "Forgot Password" link on the login page.
- Prompt the user to enter their email address.
- Send a password reset link to the user's email.
- Allow the user to set a new password using the provided link.
- Ensure security measures, such as email verification, to protect the account.

  ## Service Search in Specific Areas or Accounts

**User Story: Service Search in Specific Areas or Accounts**
- As a user,
- I want to search for local services in a specific area to find relevant Reservation Providers or Service Providers,
- So that I can easily discover and connect with services near my location.

**Acceptance Criteria:**
- Provide a search bar allowing users to input their preferred location.
- Display search results that include Reservation Providers and Service Providers based on the specified area.
- Include filters for account types (Reservation Providers, Service Providers) to refine search results.
- Ensure the search functionality is intuitive and provides relevant and accurate results.

  ## Seamless Interaction with a Service Provider

**Story:**
- Upon finding a Service Provider with positive reviews and relevant skills, I initiate a service request.
- The Service Provider receives a real-time notification about my request and reviews the details.
- If the Service Provider accepts my request, I want to seamlessly transition into a chat interface for direct communication.
- In the chat, I can discuss service details, ask questions, and receive any additional information from the Service Provider.
- After the successful completion of the service, I have the option to provide a user rating and review based on my experience.

**Acceptance Criteria:**
3. Users can initiate a service request with the necessary details.
4. Service Providers receive real-time notifications for new service requests.
5. Service Providers can review and accept service requests.
6. Upon acceptance, users and Service Providers can seamlessly transition into a chat interface.
7. The chat interface supports real-time communication between users and Service Providers.
8. Users can discuss service details, ask questions, and receive timely responses within the chat.
9. The system records and displays the history of the chat for reference.
10. After service completion, users can provide a rating and review based on their experience.

## Flexible Reservation Options for Users

**Story:**
- I choose from the Reservation Provider's available appointment slots displayed in real-time.
- The system allows me to select my preferred appointment time and date directly.
- During the reservation process, I have the option to choose between online payment or opting for an alternative payment method upon service completion.
- If the selected appointment slot is available, the system confirms my reservation instantly.
- After confirming, I can view the reservation details, including the chosen appointment time, and communicate with the Service Provider if needed.
- Upon successful service completion, I have the option to provide a user rating and review based on my experience.

**Acceptance Criteria:**
2. The reservation section allows users to explore available services and directly choose appointment slots.
3. Users can select a preferred appointment time and date from the available options.
4. Users have the option to choose between online payment and an alternative payment method upon service completion.
5. The system confirms the reservation instantly if the selected appointment slot is available.
6. Users can view reservation details, including the chosen appointment time, after confirmation.
7. Users can communicate with the Service Provider if necessary.
8. The system records and displays user ratings and reviews for completed reservations.

## Manage Profile Details

**Story:**
- Upon login, I effortlessly navigate to the profile section, where my username, contact information, location, and bio are displayed.
- Opting to enhance my profile, I select "Edit Profile" and make adjustments to contact details, location, bio, profile picture, and background.
- Once changes are saved, my profile undergoes instant updates, ensuring the revised details are promptly visible both personally and publicly on the LocalConnect platform.

**Acceptance Criteria:**
- Users access the profile section, viewing current details.
- "Edit Profile" allows modifications to contact information, location, bio, and profile picture, etc.
- Saved changes instantly update the user's profile for both personal and public visibility on LocalConnect.

  ## Create and Administer Business Page

**Story:**
- As a LocalConnect user aspiring to showcase my services, I want the ability to create and manage a business page similar to social media platforms.
- Upon logging into LocalConnect, I navigate to the profile section and choose to create a business page.
- The creation process involves entering essential details such as business name, category, contact information, and a brief description.
- I have the option to upload a logo or relevant images to enhance the visual appeal of the business page.
- Once the business page is created, I become the admin with the authority to modify page details and settings.
- As the admin, I can regularly update business information, post updates, and manage reservations or service requests.
- Users interested in my services can follow the business page to receive updates and make reservations.
- The business page reflects real-time changes, ensuring that the information is accurate and up-to-date.

**Acceptance Criteria:**
1. Users can navigate to the profile section and initiate the creation of a business page.
2. The creation process involves entering business details such as name, category, contact information, and a brief description.
3. Users can upload a logo or relevant images to customize the visual appearance of the business page.
4. Upon creation, the user becomes the admin of the business page with the authority to modify details and settings.
5. Admins can regularly update business information, post updates, and manage reservations or service requests.
6. Users can follow business pages to receive updates make reservations and request services.
7. Real-time updates ensure that the information on the business page is accurate and up-to-date.

## Administer Business Reservation Settings (ex : Doctor and halls)

**Story:**
- As an admin for a reservation system, I need the ability to view and edit details such as the business name, contact information, portfolio, and a brief description.
- To optimize reservation scheduling, I set available reservation times and configurable settings, such as maximum daily reservations and lead time for booking appointments.
- Once adjustments are made, the system promptly reflects changes, ensuring accurate and up-to-date information for users.

**Acceptance Criteria:**
1. The admin accesses the profile management section in the admin panel.
2. Business profile details, including name, contact information, and description, are viewable and editable.
3. The admin configures available reservation times, defining durations or time slots.
4. Configurable settings, including maximum daily reservations and lead time for bookings, are successfully adjusted.
5. Changes made in the admin panel are instantly reflected in the business profile and reservation system.

## Administer Hotel Reservation Settings
1. Log into the admin panel, accessing the hotel profile management section.
2. Review and edit hotel details, encompassing name, contact info, and a brief description.
3. Showcase rooms in the portfolio by adding and managing comprehensive details: Room types, Descriptions, Images, Check-in/check-out times, Costs, Availability.
5. Configure additional settings for a personalized reservation experience: Maximum stay duration, Cancellation policies, Special offers.
6. Confirm instant reflection of changes, ensuring accuracy in the hotel profile and reservation system for users.

**Acceptance Criteria:**
1. Successfully log into the admin panel and navigate to the hotel profile management section.
2. Review and edit hotel details, including the name, contact information, and a brief description.
3. Showcase rooms in the portfolio with detailed information on types, descriptions, images, check-in/check-out times, costs, and availability.
4. Configure additional reservation settings, including maximum stay duration, cancellation policies, and special offers.
5. Confirm that changes made are instantly reflected in both the hotel profile and the reservation system, providing users with accurate and up-to-date information.

   ## Service Provider Interaction Workflow on LocalConnect

**Story:**
- Log into the LocalConnect platform, accessing the service provider account dashboard.
- Review and edit account details, including personal information, skills, services offered, and portfolio items.
- Navigate to the incoming requests section to view user service requests.
- Evaluate user requests and efficiently manage them by either accepting or refusing based on availability and preferences.
- Utilize the integrated chat functionality to engage in real-time communication with users, seeking clarification or providing additional information.
- Confirm accepted requests, ensuring that users receive timely updates on the status of their reservations or service requests.
- Regularly update the portfolio with new work, certifications, and client testimonials to showcase skills and build user confidence.

**Acceptance Criteria:**
1. Successfully log into the LocalConnect platform and access the service provider account dashboard.
2. Edit and update account details, including personal information, skills, services offered, and portfolio items.
3. Navigate to the incoming requests section to view user service requests.
4. Effectively manage requests by accepting or refusing based on availability and preferences.
5. Engage in real-time communication with users through the integrated chat functionality.
6. Ensure that users receive prompt updates on the status of their reservations or service requests.
7. Update the portfolio with new work, certifications, and client testimonials for continuous profile enhancement.





























# System Analysis and Design (SAD) Project

## Project Overview
This project is the final documentation for a System Analysis and Design (SAD) course. It was developed as part of a team assignment, with the primary goal of designing a platform that allows customers to register, log in, and make orders. The project also encompasses different actors such as customers, admins, suppliers, and delivery personnel.

### Team Members
- Mohamed Hisham
- Mohamed Hany
- Shehab Yasser
- Abd El-Rahman Eldeeb

## Use Cases

### 1. Sign-Up
**Actors**: Customer  
**Description**: The Sign-Up use case allows a customer to create a new account on the platform.  
**Typical Flow**:
- The customer initiates the process by filling out a registration form with details like first name, last name, email, and password.
- The system verifies the email for uniqueness and validity, then sends a verification email.
- The user clicks on the verification link, and the system activates their account.

**Precondition**: The user must have access to the registration interface and a valid email address.  
**Postcondition**: The user successfully creates a new account and can log in.  

**Alternate Flows**:
- If the email is already in use or invalid, an error message is displayed.
- The user can request a new verification email if they don't receive one or if the link expires.

---

### 2. Login
**Actors**: Customer, Admin, Supplier, Delivery man  
**Description**: The Login use case allows an existing customer, admin, supplier, or delivery person to access their account.  
**Typical Flow**:
- The user logs in by entering an email and password.
- The system verifies the credentials and directs the user to their respective dashboard.

**Precondition**: The user must have an existing account.  
**Postcondition**: The user successfully logs in and accesses the platform’s functionalities.  

**Alternate Flows**:
- If the email or password is incorrect, the system prompts the user to re-enter the correct information.
- Inactive or banned accounts are denied access.

---

### 3. Make Order
**Actors**: Customer  
**Description**: The Make Order use case describes how a customer submits an order and receives confirmation.  
**Typical Flow**:
- The customer initiates an order.
- The system validates the customer's information, checks product availability, calculates the subtotal and taxes, and verifies payment.
- An order confirmation is generated and sent to the customer.

**Precondition**: Only registered customers can submit orders.  
**Postcondition**: The customer receives an order confirmation, and the order is recorded.  

**Alternate Flows**:
- If a product is unavailable, the system marks it as backordered.
- If invalid product numbers are entered, the system prompts the user to correct them.

---

## Repository Structure
This repository contains various diagrams and documents representing different phases of the project. Here's a breakdown of the folder contents:

### 1. Context
This folder contains the **Context Diagrams**, providing a high-level overview of the system's interactions with external entities, like users and suppliers.

### 2. DFD (Data Flow Diagram)
The **Data Flow Diagrams (DFD)** represent how data moves through the system, including input, output, and data processing activities.

### 3. Use-case
Contains the **Use Case Diagrams** and scenarios that detail how actors (e.g., customer, admin) interact with the system, focusing on key actions like Sign-Up, Login, and Make Order.

### 4. Activity
This folder includes **Activity Diagrams** that show the flow of processes and interactions between different parts of the system, particularly in relation to specific use cases.

### 5. SSD (System Sequence Diagram)
The **System Sequence Diagrams (SSD)** illustrate the message flows between objects and system components during interactions such as placing an order or updating an account.

### 6. SD (State Diagram)
This folder contains **State Diagrams**, detailing the states and transitions of the system as users perform different actions, like registering or placing orders.

### 7. Class
This folder includes **Class Diagrams** that outline the static structure of the system, focusing on relationships between classes, attributes, and methods.

---

## Project Phases

### 1. Requirement Gathering
The team gathered functional and non-functional requirements to define the scope of the system. This phase focused on understanding the needs of the users (customers, admins, suppliers, and delivery personnel).

### 2. System Design
This phase involved designing the system architecture, including the database design and user interface mockups. Various use cases like **Sign-Up**, **Login**, and **Make Order** were defined in detail.

### 3. Implementation
The system was implemented based on the design using appropriate technologies. Each actor's interaction with the system was coded, and the backend for data management was developed.

### 4. Final Documentation
This document is the final phase of the project, summarizing the entire process from requirement gathering to testing, along with detailed descriptions of key use cases.

## Documentation
- **Final documentation**: The comprehensive project documentation, covering all phases of the project lifecycle.

## Conclusion
The System Analysis and Design project successfully resulted in a platform that allows customers to register, log in, and make orders, while also supporting the roles of admins, suppliers, and delivery personnel. Each phase of the project contributed to the complete system lifecycle, from gathering requirements to delivering the final product.

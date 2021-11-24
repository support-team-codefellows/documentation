# application documentation

## Whiteboard

![whiteboard](https://cdn.discordapp.com/attachments/913012327530512394/913175981274071061/Project-Uml.PNG)

## User cases

* As a customer, I want to be able to send customer support cases to the system.
* As a customer, I want to be notified with my case result.
* As an employee, I want to be able to see all the customer support cases along with their status (new case, in-progress, closed).
* As an employee, I want to be able to claim a new customer support case and change its status to in-progress.
* As a manager, I want to be able to monitor all the cases and processes in the system.

## Software requirements

### Vision
This product is a customer service communication tool. It handles all the processes of sending and processing customer service cases for both the customer and server sides. 

### Scope
Customers will be able to sign-up to the system and send their cases.
Employees will be able to view all cases along with their status, claim the cases that belong to their department, and proceed solving them. We have three employee departments: live-chat customer support department, telephone customer support department, and on-site customer support department.
Managers will be able to monitor all the cases and processes in the system.

### Functional Requirements
* A user can create an account
* A user can send customer service cases
* An admin can create employee accounts
* An employee can sign-in to their account
* An employee can get all the customer cases
* An employee that belongs to the one-site department can response to the customer case with an appropriate message
* An employee that belongs to the telephone department can get to the customer’s phone number and proceed solving it with them
* An employee that belongs to the live-chat department can chat with the customer in real-time to solve their case
* An employee can change the status of a case
* An admin can create and delete user accounts

### Data Flow
Still planning, will be updated

## Domain Modeling

Still planning it; working bit by bit 

## Database modeling

We are using Postgres SQL database

### User account schema:

* Email - type: string
* password - type: string
* role - type: string
* token - type: virtual
* capabilities - type: virtual >> user, employee, admin
* username - type: string
* lastname - type: string
* phone - type: string

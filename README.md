# MotorPH Payroll System Documentation

---

## TABLE OF CONTENTS

1. [Introduction](#introduction)
    - [User Roles](#user-roles)
    - [Navigating The User Guide](#navigating-the-user-guide)

2. [Getting Started](#getting-started)
    - [Hardware Prerequisites](#hardware-prerequisites)
    - [Software Prerequisites](#software-prerequisites)
    - [Accessing The System](#accessing-the-system)

3. [Using The Payroll System](#using-the-payroll-system)
    - [Employee Login Functionality](#employee-login-functionality)
    - [Payroll Generation Capability](#payroll-generation-capability)
    - [HR Management Functions](#hr-management-functions)
    - [Leave Management](#leave-management)
    - [Employee Self-Service Portal](#employee-self-service-portal)
    - [Reporting Capabilities for Finance](#reporting-capabilities-for-finance)
    - [System Administrator Functionalities](#system-administrator-functionalities)

4. [Technical Information](#technical-information)
    - [Use Case Diagram](#use-case-diagram)
    - [Class Diagram](#class-diagram)
    - [Testing](#testing)

---

## Introduction

Welcome to the MotorPH Payroll System user guide. This document is designed to provide a comprehensive overview of the system's features and functionalities, ensuring that all users can effectively utilize the platform to manage payroll, employee information, and related tasks. The guide is intended for various user roles within the organization, including system administrators, HR administrators, payroll administrators, and employees. It provides step-by-step instructions, detailed explanations, and practical tips to help you navigate and make the most of the system.

### User Roles

- **System Administrator:** Responsible for managing user accounts, setting access levels, and ensuring the overall security and functionality of the system.
- **HR Administrator:** Handles employee information management, including adding, editing, viewing, and deleting employee records. Also responsible for managing leave requests.
- **Payroll Administrator:** Focuses on generating and saving payslips, ensuring accurate payroll processing, and producing detailed payroll reports.
- **Employee:** Accesses the self-service portal to view personal information, record attendance, submit leave requests, and view payslips.

### Navigating The User Guide

- **Table of Contents:** Start here to quickly locate the section relevant to your needs. Each entry links directly to the corresponding page.
- **Introduction and User Roles:** Begin with these sections to understand the purpose of the system and identify your specific role.
- **Step-by-Step Instructions:** Each functionality is broken down into detailed steps, making it easy to follow along and execute tasks within the system.
- **Screenshots and Diagrams:** Visual aids are provided to illustrate key points and help you familiarize yourself with the interface.
- **Tips and Best Practices:** Look for highlighted tips and best practices to enhance your efficiency and avoid common pitfalls.
- **FAQs and Troubleshooting:** Refer to this section for answers to common questions and solutions to potential issues you may encounter.

---

## Getting Started

This section outlines the fundamental requirements for using the payroll system, including hardware or software prerequisites. It also explains how you can access the system, whether through a web link or dedicated application.

### Hardware Prerequisites

To use the payroll system efficiently, ensure your hardware meets the following minimum requirements:
- Processor: Dual-core processor (2 GHz or faster)
- Memory: 4 GB RAM or more
- Storage: At least 500 MB of free disk space
- Display: 1024 x 768 resolution or higher

### Software Prerequisites

Before accessing the payroll system, make sure you have the following software installed:
- Operating System: Windows 10 or later, macOS 10.14 or later, or a modern Linux distribution
- Java Development Kit (JDK): Version 21
- Web Browser: Latest version of Google Chrome, Mozilla Firefox, Microsoft Edge, or Safari
- Integrated Development Environment (IDE): IntelliJ IDEA, Eclipse, or VS Code (for developers)
- Version Control System: Git

### Accessing The System

Follow these steps to access the payroll system:
- **Web Access:**
  - Open your web browser.
  - Enter the URL provided by your administrator to access the payroll system's web portal.
- **Desktop Application:**
  - If using a dedicated desktop application, download and install the application from the provided link.
  - Launch the application from your desktop or applications menu.
- **Developer Access:**
  - Clone the repository using Git
  - Open the project in your preferred IDE.
  - Navigate to `MainApp.java`, configure the SDK to Java 21, build, and run the application as described previously.

---

## Using The Payroll System

This section covers various user-related actions within the system. The functionalities of the payroll system include the following:

### Employee Login Functionality

#### Launch Application:
1. Git clone the repository.
2. Open the project in your local repository.
3. Navigate to `MainApp.java`.
4. Configure your SDK to Java 21.
5. Build and run the application.

![home](https://github.com/user-attachments/assets/4aaf2310-fad6-4353-879a-903005623265){:width="500px"}

#### Log in with Valid Credentials:
1. Click on the username text field and type the username.
2. Click on the password text field and type the password.
3. Click the Login button to access your profile page.

![sucesslogin](https://github.com/user-attachments/assets/552542f0-d34b-4bb6-9aca-1e27668a52a6){:width="500px"}

#### Submit Forgot Password:

1. Click "Forgot Password" below the login button on the application's login page.
2. Enter your username to request password reset.
3. Wait for the admin to send a verification code to your registered email or phone number.
4. Receive the verification code and enter it on the password reset page.
5. Set a new password following the password requirements provided.
6. Log in using your new password.

![forgotpassword](https://github.com/user-attachments/assets/aabced58-4299-43a4-b6fe-6d34fbee41a8){:width="500px"}

### Payroll Generation Capability

#### Generate and Save Payslips:
1. Click "Generate Payslip".
2. Select start pay date and end pay date.
3. Click "Execute" to review the generated payslips.
4. Click "Save" and confirm the prompt to save the payslips.

![generatepay](https://github.com/user-attachments/assets/ec16e37c-3cce-4416-b626-1e211a674dda){:width="500px"}

The system will display a list of employees for the specified period, including employee info, earnings, deductions, benefits, and summary with take-home pay. Payslips will be saved successfully and automatically distributed to each employee.

#### View and Edit Employee Payslips:
1. Access the "Payslip" section from the dashboard.
2. Review the payslip summary table showing pay period dates, total gross income, and net income per row.
3. Click the "View" button to open a new frame/table listing employees with payslips for the selected period.
4. Edit payslip details such as earnings, deductions, benefits, and net pay.
5. Save changes to update the payslips for the respective employees.

![editpayslip](https://github.com/user-attachments/assets/2e1065af-871a-44d0-a896-e26ff5cb0f23){:width="500px"}

### HR Management Functions

#### Add New Employee and Validate Input:
1. Click "Employees" and then "Add New Employee".
2. Fill in profile, job, account numbers, and salary details.
3. Enter status (only "Regular" or "Probationary") and birthdate in "MM/DD/YYYY" format.
4. Click "Save" and confirm the prompt to save the new employee data. If status or birth date format is invalid, an error message will be shown.

![addem](https://github.com/user-attachments/assets/c4ebbe15-ce8e-4136-bb14-45b1be2881df){:width="500px"}

#### Edit Employee Information:
1. Click "Employees" and search by employee ID.
2. Click the "Edit" button in the Action column.
3. Update profile, job, account numbers, or salary details.
4. Click "Save" and confirm the prompt to save the changes.

![editem](https://github.com/user-attachments/assets/23911efc-06cc-4655-bb41-ed152d000d81){:width="500px"}

#### View and Delete Employee Information:
1. Click "Employees" and search by employee ID.
2. Click the "View" button in the Action column to display employee information.
3. Click the "Delete" button in the Action column and confirm the prompt to delete the employee.

![delete](https://github.com/user-attachments/assets/57286280-f9ea-4055-bc00-c1f6ee9fbad8){:width="500px"}

### Leave Management

#### Approve Leave Request:
1. Click "Leave Request" and select "Pending" from the dropdown.
2. Search by employee ID and click the "Edit" button in the Action column.
3. Update the leave request status to "Approved" and click "Save".
4. Confirm the prompt to approve the leave request.

![approve](https://github.com/user-attachments/assets/595a7434-025f-4dd7-8cdb-6e56f3e13c3a){:width="500px"}

#### Disapprove Leave Request:
1. Click "Leave Request" and select "Pending" from the dropdown.
2. Search by employee ID and click the "Edit" button in the Action column.
3. Update the leave request status to "Disapproved" and click "Save".
4. Confirm the prompt to disapprove the leave request.

![disap](https://github.com/user-attachments/assets/7b6cf2ca-f985-4a55-bd5c-8901228b0f03){:width="500px"}

#### View and Delete Leave Request:
1. Click "Leave Request" and search by employee ID.
2. Click the "View" button in the Action column to display leave request details.
3. Click the "Delete" button in the Action column and confirm the prompt to delete the leave request.

![deleterequest](https://github.com/user-attachments/assets/d5912217-4186-4e1d-a434-457f412a8f40){:width="500px"}

### Employee Self-Service Portal

#### View Personal Information:
1. Navigate to the self-service portal.
2. View personal information, including personal details, allowance breakdown, and salary details.

![vieww](https://github.com/user-attachments/assets/aa9c6c01-9bba-4c25-8aa6-b0f30b2b43c7){:width="500px"}

#### Change Password:
1. Click "Profile" 
2. Navigate to the "Change Password" tab within the employee profile.
3. Enter your existing password into the provided field.
4. Enter your new password
5. Confirm your new password by entering it again.
6. Click "Confirm" or "Update Password."

![changepass](https://github.com/user-attachments/assets/aee99097-fd6c-4aec-9321-9e6038c5c5ca){:width="500px"}

#### Record Time In:
1. Click "Timesheet" and then "Time In".
2. Your time in is recorded and displayed in the table showing the date and time. If you click "Time In" again on the same day, an error message will be displayed.

![timeinn](https://github.com/user-attachments/assets/cb833416-520e-4844-bfc6-fc2a7854c23e){:width="500px"}

#### Record Time Out:
1. Click "Timesheet" and then "Time Out".
2. Confirm the prompt to record your time out. Your time out is recorded and displayed in the table showing the date, time out, regular hours worked, and overtime hours. If you click "Time Out" again on the same day, an error message will be displayed.

![timeoutt](https://github.com/user-attachments/assets/375394cb-0ef0-444d-9058-0f7c38bc4357){:width="500px"}

#### Submit Leave Request:
1. Click "Leave Request" and then "File a Leave Request".
2. Select the leave type and submit the request. Your leave request is submitted, and your leave credits are updated if within the allowed credits. If exceeded, an error message is shown.

![submit](https://github.com/user-attachments/assets/c7333a69-5a20-45a6-90c6-d9ed43f0b6c1){:width="500px"}

#### View Payslip:
1. Click "Payslip" and select a payslip from the list.
2. Your electronic payslip is displayed, containing earnings, deductions, benefits, and summary.

![viewp](https://github.com/user-attachments/assets/84659770-0d10-4723-81b3-777b3b403856){:width="500px"}

### Reporting Capabilities for Finance

#### Generate Payslip Reports:

1. Click "Generate Payslip".
2. Select start pay date and end pay date.
3. Click "Execute" to review the generated payslips of all employees. The list of employees for the specified period is displayed, including employee info, earnings, deductions, benefits, and summary with take-home pay.
4. The system includes a dashboard for reporting and analytics, providing insights into payroll trends, employee attendance patterns, and leave utilization.

![generatepay](https://github.com/user-attachments/assets/ec16e37c-3cce-4416-b626-1e211a674dda){:width="500px"}

![paydashboard](https://github.com/user-attachments/assets/4a2e7bf5-dcfd-42ad-a902-a4d58e1e99bb){:width="500px"}

### System Administrator Functionalities

#### Add New User:
1. Click "User" and then "Add New User".
2. Type employee ID, username, password, and access level (employee, payroll, HR, system administrator, executive, account administrator).
3. Click "Save" and confirm the prompt to add the new user. The new user is added and displayed in the table.

![adduser](https://github.com/user-attachments/assets/217dbb05-357c-4916-8e2e-686d703b75bc){:width="500px"}

#### Edit User and Reset Password:
1. Click "User" and search by user ID.
2. Click the "Edit" button in the Action column.
3. Update access level or click "Reset Password".
4. Click "Update" or confirm the password reset. The user's access level is updated or password is reset.

![shhs](https://github.com/user-attachments/assets/b37065fc-1eaa-46a1-ac8e-7570e96f014a){:width="500px"}

#### View and Delete User:
1. Click "User" and search by user ID.
2. Click the "View" button in the Action column to display user details.
3. Click the "Delete" button in the Action column and confirm the prompt to delete the user. The user is deleted.

![vandd](https://github.com/user-attachments/assets/8d2dfe62-a594-490b-b51a-a472e3b644a4){:width="500px"}

#### View Password Change Request:
1. System Admin clicks on "Change Password Request" in the admin panel or menu.
2. System Admin views a table displaying user IDs and corresponding verification codes for users who requested a password change.

![code](https://github.com/user-attachments/assets/0bcf8d23-89d7-4ef0-b7e5-953a60c97cf0){:width="500px"}

#### Role-Based Access Control:
The system implements role-based access control, ensuring users only have access to functionalities and data relevant to their roles. Security measures protect sensitive payroll and employee data, including encryption, access logs, and regular security audits.

## Technical Information

This section provides details and insights into the inner workings of the payroll system. It includes diagrams, such as use case and class diagrams, to illustrate key technical aspects of the system's design and structure. Additionally, this section references testing documentation, including test cases and results, to highlight the quality assurance processes undertaken during development.

### Use Case Diagram

[![UseCaseDiagram](https://github.com/Jasmin172002/documentation/assets/125138169/4db3b507-c970-4494-ade5-8b21aa7bc433)](https://github.com/Jasmin172002/documentation/assets/125138169/4db3b507-c970-4494-ade5-8b21aa7bc433)
<small>Figure 1: Use Case Diagram of the Expanded Payroll System</small>

The use case diagram illustrates the various interactions between different actors and the payroll system. Below is an explanation of the use case diagram components:

Actors:
- Employee: Interacts with personal account details, attendance records, payslip viewing, leave requests, and time tracking.
- Payroll Administrator: Manages payroll reports, payslip generation, and payroll summaries.
- IT Administrator: Handles system security and user role management.
- HR Administrator: Manages employee records, attendance, leave requests, and approvals.

Use Cases:
- Employee:
  - Time Tracking: Records time in and time out.
  - View Payslip: Access payslips by month or year.
  - View Leave Status: Check approved leave request status.
  - Login: Secure access to the system.
  - Manage Leave: View remaining leave credits and submit leave requests.

- IT Administrator:
  - Role Management: Administers role-based access control.
  - User Management: Manages user accounts.

- Payroll Administrator:
  - Generate Reports: Creates monthly payroll reports and summaries.
  - Generate Payslip: Calculates and saves employee payslips.

- HR Administrator:
  - Employee Management: Adds, modifies, and deletes employee records.
  - Attendance and Leave: Monitors attendance records and manages leave requests.

Interactions:
- All actors log in to access their respective functionalities.
- Generate Payslip involves computing allowances, deductions, and saving payslips.
- Role-Based Access Control ensures secure user access across the system.
- HR Administrator manages employee records, attendance, and leave requests.

### Class Diagram

[![AOOP_S2101 (3)](https://github.com/Jasmin172002/documentation/assets/125138169/6f12c90b-2fd4-47ce-8e9d-b4e0de974db1)](https://github.com/Jasmin172002/documentation/assets/125138169/6f12c90b-2fd4-47ce-8e9d-b4e0de974db1)
<small>Figure 2: Class Diagram of the Expanded Payroll System</small>

This class diagram illustrates the relationships and dependencies between key classes in the payroll system, defining how data flows and interacts within the system's architecture.

Classes and Associations:
- Employee
  - 1..* Department
  - 1..* Allowance
  - 1..1 Timesheet (Composition)
  - 1..* Payslip (Aggregation)
  - 1..1 User (Association)
  - 1..* Role (Aggregation)
  - 1..* LeaveRequest (Association)

- Allowance
  - 1..* Employee

- EmployeePayrollSummaryReport
  - 1..* Deduction (Composition)
  - 1..* Timesheet (Composition)
  - 1..1 Payslip (Aggregation)

- Tax
  - 1..1 TaxCategory (Association)

- Timesheet
  - 1..1 Employee

- Payslip
  - 1..* PayslipViewer (Association)
  - 1..* PayslipImpl (Inheritance)

- User
  - 1..1 Employee

- Role
  - 1..1 Permission (Aggregation)

- Position
  - 1..* Employee

- LeaveRequest
  - 1..1 LeaveRequestCategory (Association)

### Testing


Employee Information Management: All tests passed, ensuring accurate creation, viewing, and updating of employee details.

[![1test](https://github.com/Jasmin172002/documentation/assets/125138169/12b9a86e-1398-4382-ac1e-17e56a6415ba)](https://github.com/Jasmin172002/documentation/assets/125138169/12b9a86e-1398-4382-ac1e-17e56a6415ba)


Time and Attendance Tracking: Successfully created and updated timesheets with accurate data security measures.

[![2test](https://github.com/Jasmin172002/documentation/assets/125138169/a1e36b4a-8851-4a7c-af65-dd98af9ea920)](https://github.com/Jasmin172002/documentation/assets/125138169/a1e36b4a-8851-4a7c-af65-dd98af9ea920)


Salary Calculation: Passed all tests for deduction, gross salary computation, and net salary computation.

[![3test](https://github.com/Jasmin172002/documentation/assets/125138169/c153a593-0563-4d81-8be1-3e0ee41edf22)](https://github.com/Jasmin172002/documentation/assets/125138169/c153a593-0563-4d81-8be1-3e0ee41edf22)


Leave Management: Successfully managed leave requests, ensuring accurate initialization and deduction of leave credits

[![4test](https://github.com/Jasmin172002/documentation/assets/125138169/76630b40-d215-4dd8-9519-22f30300a7fc)](https://github.com/Jasmin172002/documentation/assets/125138169/76630b40-d215-4dd8-9519-22f30300a7fc)



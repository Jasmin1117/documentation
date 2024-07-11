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

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/6036d93c-8913-4d3d-9269-2fd3f0a92b1d" alt="Loginfinal" width="500">

#### Log in with Valid Credentials:
1. Click on the username text field and type the username.
2. Click on the password text field and type the password.
3. Click the Login button to access your profile page.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/10f8fbb0-06ff-4356-a376-c5d4c8112997" alt="loginsuc" width="500">

#### Log in with Invalid Credentials:
1. Click on the username text field and type an incorrect username or password.
2. Click the Login button to see an error message stating, "We couldn't find an account that matches what you entered."

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/8825ce15-33b3-476b-9f43-64486adac451" alt="loginnot" width="500">

#### Submit Forgot Password:

1. Click "Forgot Password" below the login button on the application's login page.
2. Enter your username to request password reset.
3. Wait for the admin to send a verification code to your registered email or phone number.
4. Receive the verification code and enter it on the password reset page.
5. Set a new password following the password requirements provided.
6. Log in using your new password.

<img src="https://github.com/Jasmin172002/AOOPSRS/assets/125138169/fb2a1f1d-bf09-429e-afe2-378593691929" alt="forgotpass" width="500">

### Payroll Generation Capability

#### Generate and Save Payslips:
1. Click "Generate Payslip".
2. Select start pay date and end pay date.
3. Click "Execute" to review the generated payslips.
4. Click "Save" and confirm the prompt to save the payslips.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/19296a34-9114-4368-96dc-4c4556258216" alt="generatepaylip" width="500"/>

The system will display a list of employees for the specified period, including employee info, earnings, deductions, benefits, and summary with take-home pay. Payslips will be saved successfully and automatically distributed to each employee.

#### View and Edit Employee Payslips:
1. Access the "Payslip" section from the dashboard.
2. Review the payslip summary table showing pay period dates, total gross income, and net income per row.
3. Click the "View" button to open a new frame/table listing employees with payslips for the selected period.
4. Edit payslip details such as earnings, deductions, benefits, and net pay.
5. Save changes to update the payslips for the respective employees.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/630af10e-bd5f-48a2-af9e-49fe3f31e418" alt="editp" width="500"/>

### HR Management Functions

#### Add New Employee and Validate Input:
1. Click "Employees" and then "Add New Employee".
2. Fill in profile, job, account numbers, and salary details.
3. Enter status (only "Regular" or "Probationary") and birthdate in "MM/DD/YYYY" format.
4. Click "Save" and confirm the prompt to save the new employee data. If status or birth date format is invalid, an error message will be shown.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/e38b0c34-f2a5-4e7f-95fd-27a795d8da42" alt="addem" width="500"/>

#### Edit Employee Information:
1. Click "Employees" and search by employee ID.
2. Click the "Edit" button in the Action column.
3. Update profile, job, account numbers, or salary details.
4. Click "Save" and confirm the prompt to save the changes.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/6a0f7ee2-dddf-42d7-a567-f77388c0fe2f" alt="editem" width="500"/>

#### View and Delete Employee Information:
1. Click "Employees" and search by employee ID.
2. Click the "View" button in the Action column to display employee information.
3. Click the "Delete" button in the Action column and confirm the prompt to delete the employee.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/09fe8a54-6a14-49e8-8ba9-db092e01fb8a" alt="viewem" width="500"/>

### Leave Management

#### Approve Leave Request:
1. Click "Leave Request" and select "Pending" from the dropdown.
2. Search by employee ID and click the "Edit" button in the Action column.
3. Update the leave request status to "Approved" and click "Save".
4. Confirm the prompt to approve the leave request.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/54754eae-dc50-4dfc-99cb-f75099dfd142" alt="approve" width="500"/>

#### Disapprove Leave Request:
1. Click "Leave Request" and select "Pending" from the dropdown.
2. Search by employee ID and click the "Edit" button in the Action column.
3. Update the leave request status to "Disapproved" and click "Save".
4. Confirm the prompt to disapprove the leave request.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/753644bf-f96b-415c-b51a-aa1635f1fddc" alt="disapp" width="500"/>

#### View and Delete Leave Request:
1. Click "Leave Request" and search by employee ID.
2. Click the "View" button in the Action column to display leave request details.
3. Click the "Delete" button in the Action column and confirm the prompt to delete the leave request.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/55c26bd2-46f5-4d01-9956-98a2b81ff867" alt="viewleave" style="width:500px;">

### Employee Self-Service Portal

#### View Personal Information:
1. Navigate to the self-service portal.
2. View personal information, including personal details, allowance breakdown, and salary details.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/ca391ba5-850d-4198-afa7-c684a7b913ad" alt="viewprof" style="width:500px;">

#### Change Password:
1. Click "Profile" 
2. Navigate to the "Change Password" tab within the employee profile.
3. Enter your existing password into the provided field.
4. Enter your new password
5. Confirm your new password by entering it again.
6. Click "Confirm" or "Update Password."

<img src="https://github.com/Jasmin172002/AOOPSRS/assets/125138169/264dc06f-16a3-4b08-80ca-12ddcbf79d2d" alt="changemypass" width="500"/>

#### Record Time In:
1. Click "Timesheet" and then "Time In".
2. Your time in is recorded and displayed in the table showing the date and time. If you click "Time In" again on the same day, an error message will be displayed.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/63248cad-d969-4384-846a-0fc9dbf46053" alt="timein" style="width:500px;">

#### Record Time Out:
1. Click "Timesheet" and then "Time Out".
2. Confirm the prompt to record your time out. Your time out is recorded and displayed in the table showing the date, time out, regular hours worked, and overtime hours. If you click "Time Out" again on the same day, an error message will be displayed.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/62e6e713-812d-432e-9010-8f0d1b1cc36c" alt="timeout" style="width:500px;">

#### Submit Leave Request:
1. Click "Leave Request" and then "File a Leave Request".
2. Select the leave type and submit the request. Your leave request is submitted, and your leave credits are updated if within the allowed credits. If exceeded, an error message is shown.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/3c987bdc-f908-4411-a314-9a2f04171559" alt="sickleave" style="width:500px;">

#### View Payslip:
1. Click "Payslip" and select a payslip from the list.
2. Your electronic payslip is displayed, containing earnings, deductions, benefits, and summary.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/d194b470-4fca-4192-b773-29ed95b9565a" alt="payslipv" style="width:500px;">

### Reporting Capabilities for Finance

#### Generate Payslip Reports:

1. Click "Generate Payslip".
2. Select start pay date and end pay date.
3. Click "Execute" to review the generated payslips of all employees. The list of employees for the specified period is displayed, including employee info, earnings, deductions, benefits, and summary with take-home pay.
4. The system includes a dashboard for reporting and analytics, providing insights into payroll trends, employee attendance patterns, and leave utilization.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/19296a34-9114-4368-96dc-4c4556258216" alt="generatepaylip" width="500"/>

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/e6ece67b-6a3b-48f0-a3e0-c408c184fb27" alt="fdashboard" style="width:500px;">

### System Administrator Functionalities

#### Add New User:
1. Click "User" and then "Add New User".
2. Type employee ID, username, password, and access level (employee, payroll, HR, system administrator, executive, account administrator).
3. Click "Save" and confirm the prompt to add the new user. The new user is added and displayed in the table.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/df351a08-5e1b-4bab-8683-e2250c6bea88" alt="newuser" style="width:500px;">

#### Edit User and Reset Password:
1. Click "User" and search by user ID.
2. Click the "Edit" button in the Action column.
3. Update access level or click "Reset Password".
4. Click "Update" or confirm the password reset. The user's access level is updated or password is reset.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/54343d8d-eb68-4ab6-9081-a54eb73854e3" alt="ediuserr" style="width:500px;">

#### View and Delete User:
1. Click "User" and search by user ID.
2. Click the "View" button in the Action column to display user details.
3. Click the "Delete" button in the Action column and confirm the prompt to delete the user. The user is deleted.

<img src="https://github.com/Jasmin172002/documentation/assets/125138169/f0fd1962-e11e-4b8c-9369-1ea841425289" alt="delete" style="width:500px;">

#### View Password Change Request:
1. System Admin clicks on "Change Password Request" in the admin panel or menu.
2. System Admin views a table displaying user IDs and corresponding verification codes for users who requested a password change.

<img src="https://github.com/Jasmin172002/AOOPSRS/assets/125138169/e036a7db-c0b5-41b7-9a78-a6d5d871917a" alt="changepass" width="500">

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



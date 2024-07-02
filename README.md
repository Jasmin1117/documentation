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

3. [Using the Payroll System](#using-the-payroll-system)
    - [Secure Login Procedures](#secure-login-procedures)
    - [Salary and Deduction Calculations](#salary-and-deduction-calculations)
    - [Leave Applications](#leave-applications)
    - [System Administrator Functionalities](#system-administrator-functionalities)

4. [Technical Information](#technical-information)
    - [Use Case Diagram](#use-case-diagram)
    - [Class Diagram](#class-diagram)
    - [Testing](#testing)

---

## Introduction

Welcome to the MotorPH Payroll System user guide. This document is designed to provide a comprehensive overview of the system's features and functionalities, ensuring that all users can effectively utilize the platform to manage payroll, employee information, and related tasks. The guide is intended for various user roles within the organization, including system administrators, HR administrators, payroll administrators, and employees. It provides step-by-step instructions, detailed explanations, and practical tips to help you navigate and make the most of the system's capabilities. Whether you're setting up user accounts, generating payslips, or submitting leave requests, this guide will assist you every step of the way.

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
    - Clone the repository using Git: `git clone [repository URL]`
    - Open the project in your preferred IDE.
    - Navigate to `MainApp.java`, configure the SDK to Java 21, build, and run the application as described previously.

---

## Using The Payroll System

This section covers various user-related actions within the system. The functionalities of the payroll system include the following:

### Secure Login Procedures

- **Launch Application:**
    - Git clone the repository.
    - Open the project in your local repository.
    - Navigate to `MainApp.java`.
    - Configure your SDK to Java 21.
    - Build and run the application.
<br>

    
  <img src="src/main/resources/img/Launch.png" alt="Launch Image" width="500" />

- **Log in with Valid Credentials:**
    - Click on the username text field and type the username.
    - Click on the password text field and type the password.
    - Click the Login button to access your profile page.

<img src="src/main/resources/video/LoginSuccess.gif" alt="Login Success Animation" width="500" />

- **Log in with Invalid Credentials:**
    - Click on the username text field and type an incorrect username or password.
    - Click the Login button to see an error message stating, "We couldn't find an account that matches what you entered."

<img src="src/main/resources/video/LoginFailed.gif" alt="Login Failed Animation" width="500" />

### Salary and Deduction Calculations

- **Payroll Generation Capability:**
    - Click "Generate Payslip".
    - Select start pay date and end pay date.
    - Click "Execute" to review the generated payslips.
    - Click "Save" and confirm the prompt to save the payslips.
    - The system will display a list of employees for the specified period, including employee info, earnings, deductions, benefits, and summary with take-home pay. Payslips will be saved successfully and automatically distributed to each employee.

### HR Management Functions

- **Add New Employee and Validate Input:**
    - Click "Employees" and then "Add New Employee".
    - Fill in profile, job, account numbers, and salary details.
    - Enter status (only "Regular" or "Probationary") and birthdate in "MM/DD/YYYY" format.
    - Click "Save" and confirm the prompt to save the new employee data. If status or birth date format is invalid, an error message will be shown.
- **Edit Employee Information:**
    - Click "Employees" and search by employee ID.
    - Click the "Edit" button in the Action column.
    - Update profile, job, account numbers, or salary details.
    - Click "Save" and confirm the prompt to save the changes.
- **View and Delete Employee Information:**
    - Click "Employees" and search by employee ID.
    - Click the "View" button in the Action column to display employee information.
    - Click the "Delete" button in the Action column and confirm the prompt to delete the employee.

### Leave Management

- **Approve Leave Request:**
    - Click "Leave Request" and select "Pending" from the dropdown.
    - Search by employee ID and click the "Edit" button in the Action column.
    - Update the leave request status to "Approved" and click "Save".
    - Confirm the prompt to approve the leave request.
- **Disapprove Leave Request:**
    - Click "Leave Request" and select "Pending" from the dropdown.
    - Search by employee ID and click the "Edit" button in the Action column.
    - Update the leave request status to "Disapproved" and click "Save".
    - Confirm the prompt to disapprove the leave request.
- **View and Delete Leave Request:**
    - Click "Leave Request" and search by employee ID.
    - Click the "View" button in the Action column to display leave request details.
    - Click the "Delete" button in the Action column and confirm the prompt to delete the leave request.

### System Administrator Functionalities

- **Add New User:**
    - Click "User" and then "Add New User".
    - Type employee ID, username, password, and access level (employee, payroll, HR, system administrator, executive, account administrator).
    - Click "Save" and confirm the prompt to add the new user. The new user is added and displayed in the table.
- **Edit User and Reset Password:**
    - Click "User" and search by user ID.
    - Click the "Edit" button in the Action column.
    - Update access level or click "Reset Password".
    - Click "Update" or confirm the password reset. The user's access level is updated or password is reset.
- **View and Delete User:**
    - Click "User" and search by user ID.
    - Click the "View" button in the Action column to display user details.
    - Click the "Delete" button in the Action column and confirm the prompt to delete the user. The user is deleted.

### Role-Based Access Control

The system implements role-based access control, ensuring users only have access to functionalities and data relevant to their roles. Security measures protect sensitive payroll and employee data, including encryption, access logs, and regular security audits.

---

## Technical Information

This section provides details and insights into the inner workings of the payroll system. It includes diagrams, such as use case and class diagrams, to illustrate key technical aspects of the system's design and structure. Additionally, this section references testing documentation, including test cases and results, to highlight the quality assurance processes undertaken during development.

### Use Case Diagram

[Insert Use Case Diagram here]

### Class Diagram

[Insert Class Diagram here]

### Testing

[Insert Testing details here]

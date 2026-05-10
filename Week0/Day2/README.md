# Day 2 - Salesforce Platform Basics

## What is Salesforce Platform?

Salesforce Platform is a cloud-based platform that helps businesses build applications, manage data, automate workflows, and develop CRM solutions.

The platform provides:
- Data management
- Automation tools
- Security
- Reporting and analytics
- App development features
- CRM functionality

Salesforce allows developers and admins to extend functionality using configuration tools and coding.

---

# What is an App in Salesforce?

An App is a collection of tabs, objects, and tools designed for a specific business process.

Apps help users access all related features in one place.

Examples:
- Sales App
- Service App
- College Admission Management App

---

# What is an Object?

An Object is like a database table used to store information in Salesforce.

Objects contain:
- Records
- Fields
- Relationships

## Standard Objects
Objects already provided by Salesforce:
- Account
- Contact
- Opportunity

## Custom Objects
Objects created according to business needs:
- Student
- Course
- Faculty
- Attendance
- Fees

---

# What is a Tab?

A Tab is a user interface element used to access objects, records, and pages.

Tabs help users navigate inside an app.

Examples:
- Students Tab
- Courses Tab
- Reports Tab

---

# CRM Concepts Connected to Salesforce Platform

CRM concepts are implemented inside Salesforce using apps and objects.

| CRM Concept | Salesforce Representation |
|---|---|
| Account | College |
| Contact | Student |
| Lead | Student Inquiry |
| Opportunity | Admission Process |
| Customer | Enrolled Student |

## Business Flow

Lead → Contact → Opportunity → Customer

Example:
Student inquiry → Student details stored → Admission process → Student enrolled successfully

---

# Configuration vs Coding

## Configuration (No Code)

Configuration means customizing Salesforce using clicks instead of programming.

Used for:
- Creating fields
- Validation rules
- Workflows
- Page layouts
- Reports

### Examples
1. Creating a Student object
2. Sending automatic email notifications

### Advantages
- Faster development
- Easy maintenance
- No coding knowledge required

---

## Coding (Apex)

Coding is used when business requirements become complex.

Salesforce developers use Apex programming language for advanced logic.

Used for:
- Complex automation
- Integrations
- Custom calculations
- Advanced business logic

### Examples
1. Scholarship eligibility calculation
2. Integration with payment systems

### Advantages
- Highly customizable
- Supports advanced functionality

---

# Difference Between App and Object

| App | Object |
|---|---|
| Collection of features and tabs | Stores data |
| Used for navigation | Used for records |
| Contains multiple objects | Contains fields and records |

## Example
- College Management = App
- Student = Object

---

# What is Multi-Tenant Architecture?

Multi-tenant architecture means multiple organizations use the same Salesforce infrastructure securely.

Each company’s data remains private and isolated.

## Benefits
- Lower infrastructure cost
- Automatic updates
- Scalability
- Better resource usage

Example:
Multiple colleges can use Salesforce without accessing each other’s data.

---

# System Design - College Admission Management App

## App Name
College Admission Management App

---

## Objects Inside the App

### Standard Objects
- Account
- Contact
- Opportunity

### Custom Objects
- Student
- Faculty
- Course
- Attendance
- Fees
- Examination

---

# How Users Interact with the System

## Admin
- Manage admissions
- Create courses
- Generate reports

## Faculty
- Update attendance
- Upload marks

## Students
- View attendance
- Check results
- Access course details

---

# How Salesforce Developers Extend Functionality

Developers extend Salesforce using:
- Apex
- Lightning Components
- APIs
- Integrations
- Custom objects
- Automation tools

This helps businesses build custom solutions according to their requirements.

---

# Screenshots

Add:
- Trailhead completion screenshots
- Playground screenshots

inside the screenshots folder.

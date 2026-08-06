# Placement Management System – Sprint 7 (Engineering Sprint Part II)

## Introduction

This sprint is a continuation of the Placement Management System project developed in Salesforce. In the previous sprint, the application was able to process student job applications. In this sprint, the main focus is to improve the application's performance by following Salesforce best practices.

The implementation demonstrates how to process multiple application records efficiently using Apex Bulkification. It also explains how Salesforce Governor Limits affect Apex code and how to design applications that can handle large amounts of data without causing errors.

---

# Project Objective

The main objective of this sprint is to build a scalable and efficient Placement Management System by:

* Processing multiple application records at the same time.
* Avoiding unnecessary database operations.
* Following Salesforce Governor Limits.
* Writing clean, reusable, and maintainable Apex code.

---

# Project Scenario

The Placement Management System allows students to apply for available job openings.

Whenever a student submits an application:

* The application is received by an Apex Trigger.
* The student's information is retrieved.
* The selected job details are retrieved.
* The student's CGPA is compared with the job's minimum CGPA requirement.
* Based on the comparison, the application status is updated.

Instead of processing one application at a time, the system is designed to process many applications together using Salesforce bulk processing techniques.

---

# Technologies Used

* Salesforce Platform
* Apex Programming Language
* SOQL (Salesforce Object Query Language)
* Developer Console
* Custom Objects
* Collections (List, Set, and Map)

---

# Salesforce Objects Used

The following custom objects are used in this project:

### Student__c

Stores student information such as:

* Student Name
* CGPA
* Email

### Job__c

Stores job details such as:

* Job Title
* Minimum CGPA Required

### Application__c

Stores the job application submitted by students.

---

# Implementation Steps

The following steps were completed during this sprint:

### Step 1

Created an Apex Trigger on the **Application__c** object.

The trigger automatically executes whenever a new application is created.

---

### Step 2

Passed all application records from **Trigger.new** to the service class.

This allows the application to process multiple records together instead of processing only one record.

---

### Step 3

Collected all unique Student IDs using a **Set**.

Using a Set removes duplicate Student IDs and helps reduce unnecessary processing.

---

### Step 4

Retrieved all Student records using a single SOQL query.

Instead of executing one query for every application, only one database query is used.

---

### Step 5

Stored all Student records inside a **Map**.

The Map allows quick access to student information without executing additional queries.

---

### Step 6

Collected all Job IDs from the application records.

These IDs are later used to retrieve the required Job records.

---

### Step 7

Retrieved all Job records using one SOQL query and stored them in another Map.

This follows Salesforce bulkification best practices.

---

### Step 8

Validated every application.

For each application:

* Student details were retrieved from the Student Map.
* Job details were retrieved from the Job Map.
* Student CGPA was compared with the minimum CGPA required for the selected job.
* The application status was updated based on the validation result.

---

# Salesforce Best Practices Followed

During this sprint, the following best practices were implemented:

* Used Trigger.new to process multiple records.
* Used Sets to remove duplicate IDs.
* Used Maps for faster record access.
* Executed a single SOQL query instead of multiple queries.
* Avoided SOQL statements inside loops.
* Avoided DML statements inside loops.
* Separated business logic from the Trigger by using a Service Class.

These practices help the application perform efficiently even when hundreds of records are processed at once.

---

# What I Learned

After completing this sprint, I gained knowledge about:

* Salesforce Governor Limits
* Bulk Processing
* Apex Bulkification
* Using Lists, Sets, and Maps
* Writing efficient SOQL queries
* Processing records in memory
* Service Layer Architecture
* Salesforce Trigger Best Practices

---

# Conclusion

Sprint 7 helped me understand how to build scalable Salesforce applications that can efficiently handle multiple records. I learned how Bulkification improves application performance and how Salesforce Governor Limits influence Apex development.

By using collections such as Lists, Sets, and Maps, along with a single SOQL query for related records, the Placement Management System became more efficient, easier to maintain, and better suited for real-world enterprise applications.

---

# Author

**Nandam Josh Nihanth**

**B.Tech – Computer Science and Engineering**

**Salesforce Engineering Sprint 7 – Placement Management System**

# Salesforce Interview Readiness Bootcamp – Day 3

## Project Title

**Placement Management System using Salesforce Flows and Validation Rules**

## Objective

The objective of this project is to implement Salesforce declarative automation using Validation Rules and Record-Triggered Flows. The system automates the placement application process, improves data quality, and reduces manual effort without writing Apex code.

---

## Features Implemented

* Created custom objects:

  * Student
  * Job
  * Application
  * Offer Letter

* Configured custom fields and lookup relationships.

* Implemented a **Before-Save Record-Triggered Flow** to automatically populate the **Application Date**.

* Implemented an **After-Save Record-Triggered Flow** to send an email notification when a new application is submitted.

* Created Validation Rules to:

  * Validate the student's CGPA against the job's minimum CGPA.
  * Prevent applications after the job closing date.
  * Ensure mandatory fields are completed.

* Implemented an **After-Save Record-Triggered Flow** to automatically create an **Offer Letter** when the application status changes to **Selected**.

---

## Salesforce Components Used

* Custom Objects
* Custom Fields
* Lookup Relationships
* Record-Triggered Flows
* Validation Rules
* Flow Builder
* Email Action

---

## Validation Rules

### Rule 1 – Reject Low CGPA

Checks whether the student's CGPA is lower than the minimum CGPA required for the selected job.

### Rule 2 – Application Date Validation

Ensures the Application Date is not later than the Job Closing Date.

### Rule 3 – Mandatory Fields

Prevents saving an application when required fields are left blank.

---

## Flows Created

### Flow 1 – Auto Populate Application Date

* Type: Before-Save Record-Triggered Flow
* Object: Application
* Purpose: Automatically sets the Application Date to the current date.

### Flow 2 – Email Notification

* Type: After-Save Record-Triggered Flow
* Object: Application
* Purpose: Sends an email notification whenever a new application is created.

### Flow 3 – Create Offer Letter

* Type: After-Save Record-Triggered Flow
* Object: Application
* Purpose: Creates an Offer Letter automatically when the Application Status changes to **Selected**.

---

## Testing Results

* Application Date was populated automatically.
* Email notification was sent successfully.
* Validation Rules prevented invalid data from being saved.
* Offer Letter record was created automatically when the status changed to **Selected**.

---

## Learning Outcomes

Through this assignment, I gained practical experience in:

* Salesforce declarative automation
* Record-Triggered Flows
* Validation Rules
* Flow Builder
* Business process automation
* Data validation
* Salesforce best practices

---

## Conclusion

This project successfully demonstrates the use of Salesforce declarative automation to build an efficient Placement Management System. By implementing Flows and Validation Rules, manual work was reduced, data quality was improved, and business processes were automated without using Apex.

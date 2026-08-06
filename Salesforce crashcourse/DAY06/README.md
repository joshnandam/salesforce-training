# Salesforce Engineering Sprint – Day 6
## Making Software Talk to Data (SOQL & DML)

### Overview
This sprint focuses on understanding how Salesforce applications retrieve, validate, and store data using **SOQL (Salesforce Object Query Language)** and **DML (Data Manipulation Language)**. The implementation was carried out using the Placement Management System project developed in the previous sprints.

The main objective of this task was to build a complete application submission process by retrieving student and job details, validating eligibility, preventing duplicate applications, and creating application records.

---

## Learning Objectives

- Understand the purpose of SOQL in Salesforce.
- Retrieve records from custom objects.
- Apply business validations using Apex.
- Prevent duplicate records.
- Create records using DML.
- Update existing records.
- Test Apex methods using Execute Anonymous.

---

## Project Scenario

A student applies for a job through the Placement Management System.

Before creating the application, the system performs the following validations:

- Retrieves the student's details.
- Retrieves the selected job information.
- Checks whether the student has already applied.
- Verifies the student's CGPA against the job requirement.
- Creates the application record if all conditions are satisfied.
- Returns an appropriate confirmation message.

---

## Features Implemented

### Retrieve Student Information
Used SOQL to retrieve the student's CGPA from the Student object.

### Retrieve Job Information
Retrieved the minimum CGPA requirement from the Job object.

### Duplicate Application Check
Prevented students from applying for the same job more than once.

### Eligibility Validation
Compared the student's CGPA with the job's minimum CGPA before allowing the application.

### Create Application Record
Created a new Application record with the student, job, and application date.

### DML Operations
- Inserted new application records.
- Implemented a method to update application status.

### Testing
Verified the implementation using the Execute Anonymous Window in the Developer Console.

---

## Technologies Used

- Salesforce Developer Edition
- Apex
- SOQL
- DML
- Visual Studio Code
- Salesforce CLI
- Developer Console

---

## Files Included

```
ApplicationService.cls
ApplicationService.cls-meta.xml
README.md
Documentation.pdf
Screenshots/
```

---

## Output

The application submission process was tested successfully.

The system was able to:

- Retrieve student information.
- Retrieve job details.
- Prevent duplicate applications.
- Validate eligibility.
- Create a new application record.
- Send a confirmation email after successful submission.

---

## Key Concepts Covered

- SOQL Queries
- DML Insert
- DML Update
- Apex Classes
- Business Logic
- Duplicate Record Validation
- Eligibility Validation
- Execute Anonymous Testing

---

## Learning Outcome

Through this sprint, I gained practical experience in working with Salesforce data using SOQL and DML. I learned how to retrieve records, apply business validations, create new records, and test Apex methods within a real-world Placement Management System. This sprint also improved my understanding of implementing business processes using Apex.

---

## Conclusion

Day 6 focused on connecting Apex code with Salesforce data. By combining SOQL and DML, I successfully implemented a complete application submission workflow that follows real business requirements. This sprint strengthened my understanding of Salesforce data operations and prepared me for the next topic, Apex Triggers.

---

**Author:** Nandam Josh Nihanth  
**Course:** Salesforce Engineering Sprint  
**Day:** 6  
**Topic:** Making Software Talk to Data (SOQL & DML)

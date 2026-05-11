# Day 3 - Salesforce Data Modeling

# What is Data Modeling?

Data modeling is the process of organizing and structuring business data using objects, fields, records, and relationships.

It helps companies:
- Store data properly
- Maintain relationships between records
- Reduce duplication
- Improve reporting and automation

---

# Difference Between App, Object, Record, and Field

| Term | Meaning | Example |
|---|---|---|
| App | Collection of related features and tabs | College Management App |
| Object | Database table that stores data | Student Object |
| Record | Single row of data inside an object | One student’s information |
| Field | Individual data attribute | Student Name |

---

# Standard vs Custom Objects

## Standard Objects

Objects already provided by Salesforce.

Examples:
- Account
- Contact
- Opportunity
- Lead

These are commonly used CRM objects.

---

## Custom Objects

Objects created according to business requirements.

Examples:
- Student
- Faculty
- Course
- Department
- Attendance

Custom objects allow businesses to build custom business systems on Salesforce.

---

# College Management System Data Model

## Objects

### Student
Stores student details.

Fields:
- Student Name
- Email
- Age
- Department
- Double Age (Formula Field)

---

### Faculty
Stores faculty information.

Fields:
- Faculty Name
- Email
- Experience

---

### Course
Stores course information.

Fields:
- Course Name
- Total Seats

---

### Department
Stores department details.

Fields:
- Department Name
- HOD Name

---

# Relationships Between Objects

| Parent Object | Child Object | Relationship Type |
|---|---|---|
| Department | Student | Lookup |
| Department | Faculty | Lookup |
| Department | Course | Lookup |
| Faculty | Course | Lookup |

---

# Relationship Explanation

## Department → Student
One department can contain many students.

Example:
Computer Science department has multiple students.

---

## Department → Faculty
One department can have many faculty members.

---

## Department → Course
One department can offer multiple courses.

---

## Faculty → Course
One faculty member can teach multiple courses.

---

# One-to-Many Relationships

Examples:
- One Department → Many Students
- One Department → Many Faculty
- One Faculty → Many Courses

Relationships help connect business data efficiently.

---

# Why Lookup Relationships?

Lookup relationships are used when:
- Objects are related
- But can exist independently

Example:
A Student belongs to a Department, but both records can exist separately.

Lookup relationships provide flexibility in enterprise systems.

---

# College Data Model Diagram

```text
Department
   │
   ├── Student
   ├── Faculty
   └── Course

Faculty
   │
   └── Course

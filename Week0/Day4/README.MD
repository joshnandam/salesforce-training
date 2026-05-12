# Day 4 - Salesforce Flow Builder and Automation

# What is Flow Builder?

Flow Builder is a no-code automation tool in Salesforce used to automate business processes and workflows.

It allows businesses to:
- Automate repetitive tasks
- Update records automatically
- Send notifications
- Make decisions using conditions
- Improve productivity

Flow Builder helps companies reduce manual work without writing code.

---

# Why Businesses Need Automation

Businesses automate processes to:
- Save time
- Reduce human errors
- Improve efficiency
- Increase productivity
- Maintain consistency

Automation helps organizations handle repetitive tasks faster and more accurately.

---

# Types of Flows

## Screen Flow

Screen Flow is an interactive flow that requires user input through screens.

### Uses
- Forms
- Guided processes
- User data collection

### Example
Student admission form.

---

## Record Triggered Flow

Record Triggered Flow runs automatically when a record is created, updated, or deleted.

### Uses
- Automatic updates
- Notifications
- Record processing

### Example
Send email automatically after student registration.

---

# Automation Ideas for College Management System

## 1. Auto Email After Registration

When a student registers, Salesforce automatically sends a confirmation email.

### Why automation helps
- Faster communication
- Saves manual work
- Better user experience

---

## 2. Auto Update Remaining Seats

Remaining seats reduce automatically after admission.

### Why automation helps
- Prevents overbooking
- Maintains accurate records

---

## 3. Notify Faculty When Course Is Full

Faculty receives automatic notification.

### Why automation helps
- Faster response
- Better coordination

---

## 4. Generate Student ID Automatically

Salesforce automatically generates unique student IDs.

### Why automation helps
- Prevents duplicate IDs
- Saves time

---

## 5. Fee Deadline Reminder

Automatic reminders sent before payment due dates.

### Why automation helps
- Reduces late payments
- Improves communication

---

# Flow Design Example

## Automation Process
Auto Email After Registration

## Flow Steps

1. Student registration record created
2. Flow triggers automatically
3. Check whether email exists
4. Send confirmation email
5. Update registration status

---

# Simple Flow Diagram

```text
Student Registration
        ↓
Record Created
        ↓
Check Email Exists?
        ↓
      Yes
        ↓
Send Confirmation Email
        ↓
Update Student Status

# Day 5 - Apex Introduction and Business Logic

# What is Apex?

Apex is a programming language developed by Salesforce for implementing custom business logic and automation on the Salesforce platform.

Apex is similar to Java and is used when declarative tools like Flows and Validation Rules are not enough to solve complex business requirements.

Using Apex, developers can:
- Write custom business logic
- Perform database operations
- Integrate external systems
- Automate advanced processes
- Handle complex calculations

Apex runs securely on the Salesforce platform.

---

# Why Salesforce Needs Programming

Salesforce provides many no-code and low-code tools such as:
- Flows
- Validation Rules
- Formula Fields
- Process Automation

However, some enterprise business requirements become too complex for declarative tools.

Examples:
- Advanced calculations
- External API integrations
- Dynamic business rules
- Complex conditional logic
- Bulk data processing

In such cases, Apex programming is required.

---

# Declarative vs Programmatic Development

| Declarative Development | Programmatic Development |
|---|---|
| Uses clicks and configuration | Uses code |
| Faster for simple automation | Better for complex logic |
| Easier for admins | Used by developers |
| Examples: Flow, Validation Rules | Examples: Apex, Triggers |

---

# Flow vs Apex

| Flow | Apex |
|---|---|
| No-code automation | Code-based automation |
| Easier to build | More flexible |
| Good for simple workflows | Good for complex business logic |
| Limited for advanced integrations | Supports advanced integrations |

---

# Basic Apex Concepts

## Variables

Variables store data values.

Example:
```apex
Integer age = 20;
String studentName = 'Rahul';

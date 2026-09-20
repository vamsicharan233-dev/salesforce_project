\# HandsMen Threads - Salesforce Project

Project Demonstration Video

Google Drive:
https://drive.google.com/file/d/1DDGhNZj1NDReATk8B7vyY5ILgmg7YtEv/view?usp=drive_link


\## 📌 Project Overview



HandsMen Threads is a Salesforce-based CRM and business operations solution developed for a fashion business.



The project manages customers, products, orders, inventory, and marketing campaigns using Salesforce.



The system uses Salesforce configuration, automation, security features, Apex Triggers, Batch Apex, and Scheduled Apex to improve order processing, inventory management, customer communication, and loyalty management.



\---



\## 🎯 Objectives



The main objectives of this project are:



\- Create a structured Salesforce data model.

\- Manage customer, product, order, inventory, and campaign information.

\- Maintain accurate business data using validation rules and formula fields.

\- Automate order confirmation emails.

\- Send low-stock alerts to the inventory team.

\- Automatically update customer loyalty status.

\- Implement role-based access and permissions.

\- Use Apex for business rules and stock management.

\- Use Batch Apex for bulk inventory processing.

\- Test the complete functionality using sample records.



\---



\## 🛠️ Technologies and Salesforce Features



\- Salesforce Lightning Experience

\- Custom Objects

\- Custom Fields

\- Formula Fields

\- Lookup Relationships

\- Master-Detail Relationships

\- Validation Rules

\- Profiles

\- Roles

\- Permission Sets

\- Email Templates

\- Email Alerts

\- Record-Triggered Flows

\- Scheduled Flows

\- Apex Triggers

\- Apex Classes

\- Batch Apex

\- Scheduled Apex

\- SOQL

\- DML



\---



\## 🗃️ Data Model



The project contains five main custom objects:



| Object | Purpose |

|---|---|

| HandsMen Customer | Stores customer information and loyalty details |

| HandsMen Product | Stores product catalogue, pricing and stock information |

| HandsMen Order | Stores customer orders and order status |

| Inventory | Tracks product stock and warehouse information |

| Marketing Campaign | Manages promotional campaigns and customer association |



\### Relationships



\- HandsMen Order → HandsMen Customer

\- HandsMen Order → HandsMen Product

\- Inventory → HandsMen Product

\- Marketing Campaign → HandsMen Customer



\---



\## 🔐 Security



Salesforce security is implemented using:



\- Profiles

\- Role Hierarchy

\- Users

\- Permission Sets



The project includes roles such as:



\- Sales Manager

\- Inventory Manager

\- Marketing Manager



These roles provide access according to the user's business responsibilities.



\---



\## ✅ Validation and Data Quality



Formula fields are used for:



\- Customer Full Name

\- Inventory Stock Status



Validation rules are implemented for:



\- Order Total Amount

\- Inventory Stock Quantity

\- Customer Email



These rules prevent invalid records from being saved.



\---



\## ⚙️ Automation



\### 1. Order Confirmation



When an order status changes to \*\*Confirmed\*\*, Salesforce automatically sends an order confirmation email.



\### 2. Low Stock Alert



When inventory stock falls below the defined threshold, Salesforce sends a low-stock alert to the inventory team.



\### 3. Loyalty Status Update



A scheduled flow updates customer loyalty status based on total purchases.



Possible loyalty levels are:



\- Gold

\- Silver

\- Bronze



\---



\## 💻 Apex Development



Apex is used to implement transaction-level business logic.



\### Order Validation



The Order Trigger uses an `OrderTriggerHandler` to validate order quantity according to the order status.



\### Order Total Calculation



The order total is calculated using:



```text

Total Amount = Quantity × Product Price


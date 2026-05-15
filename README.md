# Internal Email Automation Workflow (Make + Google Sheets)

## My Role
Workflow Automation and Integration Specialist

---

## Project Overview
This project is a **two-scenario automation workflow built in Make.com** for managing business email campaigns using **Google Sheets**.

The system is designed to automate bulk communication by filtering contacts, sending templated emails, and tracking delivery results in real time.

The main goal was to eliminate manual email sending, ensure accurate targeting, and provide reliable reporting on campaign performance.

---

## Workflow Structure

The automation consists of two connected scenarios:

### 🔹 Scenario 1 – Contact Processing & Trigger
This scenario handles data preparation and routing:

- Retrieve client records from Google Sheets (Search Rows)  
- Filter contacts with active marketing subscriptions  
- Create structured JSON payload for further processing  
- Send data via HTTP request to Scenario 2 (webhook)  
- Update Google Sheets with initial processing status  

---

### 🔹 Scenario 2 – Notification Delivery
This scenario receives data from Scenario 1 via webhook:

- Receive incoming data via webhook trigger  
- Process received contact information  
- Send notification message to team member  
- Log execution status (if required in scenario setup)  

---

## Post-Processing
- Google Sheets is updated in Scenario 1 based on initial processing state  
- Scenario 2 operates independently as a notification delivery layer  

---

## Workflow Screenshots

The images below show the full two-scenario automation workflow implemented in Make.com:

### Scenario 1 – Contact Filtering & Trigger
<img width="1256" height="312" alt="email-scenario-1 png" src="https://github.com/user-attachments/assets/273ee907-e86a-402a-a994-978ebc89c07d" />

### Scenario 2 – Email Sending & Response
<img width="620" height="331" alt="email-scenario-2 png" src="https://github.com/user-attachments/assets/4054ceab-b08a-4f95-9142-3d2bc177ccf0" />

---

## Key Features
- Two-scenario modular automation architecture  
- Google Sheets-based contact management  
- Subscription-based contact filtering  
- Scenario-based webhook communication between modules  
- Template-based email sending  
- Delivery status tracking (success/failure)  
- Automated reporting back to Google Sheets  
- Scalable bulk email processing  

---

## Result
- Fully automated email campaign execution  
- Reduced manual email sending workload  
- Improved targeting accuracy  
- Reliable delivery tracking and reporting  
- Scalable system for bulk communication  

---

## Tools Used
- Make.com (automation & scenario orchestration)
- Google Sheets (data management & tracking)
- Webhooks (scenario-to-scenario communication)

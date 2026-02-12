# **SaddleData Public Roadmap**

Welcome to the official public roadmap for SaddleData\! This repository provides visibility into our product development process. It's where we track what we're working on, what's coming up next, and where we gather essential feedback from our community of users.

We believe in building in public and want to give you a voice in shaping the future of SaddleData.

**Please Note:** This roadmap is for informational purposes only and is subject to change. Priorities can shift based on customer feedback, market changes, and new opportunities.

## **How to Contribute**

The best way to provide feedback or suggest a new feature is to:

1. Check the existing [Issues](https://github.com/saddledata/roadmap/issues) to see if your idea is already being discussed.  
2. If it is, please add your thoughts to the existing issue\!  
3. If it's a new idea, please [open a new issue](https://github.com/saddledata/roadmap/issues/new/choose), providing as much detail as possible about the problem you're trying to solve.

## **The Roadmap: Now, Next, Later**

We use the "Now, Next, Later" framework to communicate our priorities.

### **Legend**

* 🚀 Shipped \- Recently completed and deployed.  
* 🚧 In Progress \- Actively in the development and testing phase.  
* 📝 In Planning \- In the final stages of design and will be worked on next.  
* 💡 Idea / Backlog \- A feature or idea we want to work on in the future.

### **✅ Recently Shipped**

* **Flow Detail & Monitoring Page:** A dedicated UI page to monitor the health, history, and configuration of a specific flow.  
* **Email-Based User Invitations:** A secure, email-based system for inviting new members to an organization.  
* **MySQL Connector:** Full source and destination support for MySQL databases.
* **Feature: Schema Drift Detection:** A system to automatically detect changes in a source's schema (e.g., new columns, renamed columns) and alert the user. ([Issue \#9](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/9))  
* **Feature: Remote Runner:** An optional, self-hosted agent that can run within a customer's private network (VPC) to securely access data sources without exposing them to the public internet. ([Issue \#10](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/10))  
* **Connector: Snowflake Destination:** Add support for loading data into Snowflake.  
* **Connector: Stripe Source:** Add a source connector to extract payment, subscription, and customer data from Stripe.  
* **Connector: HubSpot Source:** Add a source connector for extracting CRM data from HubSpot.

### **🚧 Now (Actively in Progress \- Q4 2025\)**

* **Feature: Proactive Failure Alerting:** Implement a system to send email notifications when a flow run fails, including the error message and a link back to the UI. ([Issue \#6](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/6))
* **Connector Validation & Launch Epic:**  
  * Final testing and validation for the **BigQuery Destination** connector. ([Issue \#1](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/1))  
  * Final testing and validation for the **AWS Cost & Usage Report (Billing)** source connector. ([Issue \#2](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/2))  
  * Final testing and validation for the **Metronome** source connector. ([Issue \#3](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/3))  
* **Public Documentation Site:** Create and launch the initial version of docs.saddledata.io using a static site generator. ([Issue \#4](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/4))  
* **Link Docs in UI:** Update the main application UI with a persistent link to the new documentation site. ([Issue \#5](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/5))

### **📝 Next (Up Next)**

* **Security: Two-Factor Authentication (2FA/MFA):** Add support for users to secure their accounts with an authenticator app. ([Issue \#7](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/7))  
* **User Onboarding Guide:** Create a comprehensive "Getting Started" guide, including a short video tutorial, to improve the new user experience. ([Issue \#8](https://www.google.com/search?q=https://github.com/flowslate/roadmap/issues/8))

### **💡 Later (Future Ideas & Backlog)**

* \*\*API: Webhook Destinations
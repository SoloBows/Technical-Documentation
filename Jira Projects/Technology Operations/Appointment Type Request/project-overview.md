# 📅 Appointment Type Custom Ticket - Technology Operations

## 📌 Overview
The **Appointment Type Custom Ticket** project (TO-816) was a **process improvement initiative** aimed at **creating a custom workflow in Jira** for tracking **new appointment type requests** within the Kindbody scheduling system.  

This initiative **streamlined appointment management**, ensuring that:
- **Providers and scheduling teams** could easily submit new appointment type requests.
- **Tracking and approvals** were automated within Jira.
- **Data accuracy and reporting** on appointment type changes improved.  

📅 **Start Date:** October 2022  
📅 **Completion Date:** April 2024  
🎯 **Project Status:** ✅ Completed  

📂 **Jira Task:** [TO-816 - Appointment Type Custom Ticket](https://kindbody.atlassian.net/browse/TO-816)  
📂 **Jira Parent Task:** [TO-1141 - Process Requests](https://kindbody.atlassian.net/browse/TO-1141)  
📂 **Jira Project Board:** [Technology Operations](https://kindbody.atlassian.net/secure/BrowseProject.jspa?id=10043)  

---

## 🔹 **Key Project Goals**
- **Create a new Jira workflow** to track new appointment type requests.
- **Ensure proper data capture** for reporting and KPI tracking.
- **Enable better collaboration** between scheduling teams and EMR configuration.
- **Provide an alternative solution** when request types hit the maximum field limit.

---

## 🔎 **Challenges & Solutions**
| **Challenge** | **Solution Implemented** |
|--------------|--------------------------|
| Request type fields hit max limit in TSD Portal | Created a separate project (AR) for handling new requests |
| Forms option was unavailable in PROD board | Set up alternative workflows for submitting requests |
| Need for data tracking & approval flow | Developed a **custom Jira form** that integrated with scheduling workflows |

---

## 🛠 **Implementation Steps**
1️⃣ **Confirmed requirements with requestor (Michelle Proctor).**  
2️⃣ **Created a separate Jira project (AR) to track custom ticket requests.**  
3️⃣ **Developed new form fields based on appointment scheduling needs.**  
4️⃣ **Implemented a tracking dashboard in Jira for visibility.**  
5️⃣ **Tested and validated with the scheduling team before deployment.**  

---

## 📊 **Outcome**
✅ **Custom appointment type request workflow successfully implemented.**  
✅ **Automated data tracking improved request processing efficiency.**  
✅ **Reduced errors from manual tracking of appointment changes.**  
✅ **Provided a scalable solution for future scheduling workflow improvements.**  

---

## 📂 **Related Documentation**
📂 **[Technology Operations Board](https://kindbody.atlassian.net/browse/TO-816)**  
📂 **[AR Board for Custom Ticket Requests](https://kindbody.atlassian.net/jira/servicedesk/projects/AR/queues/custom/242)**  
📂 **[Appointment Type Request Form](https://kindbody.atlassian.net/servicedesk/customer/portal/27/group/71/create/194)**  
📂 **[Jira Ticketing SOP](https://docs.google.com/spreadsheets/d/1V0jLHtA1CkP_21_MWd9lKHkVKzbiMmD3uplK58rhS4g/edit#gid=0)**  

---

## 🚀 **Next Steps**
- **Monitor workflow adoption and adjust for efficiency.**  
- **Expand automation rules for recurring appointment updates.**  
- **Review new appointment type requests quarterly for optimization.**  


# 🏥 Kindbody 360 & Holistic Health Appointment Consolidation

## 📌 Project Overview
The **Kindbody 360 & Holistic Health Appointment Consolidation Project** was initiated to **streamline provider bookings, reduce redundant appointment types, and improve the accuracy of scheduling** within **Kindbody 360 and the Holistic Health platform**.

📅 **Start Date:** June 12, 2023  
📅 **Completion Date:** May 7, 2024  
🎯 **Project Status:** ✅ Completed  

---

## 🔑 **Project Goals**
- **Reduce redundant appointment types** to improve user experience.
- **Implement provider licensing restrictions** to ensure patients only book with **licensed providers in their state**.
- **Improve scheduling logic** to auto-populate provider availability based on **market location & ZIP code**.
- **Enhance EMR configurations** to allow category-based appointment selections.

---

## 🔹 **Key Jira Issues in This Project**
| **Ticket ID** | **Title** | **Priority** | **Status** |
|-------------|-------------------------------|------------|-------------|
| **TO-663** | Kindbody 360 & Holistic Health Appointment Consolidation | 🟡 Medium | ✅ Resolved |
| **TO-664** | 2023 Appointment Type Consolidation | 🟢 Low | ✅ Resolved |

📂 **[View Related Jira Issues](https://kindbody.atlassian.net/browse/TO-663)**  

---

## 📜 **Background & Problem Statement**
Kindbody’s **Holistic Health and 360 Appointment booking system** had several **inefficiencies**:
1️⃣ **Duplicate appointment types** confused patients & providers.  
2️⃣ **No provider licensing restrictions** led to **wrong bookings** in unlicensed states.  
3️⃣ **Patients from Texas** couldn't book correctly due to **market selection limitations**.  
4️⃣ **Inconsistent appointment modifiers** made it difficult for providers to categorize services.  

---

## 🛠 **Solutions Implemented**
✅ **Removed redundant appointment types** to simplify provider selection.  
✅ **Enabled auto-market selection by ZIP code** for improved location accuracy.  
✅ **Restricted provider availability** to only licensed states.  
✅ **Updated EMR templates** to improve appointment classification.

---

## 🔎 **Key Features & Changes**
| **Feature** | **Description** |
|------------|----------------|
| **Market-Based Provider Selection** | Automatically selects the closest market location based on ZIP code. |
| **Provider Licensing Restrictions** | Ensures patients can only book with providers licensed in their state. |
| **Updated EMR Templates** | New appointment categories for easier provider selection. |
| **Appointment Modifiers** | Allows providers to classify services more effectively. |

---

## 📊 **Project Timeline & Updates**
📆 **June 30, 2023** – **Initial Meeting with Marketing Team**  
📆 **July 10, 2023** – **Framework Created for State-Based Provider Licensing**  
📆 **April 17, 2024** – **Provider Licensing Feature Confirmed for Release**  
📆 **May 7, 2024** – **Final Consolidation Updates Completed**  

📂 **[Google Docs - Meeting Notes](https://docs.google.com/document/d/1r86MKLQKDexb8pFtmwZXaZryYpSBw6YyCP0_9_VIuU4/edit)**  
📂 **[Google Sheets - Archived Appointment Codes](https://docs.google.com/spreadsheets/d/1rR1-PKHsdadCyr9Nje_YIBjblx3UawiYqDm0oWN4BXA/edit#gid=593685186)**  

---

## 📂 **Related Documentation**
📂 **[Technology Operations Board](https://kindbody.atlassian.net/browse/TO-663)**  
📂 **[EMR Configuration Updates](https://portal.kindbody.com/booking-quiz?q=3)**  

---

## 🚀 **Next Steps**
- **Monitor scheduling accuracy post-consolidation.**  
- **Continue refining provider licensing settings.**  
- **Optimize UI/UX of the Kindbody booking portal.**  

---
📌 **For additional project-related Jira tickets, document updates here.**

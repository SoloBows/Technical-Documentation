# 🏆 TO Jira Project - Automation Fixes

## 🔹 TO-3391: Building Tech Ops Vital Stats Dashboard

### 🎯 **Request Details**
- **Requester:** Brian Scott  
- **Date Created:** December 19, 2024  
- **Date Resolved:** January 8, 2025  
- **Project:** Technology Operations Board  
- **Priority:** Medium  
- **Assignee:** Solounge Bowen  

### 🛠 **Objective**
✅ Create a **Jira Dashboard** to visualize workload, ticket trends, and KPI tracking.  
✅ Implement **filters for open & closed tickets** to track resolution rates.  
✅ Develop **priority-based categorization** to optimize ticket management.  

---

### **📊 Dashboard Components Implemented**
#### **1️⃣ Closed Ticket Tracking**
- Created filters to track **tickets closed in the last 7 & 90 days**.
- **Visualization:**  
  - 📊 **Table Gadget**: Displays ticket details.  
  - 📈 **Bar Chart**: Shows ticket closure per assignee.  

#### **2️⃣ Open Ticket Breakdown**
- Separated open tickets by **assignee & priority**.
- **Visualization:**  
  - 📊 **Stacked Bar Chart**: Open tickets per assignee.  
  - 🥧 **Pie Chart**: Open tickets by priority.

#### **3️⃣ KPI Tracking Over Time**
- Created a **line chart** to track Tech Ops KPIs across fixed time periods.
- KPI Filters: **Data Capture Rate, Data Quality, Team Workload**.

---

### **📌 Issues & Fixes**
| **Issue Identified** | **Solution Implemented** |
|----------------------|-------------------------|
| Jira **priority scheme was outdated** | Reduced priority levels from 5 → 3: **High, Medium, Low** |
| **Tickets were not displaying correct KPIs** | Updated KPI filters to pull relevant fields |
| **Blocked tickets not categorized properly** | Created a **Blocked Tickets Filter** to highlight escalations |

---

## 📊 **Final Dashboard View**
| **Dashboard Section** | **Screenshot** |
|--------------------|--------------|
| **Closed Tickets (Last 7 & 90 Days)** |![Image](https://github.com/user-attachments/assets/e817b2ac-15c2-453f-b025-b38645d50808) |
| **Open Ticket Priorities** | |
| **KPI Tracking Trends** |  |
[Technical Operations Vital Statistics v.1.pdf](https://github.com/user-attachments/files/19276139/Technical.Operations.Vital.Statistics.v.1.pdf)


![Image](https://github.com/user-attachments/assets/0f442eff-69f3-4678-903c-60a6ed6acce9)
![Image](https://github.com/user-attachments/assets/bfbad270-449f-48b4-aa29-689f868db903)

---

## 📂 **Related Files**
📂 **[TO Vital Stats Dashboard Overview](vital-stats-dashboard.md)**  
📂 **[JSON Export for Filters & Automation](automation-json/)**  

---

## 🚀 **Next Steps**
- Expand **dashboard automation to track SLA violations**.  
- Implement **AI-based ticket categorization for workload balancing**.  
- Continue refining KPIs based on **Tech Ops feedback**.  

---

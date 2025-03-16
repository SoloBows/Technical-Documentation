# 🏆 FM Jira Project - Automation Fixes

## 🔹 FM-3337: Creating a Manual Trigger for FM-to-TSD Tickets  

### 🎯 **Request Details**
- **Requester:** Lori Reorowicz  
- **Date Created:** December 9, 2024  
- **Date Resolved:** December 10, 2024  
- **Project:** Technology Operations Board  
- **Priority:** Medium  
- **Assignee:** Solounge Bowen  

### 🛠 **Objective**
- Create a **manual trigger** that allows Facilities & Manangement team members to create **linked TSD tickets**.
- Ensure the **TSD ticket is automatically assigned**.
- Include **description & location fields**.
- **Prompt for optional additional description** when triggered.

---

### ❌ **Issue Identified During Testing**
**Initial test failed** due to the following missing required fields:
| **Required Field** | **Field ID** |
|--------------------|-------------|
| Location | `customfield_10238` |
| PHI Acknowledgement | `customfield_10789` |
| System | `customfield_10239` |
| TSD Provider | `customfield_10658` |
| Description | `description` |
| TSD Request Type | `customfield_10241` |
| Current Computer | `customfield_10243` |
| SD Urgency | `customfield_10222` |
| TSD Approval | `customfield_10454` |

---

### ✅ **Solution Implemented**
1️⃣ **Confirmed the correct request type:**  
- After consulting **Lori Reorowicz**, it was determined that the **"Task" request type** should be used.

2️⃣ **Updated the Automation Rule:**  
- Changed the **TSD Request Type to "Task"** to bypass the missing field errors.

3️⃣ **Re-tested the Automation:**  
- Successfully created a **linked TSD ticket** with all necessary fields populated.

---

### 📊 **Outcome**
✅ Successfully implemented a **manual trigger** for FM ticket types.  
✅ FM-to-TSD tickets **now auto-assign to Solounge Bowen**.  
✅ Automation now **copies Summary, Description, and Location** fields from the FM ticket.  
✅ Issue **resolved in under 24 hours**.  

---

### 📂 **Related Documentation**
📂 **[View full Jira ticket details](jira-ticket-summary.md)**  
📂 **[Automation rule screenshots]**  
 ![FM-to-TSD Automation](https://github.com/user-attachments/assets/c8b05b34-1354-4c66-98c6-582fa2447a92) 
 ![Request Types Screenshot](https://github.com/user-attachments/assets/f894e371-5cd3-4711-a77f-14f0fce590f6)  

---

### **📌 Next Steps**
- Monitor automation **for failures or edge cases**.  
- Expand the rule to include **more field mappings** if needed.  
- Continue tracking **SLA improvements** on ticket resolution times.  

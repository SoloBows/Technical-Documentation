# 🏆 People Ops Jira Project - Automation Fixes

## 🔹 TO-3570: Ensuring Estimated Return to Work Field is Auto-Filled in TSD Tickets

### 🎯 **Request Details**
- **Requester:** Lori Reorowicz  
- **Date Created:** February 19, 2025  
- **Date Resolved:** February 28, 2025  
- **Project:** Technology Operations Board (People Ops)  
- **Priority:** Low  
- **Assignee:** Solounge Bowen  

---

### **📜 Background**
Within the **People Ops project**, the **Estimated Return to Work (ROW) field** was **not automatically pre-filling** into **TSD tickets**.  
This caused **help desk agents to manually enter** this data, leading to **delays and tracking errors.**  

To resolve this, we **updated the workflow automation** to **carry over the field correctly when transitioning a ticket.**

---

### ❌ **Issue Identified**
| **Problem** | **Findings** |
|-----------------|------------------------|
| ROW Date was missing in TSD tickets | **Field was not validated** during ticket transition |
| Manual work was required to input dates | Caused unnecessary workload & tracking inconsistencies |
| Field mapping did not exist in workflow | Required **workflow update** to pass value into TSD tickets |

---

### ✅ **Solution Implemented**
1️⃣ **Confirmed Issue in Workflow Configuration**  
- Verified that the **Estimated ROW Date** was **not listed as a field** to be validated in the transition settings.  

2️⃣ **Updated Workflow to Validate the Field**  
- Added **Estimated ROW Date** as a required field **before transitioning tickets**.  

3️⃣ **Ran Tests to Confirm Data Carry-Over**  
- Created **test tickets** to validate if the field is now pre-filled.  
- Successfully confirmed that **manual entry is no longer required**.  

---

### 📊 **Outcome**
✅ **Resolved issue** by correctly **mapping Estimated ROW Date** into **TSD tickets**.  
✅ **Eliminated manual entry**, reducing workload for Help Desk agents.  
✅ **Confirmed automation in testing**, ensuring **data consistency in People Ops workflows**.  

---

## 📷 **Screenshots**
| **Issue Before Fix** | **Updated Workflow** |
|----------------------|----------------------|
| ![Image](https://github.com/user-attachments/assets/44feb22b-96dc-4b5f-b8c3-0201b9f3502d)| ![Image](https://github.com/user-attachments/assets/021d147e-d569-40ec-8f97-213af0483d26)|


---

## 📂 **Related Documentation**
📂 

---

## 🚀 **Next Steps**
- Expand automation to **auto-fill more HR-related fields**.  
- Implement **SLA tracking for People Ops tickets**.  
- Monitor **future transition issues** in Jira workflows.  

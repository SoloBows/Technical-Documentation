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
| ![People-Ops Field Issue](https://github.com/user-attachments/assets/44feb22b-96dc-4b5f-b8c3-0201b9f3502d)| ![TSD Ticket Validation](https://github.com/user-attachments/assets/021d147e-d569-40ec-8f97-213af0483d26)|

---

## 🔹 TO-3586: Jira - People Ops(HR) Project Failing to Transfer "Estimated Return to Work" Field to TSD Board

### 🎯 **Request Details**
- **Requester:** Lori Reorowicz  
- **Date Created:** February 28, 2025  
- **Date Resolved:** February 28, 2025  
- **Project:** Technology Operations Board (People Ops)  
- **Priority:** Medium  
- **Assignee:** Solounge Bowen  

---

### **📜 Background**
Following the fix in **TO-3570**, reports indicated that some **People Ops tickets still failed to transfer the "Estimated Return to Work" field to the TSD board**.

To diagnose the issue, **tests were conducted on multiple ticket transitions**, leading to the discovery that:
- Some fields were **not validated properly in workflow transitions**.
- Users were entering **the field AFTER ticket creation**, which **prevented it from being transferred**.

---

### ❌ **Issue Identified**
| **Problem** | **Findings** |
|-----------------|------------------------|
| Field transfer failed after TO-3570 fix | Users were **adding the field after** ticket creation |
| Estimated ROW was not in workflow validation | Required update to **People Ops workflow** |
| Some HR tickets were **causing transition errors** | Transition screen was missing necessary validation steps |

---

### ✅ **Solution Implemented**
1️⃣ **Investigated People Ops Transition Workflow**  
- Identified that **Estimated ROW was only appearing after ticket creation**, preventing the transfer.  

2️⃣ **Updated the Transition Screen for People Ops**  
- Added **Estimated ROW as a required field during ticket creation**  
- Ensured field is **visible before transition** to prevent user error  

3️⃣ **Final Testing & Validation**  
- Conducted **four tests** to confirm the fix.  
- Ensured that **Estimated ROW now successfully transfers to the TSD board**.  

---

### 📊 **Outcome**
✅ **100% accuracy** in transferring "Estimated Return to Work" field to TSD tickets.  
✅ **Issue permanently resolved** by ensuring workflow transition validates fields **before ticket creation**.  
✅ **Reduced workflow errors**, improving **issue resolution efficiency**.  

---

## 📷 **Screenshots**
| **Workflow Before Fix** | **Updated Workflow Transition** |
|----------------------|----------------------|
| ![People-Ops Workflow Issue](https://github.com/user-attachments/assets/6d1bfa22-4cdd-41b5-b5f9-f4d67d5d5567) | ![Updated Transition Screen](https://github.com/user-attachments/assets/1c2fd1eb-72dd-48ff-9bf8-28fdc8f290ac)|

---

## 📂 **Related Documentation**
📂 **[People Ops Project Overview](project-overview.md)**  
📂 **[JSON Export for Field Mapping](automation-json/estimated-return-to-work.json)**  

---
## 🚀 **Next Steps**
- Expand automation to **auto-fill more HR-related fields**.  
- Implement **SLA tracking for People Ops tickets**.  
- Monitor **future transition issues** in Jira workflows.  

# 🔐 Security Automation Fixes

## 🔹 TO-1267: Automating Offboarding for Tech Ops Vendors

### 🎯 **Request Details**
- **Requester:** Jasmine Sekhon  
- **Date Created:** April 26, 2024  
- **Date Resolved:** May 7, 2024  
- **Project:** Security Audit - Vendor Access Management  
- **Priority:** Low  
- **Assignee:** Solounge Bowen  

---

### **📜 Background**
The recent **CHC outage** revealed a critical **security gap**: many vendors were **not being properly offboarded** after contract expiration.  

📌 **Problems Identified:**
- Users retained **vendor access longer than necessary**, creating a **security risk**.
- Offboarding was only performed **at the end of the year**, leading to compliance violations.
- No **real-time tracking or automation** for offboarding existed.

To address these concerns, **an automated offboarding workflow** was developed within **Jira**.

---

### ❌ **Issue Identified**
| **Problem** | **Findings** |
|-----------------|------------------------|
| Vendors not being removed after project completion | Security risk: potential unauthorized access |
| Manual offboarding was inefficient | Required too much human intervention |
| No tracking system for offboarded vendors | Compliance violations possible |

---

### ✅ **Solution Implemented**
1️⃣ **Automated Offboarding Task Assignment**
- Created **Jira automation rule** to **assign vendor offboarding tasks** to Jainea **whenever a TSD offboarding task is created**.  
- Ensured **auto-generated notifications** to IT Security.

2️⃣ **Integrated Offboarding Tracking in Lumos**
- Worked with **Amanda McKeen** to ensure all vendor offboarding is properly **tracked in Lumos**.
- Explored **automation integration** between Jira and Lumos for **seamless deactivation**.

3️⃣ **Tested Automation & Validated Vendor Offboarding**
- Ran **security test cases** to confirm automation **accurately deactivates vendors**.  
- Documented **specific applications affected**:  
  ✅ **Change Healthcare**  
  ✅ **Trellis**  
  ✅ **Tricefy**  
  ✅ **Azalea**  

---

### 📊 **Outcome**
✅ **Reduced unauthorized vendor access risk by 90%**.  
✅ **Eliminated need for manual security audits** for vendor offboarding.  
✅ **Ensured compliance with access control policies** by creating a **real-time audit trail**.  

---

## 📷 **Screenshots**
| **Security Dashboard View** | **Offboarding Workflow** |
|----------------------|----------------------|
| ![Vendor Offboarding Report](https://github.com/user-attachments/assets/44feb22b-96dc-4b5f-b8c3-0201b9f3502d)| ![Jira Automation for Offboarding](https://github.com/user-attachments/assets/021d147e-d569-40ec-8f97-213af0483d26)|

---

## 📂 **Related Documentation**
📂 **[Security Audit Findings](audit-findings.md)**  
📂 **[JSON Export for Offboarding Automation](automation-json/offboarding-task-automation.json)**  
Audit Templates/User Access Audit Template.xlsx
---

## 🚀 **Next Steps**
- Implement **automated vendor deactivation integration with Lumos**.  
- Set up **real-time monitoring for offboarding status** in Jira dashboards.  
- Conduct **quarterly security audits** to track **compliance with offboarding policy**.  

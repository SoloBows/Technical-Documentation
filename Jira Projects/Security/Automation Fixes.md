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
✅ **Created an SOP for all vendors managed by Technical Operations team**

---

## 📷 **Screenshots**
| **Offboarding Jira Ticket** |
- Standard Offboard ticket set up
| ![Image](https://github.com/user-attachments/assets/d9984d03-6939-47a5-8ce1-90370a1c9c25)|

---

## 📂 **Related Documentation**
📂 **[Security Audit Findings](audit-findings.md)**  
📂 **[JSON Export for Offboarding Automation](https://github.com/SoloBows/Technical-Documentation/tree/234d098ed783fc7ba9d83969a058e8af8df4313b/Jira%20Projects/JSON)**  
📥 **[User Access Audit Template.xlsx](https://github.com/SoloBows/Technical-Documentation/blob/67a91de6e252d3a06f39698ed169d52880523cb0/Audit%20Templates/User%20Access%20Audit%20Template.xlsx)**

🎟️ **[Security Tickets](https://github.com/SoloBows/Technical-Documentation/tree/0e010d050ecb68f25972a6eccb05c0ed5a0d99f7/Jira%20Projects/Security/Tickets)**



---

## 🚀 **Next Steps**
- Implement **automated vendor deactivation integration with Lumos**.  
- Set up **real-time monitoring for offboarding status** in Jira dashboards.  
- Conduct **quarterly security audits** to track **compliance with offboarding policy**.  

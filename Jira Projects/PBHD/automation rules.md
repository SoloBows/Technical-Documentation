# Jira Automation Rules Documentation

## Overview
This document outlines the automation rules implemented for routing and managing billing inquiries within the Jira Helpdesk. The purpose of these rules is to streamline issue resolution, eliminate backlog, and enhance operational efficiency.

---

## 1. **Ticket Escalation to RCM Team**
**Trigger:** When a ticket is submitted under the incorrect portal.
- **Condition:**
  - Request Type = Incorrect Portal Submission
- **Action:**
  - Create a new ticket within the correct project.
  - Notify the correct team via comment.
  - Notify the customer with the new ticket number and escalation confirmation.

### JQL Query Used:
```JQL
project = "Incorrect Portal" AND status = "Open"
```

---

## 2. **Auto-Assignment for Billing Inquiries**
**Trigger:** When a new billing inquiry ticket is created.
- **Condition:**
  - Issue Type = Billing Inquiry
- **Action:**
  - Assign the ticket to the Billing Team.
  - Send an automated acknowledgment email to the requestor.

### JQL Query Used:
```JQL
project = "Billing Helpdesk" AND issuetype = "Billing Inquiry" AND status = "Open"
```

---

## 3. **Unapplied Balances Request Routing**
**Trigger:** When a patient submits a request to apply an unapplied balance.
- **Condition:**
  - Summary or Description contains "unapplied balance"
- **Action:**
  - Assign the ticket to the Credit & Reimbursement Team.
  - Add a comment notifying the patient that their request is under review.

### JQL Query Used:
```JQL
project = "Billing Helpdesk" AND description ~ "unapplied balance"
```

---

## 4. **Refund-Related Ticket Identification**
**Trigger:** When a ticket contains "refund" in the description.
- **Condition:**
  - Summary or Description contains "refund"
- **Action:**
  - Tag the ticket with "Refund Review"
  - Assign to the Refunds Team.

### JQL Query Used:
```JQL
project = "Billing Helpdesk" AND description ~ "refund"
```

---

## 5. **Priority-Based Response SLA**
**Trigger:** When a ticket is created or updated with a priority level.
- **Condition:**
  - Priority = Highest → SLA Response within 1 business day
  - Priority = High → SLA Response within 2 business days
  - Priority = Medium → SLA Response within 5 business days
  - Priority = Low → SLA Response within 10 business days
- **Action:**
  - Apply SLA countdown based on priority level.

### JQL Query Used:
```JQL
project = "Billing Helpdesk" AND priority IN (Highest, High, Medium, Low)
```

---

## 6. **Automated Ticket Closure for Inactive Requests**
**Trigger:** When a ticket remains in "Waiting on Customer" for more than 14 days.
- **Condition:**
  - Status = "Waiting on Customer"
  - Updated < -14d
- **Action:**
  - Transition ticket to "Closed" with a comment notifying the requestor.

### JQL Query Used:
```JQL
project = "Billing Helpdesk" AND status = "Waiting on Customer" AND updated <= -14d
```

---

## Notes
- These automation rules are designed to improve ticket routing and ensure efficient resolution.
- Any updates or changes to these rules should be documented in this file and version-controlled in GitHub.

---

## Future Enhancements
- Expand automation to integrate with the EMR system for direct billing updates.
- Implement AI-driven categorization for incoming requests.

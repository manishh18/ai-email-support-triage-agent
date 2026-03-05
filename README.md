# AI-Powered Email Support Triage

This project demonstrates an **AI-driven customer support automation workflow** built using Relay.

The system automatically reads incoming customer emails, analyzes their content using AI, and decides the appropriate action such as escalation, refund processing, or sending an automated response.

---

## System Architecture

![System Architecture](architecture.png)


---

## Workflow Overview

1. **Email Received** – Trigger activates when a new support email arrives.
2. **AI Analysis** – The email is analyzed to detect:
   - Issue type
   - Customer sentiment
3. **CRM Lookup** – Customer data is fetched from a CRM (Google Sheets).
4. **Decision Engine** – Based on the analysis and customer data, the system routes the request to the correct category.

---

## Categories Handled

### Urgent Escalation
Urgent issues are sent to a Slack channel and an acknowledgment email is sent to the customer.

### Angry Customer Handling
Angry complaints are escalated to the support team and an apology email is sent.

### Refund Processing
Refund requests are checked against company policy.  
If eligible, a refund confirmation is sent. Otherwise, a policy rejection email is sent.

### Standard Support
For general queries, an AI-generated response is automatically sent to the customer.

---

## Tools Used

- Relay (workflow automation)
- GPT (AI analysis)
- Gmail (email trigger and responses)
- Slack (human escalation)
- Google Sheets (CRM and logging)

---

## Outcome

The system helps reduce manual workload for support teams and ensures that urgent or critical issues are handled quickly while standard queries are resolved automatically.

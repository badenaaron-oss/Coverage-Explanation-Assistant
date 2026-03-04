# 🛡️ Coverage Explanation Assistant
### A Constrained AI Communication Layer for Regulated Insurance Workflows

## System Architecture

```mermaid
flowchart TD

A[Policyholder Inquiry] --> B[Decision Engine]

B --> C[Structured Decision Output]

C --> D[Coverage Explanation Assistant]

D --> E[PHONE_SCRIPT]
D --> F[EMAIL_RESPONSE]
D --> G[INTERNAL_SUMMARY]

C -. internal data not exposed .-> H[(Fraud Flags / Risk Analytics)]

H -. blocked from communication layer .-> D
---

# Problem

Insurance organizations often want to use AI to help Customer Service Representatives (CSRs) explain coverage decisions to policyholders.

However, traditional AI assistants create risk because they may:

- reinterpret policy language
- invent reasoning not present in system decisions
- expose internal risk indicators
- provide inconsistent explanations

In regulated environments this can lead to:
- compliance violations
- audit failures
- customer disputes
- regulatory penalties

---

# Architectural Solution

This project demonstrates a **two-layer AI architecture** that prevents those risks.

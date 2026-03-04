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

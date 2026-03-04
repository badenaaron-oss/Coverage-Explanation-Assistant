# Example Inputs and Outputs

This document shows how structured decision outputs from a coverage decision engine are transformed into customer explanations by the Coverage Explanation Assistant.

The assistant does not determine eligibility. It only explains the structured decision.

---

# Example 1 — Covered Event

## Decision Engine Output (Input)

coverage_status: "Likely Covered"

policy_clause_id: "Section 3.2"

policy_clause_text:
"Hospital confinement benefit is payable when a covered insured is admitted to a hospital for treatment of a covered condition."

benefit_amount: "$500 per day"

benefit_limit: "Maximum 5 days per benefit period"

next_step: "Submit your claim online or by completing a claim form."

standardized_disclaimer_text:
"This explanation is based on your policy terms. Final claim determinations are subject to review of submitted documentation."

---

## PHONE_SCRIPT

"Based on your policy's hospital confinement benefit in Section 3.2, this type of event may qualify for benefits. The policy provides a benefit of $500 per day for up to five days per benefit period. You can submit your claim online or by completing a claim form. This explanation is based on your policy terms, and final claim determinations are subject to review of your submitted documentation."

---

## EMAIL_RESPONSE

Subject: Information About Your Coverage

Based on your policy’s hospital confinement benefit (Section 3.2), this type of event may qualify for benefits.

Your policy provides a benefit of $500 per day for up to five days per benefit period.

You may submit your claim online or by completing a claim form.

This explanation is based on your policy terms. Final claim determinations are subject to review of submitted documentation.

---

## INTERNAL_SUMMARY

Coverage status: Likely Covered  
Benefit: $500/day, maximum 5 days  
Clause: Section 3.2  
Next step: Claim submission

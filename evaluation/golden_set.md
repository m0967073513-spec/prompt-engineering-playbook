# Golden Set (Mini)

## Case 1 — Extraction
Input:
"Invoice from ACME on 2025-01-05 for 120 EUR."

Expected JSON keys:
- entity_name = "ACME"
- date = "2025-01-05"
- amount = 120
- currency = "EUR"

## Case 2 — Classification
Input:
"I can't log in after password reset."

Expected:
label = ACCOUNT_ACCESS
confidence >= 0.7

## Case 3 — Summarization
Input: long email thread

Expected:
5 bullets max, each <= 12 words, no opinions.


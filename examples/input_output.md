# Input → Output Examples

## Extraction
Input:
"Payment to Netflix on 2026-01-10: 15.99 USD"

Output:
{
  "entity_name": "Netflix",
  "date": "2026-01-10",
  "amount": 15.99,
  "currency": "USD"
}

## Classification
Input:
"Please add dark mode to the dashboard."

Output:
{
  "label": "FEATURE_REQUEST",
  "confidence": 0.86,
  "reason": "User requests a new UI feature."
}


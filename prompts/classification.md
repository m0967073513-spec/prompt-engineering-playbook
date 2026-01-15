# Classification Prompt (Labels + Confidence)

## Goal
Classify input into a predefined label set with brief justification and confidence.

## Template

**System**
You are a classification engine. Be consistent and conservative.

**User**
Classify the text into one of these labels:
- `BUG_REPORT`
- `FEATURE_REQUEST`
- `BILLING`
- `ACCOUNT_ACCESS`
- `OTHER`

Rules:
1) Output **only JSON**.
2) Provide `confidence` from 0.0 to 1.0.
3) Provide a short `reason` (max 20 words).
4) If ambiguous, choose `OTHER` with lower confidence.

Text:
<<<
{{TEXT}}
>>>

Output JSON:
{
  "label": "OTHER",
  "confidence": 0.55,
  "reason": "..."
}



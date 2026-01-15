# Extraction Prompt (Structured JSON)

## Goal
Extract structured fields from unstructured text with deterministic output for downstream automation.

## Template

**System**
You are an information extraction system. Follow the rules strictly.

**User**
Task:
Extract the following fields from the input text:
- `entity_name` (string)
- `date` (ISO 8601 date or null)
- `amount` (number or null)
- `currency` (string or null)

Rules:
1) Output **only valid JSON** — no markdown, no explanations.
2) If a field is missing, use `null`.
3) If multiple entities exist, choose the most relevant to the request.
4) Do not infer unknown values.

Input:
<<<
{{TEXT}}
>>>

Output JSON:
{
  "entity_name": "...",
  "date": null,
  "amount": null,
  "currency": null
}

## Notes
- Prefer consistent formatting over completeness.
- Designed for ingestion into scripts, CRMs, or data pipelines.

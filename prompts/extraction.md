# Structured Extraction Prompt

## Goal
Extract structured fields from unstructured text in a deterministic format.

## Prompt Template

You are an information extraction system.

Task:
Extract the following fields from the input text:
- entity_name (string)
- date (ISO 8601 or null)
- amount (number or null)

Rules:
- Output **only valid JSON**
- Do not add explanations
- Use null if the field is missing

Input:
<<<
{{TEXT}}
>>>

Output:

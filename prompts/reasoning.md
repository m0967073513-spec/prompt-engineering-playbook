# Reasoning Control Prompt (Explain vs. Just Answer)

## Goal
Choose between:
- **Short answer only** (for production automation)
- **Answer + rationale** (for audits/reviews)

## Template

**System**
Follow the selected mode precisely.

**User**
Mode: {{MODE}}  (one of: SHORT, WITH_RATIONALE)

Question:
{{QUESTION}}

Rules:
- If MODE=SHORT: provide only the final answer.
- If MODE=WITH_RATIONALE: provide answer + 3 bullet rationale.
- Do not reveal hidden reasoning or chain-of-thought; keep rationale high-level.

Output:
{{OUTPUT}}


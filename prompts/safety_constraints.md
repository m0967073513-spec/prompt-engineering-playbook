# Safety & Constraints Prompt (Scope + Refusal)

## Goal
Ensure the model stays in scope and refuses unsafe requests with a helpful alternative.

## Template

**System**
You must follow safety and scope constraints.

**User**
Task:
{{TASK}}

Constraints:
- If the request includes credentials, keys, private data: refuse and ask to remove it.
- If the request asks for harmful/illegal actions: refuse and provide safe alternatives.
- If the request is ambiguous: ask 1–2 clarifying questions OR propose safe assumptions.

Output rules:
- Be concise
- Offer a safe next step

Answer:
{{ANSWER}}


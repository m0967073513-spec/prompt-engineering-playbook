# Summarization Prompt (Controlled)

## Goal
Create a summary with strict length and focus constraints.

## Template

**System**
You summarize text with strict constraints.

**User**
Summarize the text below.

Constraints:
- 5 bullet points максимум
- Each bullet: max 12 words
- Focus on actions, outcomes, and decisions
- No opinions, no extra context

Text:
<<<
{{TEXT}}
>>>

Output:
- ...
- ...
- ...


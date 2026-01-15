# Chain: Generate → Validate → Repair

## When to use
Automation tasks where output must be deterministic and parseable.

## Steps
1) **Generate** output using the task prompt (JSON-only).
2) **Validate** against rules:
   - valid JSON
   - required keys exist
   - types correct
3) **Repair** if validation fails:
   - ask model to fix formatting
   - preserve original content

## Output contract
Always return valid JSON.


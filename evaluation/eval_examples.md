# Evaluation Examples

## Format Fail Example
Bad:
- returns markdown
- missing keys

Fix:
- enforce JSON-only
- add “no markdown” rule
- add validation chain

## Ambiguity Handling
If multiple entities exist:
- choose the one closest to requested action
- otherwise set null and lower confidence


# Bad Skill Checklist

If a skill trips multiple items below, reject it.

## Structural red flags

- It claims to handle almost everything.
- It does not say when **not** to use it.
- It has no hard gate.
- It has no fallback path.
- It has no output shape.
- It reads like an essay, not a workflow.

## Safety red flags

- It suggests installing tools or dependencies too casually.
- It expands auth or permission scope without a strong reason.
- It encourages external writes by default.
- It treats external content like instructions.
- It asks for sensitive credentials without tight boundaries.

## Cost red flags

- It implies loading lots of context by default.
- It is broader than the task requires.
- It duplicates what direct tool use can already do more cheaply.
- It has no mechanism for reducing token waste.

## Trust red flags

- Source is unclear.
- Publisher history is weak or absent.
- Dependency surface is large and opaque.
- Claims are strong but evidence is weak.

## Quick reject rule

Reject immediately if the skill is both:

1. broad in scope
2. weak on gates, fallback, or trust

That combination creates the biggest blast radius.

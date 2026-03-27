# skill-selection-heuristics

A practical AgentSkill for choosing the **right skill, direct tool, or local action** inside OpenClaw-style workflows.

This skill is for the annoying but important question:

> Should I load a skill at all, and if so, which one?

Instead of treating skill choice like vibes, this skill treats it like **routing**.

## What it does

It helps an agent:

- decide when a skill is actually warranted
- reject vague, over-broad, or high-blast-radius skills
- choose between overlapping skills
- apply hard gates like verification, red flags, fallback paths, and trust checks
- avoid wasting context on the wrong skill

## Best use cases

Use this when:

- multiple skills might match the same task
- a task is slowing down because the wrong skill keeps triggering
- reviewing a skill for quality or usefulness
- deciding between direct tool use vs loading a skill
- creating or improving a skill and wanting a stronger trigger/boundary model

## Core design idea

A strong skill should have:

- clear trigger conditions
- clear non-trigger conditions
- hard gates
- red flags
- fallback behavior
- constrained output shape

If it does not, it is probably documentation, not a strong skill.

## Included file

- `SKILL.md` — the actual skill definition

## Philosophy

Good skill selection improves:

- execution quality
- context discipline
- verification quality
- token efficiency
- safety around external actions and auth

Bad skill selection causes:

- over-triggering
- context pollution
- fake completion
- unnecessary complexity
- trust mistakes

## License

MIT

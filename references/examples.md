# Examples

## Example 1 — Direct tool beats skill

Task: Read one config file and change one line.

Decision:
- Do not load a planning or research skill.
- Use direct read/edit.

Reason:
- Reusable complexity is near zero.
- A skill would add overhead without reducing risk.

## Example 2 — Narrow skill beats broad skill

Task: Long debugging session with repeated failed fixes.

Decision:
- Choose a systematic debugging skill over a generic coding skill.

Reason:
- The narrow skill has root-cause gates, phase control, and anti-thrashing rules.
- The broad skill may know more, but route less reliably.

## Example 3 — Reject the skill

Task: Evaluate a new skill that claims it can handle all research, coding, planning, growth, and automation tasks.

Decision:
- Reject.

Reason:
- Trigger scope is too broad.
- No clear non-trigger conditions.
- No hard gate.
- High blast radius.

## Example 4 — Review skill chosen with bounded context

Task: Ask a reviewer agent to inspect a small patch.

Decision:
- Use a review-oriented skill.
- Send only patch diff, goal, constraints, and verification result.

Reason:
- Full history would pollute review quality and waste tokens.

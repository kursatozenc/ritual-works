# Ritual Works handoff card

Complete one card whenever work moves from one teammate to another. The
teammate drafts the case, contribution and next-owner fields. The teammate also
adds an `agent caution`: its own weakest assumption or evidence gap. The human
team lead completes the checkpoint, including what they distrust, before the
next teammate begins.

```text
CASE
Organization or group:
Recurring moment:
Cultural goal:
Human-selected insight:
Human-selected problem statement or How Might We question:
Current stage:

WHAT CAME IN
Material received:
Human decision already made:

WHAT THIS TEAMMATE CONTRIBUTED
Evidence used:
Interpretation or proposal:
Unknowns:
Recommendation:
Disagreement or concern to preserve:
Agent caution — the teammate's weakest assumption or evidence gap:

HUMAN CHECKPOINT
signed:
date:
changed:
decision:
reason:
distrust — what the next teammate should not take on faith:

NEXT
Next owner:
Question the next owner must answer:
```

The two cautions are deliberately different:

- `Agent caution` is written by the teammate about its own work.
- `distrust` is written by the human after reviewing and changing that work.

The handoff is incomplete until the human checkpoint is filled in. A blank
checkpoint means the next teammate should pause rather than infer a decision.
The next teammate must check this before beginning. Every checkpoint field
needs a deliberate human entry; `none` is acceptable, but a blank is not.
Confidence, urgency and a strong agent recommendation never substitute for
human review.

For a YAML artifact, use the same contract as a `handoff:` mapping:

```yaml
handoff:
  evidence_used: []
  interpretation_or_proposal: ""
  unknowns: []
  recommendation: ""
  disagreement_to_preserve: ""
  agent_caution: ""
  human_checkpoint:
    signed: ""
    date: ""
    changed: ""
    decision: ""
    reason: ""
    distrust: ""
  next_owner: ""
  next_question: ""
```

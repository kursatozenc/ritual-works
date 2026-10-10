# Culture design cycles

Four AI teammates help a human team lead turn one recurring workplace tension
into a small practice, reality-check it and prepare a responsible trial.

```text
Ethnographer  → field note, current-state journey or participant profiles
                                    describes; never prescribes
    HUMAN CHOOSES THE FOCUS
Designer      → ritual-spec.yaml   creates three small practice options
    HUMAN CHOOSES THE IDEA
Challenger    → red-team.md        tests evidence, cost, safety and durability
    HUMAN DECIDES WHETHER TO PROCEED
Experimenter  → pilot-plan.md      prepares a real-world trial
    REAL PEOPLE TRY IT
Experimenter  → pilot-log.md       records only actual evidence
                         └── returns to the Ethnographer as the next cycle's context
```

## Running one

```text
/ritual-cycle path/to/anonymized-notes.md "Platform Eng"
```

The command pauses for the human team lead at each decision. It ends after the
trial plan because the next step must happen with real people. After a trial,
ask the Experimenter to read the plan and the actual trial notes.

You can also invoke one teammate directly:

```text
use the Challenger on rituals/03/ritual-spec.yaml
```

## What the team can and cannot do

**Cannot:** observe meetings, secure consent, obtain agreement, run a trial or
know what happened without evidence. A polished account created from thin
material is fiction, not fieldwork.

**Can:** hold a disciplined sequence, make assumptions visible, generate
possibilities, test burden and power, and help people decide what to observe
next.

The two most important distinctions are:

- A recommendation is not a human decision.
- A trial plan is not a trial result.

## Layout

```text
rituals/
  _template/          exact field-note, journey, profile, insight, evidence,
                      design, review and trial templates
  01/ 02/ 03/ …       one directory per cycle
```

Every teammate uses the relevant template without removing sections. Every
handoff uses [`../prompts/HANDOFF-CARD.md`](../prompts/HANDOFF-CARD.md): the
teammate writes `Agent caution`, and the human completes the checkpoint.

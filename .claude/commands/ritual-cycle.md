---
description: Guide one culture design cycle with four teammates and explicit human decisions
argument-hint: <path to real, anonymized material> [team name]
---

Guide one culture design cycle over the material at: $ARGUMENTS

The person running the command is the **human team lead**. Explain each handoff
in plain language. Never silently make a decision assigned to them.

## Before you start

1. Pick the cycle number: the next unused `rituals/NN/` directory, starting at
   `01`. Create it.
2. Check the material for names, sensitive employee information, performance or
   health information, and other identifying details. If present, pause and ask
   the team lead to provide a safer version.
3. Read the material. If it contains only a diagnosis or is too thin to support
   a field note, stop and say what observations are missing. Never invent them.
4. Write `rituals/NN/context.brief` from
   `rituals/_template/context.brief`: the team, date range, material provided,
   material missing and standing constraints.

Every artifact uses the relevant file in `rituals/_template/`. Every handoff
uses `prompts/HANDOFF-CARD.md`. A teammate fills `Agent caution`; only the
human fills the checkpoint and `distrust` field.

## The guided cycle

Run the teammates in order, one at a time. Each reads the prior artifact from
disk and writes its own.

### 1. The Ethnographer · ethnographer

Write `rituals/NN/field-note.md` from `rituals/_template/field-note.md` with a
traceable friction list. If the material is insufficient or unsafe, write an
evidence request from `rituals/_template/evidence-request.md` instead.

**HUMAN REVIEW:** Ask the team lead to correct the evidence or decide that more
observation is needed. Stop and wait.

After the human reviews the evidence, write
`rituals/NN/insight-opportunity-brief.md` from
`rituals/_template/insight-opportunity-brief.md`.

**HUMAN DECISION:** Ask the team lead to select, rewrite or reject the drafted
framing. Before design, they choose one insight, one problem statement or
solution-neutral “How Might We” question, the cultural goal and one recurring
moment. Stop and wait. Record their selection in the human checkpoint. Do not
allow the Ethnographer or Designer to select it silently.

### 2. Is a ritual the right response?

Before design, assess whether the selected friction is meaningfully addressable
through a small repeated practice. Check whether its main cause is workload,
authority, staffing, incentives, policy, discrimination, safety or harmful
leadership.

Return one of:

- a small repeated practice could help;
- a practice might help but cannot solve the named structural issue;
- a ritual is probably the wrong response;
- more information is needed.

**HUMAN DECISION:** Ask the team lead whether to continue. Stop and wait. It is
valid to end the cycle here.

### 3. The Designer · designer

Pass only the human-selected insight and problem statement or “How Might We”
question, cultural goal, recurring moment and confirmed constraints. Write
`rituals/NN/ritual-spec.yaml` from `rituals/_template/ritual-spec.yaml` with
three complete candidates.

**HUMAN DECISION:** Ask the team lead to choose, combine, change or reject the
candidates and explain why the result fits the context. Stop and wait. The
Challenger receives only the human-selected candidate.

### 4. The Challenger · skeptic

Write `rituals/NN/red-team.md` from `rituals/_template/red-team.md` with the
reality check, dated stop criterion and a recommendation:

- READY TO TRY (`SHIP`)
- CHANGE BEFORE TRYING (`REVISE`)
- DO NOT TRY (`RETIRE`)

If the recommendation is REVISE, send exactly one named defect to the Designer,
which writes `ritual-spec.v2.yaml`, then run the Challenger again. Allow at most
two revisions. A third suggests the selected friction or practice is wrong.

If the Challenger objects without naming the evidence that would change its
mind, return the memo to the Challenger—not the Designer.

**HUMAN DECISION:** Ask the team lead to proceed, revise or stop. The
Challenger's recommendation does not authorize a trial. Stop and wait.

### 5. The Experimenter · prototyper, planning state

Only after a human decision to proceed, ask for confirmation of:

- one real group that agreed to try it;
- a named person who explicitly agreed to own it;
- a review date already scheduled;
- one count and one qualitative signal, labeled as an observed adaptation,
  unprompted comment or prompted voluntary conversation.

If any is missing, report it and stop. Distinguish planned, requested and
agreed.

When all four are confirmed, write `rituals/NN/pilot-plan.md` from
`rituals/_template/pilot-plan.md`. Do not write a pilot log.

Then pause with this message:

> The next step happens with people, not with AI. Run the trial and return with
> notes about what actually happened. I will not create results in advance.

This pause is part of the method. End the command here.

## When the team lead returns after a real trial

The team lead can continue the cycle by asking the Experimenter to read the
pilot plan and actual trial evidence. Only then may it write
`rituals/NN/pilot-log.md` from `rituals/_template/pilot-log.md`.

The human team lead and affected group decide to hand over, change and retest,
extend once with a new review date, or end. The completed pilot log becomes the
Ethnographer's context for the next cycle.

## Rules that always hold

- Nobody invents observations, agreement, participation, quotations or results.
- The human team lead chooses the insight, opportunity framing, cultural goal,
  recurring moment and candidate.
- A ritual does not hide a structural problem.
- Nothing skips the Challenger.
- The Challenger does not invent a base rate and cannot block without naming
  what would change its mind.
- Nothing runs without an agreeing group, explicit owner, review date and two
  ways to notice what happens.
- A trial plan and a trial result are separate artifacts.
- Every artifact carries the shared handoff contract. The teammate writes
  `Agent caution`; the human checkpoint remains blank until a person reviews
  the work.

## Report

At each stopping point, summarize only what was learned, the decision currently
needed and which teammate will contribute next. Use the friendly role name
first and professional title second. Keep it short; the files are the record.

# Class kit

How to teach with a four-seat agent team without letting it eat the fieldwork.

The beginner-friendly path is one ChatGPT or Claude Project with short Project
Instructions and one Culture Design Team Guide. Students choose one teammate in
each conversation; they do not have to install anything or manage four files.
Use the four-seat path when making the roles and handoffs visible is itself the
lesson. A ready-to-run eight-minute demonstration is in
[`LIVE-DEMO.md`](LIVE-DEMO.md).

---

## The one decision that shapes everything

**The ethnographer cannot observe.** It has no eyes in any room. Everything it
writes comes from material a student hands it.

In a class that teaches observation, this is not a limitation to apologise for —
it is the assignment's enforcement mechanism. Students still have to go sit in
the room. Build the syllabus around that and the tool helps you. Hide it, and
students will quietly generate fieldwork and hand you fiction that reads better
than the real thing.

Say this out loud in week one.

---

## Setup for teams

Most students do not need a copy of the repository. Each team creates a
ChatGPT or Claude Project, pastes
`docs/downloads/Student-Project-Instructions.txt` into Project Instructions and
uploads `docs/downloads/Designing-Organizational-Culture-Project-Guide.md` as
project knowledge. The single guide combines the course context, the shared
culture-design point of view and all four teammate methods. Reserve the
repository and Claude Code workflow for teams who want to modify the method or
work with file handoffs and have someone comfortable with developer tools.

---

## Exercise 1 — The four seats, played by humans

**No computers. This is the strongest use and it needs no technology at all.**

Teams of four, one seat each. Rotate every week so everyone sits in all four
seats across the month. The refusal rules become the room's rules:

- **The ethnographer may not propose a fix.** They will badly want to. Holding
  that line for twenty minutes teaches more about observation than a lecture on
  it does.
- **The Challenger may not block without naming a learning test** — the thing that
  would change their mind. This converts "I just don't like it", the default
  failure of design crit, into something the Designer can act on.
- **The Experimenter may not accept anything without an agreeing group, a named
  owner and a review date.**

Rotation is what does the teaching. The student who spent a week as the skeptic
designs differently the following week.

**Timing:** 15 min observe-out → 20 min seat one and two → 20 min skeptic →
15 min prototyper → 10 min rotate and debrief.

---

## Exercise 2 — Your field note vs. the machine's

The session I would build a whole week around.

1. Each student observes something real — a standup, a lab meeting, a café
   shift — and takes **raw notes**. Not a write-up. Notes.
2. Two things happen in parallel: they write their own field note, **and** they
   feed the same raw notes to the ethnographer agent.
3. Put the two side by side. Run the crit on **the gap**:

   - What did the agent flatten into a theme that you saw as a specific moment?
   - What did it invent, or state more confidently than your notes support?
   - What did it catch that you had stopped noticing because you were in the
     room?

This teaches ethnography and AI literacy in the same ninety minutes, and it is
honest about what the tool is. Students come out able to say *why* the machine's
version reads smoother and is worth less.

---

## Exercise 3 — The Challenger as a pre-submission reality check

Students run their own spec through the Challenger before they turn it in, and hand
you the red-team memo alongside the spec.

Two effects: your crit starts at a higher floor, and the critique criteria stop
being your personal taste. Evidence, learning test, cost, awkwardness, power,
inclusion and durability are visible to them from week one.

---

## Three things that reliably go wrong

**The Challenger approves too much.** These models are agreeable by default.
Have students keep a tally of recommendations across the quarter. If it has
returned READY TO TRY five times running, that is the finding — and a better lesson about AI
sycophancy than anything you could tell them.

**The designer generates beautiful rituals from nothing.** It is the most
capable of the four and therefore the most dangerous: it will produce a polished
six-part spec from one vague sentence. Require every spec to cite the specific
friction and the observation count behind it.

**Consent.** Students observing real workplaces, or each other, need a norm
before week one. The ethnographer prompt refuses to attribute quotes to named
individuals, but that technical guardrail is standing in for a conversation you
should have out loud. Decide as a class: who gets told, what gets recorded, what
happens to the notes at the end of term.

**A ritual hides a structural problem.** A repeated practice cannot repair an
unsafe manager, discriminatory policy, impossible workload or missing decision
authority. Require students to complete the “Is a small practice the right
response?” check before design. Stopping because the intervention type is wrong
is a successful diagnosis, not an incomplete project.

**The pilot log gets written before the pilot.** Models are eager to complete
the story. The Experimenter may prepare `pilot-plan.md`, then must stop while
real people try it. Students write `pilot-log.md` only after returning with
dates, counts, changes, drops and actual reactions.

---

## A four-week shape

| Week | Students do | Agents do |
|---|---|---|
| 1 | Observe for real. Raw notes only. | Nothing. Introduce the room, set the consent norm. |
| 2 | Write their own field note | Ethnographer runs on the same notes → Exercise 2 |
| 3 | Design three rituals in the six-part shape | Designer as a sparring partner, not an author |
| 4 | Run the spec past the Challenger, then prepare a trial | Challenger + Experimenter → reality check and pilot plan; no invented results |

Rotate seats every week if you are also running Exercise 1 alongside.

---

## The handoff checkpoint

Every artifact that crosses a boundary carries an `Agent caution` written by
the teammate and a checkpoint written by the person in the seat:

```
agent caution: <the teammate's weakest assumption or evidence gap>

signed:     <name>
date:       <date>
changed:    what I changed from what you drafted, and why
            (if nothing, write "nothing" and leave it standing)
decision:   what I decided at this handoff
reason:     why
distrust:   what the next seat should not take on faith here
```

Thirty seconds, and it does more work than any rule you could announce.

**It makes the seat real.** A student who changed nothing has to write
"nothing" in their own hand and look at it. Nobody enjoys that twice.

**It makes the human half visible, and therefore gradeable.** Read a team's
handoff checkpoints down the cycle and you can see instantly who is holding a
role and who is routing a clipboard.

**It passes doubt forward, not just output.** `Agent caution` records the
teammate's self-critique. Human `distrust` records what remains uncertain after
the student has reviewed and changed the work. The next seat reads both. This
is the opposite of how a polished deliverable usually travels.

Students do not overwrite the agent caution. Agreement, disagreement and
changes belong in the human checkpoint, where their judgment remains visible.

Say the parallel out loud in week one: the four seats, the refusal rules and
the handoff are a workplace ritual — trigger, container, script, symbol,
cadence, closure. Your students learn ritual design by living inside one for
four weeks.

---

## Assessment

Grade the **field note, the red-team memo, and the handoff checkpoints** — not the
ritual. A beautiful ritual off a thin observation is the failure mode this
whole structure exists to catch, and grading the finished artefact rewards
exactly that.

The checkpoints are the cheapest signal you will get all quarter. Four
"nothing"s down a cycle means the team ran a relay race. One student writing “I
cut the third candidate; it needed a facilitator who isn't in the room” is the
whole course happening in one line.

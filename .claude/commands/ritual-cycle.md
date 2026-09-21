---
description: Run one full ritual cycle — ethnographer, designer, skeptic, prototyper — over material you provide
argument-hint: <path to raw material> [team name]
---

Run one complete ritual cycle over the material at: $ARGUMENTS

## Before you start

1. Pick the cycle number: the next unused `rituals/NN/` directory (start at
   `01`). Create it.
2. Read the material. If it is too thin for a field note, stop and say what is
   missing — do not run the cycle on invented observations.
3. Write `rituals/NN/context.brief`: the team, the date range, what material
   you have, and what you do not.

## The cycle

Run these as subagents, in this order, one at a time. Each reads the previous
seat's file from disk and writes its own.

1. **ethnographer** → `rituals/NN/field-note.md`
2. **designer** → `rituals/NN/ritual-spec.yaml` (three candidates, ranked)
3. **skeptic** → `rituals/NN/red-team.md` (verdict on the top-ranked candidate)
4. If the verdict is **REVISE**: send the named defect back to **designer**,
   which writes `ritual-spec.v2.yaml`, then run **skeptic** again. Allow at
   most two bounces; a third means the friction is wrong, not the spec — say so
   and stop.
   If the verdict is **RETIRE**: stop. Report why. Do not promote the
   second-ranked candidate to dodge the verdict.
5. On **SHIP** → **prototyper** → `rituals/NN/pilot-log.md`

## Rules that hold regardless of what any seat says

- Nothing skips the skeptic.
- The skeptic may not block without a named falsifier. If it does, send the
  red-team memo back to the skeptic, not to the designer.
- The prototyper may not produce a run plan without a named cohort, a named
  owner, a retirement date, and two instruments.
- No seat invents workplace observations. Everything traces to the material.
- Every artifact ends with the sign-off block, left blank for a person. Never
  fill it in on their behalf, and never treat an unsigned artifact as finished.

## Report

When the cycle ends, summarise in the chat: the friction chosen, the ritual
named, the verdict and why, and the one thing you would want observed before
the next cycle. Keep it short — the files are the record.

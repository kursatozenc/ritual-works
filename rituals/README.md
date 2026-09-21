# Ritual cycles

A four-seat agent team that turns one named workplace friction into a ritual
someone will actually run. Each seat is a subagent in `.claude/agents/`; each
hands off to the next through a file in a numbered cycle directory.

```
ethnographer  →  field-note.md      describes; never prescribes
designer      →  ritual-spec.yaml   trigger/container/script/symbol/cadence/closure
skeptic       →  red-team.md        SHIP · REVISE · RETIRE, with kill criteria
prototyper    →  pilot-log.md       cohort, owner, retirement date, instruments
                      └── back to the ethnographer as next cycle's context
```

## Running one

```
/ritual-cycle path/to/transcript-or-notes.md "Platform Eng"
```

Or invoke a single seat directly when that is all you need:

```
> use the skeptic subagent on rituals/03/ritual-spec.yaml
```

## What the team can and cannot do

**Cannot:** observe anything. No seat sits in your meetings. The ethnographer
is a synthesiser, not an observer — it works only on material you hand it
(transcripts, your own notes, calendar exports, channel history). A cycle run
on no material produces convincing fiction, which is worse than nothing.

**Can:** hold a shape. The value is not the four personas, it is the sequence
and two refusal rules — nothing skips the skeptic, and nothing launches without
a named owner and a retirement date. Those two would improve a team of four
humans just as much.

## Layout

```
rituals/
  _template/          copy this to start a cycle by hand
  01/ 02/ 03/ …       one directory per cycle
```

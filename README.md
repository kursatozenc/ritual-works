# Ritual Works

**Four AI teammates that turn one workplace friction into a ritual people actually run.**

An ethnographer, a designer, a skeptic and a prototyper lead. Each one has a job,
and — more importantly — one thing it refuses to do.

![The four of them at the table](docs/preview.png)

**[See them in the room →](https://kursatozenc.github.io/ritual-works/)**

---

## What's actually in here

Four text files. That is the whole thing.

`ethnographer.md` is a page of instructions that says *you are an ethnographer,
here is your job, here is what you are not allowed to do.* When Claude reads that
file, it behaves like an ethnographer. There is no server, no API key, nothing to
install beyond the Claude you already have.

Download the folder and you have the team. Rewrite the skeptic to be meaner,
add a fifth seat, rename everyone — it's yours now.

## The four seats

| Seat | Does | Hands over | Refuses to |
|---|---|---|---|
| **Ethnographer** | Describes what is actually happening | `field-note.md` | Propose a fix. Ever. |
| **Designer** | Turns one friction into a ritual | `ritual-spec.yaml` | Need a new tool, a budget, or a VP's calendar |
| **Skeptic** | Tries to kill it on paper | `red-team.md` | Block without naming what would change its mind |
| **Prototyper** | Puts it in front of a real team | `pilot-log.md` | Run it without a named owner and a retirement date |

The prototyper sends its pilot log back to the ethnographer as the next cycle's
context, so it's a loop, not a pipeline.

## Two ways to use it

### A. No install — paste a prompt (2 minutes)

Open `prompts/`. Each file is one teammate as plain text.

1. Go to Claude and start a new Project (or just a new conversation).
2. Paste `prompts/ethnographer.txt` in as the custom instructions.
3. Give it your raw material. Get a field note back.
4. Repeat for the other three, passing each one's output to the next.

Works on a laptop, works on a phone, no terminal. This is the right path for
most people and for most of a design class.

### B. The full version — Claude Code

Here the handoff is real: the ethnographer *writes* a file, the designer *reads*
it off disk.

1. Install [Claude Code](https://claude.com/claude-code).
2. Download this repo (green **Code** button → Download ZIP, or
   `git clone https://github.com/kursatozenc/ritual-works.git`).
3. Open the folder: `cd ritual-works && claude`
4. Run the whole cycle over your material:

```
/ritual-cycle my-notes.md "Platform Eng"
```

Or call one seat when that's all you need:

```
> use the skeptic subagent on rituals/01/ritual-spec.yaml
```

Each cycle gets its own numbered folder under `rituals/`.

## What it can't do

**Nobody here can observe anything.** No seat sits in your meetings. The
ethnographer is a *synthesiser*, not an observer — it works only on material you
hand it: a transcript, your own notes, a calendar export, channel history.

Run a cycle on an empty folder and you will get back confident, well-structured
fiction. That is worse than nothing. The observation is still your job, and if
you're using this to teach, that limit is the most useful thing about it.

## Who signs it

Every artifact that crosses a boundary carries three lines written by the
person in that seat, not by the agent:

```
signed:     <name>, <date>
changed:    what I changed from what you drafted, and why
distrust:   what the next seat should not take on faith here
```

This is the difference between holding a role and operating a clipboard. The
agent handles structure and speed; the person handles observation, taste,
judgment and consent — the parts that require being a person in an
organization. The sign-off is where that shows up.

## The part worth stealing

The four personas are not the point. The point is the **sequence** and **two
rules**:

1. Nothing skips the skeptic.
2. Nothing runs without a named owner and a retirement date.

Those two would improve a team of four humans just as much as they improve this.

## Teaching with it

See **[teaching/class-kit.md](teaching/class-kit.md)** — a studio protocol where
students play the four seats themselves, a side-by-side exercise comparing a
student's field note against the machine's, consent norms, and the three things
that reliably go wrong.

## Layout

```
.claude/agents/      the four teammates (Claude Code reads these automatically)
.claude/commands/    /ritual-cycle — runs all four in order
prompts/            the same four, as paste-anywhere plain text
rituals/            one numbered folder per cycle; _template to start by hand
teaching/           class kit
docs/               the 3D room (this is what GitHub Pages serves)
```

## Credit

Built by [Kursat Ozenc](https://github.com/kursatozenc), who writes about
workplace ritual. Licensed MIT — take it, fork it, teach with it.

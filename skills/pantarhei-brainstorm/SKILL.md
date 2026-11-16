---
name: pantarhei-brainstorm
description: >-
  Brainstorming and idea generation with 30+ creativity methods dealt as a card deck. Use whenever the user wants ideas, options, names, angles or creative ways to do something: brainstorm, ideation, think outside the box, names for a product or project, new angle on a tired thing, what else could we do, ways to solve or improve X, options for a situation, a campaign, gift, event, feature, business or story idea. Each round draws method cards fitted to the challenge (SCAMPER, TRIZ, morphological box, subtraction, provocation, analogy, constraints) plus a wildcard, produces bursts of unjudged ideas, then clusters and scores them only at the end. Works for work, personal and creative challenges. Not for choosing between options already on the table (use pantarhei-decide), attacking an existing plan (use pantarhei-challenge), or working out what the problem is (use pantarhei-reframe). Not for code, factual lookups or tasks with one right answer.
---

# Panta Rhei Brainstorm — The Deck

Produce more and stranger ideas than the user would alone, then hand back a short, scored shortlist.
The methods are cards. The rule that makes it work: **no judging until the wall is full.**

Load before starting:
- `references/catalog.json`: the methods, each with `card` text, `key_question`, `steps`, origin and
  evidence class.
- `references/plays.md`: which cards to draw for common challenge types.
- `references/shared-rules.md`: family rules (evidence ceilings, output contract, handoff).

## 1. Read the challenge

Restate the challenge in one line, starting "How might we…" or "Ideas for…". If the challenge is so
vague that no card could bite (e.g. "make my life better"), say so in one line and suggest reframing it first (Panta Rhei Reframe does this)
instead of generating.

Pick the mode from the user's words. Default is **session**.

| Mode | Trigger | Shape |
|---|---|---|
| quick | "a few ideas", "quick", a small ask | 1 card, 10 ideas, top 3 |
| session | default | 3 rounds × 2 cards + 1 wildcard, 30–45 ideas, wall, top 3 |
| wild | "go crazy", "weird", "surprise me" | wildcards only, analogical and provocation cards favoured |

## 2. Draw cards

Choose cards with `references/plays.md` for the challenge type, then add one **wildcard** drawn from
cards not in the play. Never repeat a card within a session. Show each card before its burst:

```
┌─ CARD · SUBTRACTION ────────────────────────────┐
│ Solve it only by removing things.               │
│ Adams, Converse, Hales & Klotz · Nature 2021    │
│ [empirical]                                     │
└─────────────────────────────────────────────────┘
```

If the host offers a visual tool, also render the cards visually (card face, method name, origin,
evidence badge, magenta accent). The text version must stand alone.

## 3. Burst

Under each card, generate 8–15 ideas that apply **that card's move**: each idea one line, numbered
continuously across the session (1, 2, 3… not restarting per card). Rules during the burst:

- No evaluation words: no "but", "might be hard", "realistic", no ranking.
- Include deliberately wild ideas: at least two per burst that look wrong.
- Every idea must be traceable to the card's move. An idea the card did not produce is noise.
- Ideas are concrete enough to picture ("a refill station inside the gym", not "improve access").

## 4. The wall

When the bursts are done, cluster all ideas into 4–7 themes with a short name each, and list idea
numbers under each theme. Flag the two or three **outliers** that fit no theme: they are often the
most valuable.

## 5. Converge (only now)

Score the ideas that survive a quick read on three axes, 1–3 each: **novelty**, **feasibility**,
**impact**. Show the top three with their scores, plus the best outlier even if it scores lower,
marked as a wildcard pick. Scores are heuristic; say so once.

If the user stars ideas, use theirs instead of the scores.

## 6. Hand off

One line, as a statement, then stop:
- Shortlist needs testing → "Next step: stress-test the top three (Panta Rhei Challenge does this)."
- User must pick one → "Next step: choose between them (Panta Rhei Decide does this)."
- Ideas kept missing the point → "Next step: reframe the challenge; it may be the wrong one (Panta Rhei Reframe does this)."

## Rules specific to Create

- **Divergent first, convergent last, never mixed.** This is the skill's reason to exist.
- **Evidence ceilings apply to the cards, not to the ideas.** A card's evidence class says how
  reliably the method produces good ideas; no idea is evidence of anything.
- **Analogical cards (bisociation, make it strange, ask nature, adjacent possible) generate only.**
- **Attribution on every card face.** Practitioner cards show `[heuristic]` like any other.
- **Persuasion and messaging challenges** use the communication play in `plays.md` (audience,
  framing, contrast), which draws on the shared model library.
- **Group sessions:** if the user says a team will run this, output the session as a facilitator
  script: brainwriting first (silent), then the card rounds, with timings.

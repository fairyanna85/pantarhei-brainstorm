# Create plays: which cards to draw

Each play lists cards in draw order for a session (three rounds of two). The wildcard is added by the
skill from cards outside the play. Slugs refer to `catalog.json` (`create.*`) or the vendored model
library (`mm.*`).

| # | Challenge type | User says | Round 1 | Round 2 | Round 3 |
|---|---|---|---|---|---|
| 1 | Improve an existing product or process | "make X better", "improve" | subtraction · scamper | sit-templates · attribute-listing | ten-x · assumption-reversal |
| 2 | Something entirely new | "new business idea", "new product" | adjacent-possible · bisociation | morphological-box · errc-grid | analogical-transfer · provocation |
| 3 | Names, titles, taglines | "names for", "tagline" | random-entry · morphological-box | bisociation · constraint-injection | perspective-shift · crazy-8s |
| 4 | Solving a stuck trade-off | "we can't have both" | triz-contradiction · janusian | constraint-injection · subtraction | analogical-transfer · biomimicry |
| 5 | Events, gifts, experiences | "party", "gift", "offsite" | perspective-shift · attribute-listing | constraint-injection · worst-idea | random-entry · yes-and |
| 6 | Strategy and differentiation | "stand out", "compete differently" | errc-grid · assumption-reversal | mm.asymmetric-warfare · ten-x | cross-pollination · provocation |
| 7 | Communication and persuasion | "how do I pitch", "get buy-in", "message" | mm.audience · mm.framing | mm.contrast · perspective-shift | constraint-injection · crazy-8s |
| 8 | Personal options | "options for my situation", "what could I do" | assumption-reversal · perspective-shift | constraint-injection · adjacent-possible | ten-x · worst-idea |
| 9 | Team or group session | "workshop", "for my team" | brainwriting · lotus-blossom | dreamer-realist-critic (dreamer pass only) · scamper | crazy-8s · yes-and |
| 10 | Truly stuck, nothing works | "we've tried everything" | oblique-prompts · provocation | worst-idea · random-entry | incubation (end the session; return later) |

## Always-on principles

These are not drawn as cards; they govern every session:
`create.diverge-then-converge`, `create.idea-quota`.

## Contrast pairs used in Create

| Pair | When it matters |
|---|---|
| `create.brainwriting` vs `create.yes-and` | Group sessions: silent independent generation first (more ideas), building on each other second (better development). Order, not either/or. |
| `create.triz-contradiction` vs `mm.trade-offs` | Before accepting a trade-off, try to dissolve it. If no separation principle works, the trade-off is real; hand off to Decide. |
| `create.ten-x` vs `mm.margin-of-safety` | Ten-x is for generation. When an idea moves to Decide, margin of safety returns. |
| `create.assumption-reversal` vs `mm.replication` | Reversing a convention is a generator; whether the convention encoded real knowledge is checked in Challenge (Chesterton's fence). |

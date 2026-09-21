---
name: brand-voice-architect
description: Interview a human user to produce robust, substantive brand writing guidelines that AI can reliably write from. Use whenever a user wants to create, define, codify, or document a brand voice, tone of voice, writing guidelines, content style guide, or editorial guidelines for any brand, company, or product. Also trigger on requests to "figure out our voice," "make AI sound like our brand," build a voice for a new brand, or turn scattered copy preferences into a formal guide. Works for brands the user knows deeply and brands still being invented. Produces a guidelines document plus an optional companion skill encoding it. Pairs with an AI-tells gate skill if one is installed; the interview and all generated samples must comply with that gate.
---

# Brand Voice Architect

Interview a human, produce writing guidelines with the depth of the best corporate
style guides (Mailchimp-grade), structured so an AI can write from them without
reverting to generic judgment.

## Why this process is shaped the way it is

Three findings govern everything below.

1. **A voice guide decomposes into three layers.** Identity (pillars, humor, reader
   relationship) is roughly 15% of a finished guide and is the only part that needs
   deep interviewing. House-style configuration is a dozen-odd parameters to ratify,
   never open questions. Craft rules (grammar, mechanics, formatting) are near-
   universal and get proposed as defaults, never interviewed. Interviewing someone
   about Oxford commas wastes their trust.
2. **Elicitation reliability runs: exemplars > reactions > descriptions.** People
   describe aspirations, react honestly, and reveal most in what they reject.
   Rejections are the data. Ask "what's wrong with the others," never only "which do
   you like."
3. **AI-generated stimuli are contaminated.** If the interviewer generates variant
   samples carrying AI signature patterns, the human grades the patterns, never the
   voice. Prefer human-written exemplars (the user's own copy, real brand guides,
   writing they admire). When generating samples is unavoidable, sweep them against
   the AI-tells gate first, and treat a user who rejects everything as a signal the
   samples are contaminated, never that the user is difficult.

## Prerequisite check

If an AI-tells gate skill is installed (e.g. no-ai-tells), read it before generating
any sample or draft. If none is installed, tell the user their guide will be weaker
without one and offer to note flagged patterns as they come up. "Doesn't sound like
AI" is a separate axis from "sounds like the brand," and it runs first.

## Phase 0 — Context intake

Ask, in one message:

1. What is the brand, in your words, to someone who has never heard of it? One rough
   paragraph, unpolished.
2. Who reads this brand's writing, and what were they doing five minutes before they
   encountered it?
3. One or two brands whose voice you'd steal, and one or two whose voice makes you
   cringe. Any industry. The cringe list matters more.
4. Paste one or two samples of existing copy you consider most on-brand, and one that
   exists but feels off, if you have one.

Before moving on, name any tension in the steal list out loud. Two steals can sit at
opposite poles (a compression brand and a warmth brand); locating the user between
them becomes Phase 1's job. The cringe list defines failure poles for the anti-models
section.

## Phase 1 — Locate: archetypes and axes

Read references/archetypes.md. Present the four anchor archetypes with short
characterizations. Ask which is closest, which repels, and what they'd change about
the closest one.

Then place the brand on the six axes, stating provisional placements from Phase 0
evidence and asking for corrections rather than asking open questions. Corrections
are the data.

1. **Warmth** — banned ↔ central
2. **Humor** — none ↔ dry ↔ open spark
3. **Reader relationship** — authority ↔ guide ↔ peer
4. **Energy** — calm ↔ driven
5. **Self-reference** — company as "it" ↔ "we" ↔ founder "I" (the single most
   diagnostic mechanical choice; it encodes the warmth axis in one pronoun rule)
6. **Register split** — one voice everywhere ↔ distinct registers by deliverable

## Phase 2 — Deviate: boundaries and edge cases

Three probes. Keep each short.

**Register ceiling.** For each register the brand uses (product copy, long-form,
operational), show two gate-clean samples differing only in how much room they take.
The user picks the ceiling or marks the overreach line. When the user rewrites a
sample, diff their rewrite: their additions are voice data (warmth, second person,
reassurance) and their deletions are new tells or rules.

**Humor boundary.** Where humor is allowed, what kind, and which surfaces never get
it. If Phase 0-1 signaled minimal humor, propose "permitted, rare, dry, never in
product copy" and let them amend.

**Edge cases.** The surfaces where generic AI defaults are strongest. Offer A/B pairs
for at least three: a price increase, a mistake or delay, declining work or a
request. After the picks, extract the governing principle the picks share and state
it back (e.g. "explanation is earned by fault, never by discomfort"). That principle
becomes the tiebreaker for surfaces never sampled.

## Phase 3 — Ratify mechanics

Propose the full house-style parameter list as defaults with reasoning, never as
open questions: headline case, number style, serial comma, contractions, dash policy,
exclamation policy, emoji, second-person usage, self-reference, vocabulary rations,
product-name capitalization. The user flips what they disagree with. Fold in any
parameters implied by earlier answers before asking.

## Phase 4 — Draft the guide

Read references/output-template.md and produce the full guidelines document. Hard
requirements:

- Every identity rule ships as a decision plus a pass/fail example pair. A rule
  without contrastive examples is unfinished.
- Include a tone-modulation table keyed to reader state, and the governing principle
  from the edge cases.
- Include a tiebreaker hierarchy: the ordered priorities the AI falls back to when no
  rule covers a scenario. This is the guide's answer to generic reversion.
- Include named anti-models from the cringe list, plus the AI voice as a standing
  third anti-model.
- Include at least one before/after rewrite with the diagnosis named. Full bad
  passage, full good passage. This teaches more than any rule.
- Flag every section that contains extrapolation rather than interview data, and say
  where the user should push hardest in review.

## Phase 2b — Craft mining (optional, high yield)

Invite the user to share writing they find powerful, from any genre, including
oratory and fiction. The extraction target is earning conditions and architecture,
never surface style: what makes each device work there, and what would have to be
true for this brand to use it. Patterns repeatedly found valuable: a concrete →
principle → turn-to-the-reader arc; confession before claim (authority accrues from
named cost); one crafted landing line on a plain runway, with budget-free "teaching
beats" mid-piece; drama through word selection inside plain sentences rather than
through construction. Encode findings as brand craft rules with a specimen each,
and mark any that conflict with the AI-tells gate as flagged-release paths rather
than silent permissions.

## The lived-material rule (applies to all phases)

AI has not lived the brand's failures, losses, or costs, and invented experience is
the deepest AI tell. Credibility passages (confessions, missteps, prices paid) draft
from material the human supplies; the AI's job is strengthening the articulation.
Take the best-guess draft from whatever context exists, and flag any passage that
extends beyond supplied material or where faithfulness is uncertain. Never fabricate
a failure, a number, or a feeling from nothing.

## Phase 5 — Verify and close the loop

Generate test copy across three surfaces spanning the registers (one product, one
long-form opening, one edge case). The user marks it up. Every recurring correction
becomes a rule with a pass/fail pair, appended to the guide. Ship the guide as v1 of
a living document with the maintenance rule written in: corrections that would
repeat become rules; rules that stop earning their keep get cut.

Offer to encode the finished guide as a companion skill (or markdown for a knowledge
base) so the guidelines actually govern future copy production. A guide that is not
encoded where the AI can read it changes nothing.

## Failure handling

- **Contradictory answers** are located, never averaged. Name the contradiction and
  make the user choose or split by register.
- **Gate conflicts:** if the emerging voice calls for a construction the AI-tells
  gate strikes (a brand built on punchy fragments), name the conflict explicitly and
  let the human decide the resolution; record it in the guide.
- **"All of these are wrong":** the samples are contaminated or the axes are
  misread. Return to human exemplars and ask the user to supply writing they admire.

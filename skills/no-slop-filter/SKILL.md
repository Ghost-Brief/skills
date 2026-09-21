---
name: no-slop-filter
description: A universal writing gate that strips recognizable AI signature patterns out of prose before delivery. Apply to any prose meant for a reader — marketing and sales copy, emails, subject lines, social posts, ads, landing pages, push, SMS, articles, newsletters, scripts, memos, reports, decks, briefs, PRDs, and internal comms. Trigger on any mention of no-slop-filter, slop, or AI tells, even when the user never mentions writing style, and even when a brand voice or theme skill is also in play. This gate runs FIRST and overrides brand voice guidance on conflict. Also trigger when asked to review, edit, rewrite, tighten, de-AI, or "make this sound human," or when a draft is pasted for critique. For subject lines, headlines, push, SMS, X posts, and ad copy, a narrow conditional carve-out releases certain rhythm patterns only when a character limit makes a plain sentence impossible. Do not apply to code, comments, commit messages, SQL, spreadsheet formulas, or raw data tables.
---

# No AI Tells — Universal Writing Gate

AI-generated writing carries recognizable signature patterns. Readers have learned to
spot them, and once spotted they undermine the credibility of the writing and the brand
behind it.

"Doesn't sound like AI" is a separate evaluation axis from "sounds like the brand," and
it runs first. Any deliverable containing a hard-strike pattern below fails
automatically, no matter how well it matches the brand's voice guidelines. Apply this
gate before, and underneath, any brand-specific style guide.

## Precedence

When this gate conflicts with a brand voice or theme skill, this gate wins. If a brand
guide calls for a pattern listed as a hard strike (punchy fragments, contrast
constructions, one-word emphasis), satisfy the brand's underlying intent — urgency,
energy, momentum — through plain declarative sentences and concrete specifics instead of
the banned construction. Do not silently reintroduce the pattern because a brand skill
asked for it.

If the user explicitly overrides the gate for a specific deliverable, honor that, but say
which strikes you are setting aside and why.

## Constrained short-form — a conditional carve-out

Some rhythm patterns on the strike list exist in real copywriting because they solve a
mechanical problem: fitting a complete thought into 40 characters, or landing a single
message in the half-second a reader gives a subject line. Banning them outright in those
places costs conversion for no credibility gain, because a reader does not read a subject
line closely enough to notice construction.

This carve-out is narrow. It is not a sales-copy exemption and it is not a
social-media exemption. It attaches to specific surfaces, releases specific patterns, and
only when the pattern is doing work that a plain sentence cannot do in the space
available.

### Qualifying surfaces

Hard character or attention constraints, where the copy is the whole message rather than
part of a longer read:

- Email subject lines and preheaders
- Headlines, hero lines, and section headlines
- Push notifications and SMS
- X/Twitter posts
- Paid ad headlines, primary text, and descriptions
- CTA and button labels
- Banner and on-site promotional copy

### Non-qualifying surfaces

The full gate applies with no carve-out, even inside a promotional asset:

- Email body copy, including the body of an email whose subject line qualified
- Instagram, Facebook, LinkedIn, and TikTok captions of more than roughly two sentences
- Landing page and website body copy
- Blog posts, articles, newsletters, scripts
- Anything where the reader is already committed to reading a paragraph

Length governs, not platform. A long X thread is body copy. A two-word Instagram caption
is constrained short-form.

### Patterns conditionally available

Only these, and only under the test below:

- **Strike 3, stacked short fragments.** Real character economy. "Sale ends midnight.
  200% bonus." carries two facts a full sentence could not fit.
- **Strike 9, one-word sentences.** Where the single word is the message.
- **Strike 12, rule-of-three.** As list economy, when three items are genuinely being
  listed.
- **Strike 8, repetition.** High bar. Repetition costs characters, so it is rarely the
  efficient choice; allow it only when the repeated element is the offer itself.
- **Strike 13, colon headlines.** In subject lines and ad headlines the colon is a
  labeling convention readers scan for, not a reveal device. "Flash Sale: 200% Bonus" is
  fine. "Tool Sprawl: Why Your Stack Keeps Growing" is still a strike, because the colon
  is setting up an essay.
- **Strike 11, questions.** A question that is the entire message is fine. A question
  that sets up an answer you then supply is still a strike.
- **Strike 1, em dash as separator.** Only in the separator role in a headline or subject
  line, where it functions like a pipe or bullet. The mid-sentence aside stays banned
  everywhere.

### Patterns that stay banned everywhere

These are cleverness, not compression, and they read worse under a character limit than
in a paragraph because there is nowhere to hide:

- Strike 2, "X, not Y" contrast
- Strike 4, engineered symmetry and visible cleverness
- Strike 5, fragment-stack accumulation
- Strike 6, two-beat reversals
- Strike 7, "That's not X. It's Y."
- Strike 10, "Here's the thing" pivots
- Strikes 14-20, all structure and tone strikes
- Strikes 21-22, false precision and context assumption. These are coherence failures,
  not rhythm devices, so no character limit ever releases them.
- The vocabulary ration, unchanged. Headlines in particular still take none of those
  words. "Unlock your bonus" is a category cliché and a tell at the same time; write what
  the player actually gets.

Strike 19, performed enthusiasm, is worth a note rather than an exemption. The strike is
enthusiasm about mundane things. A 200% bonus expiring at midnight is not mundane, so
energy about it is honest. Manufactured excitement about a routine login or a newsletter
is still a strike.

### The test before using a released pattern

1. **Write the plain declarative version first.** Subject, verb, object.
2. **Check whether it actually fails.** Does it exceed the character limit, or does it
   drop information the reader needs? If the plain version fits and carries the message,
   the plain version ships. Preference for rhythm is not a constraint.
3. **Name the pattern and the constraint.** If you cannot say which released pattern you
   are using and which limit forced it, you are reaching for rhythm.
4. **One released pattern per asset.** A subject line does not get fragments plus a
   one-word sentence plus a triad. Two or more stacked patterns in eight words is the
   fingerprint this whole gate exists to remove.

### Scope of a granted exemption

The exemption is per-instance, not per-project. It does not carry from a subject line to
the email body, from an ad headline to the ad's landing page, or from one asset in a
campaign to the next. Sweep every piece separately.

When producing a set of variants, do not make the released pattern the house style across
all of them. If five of five subject lines are fragment stacks, the set is patterned even
though each line passed on its own. Vary the construction across the set.

## Hard strikes — syntax and rhythm

1. **Em-dash overuse.** Drastically reduce em-dash frequency: most deliverables should
   contain zero, and long-form earns at most one or two. When one is used, it must serve
   a legitimate grammatical function (break in structure, parenthetical,
   colon-replacement, summary, attribution) per `references/em-dash-rules.md`. The
   reflexive mid-sentence aside as a rhythm device is the tell and is banned.
2. **"X, not Y" contrast constructions.** "A system, not a spreadsheet." "Built like
   software, priced like a template."
3. **Stacked short fragments as rhythm.** "Drag, drop, ship."
4. **Engineered symmetry / visible cleverness.** "It took 40 hours to build so your
   Mondays take one less." Copy that performs its own construction.
5. **Fragment-stack accumulation narratives.** "A CRM for the sales handoff. A scheduler
   because the CRM's calendar is bad. A reporting layer because now the data lives in six
   places."
6. **Two-beat reversal endings.** "Each decision made sense. The stack doesn't."
7. **"That's not X. It's Y." reframing.**
8. **Anaphora / triple repetition.** "Eleven tools. Eleven logins. Eleven renewal dates
   nobody tracks."
9. **One-word dramatic sentences.** "Simple." "Done." "Exactly."
10. **"Here's the thing:" / "Here's why that matters:" pivots.**
11. **Rhetorical questions as setup.** "So what does this actually mean?"
12. **Relentless rule-of-three.** Three adjectives, three examples, three clauses as the
    default shape. A deliberate, occasional triad is allowed; the pattern-as-reflex is the
    tell.
13. **Colon headlines.** "Tool Sprawl: Why Your Stack Keeps Growing."

## Hard strikes — structure

14. **Tidy-bow conclusions** that restate the thesis. "Ultimately, the goal isn't X, it's
    Y."
15. **Balanced hedging on every claim.** "While X has merits, Y..."
16. **Signposting.** "Let's break this down." "First, let's look at."
17. **Uniform paragraph lengths** — every section the same shape and size.

## Hard strikes — tone

18. **False intimacy.** "Let's be honest." "We've all been there."
19. **Performed enthusiasm** about mundane things.
20. **Hedged authority.** "Arguably one of the most important."

## Hard strikes — content and coherence

21. **False precision.** Oddly specific invented numbers used as texture: "eleven
    tools," "six of them." When a number is illustrative, round it the way a person
    talks: "a dozen tools," "a fraction of them." Real data keeps its real numbers;
    "$4,300 a month" from an actual audit stays precise. Precision is the tell only
    when the number is fabricated for flavor. This refines the "concrete specifics"
    replacement principle below: specifics must be real, never manufactured.
22. **Context assumption between sentences.** An early sentence leaning on a frame
    the reader has not been given yet, such as "The overlap is expensive" before
    stack-auditing has been established as the topic. Each early sentence re-anchors
    the subject until the frame is set. The reader should never need the headline to
    parse sentence two.

## Frequency reduction — vocabulary (rationed, not banned)

These words are legitimate English; the tell is density. Default to a plainer
alternative, and never use more than one of these per deliverable, none in headlines:

elevate, seamless, robust, leverage, unlock, empower, transform, streamline, harness,
supercharge, delve, unpack, dive deep, landscape, journey, game-changer, navigate the
complexities of, in today's fast-paced world, at the end of the day.

## Replacement principle — what to write instead

A ban list alone produces bland mush, which is its own tell. Fill the vacuum with:

- **Plain declarative sentences.** Subject, verb, object. Say the thing.
- **Varied sentence length by content, not rhythm.** Long when the idea is long, short
  when it's short. Never short for drama.
- **Concrete specifics over abstraction.** Named tools, real numbers, actual situations.
  "Costs $4,300 a month" beats "expensive." Real numbers only: an invented specific is
  strike 21, so when no real figure exists, round like a person speaking.
- **No visible cleverness.** If a sentence shows off its own construction, cut it. The
  reader should notice the idea, never the writing.
- **Earn transitions with logic, not phrases.** If paragraph B follows from paragraph A,
  the connection should be obvious without "That said" or "Here's why."

## Earned release — high-stakes craft (flag for review)

The banned rhythm devices are the machinery of genuinely powerful human writing;
they became tells through unearned deployment at zero stakes. Two conditions can
earn one back, and the mechanism is a review flag, never silent use:

- **Fragments (strikes 3 and 5):** when the point carries real weight and the words
  themselves are load-bearing ("Calm, kindness, kinship, love" — simple words,
  tremendous cargo), a fragment sequence may be used. Actively look for these
  genuine opportunities; never manufacture stakes to justify one. Fragment stacks
  carrying mundane cargo (product features, tool descriptions) stay struck no
  matter the construction.
- **Flag format:** mark the passage for the human reviewer — e.g. [FLAG: fragment
  release — verify stakes and word choice] — so context and word selection get
  judged at the edit. The flag is the license; pre-clearance is not required, and
  an unflagged release is a violation.

Related doctrine: dramatize through word selection inside plain sentences (one
weight-bearing verb or noun — "crumble" over "lose"), never through construction.
Construction-drama is what the strikes ban; selection-drama is always legal and
needs no flag.

## Process

Draft first, then sweep the draft against strikes 1-22 and the vocabulary ration before
delivering. For a constrained short-form asset, sweep against the full list, then check
any surviving pattern against the four-question test in the carve-out above rather than
assuming the surface grants it. The sweep is not optional and it is not the same as writing carefully; these
patterns reassert themselves during drafting and only a deliberate pass catches them.

When a strike is found, rewrite the sentence from its idea, not by lightly rephrasing the
pattern. Rephrasing a banned construction usually produces a different construction from
the same list.

Deliver only the finished prose. Do not append a report of which strikes were caught
unless the user asked for a review or is iterating on the gate itself.

## Reference

- `references/em-dash-rules.md` — the six legitimate em-dash functions, mechanics,
  en-dash vs em-dash, and the distinction between the tool and the tell. Read it whenever
  a draft contains an em dash and you need to judge whether it is earned.

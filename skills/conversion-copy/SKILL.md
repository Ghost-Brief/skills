---
name: conversion-copy
description: Voice-of-customer driven conversion copywriting engine. Use this skill whenever the user asks for copy on any decision surface — sales pages, landing pages, signup pages, registration flows, marketing emails, email sequences, subject lines, paid ads, CTAs, value propositions, or social posts whose job is to drive a click or signup. Trigger even when the user just says "write the copy for X" or "I need a headline" without mentioning conversion. Works for any brand (Ghost Brief, client work, or unbranded). Do NOT use for editorial content, articles, newsletters-as-content, or brand-awareness pieces with no direct action — those are not decision surfaces.
---

# Conversion Copy

A copy-construction engine built on one discipline: **the customer's language is the source of the copy, not inspiration for it.** Winning copy is assembled from what real people actually say, slotted into a framework chosen by a decision rule — never by taste, never by guessing.

The reference case: a clothing brand's control headline was "Find clothes you love" (a marketer's summary). The winning headline was "Big bum, thick waist, not so perky boobs?" — a customer's exact words. Same message, but verbatim beat paraphrase because paraphrase sands off the specificity that makes people feel seen. Every step below exists to protect that specificity from draft to delivery.

## Scope check (before anything else)

This skill applies only to **decision surfaces**: assets where the reader is meant to move from reading to a decision — buy, sign up, click, register, reply. Sales pages, landing pages, emails that sell, subject lines, ads, CTAs, signup flows.

It does not apply to editorial content, thought-leadership posts, or brand moments with no ask. If the request is for those, say so and step out of this skill.

## Step 0 — Intake gate

Four inputs are required. **Check the request and conversation first; only ask what's missing.** Never re-ask something already answered. Most requests need one or two questions at most; a fully specified request needs none.

1. **Asset type** — what surface is this? (Determines the surface pattern in Step 3.)
2. **VOC** — "Paste any raw customer language you have: reviews, survey answers, support tickets, community threads, sales-call lines, DMs. Unedited, exactly as written. If you have none, say 'none' and I'll work in proxy mode."
3. **Offer + single action** — what is being sold/offered, and what one action should the reader take?
4. **Voice layer** — which brand voice system applies, if any? (Skip if obvious from context.)

Ask these as one short message, not an interview. Then proceed without further check-ins until options are delivered.

## Step 1 — VOC coding

Take the raw language and code it. Do not summarize, clean up, or improve any line while coding. Grammar stays broken. Slang stays in.

Sort every usable line into buckets:

- **Problem messages** — pain with the current solution or situation
- **Desire messages** — the outcome they want, stated as a want ("I wish...", "I just want...")
- **Objection messages** — why they hesitate, what they don't trust
- **Outcome language** — how past customers describe results, in their words (this is testimonial fuel)

Tag each line with its **altitude**: category-level (problems with this *kind* of product) vs. product-level (problems with a *specific* solution). Category-level lines make hooks and headlines; product-level lines make body copy and differentiation.

Flag **edge-case lines** separately: anything phrased in a way you'd never write yourself — unexpected metaphors, blunt phrasing, oddly specific detail. These are disproportionately likely to be the winning hook precisely because they don't sound like marketing.

### Proxy mode (no VOC available)

When the user has no customer language, do not fabricate quotes and do not silently guess. Instead:

1. Source proxy VOC where the target reader already talks: community threads (Reddit, Slack, Discord), reviews of *competing* products, comment sections under relevant creators, the user's own inbound DMs/replies. Use web search where available. Collect real phrasing, not summaries of it.
2. If no proxy sourcing is possible, build from the user's stated understanding of the reader — and write the copy as testable hypotheses, not truths.
3. **Label the output.** Every deliverable built without real VOC carries a one-line flag: "Built on proxy/assumed VOC — validate against real customer language before scaling spend behind this." Never present proxy-built copy as research-backed.

Real VOC always outranks proxy VOC, which always outranks assumption. When real customer language contradicts the user's beliefs about their customer, the customer language wins — say so.

## Step 2 — Hook selection

The hook is the single strongest line of coded VOC — the one most likely to stop the right reader. Choose it from the buckets, favoring edge-case lines and category-level altitude for cold audiences.

**The hook's shape decides the argument framework. This is the core decision rule — no framework menus, no guessing:**

| Hook shape | Framework |
|---|---|
| Problem-shaped ("I hate how...", "X doesn't work") | **PAS** |
| Desire-shaped ("I wish...", "I just want...") | **DOS** |
| Audience doesn't know the problem exists | **ACCA** |
| Skeptical audience, high ticket, or trust-poor category | **PAPA** (or add explicit proof structure to PAS/DOS) |
| Email sequence building to a sale | **PASOP** |

Framework mechanics live in `references/frameworks.md` — read it before executing Step 3.

## Step 3 — Two-axis execution

Copy is built on two axes at once:

- **Axis 1 — asset type → surface pattern.** Subject lines, CTAs, value props, headlines, bullets, testimonials, and ads each have a proven structural pattern. The asset named in Step 0 selects it.
- **Axis 2 — hook shape → argument framework.** Anything with body copy (page, email, long ad) gets its argument structured by the framework from Step 2.

A landing page therefore uses both: PAS or DOS shapes the argument down the page, while the headline, CTA button, and any bullets each follow their surface pattern. A subject line uses only Axis 1.

Both axes are specified in `references/frameworks.md`. Read the sections relevant to the current asset. Execute with the coded VOC as raw material — the strongest lines go into the copy as close to verbatim as the surface allows.

## Step 4 — QA checks

Run every draft through these before it goes anywhere near voice or delivery:

1. **So what? Prove it.** Every claim must survive both questions. Claims that can't be proven get cut or backed with specifics from the VOC or the user's real numbers. Never invent proof.
2. **CTA timing.** The ask arrives only after the reader has what they need to say yes. On long pages the CTA comes late by design. A premature hero button on a considered purchase produces unqualified clicks, not conversions.
3. **Proof real estate.** Proof gets explicit space (testimonials, numbers, demos, guarantees), not implication. If the draft has no proof section and the audience has any skepticism, that's a defect.
4. **4 Cs / 4 Us.** Clear, concise, compelling, credible. Useful, urgent, unique, ultra-specific. "Concise" never means cutting the specific phrase that carries the meaning.

## Step 5 — Stacking order (voice and gate)

Layering is strict and runs in this order:

1. **Framework structures the argument** (Steps 1–4, this skill)
2. **Voice layer colors it** — apply the applicable brand voice skill (e.g., `ghost-brief-theme` for Ghost Brief work, a client's voice system for client work). Voice adjusts word choice, rhythm, and register. Voice never restructures the argument or replaces VOC-derived hooks with brand-sounding ones.
3. **`no-slop-filter` gates it last** — if that skill is installed, it runs on the final prose and wins on conflict, with one exemption:

**The VOC exemption:** verbatim customer quotes are exempt from the no-slop-filter gate and from voice smoothing. Customers talk in fragments, clichés, and broken grammar; that is the point. The exemption covers only true verbatim material (quoted or headline-lifted), not copy you wrote *around* it. If a gate rule and a verbatim quote collide, the quote stays and the surrounding prose adapts.

Name any unresolvable conflict between layers to the user rather than silently resolving it.

## Step 6 — Deliver options

Output is **2–3 strategically distinct options** — different angles, not rewordings:

- Different hooks from different VOC buckets (e.g., problem-led vs. desire-led), or
- Different altitudes (category-level vs. product-level), or
- Different frameworks where the hook genuinely supports more than one

Each option is labeled with: the hook, its VOC source line (or proxy flag), and the framework used. One line each — enough for the user to judge the strategic bet, not a memo. If one option is clearly strongest, say which and why in a sentence.

Never deliver three variations of the same angle and call them options.

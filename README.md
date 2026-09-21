<p align="center">
  <img src="assets/banner.png" alt="Ghost Brief · Skills for Marketing Operators" width="100%" />
</p>

# Skills for Marketing Operators

The agent skills we use to run Ghost Brief's own marketing work, published straight from the studio.

A skill is a small instruction file that teaches an AI assistant a repeatable discipline. Most AI marketing output comes out generic because the model is writing from a blank prompt, with none of the context that makes work specific. These files encode that context. Each one holds a method we actually use, written so an agent can run it the same way every time.

They're small, easy to adapt, and brand-agnostic. Take them, edit them, and fold them into your own setup.

## The skills

**[conversion-copy](skills/conversion-copy/SKILL.md)**: a voice-of-customer copywriting engine for decision surfaces (sales pages, landing pages, emails, ads). It codes real customer language, selects a framework from the shape of the hook, and returns strategically distinct options instead of three rewordings.

**[no-ai-tells](skills/no-ai-tells/SKILL.md)**: a writing gate that strips recognizable AI patterns from prose before delivery. A ledger of the constructions that make writing read as machine-made, enforced as automatic failures.

**[brand-voice-architect](skills/brand-voice-architect/SKILL.md)**: an interview engine that turns scattered copy preferences into brand writing guidelines substantive enough for an AI to write from reliably.

They compose. Voice guidelines built with brand-voice-architect become the voice layer inside conversion-copy, and no-ai-tells gates whatever either one produces.

## Install

**Claude (claude.ai)**: download the packaged file for the skill you want from [`dist/`](dist/) and upload it as a skill in your Claude settings. This is the fastest path if you don't work in a terminal.

**Claude Code and other agents**: copy the skill's folder from [`skills/`](skills/) into the skills directory of your project.

Each skill is self-contained. Install one, install all three, or lift the parts you like into skills of your own.

## Why we publish these

Ghost Brief is an independent product studio. We build products and systems for marketing operators, and we document the work as we go. This repo is part of that. The skills here are the ones we run daily, and when the real workflow changes, these files change with it.

The working notes behind them run in The Brief, our newsletter on what we're building and what we're learning.

**[Subscribe to The Brief →](https://brief.ghostbrief.co)**

## Use

Use these freely in your own work and in client work. Attribution is appreciated. Please don't repackage the repo itself for sale.

---

<sub>GHOST BRIEF · GHOSTBRIEF.CO · INVISIBLE CRAFT. UNMISTAKABLE PRODUCT.</sub>

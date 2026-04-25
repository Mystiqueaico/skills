---
name: writing-principles
description: Apply universal voice and substance rules to edit, audit, or rewrite any short-form content — LinkedIn posts, ad copy, content drafts, emails, internal briefs. Use whenever the user asks to "edit this draft," "apply writing principles," "voice-check this," "rewrite for voice," "make this more on-brand," "polish this," or shares writing for review. Enforces two always-apply layers — Hormozi sentence craft (3rd grade readability, active voice, kill adverbs/fillers, one comma max, positive language, concrete-over-abstract) and Every substance and voice (show the mess, open with friction, one big idea, personal stakes, endings that extend not recap, resonance test). Pair with an AI-pattern scrubbing skill (e.g., `avoid-ai-writing` by Conor Bronsdon) as a final pass.
metadata:
  version: 2.0.0
  contributors: Hormozi (sentence craft), Every / Working Overtime + Source Code (substance and voice)
  license: MIT
---
# Writing Principles — Sentence Craft + Substance & Voice

You're applying a two-layer voice system. Both layers are always-apply — every sentence, every draft, every edit. No exceptions.

**The mental model:**
- **Layer 1 — Sentence Craft.** Mechanical rules at the word/sentence level. How each sentence reads. Sources: Hormozi (readability, voice, adverbs, fillers, comma rule, redundancy) and Every (concrete-over-abstract, embodied specificity, anti-patterns table — hedges, correlatives, rhetorical filler, boilerplate authority, fake profundity, symmetrical-flourish, saggy recap).
- **Layer 2 — Substance & Voice.** How the post lands at the post level — what it's about, how it opens, how it ends, whether it resonates. Source: Every / Working Overtime + Source Code.
- **Editing checklist runs last** — a final pass before shipping.

A style guide is not a prompt. Prompts tell you what to write; this skill establishes how to sound while writing it.

This skill handles voice and substance only. Pair it with:
- **A structural-framework skill** (ABDCE, atomic essay, hook formats, etc.) when drafting from scratch — this skill audits and rewrites; it doesn't pick the structure.
- **An AI-pattern scrubbing skill** (e.g., the `avoid-ai-writing` skill by Conor Bronsdon) — run that as the final pass to catch em-dashes, sycophantic openers, "in conclusion," header-density tells, and other AI-specific tells this skill doesn't check for.

---

## How to Use This Skill

This skill audits and rewrites existing copy. Workflow:

1. Read the draft once for meaning. What's the post trying to do?
2. Identify Layer 1 violations (passive voice, adverbs, fillers, hedges, correlatives, rhetorical questions, two-comma sentences, "don't X" framing, abstract language where specifics are available, fake profundity, symmetrical-flourish constructions).
3. Identify Layer 2 violations (meandering open, no friction, no personal stakes, no mess shown, saggy recap ending, no clear "one big idea," fails the resonance test).
4. Rewrite. Show the rewrite first, then a brief "what changed and why" note (3-5 bullets max — don't lecture).
5. Run the editing checklist as a final pass before handing back.

**If the user wants to draft from scratch** (raw notes, topic + audience, idea dump), redirect them to `/writing-frameworks` — that skill picks the right structural framework, drafts, then chains back through this skill and `avoid-ai-writing` automatically.

---

## LAYER 1 — Sentence Craft

Mechanical rules at the word/sentence level. Sources: Hormozi (the foundational rules) plus Every (concrete-over-abstract, embodied specificity, anti-patterns table). These run on every single sentence. Internalize them; don't deviate.

### Readability
- **3rd grade reading level.** If a 9-year-old can't understand it, rewrite it. The test isn't "would my peers get it" — it's "would a 9-year-old get it on first read."
- **Simple words beat complex words.** "We borrow money so we can buy bigger stuff" beats "We utilize leverage to gain higher returns on our equity checks." When you reach for a long word, ask if a short one carries the same meaning. It almost always does.

### Voice
- **Present tense.** "When you create your sales page" beats "When you're creating your sales page." Present tense puts the reader in the moment.
- **Active voice.** "We carried the body out of the room" beats "The body was carried out of the room." Subject does the verb. If you find yourself writing "was [verb]ed by," flip it.
- **Positive language.** "Keep going" beats "Don't stop." "Stay inside" beats "Don't leave." Brain processes the noun even after a "don't" — so frame the action you want, not the one you're avoiding.

### Sentence Craft
- **Kill adverbs.** Use stronger verbs instead. "We slammed the door" beats "We shut the door really hard." If a verb needs an adverb to land, the verb is wrong.
- **Avoid filler words and hedges.** Cut these on sight: *very, super, way, actually, really, just, basically, maybe.* They add syllables, not meaning. Hedges especially make the writer sound unsure of their own claim — if the claim needs hedging, sharpen the claim instead.
- **One comma max per sentence.** Two commas means two thoughts crammed into one sentence — split them. Short sentences land harder.
- **Remove redundant words.** "We left at the same time" beats "We simultaneously left at the same time." If two words mean the same thing, keep the shorter one.
- **Remove unnecessary words.** If cutting a word doesn't change the meaning, cut it. "He exited his car" beats "He was able to get out of his car." This is the single highest-leverage edit you'll make.

### Concrete Over Abstract
Specificity is the single biggest tell of human-grade writing. Make every claim physical, named, numbered, or dated.
- **Use:** *"Claude spun up five PRs while I drank coffee"* — not *"optimized workflows."*
- **Use:** *"$400/month replacing $400k/year"* — not *"cost-effective."*
- **Use:** *"Gmail rate limits blocked 2,000 email operations"* — not *"ran into scaling issues."*

When you reach for a generic abstraction (workflow, scale, transformation, value), pause and replace it with the actual thing — the click, the number, the name, the moment. Abstractions are where attention dies.

### Embodied Specificity at Emotional Beats
When the post hits a moment of feeling — relief, dread, satisfaction, defeat — make the feeling physical, not abstract.
- **Use:** *"the relief felt as physical as the dread had been"* — not *"I felt better."*
- **Use:** *"a rush of satisfaction"* / *"I collapse afterward"* — not *"it was rewarding."*

The test: would this exact line apply to anyone, in any situation? If yes, it's abstract. Make it specific to *this* moment and *this* body.

### Anti-Patterns to Cut on Sight
| Pattern | What it looks like | Fix |
|---------|--------------------|-----|
| **Hedges** | *actually, maybe, just, kind of, sort of* | Delete the hedge or sharpen the claim |
| **Correlative constructions** | *"It's not X, but Y."* / *"Not just A — but B."* | Rewrite as a single direct claim. The construction performs balance instead of saying something. |
| **Rhetorical questions as filler** | *"But what does that really mean? Well..."* | Cut the question, lead with the answer. Or convert to a statement. |
| **Boilerplate authority** | *"Studies show..."* / *"Research suggests..."* (without naming the study) | Name the source or cut. Vague authority reads as bluffing. |
| **Fake profundity** | *"At the end of the day, it's just a tool."* / *"Sometimes the simplest answer is the right one."* | Cut. These sentences sound deep but say nothing. |
| **Overly symmetrical constructions** | *"Move fast, move smart. Build hard, build right."* | The symmetry signals manufactured polish. Pick one half, expand it. |
| **Saggy recap conclusions** | *"So as we've seen, X leads to Y..."* | End by *extending* or *reframing*, not summarizing. (See Layer 2 — Endings.) |

### Why Layer 1 Matters
LinkedIn (and most short-form social) rewards skim-readability. Every adverb, filler, or comma that doesn't earn its keep is a reason for the reader to bounce. Layer 1 rules aren't stylistic preferences — they're conversion mechanics. A 3rd-grade-readable post with active voice, short sentences, and concrete specifics will outperform a "more sophisticated" post written for the writer's ego, every time.

---

## LAYER 2 — Substance & Voice

Always-apply but operates at the post level — what the post is *about* and how it *lands*, not how each sentence reads. Source: Every's Working Overtime + Source Code style guide.

### Show the Mess
Include failures, frustrations, false starts, honest limitations. The polished case study where everything worked is the least credible thing on the feed. Readers reward writers who say what didn't work — the false starts make the framework believable.

When you have a "and then it worked" beat, ask: *what did I try first that didn't?* That's usually the more interesting line. Lead with the friction.

### One Big Idea Per Post
Each piece must coin, claim, or crystallize one memorable concept — a discipline, lesson, framework, architecture, or practice shift. If the post has two ideas, split it into two posts.

This is stricter than "one topic." Aim for one *load-bearing claim* the reader could quote back to a friend. Everything else in the post supports that claim.

### Open with Friction, Not Context
Most drafts start 3-4 sentences too early — a setup paragraph, a meandering intro, a "let me tell you about." Cut all of it. Start in the middle of something happening: a failure, a doubt, a surprise, a moment of career anxiety.

If the user's draft takes more than 3 paragraphs to reach the stakes, the opening is broken. Rewrite it to start with friction.

The diagnostic: read just the first paragraph. Does it make a reader want the second paragraph? If no, it's preamble — cut.

### Personal Stakes Ground the Post
Even analytical or how-to posts work better with the writer's stakes visible. Abstract industry analysis without personal stakes underperforms by ~80% on engagement (Every's data on Working Overtime).

Stakes don't mean the post is *about* the writer. They mean the writer's perspective is in the post — what they tried, what they learned, what changed for them. The argument is filtered through a real situation, not floated abstractly.

### Endings Extend, They Don't Recap
A bad ending summarizes what the post just said. A good ending does one of three things:
1. **Extends** — pushes the idea one step further than the body did
2. **Reframes** — recasts the body's claim from a new angle
3. **Opens** — leaves the reader with a question, contradiction, or next-step they have to resolve

If the closing paragraph could be cut and the post would still make its point, the closing is dead weight. Rewrite it.

### Resonance Test
After drafting, ask: *would a reader in the target audience read this and say "I'm not alone in feeling this"?* If yes, the post has resonance. If no, it's information without recognition — and information without recognition doesn't get shared.

This matters most for first-person operator content where the whole game is making the reader feel seen.

---

## Final Pass — Editing Checklist

Before you show the draft to the user, run this checklist. If anything fails, fix it. Don't ship known violations.

**Layer 1 — Sentence Craft:**
- [ ] Active voice throughout?
- [ ] Zero adverbs? Zero filler words / hedges (very, super, way, actually, really, just, basically, maybe)?
- [ ] 3rd grade reading level — would a 9-year-old understand every sentence?
- [ ] Short sentences, one comma max each?
- [ ] Positive language (no "don't X" framings — say "do Y" instead)?
- [ ] No redundant or unnecessary words?
- [ ] Present tense?
- [ ] Concrete, not abstract — every claim is named, numbered, dated, or physical?
- [ ] No correlatives ("not X, but Y"), rhetorical filler questions, boilerplate authority ("studies show..."), fake profundity, or symmetrical-flourish constructions?
- [ ] Emotional beats are embodied (physical, specific to *this* moment), not generic?

**Layer 2 — Substance & Voice:**
- [ ] Stakes clear by paragraph one — does friction land before any setup or context?
- [ ] One big idea — could the reader quote one load-bearing claim back to a friend?
- [ ] Personal stakes visible — is the writer's perspective in the post, not just floating analysis?
- [ ] Some mess shown — at least one false start, frustration, or honest limitation?
- [ ] Ending extends or reframes (not recaps) — could the closing paragraph be cut without losing the point? If yes, rewrite it.
- [ ] Resonance test — would a reader in the target audience say "I'm not alone in feeling this"?

If any box is unchecked, either fix it or explicitly flag the tradeoff to the user ("I kept the recap ending because X — let me know if you want me to rewrite it").

Structural concerns (hook strength, post type fit, framework choice, length targets, CTA format) are handled by the `writing-frameworks` skill — if the draft has a structural issue beyond voice and substance, flag it and recommend `/writing-frameworks` for a structural pass.

---

## After This Skill — Run avoid-ai-writing

This skill handles voice + substance. AI-pattern detection (em-dashes, sycophantic openers, "in conclusion," header-density tells, etc.) is handled by the `avoid-ai-writing` skill. Always run that skill as the final pass — it catches a different class of issues than what this skill checks for.

The clean chain when editing existing copy:
1. **`writing-principles`** (this skill) — sentence craft + substance & voice
2. **`avoid-ai-writing`** — scrub AI-specific tells

When drafting from scratch, prepend `writing-frameworks` first to pick the structural tool, then run this skill, then avoid-ai-writing.

When invoked via `/writing-principles`, the slash command chains both skills automatically.

---

## What to Show the User

1. The rewritten draft (clean, ready to ship — no markdown headings unless the platform supports them).
2. A short "what changed" note — 3-5 bullets max. Format: *"Cut [specific filler/adverb/redundancy], rewrote [passive→active], added [specific number/example], reframed [meandering open] to friction-first, rewrote saggy recap ending to extend the idea."*
3. Don't lecture. The user knows the rules. Just show them the diff in plain language.

---

## What This Skill Does NOT Do

- **Doesn't pick structural frameworks.** Use a separate framework-selection skill (ABDCE, atomic essay, hook formats, etc.) for drafting from scratch — this skill audits and rewrites.
- **Doesn't scrub AI-isms.** Pair with the `avoid-ai-writing` skill (Conor Bronsdon, MIT) as the final pass.
- **Doesn't enforce brand voice.** Brand-specific voice rules sit *on top of* this skill, applied by the agent calling it. This skill handles universal voice mechanics, not brand identity.

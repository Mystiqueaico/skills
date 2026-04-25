---
name: writing-frameworks
description: A toolbox of writing structure frameworks for short-form content — picks and applies the right structural tool when drafting a LinkedIn post, content piece, or short essay. Use whenever the user wants to "draft a post," "write something on [topic]," "turn these notes into a post," "structure this piece," "what framework should I use for X," "give me hook options," or "I want to write about [topic] but don't know how to frame it." Scans the user's input (raw notes, transcript, topic, idea), recommends the best-fit framework(s), then drafts using that structure. Covers 8 frameworks — ABDCE story, atomic essay, writing warm-up, 11 hook formats, Hook→Point→Action, post type rotation, the borrowed lens, and objection-handling. Pairs with `writing-principles` (always-apply voice/substance rules) — run this skill for structure, then run writing-principles for sentence-level polish, then run avoid-ai-writing for AI-pattern scrub.
metadata:
  version: 1.0.0
  contributors: Nicolas Cole (ABDCE, atomic essays), Dickie Bush (writing warm-up), LinkedIn AI Writing Library (11 hook formats), Every / Working Overtime + Source Code (borrowed lens, objection-handling)
  license: MIT
---
# Writing Frameworks — Toolbox for Short-Form Drafting

Eight structural frameworks for short-form content. Don't force every framework into every post — the job is to scan what the user gave you, recommend the right tool, then draft with it.

This skill handles **structure**. Voice/sentence rules are handled separately — after drafting with a framework here, run `writing-principles` for the always-apply baseline (Hormozi sentence craft + Every substance & voice), then `avoid-ai-writing` for AI-pattern scrub.

---

## How to Use This Skill

### Step 1 — Read what the user gave you

What did they hand over? Three common shapes:

| Input shape | Likely path |
|-------------|-------------|
| **Raw notes / transcript / idea dump** | Start with §3 (Writing Warm-Up) → extract candidate hooks → pick a framework based on which hook lands |
| **A topic + audience** ("write a post for agency owners about exits") | Pick framework from §6 (Post Type Rotation) → apply §1-5 as needed → §4 for hook variants |
| **A draft they want restructured** | Diagnose: what's the post actually doing? Then map to one of §1, §2, §5, §7, or §8 |

### Step 2 — Pick the framework

Use this selection guide. When two frameworks fit, pick the one that does more work — usually the one that handles structure end-to-end (ABDCE, Hook→Point→Action) over a single-layer tool (just hooks, just scope).

| If the post is... | Reach for |
|-------------------|-----------|
| A first-person story with a turning point | **§1 ABDCE Story** |
| A focused single-idea observation | **§2 Atomic Essay** (also: scope test for any draft) |
| Drafted from raw notes / transcripts / ideas | **§3 Writing Warm-Up** first, then a hook format |
| Weak in the first 2 lines | **§4 11 Hook Formats** |
| Any post that needs end-to-end structure | **§5 Hook → Point → Action** (universal) |
| A new entry in a content calendar | **§6 Post Type Rotation** (variety check) |
| About a played-out topic | **§7 The Borrowed Lens** (use unexpected discipline as frame) |
| For a skeptical audience | **§8 Objection-Handling** |

### Step 3 — Draft + recommend the next pass

After drafting, tell the user:
1. Which framework you used and why (1-2 sentences max)
2. The draft itself
3. *"Now run `/writing-principles` to apply the always-apply voice rules + AI-pattern scrub."*

Don't run writing-principles inline yourself — keep this skill focused on structure. Composition stays clean when each skill does one thing.

---

## 1. ABDCE Story Framework (Nicolas Cole)

Use for story-driven posts — typically the highest-performing format on LinkedIn for operator/founder audiences.

| Letter | Element | What it does |
|--------|---------|--------------|
| **A** | Action | Open in the middle of something happening. Drop the reader into a scene. No preamble. |
| **B** | Background | Now step back and give context. Who are you? Why does this matter? What led here? |
| **D** | Development | The journey. What happened next? What changed? What did you try? |
| **C** | Climax | The turning point. The moment of insight, the deal closing, the realization. |
| **E** | Ending | The takeaway. What you learned. What the reader should take from this. |

### Why this works on LinkedIn
- **A** = the hook (first 1-2 lines). Drops the reader into action, forces "see more."
- **B** = establishes credibility naturally without bragging ("I'd been running my agency for 4 years…")
- **D** = the meat of the post. Keeps people reading.
- **C** = the payoff. The moment that makes the post shareable.
- **E** = the CTA or lesson. Drives comments and saves.

### Example
> **A:** I almost walked away from the deal that changed everything.
> **B:** I'd been running my agency for 4 years. Good revenue, good team, good clients. But I was burned out.
> **D:** When the acquirer reached out, the first offer felt low. I sat on it for a week. My advisor said one thing that reframed everything.
> **C:** "You're not selling your revenue. You're buying back your time."
> **E:** That conversation cost me $0 and saved the deal. If you're an agency owner weighing an exit — the math isn't just financial. DM me if you want to talk through it.

### When NOT to use ABDCE
- The post is making a single quick observation (use atomic essay scope instead).
- There's no real turning point or climax — forcing the C makes the post feel manufactured.
- The user wants a framework/listicle/teardown — those have their own structures.

---

## 2. Atomic Essays (Nicolas Cole / Ship 30 for 30)

An atomic essay is a **250-word focused piece on one single idea.** It's the building block of all good social content. Use this as a scope test for any draft, even when you're not writing a "pure" atomic essay.

### Rules
1. **One idea per post.** If you have two ideas, write two posts.
2. **250 words max.** Forces clarity. Cuts fluff.
3. **Strong title/hook.** The first line IS the title. It must stand alone.
4. **1-3-1 structure:**
   - 1 sentence hook
   - 3 supporting points (evidence, story, framework)
   - 1 sentence conclusion or CTA
5. **No throat-clearing.** Don't "set up" the idea. Start with it.
6. **Specificity wins.** "$5k refundable offer" beats "a bold offer."

### How to use this as a scope test
After drafting any post, ask: "Is this one idea, or did I sneak in two?" If two, split into two posts. The second one becomes a future-calendar item — don't waste it.

### Common scope failures
- Mixing "what I learned" with "here's the framework I built from it" — those are two posts. Pick one.
- Stacking three examples when one carries the idea — cut to the best one.
- Adding a "P.S. by the way…" that introduces a new theme — delete the P.S. or make it the next post.

---

## 3. Writing Warm-Up Routine (Dickie Bush)

Use this when staring at a blank page or when handed raw notes / transcripts / idea dumps.

### The 5-Minute Warm-Up
1. **Pick one idea** from the source material (meeting notes, journal, inbox captures, transcript).
2. **Write the worst version** — dump thoughts for 2 minutes, no editing, no order.
3. **Circle the one sentence** that's actually interesting. The sentence you'd quote to a friend if they asked "what was that about?"
4. **That sentence is the hook.** Build the post around it.
5. **Cut everything before the hook.** Most first drafts start 3-4 sentences too early.

### How to apply when generating from source material
When you're given raw notes, transcripts, or idea dumps:
- Extract 3-5 candidate "interesting sentences" from the source.
- Present them as hook options to the user.
- Let the user pick one, then build the outline around it.
- This makes the user the editor and you the generator — fastest path to a draft they'll actually ship.

---

## 4. 11 LinkedIn Hook Formats

Eleven proven hook patterns. Rotate through these — don't reuse the same format three posts in a row.

### Format 1: Most Powerful
Declarative statement + credibility parenthetical.
> The single most powerful lesson from selling my agency:
> (I wish someone told me this 5 years ago)

### Format 2: Big Number vs Small Number
Contrast creates curiosity.
> In 18 months, we've evaluated 200+ agencies.
> Only 12 made it through diligence.

### Format 3: The Call Out
Direct address to target audience.
> Agency founders doing $1-5M:
> These 5 mistakes are killing your valuation.

### Format 4: The Secret
Achievement + "the secret?"
> I sold my agency in under 90 days.
> The secret?

### Format 5: The Oddly Ignored
Positions something as contrarian or underrated.
> The most underrated skill for agency founders in 2026:
> Knowing when to stop selling services.

### Format 6: The Struggle
Before/after transformation.
> I burned out running a 15-person agency.
> Now I help founders avoid the same mistakes:

### Format 7: How To
Problem/benefit + specific solution + objection handler.
> How to know if your agency is actually worth selling (even if you think it's too small):

### Format 8: Belief Flip
Common belief → contradictory evidence.
> I used to think selling your agency meant giving up.
> Turns out, it was the most entrepreneurial thing I've ever done.

### Format 9: The List
3+ items creating an open loop.
> When I sold my agency, I lost:
> - My title
> - My team
> - My identity
> But I gained something better.

### Format 10: The Crazy Part
Achievement + "the crazy part?"
> We went from first conversation to signed LOI in 3 weeks.
> The crazy part?

### Format 11: Everyone Should
Universal empowerment + specific outcome.
> Every agency founder should know what their business is worth.
> Most never find out until it's too late.

### Hook Quality Test
- Does it work in isolation? (If someone only reads the first 2 lines, do they want more?)
- Is the specificity load-bearing? (A specific number/name/timeframe beats a vague claim.)
- Would the user click "see more" themselves?

If the answer to any of those is no, rewrite the hook before drafting the body. Hooks are 80% of LinkedIn performance.

---

## 5. Post Structure: Hook → Point → Action

Every post follows this structure regardless of format.

### Hook (lines 1-2)
- Must work in isolation. If someone only reads the hook, they should want more.
- Maximum 2 short sentences before the "see more" fold.
- Use one of the 11 hook formats above.

### Point (body)
- Single-sentence paragraphs. Lots of whitespace.
- 5-8 main points max — more than that and the post bloats.
- Use bullets and lists when delivering frameworks or steps.
- Each line should give a reason to keep reading the next one.
- End with a big takeaway — the line the reader will quote.

### Action (closer)
- Ask a question, invite a DM, or point to "link in comments."
- Should feel conversational, not salesy.
- Examples that work: *"What's your version of this?"* / *"DM me if you're thinking about this."* / *"Link in comments."*
- Examples that don't: *"Click here to learn more!"* / *"Book a call today."* — too transactional for the format.

---

## 6. Post Types to Rotate

Variety across the calendar. If three posts in a row are all stories, the feed feels samey. Rotate.

| Type | What it is | When to use |
|------|------------|-------------|
| **Framework** | Teach a concept with a named structure | When you have a repeatable insight ("The 3-Question Agency Valuation Test") |
| **Story** | First-person narrative using ABDCE | When you have a specific experience to share |
| **Listicle** | Numbered list of tips/lessons/mistakes | When you want high saves and shares |
| **Teardown** | Break down a real example | When you have a specific case study (cold email, website, deal) |
| **Hot take** | Contrarian opinion with evidence | When you genuinely disagree with conventional wisdom (don't manufacture takes) |
| **Build-in-public** | Share what's happening right now | When you have a real update, number, or behind-the-scenes moment |

### Calendar variety rule
Across any 5 posts, aim for at least 3 different post types. Repetition isn't bad if it's working — but if engagement is dropping, rotation is the first lever to pull.

### Don't manufacture
Hot takes especially — if you don't actually have a contrarian view, don't fake one for engagement. Readers smell manufactured outrage. Stick to types where you have real material.

---

## 7. The Borrowed Lens (Every / Working Overtime)

Pull a concept from an unexpected discipline as the interpretive frame for the post. Every's writers do this with dance, textual criticism, advertising, improv, classical music, architecture — fields outside the post's nominal subject.

### Why it works
The agency / SaaS / AI feed is saturated. Every operator is reading the same Hormozi clips, the same Welsh frameworks, the same Cole hook patterns. A post that frames "agency exits" through *textual criticism*, or "client onboarding" through *improv*, breaks pattern. The borrowed lens does the differentiation work for you.

### How to apply
1. **Name the dominant frame in the space.** What's the cliché lens everyone uses for this topic? (For agency exits: financial / valuation / multiples.)
2. **Pick a frame from somewhere else.** A field you have real exposure to — sport, art, music, science, craft, parenthood, history. Don't fake it; the reader can tell.
3. **Map the borrowed concept onto the topic.** Where does the metaphor hold? Where does it break? The breakage is often where the insight lives.
4. **Use the lens to reframe the climax of the post.** The borrowed concept earns its keep when it makes the takeaway sharper than the conventional frame would have.

### Example
- **Conventional lens:** *"Selling your agency is a financial decision."*
- **Borrowed lens (rock climbing):** *"Selling your agency is a route choice. The wall doesn't change. Your route does. And every climber you ask will give you a different beta."*

The climbing frame doesn't replace the financial analysis — it adds a layer of operator empathy the financial frame misses. That's what makes it shareable.

### When NOT to use this
- The post is a quick build-in-public update — too compressed for a layered metaphor.
- You don't actually know the borrowed field. Surface-level metaphors read as performative.
- The metaphor doesn't break in an interesting place. If it's a clean 1:1 map, it's just decoration.

---

## 8. Objection-Handling Framework (Every / Source Code)

When the audience comes in skeptical (about a tool, a method, a claim), name the objection inside the post. Don't pretend it isn't there.

### The pattern
Stack 2-4 objection → reframe pairs in the body of the post. Each pair is one short paragraph or one bullet.

### Example structure
> *"AI wrappers are overdone."* → The opportunity is just beginning. Most wrappers wrap the wrong layer.
> *"Agents can't handle real engineering work."* → Here's a morning in my workflow. Five PRs, one human review pass, ship.
> *"I tried vibe coding and it was chaos."* → You skipped the planning step. The plan is the moat, not the prompt.

### Why it works
- **Disarms the skeptic** — they came in ready to argue; the post argues their case for them, then answers it.
- **Builds trust faster than a one-sided pitch** — acknowledging the counter-argument is a credibility move.
- **Forces specificity** — vague objections get vague rebuttals. Sharp objections force sharp answers, which produces better content.

### How to source objections
- Read the comments on competing posts in your space — common pushbacks become your objections.
- Listen for what skeptical friends actually say at dinner.
- Pull from sales call transcripts — the objections buyers raise on calls translate directly to content.

### When NOT to use this
- The audience is already bought-in (preaching to the choir wastes the structure).
- You can't answer the objection well. Naming an objection you can't rebut weakens the post.
- The post is a story — objection-handling fits framework / hot-take / teardown formats better than narrative.

---

## What This Skill Does NOT Do

- **Doesn't enforce sentence-level voice rules.** That's `writing-principles`. After drafting here, run that skill.
- **Doesn't scrub AI-isms.** That's `avoid-ai-writing`. Run last in the chain.
- **Doesn't enforce brand voice.** Brand-specific voice rules sit on top of all three skills, applied by the agent calling them. This skill handles universal structural mechanics, not brand identity.

The clean chain when drafting from scratch:
1. **`writing-frameworks`** — pick the structure, draft
2. **`writing-principles`** — tighten sentence craft + substance
3. **`avoid-ai-writing`** — scrub AI tells

When editing an existing draft, you can usually skip step 1 and go straight to writing-principles → avoid-ai-writing.

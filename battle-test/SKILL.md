---
name: battle-test
description: "When the user wants to pressure-test an offer, ad, landing page, sales copy, email sequence, product launch, positioning statement, or go-to-market artifact through the lens of six deliberately chosen operator voices (Brunson, Cole Gordon, Hormozi, Matt Gray, Justin Welsh, Dickie Bush by default). Also use when the user mentions 'battle test,' 'pressure-test,' 'red team this,' 'punch holes in this,' 'critique this before I launch,' 'offer review,' 'what would [Hormozi/Brunson/Welsh] say,' or wants a pre-launch QA pass on any marketing/sales artifact. Produces a numeric scorecard, pattern analysis, and ship-now/defer/reject triage so the user leaves with concrete adjustments — not six contradictory opinions. Invoke any time the user is about to launch, publish, or commit resources to a marketing/sales artifact and wants structured dissent before they ship."
metadata:
  version: 1.0.0
---

# Battle Test

You are a six-voice adversarial panel. Your job is to pressure-test a marketing or sales artifact before the user ships it — through the deliberately contrasting worldviews of six operators with different biases about what makes an offer work.

This is not consensus review. It's structured dissent. Six strong opinions, scored numerically, triaged into actionable buckets.

## When to Use This Skill

**Use when the user is about to ship:**
- An offer (core product + price + guarantee + stack)
- Ad creative (copy + hook + visual direction)
- A landing page (headline, flow, CTA)
- Sales copy (pitch deck, proposal, email pitch)
- A product launch plan (funnel, positioning, bait/tripwire structure)
- An email sequence (nurture, cold outreach, post-purchase)
- Positioning / category language / manifesto

**Don't use for:**
- Subjective art or design choices (the panel isn't tuned for aesthetic judgment)
- Code review, engineering architecture, or technical QA
- B2B enterprise sales proposals where the buyer is an executive committee (the panel is tuned for direct-response, product-led, and operator-led GTM — not complex enterprise sales cycles)
- Editorial prose (use `copy-editing` instead)

## Core Philosophy

**Six operators with deliberately different biases > any one guru.** Each guru represents a different bottleneck in a go-to-market:

| Bottleneck | Guru | Their obsession |
|---|---|---|
| Funnel mechanics | **Russell Brunson** | Value ladder, bait→tripwire→core→profit max, lead capture |
| Backend conversion | **Cole Gordon** | High-ticket sales, discovery calls, hard CTAs |
| Offer construction | **Alex Hormozi** | Grand slam offer, guarantees, value-to-price ratios |
| Distribution | **Matt Gray** | Organic-first, LinkedIn audience, founder OS |
| Product & pricing | **Justin Welsh** | Operator voice, digital products, ladder economics |
| Delivery format | **Dickie Bush** | Cohort > self-serve, community-driven completion |

When the same critique surfaces from 3+ gurus across different worldviews, that's real signal. When one guru raises it in isolation, that's personal bias — file but don't necessarily act.

**The skill's value isn't the opinions. It's the triage.** The user should leave with 3–5 ship-now adjustments they can implement this week, a deferred parking lot with dates, and a list of intentional rejections so the dissent is documented not dismissed.

## Inputs

At minimum:
- **The artifact** being tested (offer, copy, ad, landing page, positioning, etc.) — pasted inline, linked, or file path
- **The stage** (pre-launch, live, iterating) — changes what adjustments are actionable

Helpful but optional:
- **The ICP / buyer** — who it's for
- **Intentional design choices** — decisions the user has already made deliberately (e.g., "direct-response only, no lead capture," "$47 price locked," "faceless brand") so the skill can flag gurus pushing against these as conscious-reject rather than ship-now
- **Custom panel** — user can swap or add gurus (see `references/gurus.md` for panel options)

If any of these are missing and would materially change the output, ask the user before proceeding. Don't guess on intentional choices — silently converting an intentional decision into a ship-now recommendation is the failure mode to avoid.

## Workflow

### Step 1 — Read the artifact in full

Read whatever the user provided. If it's a file path, read the file. If it's a URL, fetch it. If it's inline, parse it. Understand both what it says and what structural choices it reflects (price, format, funnel mechanic, target audience).

### Step 2 — Score each guru on two dimensions

For each of the six gurus, produce:
- **Angle score (1–10):** positioning, offer, avatar, message-market fit, emotional hook
- **Format score (1–10):** delivery mechanism, price, funnel mechanics, distribution, friction, guarantees

Each score comes with **one sentence of main pushback** in that guru's voice. Use their characteristic vocabulary (Hormozi says "grand slam offer," Brunson says "value ladder," Welsh says "solopreneur ladder"). The voice matters — it's the difference between structured dissent and generic critique.

Detailed lens for each guru (their obsessions, signature language, typical pushbacks, known blind spots) is in `references/gurus.md`. Read it when scoring if the guru's position on a specific dimension isn't obvious.

### Step 3 — Surface the pattern

After the scorecard, compute:
- **Average angle score** and **average format score** across all six
- **The cluster:** which critiques surface from 3+ gurus independently? Those are real signal.
- **The singletons:** which critiques surface from just one guru? Those are personal bias or niche.

The gap between cluster and singleton is the heart of the output. A cluster of "price too low" from Hormozi + Welsh + Bush is a real issue. Hormozi alone saying "add a guarantee" is a real suggestion but lower urgency.

### Step 4 — Triage into three buckets

Every critique from the panel goes into exactly one of three buckets:

1. **Ship-now** — adjustments the user can implement this week that would materially improve the artifact *within the user's existing constraints*. Aim for 3–5 per battle test. Each includes: what, why, effort estimate, which guru(s) it came from.

2. **Defer** — critiques that are real but out of scope for this launch. Each includes: what, when to revisit (specific trigger: "post-launch if CPA > X" / "W18+ when diagnostic ships" / "after first case study"), which guru(s) raised it.

3. **Consciously reject** — critiques that push against an intentional design choice the user made deliberately. Each includes: the critique, the user's stated reason for the choice, why we're rejecting the guru's pushback for *this launch*, and under what future condition we'd reconsider.

The bucket allocation is the output's value. A battle test with no rejections means the skill didn't understand the user's intentional constraints. A battle test with no ship-now items means the panel wasn't honest.

### Step 5 — Present the output

Use the structured output format below. Present results to the user cleanly. Don't editorialize beyond what the panel says — the user can make the final call on implementation.

## Output Format

Always use this structure:

```markdown
# Battle Test — [Artifact name]

## Scorecard

| Guru | Angle | Format | Main pushback |
|---|---|---|---|
| Russell Brunson | X | Y | "Quote-style pushback in Brunson's voice." |
| Cole Gordon | X | Y | "In Gordon's voice." |
| Alex Hormozi | X | Y | "In Hormozi's voice." |
| Matt Gray | X | Y | "In Gray's voice." |
| Justin Welsh | X | Y | "In Welsh's voice." |
| Dickie Bush | X | Y | "In Bush's voice." |

**Average:** Angle X.X / Format Y.Y

## Pattern

[2–4 short paragraphs. Name the clusters (critiques from 3+ gurus). Name the singletons (1-guru opinions). Call out which dimension is the weak spot (usually format > angle or vice versa).]

## Triage

### Ship now — [N] adjustments

1. **[Adjustment name].** What to change + why. Effort: [S/M/L]. Raised by: [gurus].
2. [...]

### Defer — [N] items

- **[Item].** Revisit when [specific trigger]. Raised by: [gurus].
- [...]

### Consciously reject — [N] items

- **[Critique].** [Guru(s)] pushed on this; we're rejecting because [user's stated intentional reason]. Reconsider if [future condition].
- [...]

## Net verdict

[One-paragraph summary: ship / ship with adjustments / rework. Honest about where the artifact stands.]
```

## Quality Rules

- **Stay in-voice.** Each guru's pushback should use their actual vocabulary. Generic critique fails the skill. If you can swap a guru's pushback between two gurus and it still reads true, the voices are too similar — sharpen them.
- **Numeric scores are decisive, not wishy-washy.** A 7 means different things from a 6. Don't rate everything 6-7 to avoid commitment.
- **Flag intentional rejections, don't silently convert them.** If the user told you "$47 price is locked" and Welsh says "raise to $150," that goes in "consciously reject" with the rationale. Not in ship-now.
- **Ship-now bucket must be actionable this week.** "Rebuild your distribution around LinkedIn organic" is not ship-now — that's defer. "Add a guarantee to the landing page" is ship-now.
- **Don't over-triage.** If every critique ends up in "consciously reject," the skill isn't challenging the user. If none end up there, the skill isn't listening to the user's constraints. Expect a mix.
- **When running the skill iteratively on the same artifact, track deltas.** If the user incorporated ship-now adjustments from the last battle test, the next test should score higher on those dimensions. If scores didn't move, the adjustment didn't land.

## Custom Panels

The canonical 6 (Brunson / Gordon / Hormozi / Gray / Welsh / Bush) cover direct-response, product-led, and operator-led GTM. For artifacts outside that range, swap in more relevant voices.

**When to swap:**
- **Enterprise B2B sales** → replace with Chris Orlob, Blair Enns, April Dunford, David C. Baker, Jonathan Stark, Philip Morgan
- **Creator-economy product** → replace with Nathan Barry, Pat Flynn, Ali Abdaal, Nicolas Cole, Dickie Bush, Justin Welsh
- **SaaS / product-led growth** → replace with Lenny Rachitsky, Wes Kao, Elena Verna, Kieran Flanagan, Corey Haines, April Dunford
- **Agency sales / positioning** → replace with Blair Enns, David C. Baker, Karl Sakas, Louis Grenier, Marcus Sheridan, Chris Do

See `references/gurus.md` for each alternate's lens + signature pushbacks. If the user names a specific guru to add or swap, honor that even if it breaks the default 6.

## Reruns

Battle tests compound. Each rerun on the same artifact should:
- Reference the previous test's ship-now adjustments and check whether scores improved
- Keep the deferred parking lot — items don't graduate to ship-now unless the trigger condition fires
- Update consciously-rejected items if the user's intentional constraints have shifted

Save prior battle tests alongside the artifact so future reruns have memory. For agent workspaces, the convention is:
- `<artifact-folder>/battle-tests/YYYY-MM-DD-v1.md`
- `<artifact-folder>/battle-tests/YYYY-MM-DD-v2.md`

## Output Handling

When called, save the battle test alongside the artifact being tested (the offer doc, ad creative, landing page draft, etc.) — not to the skills directory itself. The output is a working artifact, not a reusable resource.

The panel's judgment is consistent regardless of which agent or user invokes it. What changes is what the caller does with the output — ship-now adjustments get applied, deferred items go to a parking lot, rejected critiques get logged for context.

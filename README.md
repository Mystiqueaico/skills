# Mystique Skills

A library of agent skills for AI-native operators.

These are operating procedures behind [Mystique](https://mystiqueai.co) — distilled, packaged, and shared as the same SKILL.md files our agents run on. Drop one into your AI assistant's skill directory and it triggers automatically when the prompt matches.

## What is a skill?

A skill is a self-contained Markdown file (`SKILL.md`) with YAML frontmatter that defines when it triggers and what the agent does when it runs. The format follows the [agentskills.io](https://agentskills.io) spec and works with any compatible agent — Claude Code, Cursor, VS Code Copilot, OpenHands, and more.

## Available Skills

### [writing-frameworks](./writing-frameworks/)
A toolbox of eight structural frameworks for short-form drafting — ABDCE story, atomic essay, the writing warm-up, eleven hook formats, Hook→Point→Action, post type rotation, the borrowed lens, and objection-handling. Picks the right structural tool for the input (raw notes, topic + audience, or an existing draft to restructure), then drafts with it. Pairs with `writing-principles` and `avoid-ai-writing` as the full short-form writing chain — frameworks → voice → AI-pattern scrub.

### [writing-principles](./writing-principles/)
Apply universal voice and substance rules to edit, audit, or rewrite short-form content. Two always-apply layers — Hormozi sentence craft (readability, active voice, kill adverbs/fillers, concrete-over-abstract) and Every substance and voice (show the mess, open with friction, one big idea, personal stakes, endings that extend not recap, resonance test).

### [battle-test](./battle-test/)
A six-voice adversarial panel for pressure-testing offers, ads, landing pages, sales copy, or product launches before shipping. Default panel: Brunson, Cole Gordon, Hormozi, Matt Gray, Justin Welsh, Dickie Bush. Output is a numeric scorecard, pattern analysis, and ship-now / defer / reject triage — structured dissent, not consensus review.

### [session-context](./session-context/)
End-of-session self-improvement cycle. At the close of any working session, the skill audits the conversation, captures decisions and lessons in dated memory files, applies fixes to skills or `CLAUDE.md` when the session revealed a concrete gap, and opens a PR with all changes scoped for under-2-minute review. Triggered by `/session-context` or natural language like "done for today," "wrap up," or "signing off." Requires git + GitHub CLI.

## Install

Copy the skill directory into your agent's skill location:

- **Claude Code** — `~/.claude/skills/<skill-name>/` (global) or `.claude/skills/<skill-name>/` (project)
- **Cursor / VS Code** — see your editor's skill setup; most read from a `.skills/` or equivalent directory
- **Custom agents** — point your skill loader at the `SKILL.md` file

Once the skill is in place, the agent loads it and triggers automatically when a matching prompt arrives.

## Why publish these?

Agencies running AI-native operations need shared SOPs more than they need closed playbooks. Every operator running an AI workflow is reinventing the same primitives — voice rules, pre-launch reviews, content frameworks. Sharing the operating procedures means the field moves faster than any one shop can.

These are the skills behind Mystique's day-to-day. New ones get added as patterns prove out.

## Contributing

Open for now. If you adapt one of these skills and find an improvement worth sharing, open a pull request. If you want to propose a new skill, open an issue with a draft `SKILL.md` and we'll review.

## License

MIT. Use them freely, fork them, ship them in your own products. Credit appreciated, not required.

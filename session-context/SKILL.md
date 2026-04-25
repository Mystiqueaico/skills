---
name: session-context
description: >
  End-of-session self-improvement cycle. Captures learnings, updates memory,
  improves skill files or CLAUDE.md, and creates a PR with the changes.
  Trigger phrases: "/session-context", "done for today", "let's wrap it up",
  "wrap up", "that's it for now", "end of session", "let's call it",
  "signing off", "good night", "close out the session"
metadata:
  version: 1.0.0
  license: MIT
---

# Session Context — Self-Improvement Cycle

Captures everything valuable from the current session and turns it into durable improvements: memory updates, skill refinements, and configuration fixes — then opens a PR so the changes are tracked and reviewable.

## Dependencies

- Git (required — for branching and committing)
- GitHub CLI `gh` (required — for creating PRs)

## Inputs

- The current conversation history (automatically available)

## Workflow

### Phase 1: Session Audit

Review the entire conversation and extract:

1. **New facts & decisions** — Strategy shifts, pricing decisions, new contacts, process changes, anything that should persist across sessions.
2. **Lessons learned** — What worked, what didn't, what to do differently. Tool issues, workflow improvements, surprising outcomes.
3. **State changes** — Anything tracked in the agent's memory file (project status, pipeline movements, deliverable status) that needs updating.
4. **Skill gaps or improvements** — Did any skill produce subpar output? Did the agent struggle with a workflow? Did the user correct the agent's approach?
5. **Configuration issues** — Missing permissions, broken integrations, settings that need updating.
6. **Template or playbook updates** — Corrections to existing templates, new templates needed, playbook steps that are wrong or missing.

If nothing meaningful was learned (e.g., a very short session with no new information), say so honestly and skip the PR.

### Phase 2: Write Changes

For each finding from Phase 1, make the appropriate file update:

#### Memory Updates

- **Session log** — Create a dated session log file in the agent's memory directory (e.g., `workspace/memory/YYYY-MM-DD-<topic>.md`) with a structured summary of the session.
- **MEMORY.md** — Update the agent's top-level memory file:
  - State tables (project state, pipeline, deliverables) — if anything moved
  - Key Decisions & Context — if any strategy decisions were made
  - Lessons Learned — any new learnings (always append, never delete)
  - People & Relationships — if new contacts were discovered

#### Skill Improvements

- If a skill's workflow was wrong or incomplete, update the relevant `SKILL.md`.
- If a new skill pattern emerged from the session, note it but don't create a full skill (flag it for future creation).

#### Agent Configuration

- If the agent's `CLAUDE.md` (or equivalent system prompt) needs updates, apply them.
- If `settings.json` permissions need updating, apply them.

#### Shared Resources

- Update files in shared or cross-agent directories if session work produced changes that should persist beyond a single agent.

### Phase 3: Branch, Commit & PR

1. Create a descriptive branch: `session-context/YYYY-MM-DD-<topic>`
2. Stage only the files that were meaningfully changed — do not stage unrelated files.
3. Commit with a clear message summarizing what was learned and what was updated.
4. Push the branch and create a PR with:
   - **Title:** `[Session Context] <date> — <1-line summary>`
   - **Body:** Structured summary of all changes grouped by category (memory, skills, config, shared).

## Output Format

Present a summary to the user before creating the PR:

**Session Context — [Date]**

**What I Learned:**
- [Bullet list of key takeaways]

**What I'm Updating:**
- [File path] — [What changed and why]
- [File path] — [What changed and why]

**What I'm Flagging (no change needed now):**
- [Any observations that don't warrant a file change yet]

Then after the PR is created:

**PR Created:** [link]
Changes are ready for review. Nothing is merged until you approve.

## Quality Checks

- Never delete existing content from MEMORY.md — always append (strike through outdated entries instead of removing)
- Session logs must include: date, session source, conversation summary, key outcomes, and open items
- Only update skills if the session revealed a concrete workflow gap — don't make speculative improvements
- Every file change must have a clear reason tied to something that happened in the session
- Don't fabricate or embellish — if the session was light, the context update should be light
- The PR should be reviewable in under 2 minutes — keep changes focused

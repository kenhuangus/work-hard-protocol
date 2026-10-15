---
name: work-hard-protocol
description: >
  Operating protocol for ambitious agent work across writing, coding,
  research, and general task completion. Adapted from Felix Rieseberg's
  tutorial "How to be more ambitious: A tutorial for humans with models"
  (felixrieseberg.com, Oct 2026). Load this skill when baseline execution
  is not enough and the work should be pushed toward the outcome, the
  expert standard, and outside disciplines.
---

# Work-Hard Protocol

Source: Felix Rieseberg, "How to be more ambitious: A tutorial for humans
with models". The protocol below translates his human-facing tutorial into
agent operating rules. Ambition has three axes: Altitude (higher
abstraction), Depth (expert-level execution), Range (multiple fields).
Speed (same work faster) is not covered; it needs no protocol.

## When to use this skill

- Ken says "work hard", "be ambitious", "go deeper", or similar.
- Any writing, coding, research, or task-completion job where a correct
  baseline answer exists but a better outcome is possible.
- Do not load for quick factual lookups or single-step actions.

## Hard rules (always)

1. Name the outcome, not the task. Execute toward the outcome.
2. Ask for the goal beyond the goal before acting.
3. Use the instruments a top professional in the field would use, not
   vocabulary that imitates them.
4. Set a hard, specific target. "Do your best" is not a target.
5. Never validate your own work. Define an outside judge before starting.
6. Borrow techniques from other fields. Do not roleplay characters.
7. Failure is allowed on scratch work and exploration. It is not allowed
   past the final check.

## Protocol 1 — Altitude: work at the highest useful abstraction

For any task, climb three rungs and state each before executing:

- Rung 1 (task): the literal request.
- Rung 2 (outcome): what the requester actually wants to happen next.
- Rung 3 (mechanism): a durable way to produce that outcome, which may
  replace the current workflow entirely.

Work at the highest rung the available data, tools, and access allow. If
access or instruments block rung 3, say exactly what is missing and work
at rung 2. Setting up the missing access (connectors, data feeds, tool
permissions) is itself rung-3 work and is worth doing first.

Tell-tale sign altitude applies: the result will be discussed in meetings
or reused by others. It applies less to pure creative work.

Ken-specific mappings:

- Coding: rung 1 = fix this file; rung 2 = this bug is gone and stays
  gone; rung 3 = suite-green, PR-ready change that the repo's review
  rules accept.
- Substack: rung 1 = write this section; rung 2 = a draft that meets the
  standing publication spec; rung 3 = the full pipeline (draft, blunt
  review, diagrams, QA, paste-ready docx).

## Protocol 2 — Depth: execute like the best professional in the field

Five moves. Apply all five to any deep task.

1. **Instruments.** Use the tools the field's best use. Databases and
   statistical models, not markdown tables. Full test suites and real
   reproductions, not edited snippets. Primary sources, not summaries.
   If you do not know what the experts use, find out before executing.
2. **Hard goals.** State a target that feels unreasonable, then treat it
   as reasonable. When the first pass reports it is impossible, keep
   going instead of lowering the target.
3. **Challenge assumptions.** Take the rawest material available and
   check the beliefs behind the task. Reproduce the claim from the raw
   data before accepting it. Business assumptions are rough
   approximations; test them.
4. **New knowledge.** Once inside the data, find what is not yet known.
   Build the simplest model or simulation that can surface a blind spot,
   and test it on data it has not seen.
5. **Outside judge.** Define the external check before starting. A judge
   the model runs on its own output does not count. The judge must be
   able to run and give feedback during the work, not only at the end.

**Depth-rewrite checklist.** Before executing a deep task, write down:

1. What a top professional in this field would do that the current plan
   skips.
2. The rawest material they would start from, instead of what has
   already been digested.
3. The specific methods and tools they would use.
4. The external check, other than you or the model, that would show the
   result is right.

Then rewrite the plan to ask for exactly that.

## Protocol 3 — Range: pull in other fields

1. **Nouns to verbs.** Restate the task as what it does, not what it is.
   A quarterly review is not "a deck"; it is "getting busy people to
   believe a story about cause and effect and to decide under uncertainty
   in 30 minutes." The verbs reveal which fields own useful methods.
2. **Assemble the crew.** Pick two to four roles from other fields whose
   methods apply (analyst, journalist, editor, short seller, forensic
   accountant, statistician). Extract what each role does to research or
   check its position. Do not ask the model to write or act as the role;
   ask it to perform the role's methods on the task.

Range works best with multi-agent execution: give each discipline its own
thread or subagent, then reconcile.

## Operating norms

- Specific hard goals beat "do your best". This is established
  goal-setting research, not opinion.
- Watching someone else do the hard thing first helps. When stuck,
  find the worked example or the person who did it and study the steps.
- Permission to fail applies to scratch, exploration, and drafts. It
  never applies to finished work.
- Treat missing data, tools, and access as first-class blockers. Name
  them before executing, not after failing.

## Domain playbooks

### Writing (Substack articles)

- Altitude: the deliverable is a publish-ready draft at the standing
  spec (plan first; blunt review with section references; fixes only on
  approval; diagrams; paste-ready docx). State the article's thesis as
  the outcome before drafting.
- Depth: instruments = the evidence stack (primary sources, verified
  URLs, the QA linter, the link verifier). Every number gets a source;
  unverifiable claims get replaced, never kept. The outside judge is the
  mandatory blunt end-to-end review before diagrams.
- Range: run the draft through a second discipline's lens (security,
  economics, statistics) wherever it strengthens the thesis.
- Standing constraints: Ken's voice rules win (we/us, no metaphors,
  STE100 where it fits); paywall placement is his; never auto-publish or
  schedule.

### Coding (gateway and agent work)

- Altitude: deliver the acceptance state, not the patch. Before
  starting, state it (suite green, repro confirmed, PR-ready under the
  repo's review rules).
- Depth: instruments = full test suite, type checks, a reproduction on
  the real environment. Challenge the assumption inside the bug report
  against raw logs and data before fixing.
- Range: attack the change the way a red team would. Where relevant,
  check the change against the PAA10 categories.
- Standing constraints: all work lands via PRs with code review; no
  direct pushes to main; Ken approves merges.

### Research

- Altitude: start by naming the decision the research must support. The
  deliverable serves that decision; everything else is appendix.
- Depth: primary sources first. Every finding gets a source line.
  Challenge the leading hypothesis against the rawest data available.
  Produce new knowledge where the data allows it.
- Range: synthesize through at least one outside discipline's
  framework. Name the discipline and say why it applies.

### General task completion

Run this pre-flight checklist before acting on any non-trivial task:

1. Outcome statement (altitude rungs 2 and 3).
2. One hard, specific target.
3. Instruments list (what the best in the field would use).
4. Outside judge defined (what proves it right, other than you).
5. One outside-field method to try.
6. What failure is allowed on (scratch only).

## Worked examples

**Writing.** Task: "summarize this paper." Rung 2: a summary Ken can
publish as a briefing. Rung 3: a briefing with every claim traced to a
verified source line, blunt-reviewed, diagram included. Depth move 3:
check the paper's key claim against its own raw figures before
repeating it. Range: read it once through a security lens, once through
an economics lens; keep what survives both.

**Coding.** Task: "fix the failing test." Rung 2: the failure is gone
and cannot return. Rung 3: full suite green, root cause covered by a new
test, PR-ready. Depth move 1: reproduce on the real environment with the
project's own test runner, not a guess. Depth move 5: the suite plus
code review is the judge. Range: ask how a red team would exploit the
original bug class elsewhere in the codebase.

**Research.** Task: "compare three vendors." Rung 2: a recommendation
Ken can act on. Rung 3: a comparison with primary pricing and docs,
assumptions challenged against raw data, scored on the criteria that
drive his decision. Range: score once as an engineer, once as a
finance officer.

**General.** Task: "book the dentist." Rung 2: an appointment Ken keeps.
Rung 3: the best-fit appointment with confirmations logged and a tracked
item so nothing falls through. (His dentist search is still open; this
is the pattern it should follow.)

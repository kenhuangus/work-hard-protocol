# work-hard-protocol

An operating protocol for ambitious AI agent work — across writing, coding,
research, and general task completion. It tells an agent (or a human working
with one) how to push past the literal request and toward the outcome, the
expert standard, and the outside discipline that would do it better.

The skill is a single file: [`SKILL.md`](SKILL.md). Drop it into any agent
that loads skills from markdown, and invoke it when baseline execution is
not enough.

## Origin

This protocol is adapted from Felix Rieseberg's tutorial
**["How to be more ambitious: A tutorial for humans with models"](https://x.com/felixrieseberg/status/2110023283169247623)**
(felixrieseberg.com, October 13, 2026).

Rieseberg — an engineering lead working on Claude at Anthropic — argues that
model capabilities are uneven: astounding in some directions, inadequate in
others. A few people learn to pilot the astounding parts; most people ask
for the capital of France. His tutorial makes "be more ambitious" concrete
through three axes: **Altitude** (work at a higher abstraction),
**Depth** (execute like the field's best expert), and **Range** (pull in
other fields).

His tutorial is written for humans using models. This skill translates it
into operating rules for the agent itself: instead of advice a human reads
once, it is a protocol the agent runs every time — with checklists,
worked examples, and domain playbooks. Credit for the ideas belongs to the
original post; any errors in the translation are ours.

## The three protocols

**1. Altitude — work at the highest useful abstraction.**
Every task has three rungs: the literal request, the outcome the requester
actually wants, and the durable mechanism that produces that outcome. The
agent states all three before acting and works at the highest rung its data,
tools, and access allow. If access blocks the top rung, it says exactly what
is missing instead of silently doing the shallow thing.

**2. Depth — execute like the best professional in the field.**
Five moves: use the instruments the experts use (databases, not markdown
tables; full test suites, not edited snippets; primary sources, not
summaries); set a target that feels unreasonable and treat it as reasonable;
challenge the assumptions behind the task against the rawest material
available; produce new knowledge once inside the data; and define an outside
judge before starting — never validate your own work. A depth-rewrite
checklist runs before any deep task: name what a top professional would do
that the plan skips, the rawest material they would start from, the methods
they would use, and the external check that would prove the result right —
then rewrite the plan to ask for exactly that.

**3. Range — pull in other fields.**
Restate the task as what it does, not what it is (nouns to verbs), which
reveals which disciplines own useful methods. Assemble a small crew of
roles from other fields — analyst, journalist, red teamer, forensic
accountant — and borrow their *methods*, never roleplay the characters.

**Operating norms:** specific hard goals beat "do your best"; failure is
allowed on scratch work and never on finished work; missing data, tools,
and access are first-class blockers to name before executing.

## How to use it

**Claude Code / Muse.** Copy `SKILL.md` into a skills directory the agent
reads, preserving the path shape `<skill-name>/SKILL.md`:

```bash
mkdir -p ~/.claude/skills/work-hard-protocol
cp SKILL.md ~/.claude/skills/work-hard-protocol/SKILL.md
```

Project-scoped instead of global: use `<project>/.claude/skills/work-hard-protocol/SKILL.md`.
Other agent frameworks that load skills from markdown (OpenAI-style
`skills/` directories, custom harnesses) work the same way: one directory,
one `SKILL.md`, the YAML frontmatter at the top declares the name and
trigger description.

**Trigger phrases.** Load the skill when you (or your orchestrator) say
"work hard", "be ambitious", or "go deeper" — or automatically for writing,
coding, research, and task-completion jobs where a correct baseline answer
exists but a better outcome is possible. Do not load it for quick factual
lookups or single-step actions.

**Domain playbooks.** `SKILL.md` includes worked playbooks for four
domains, each mapping the three protocols to concrete moves:

- *Writing* — the deliverable is the publish-ready outcome, not the
  section; evidence standards are the instruments; an independent review
  is the outside judge.
- *Coding* — the deliverable is the acceptance state (suite green,
  repro confirmed, review-ready), not the patch; attack the change the
  way a red team would.
- *Research* — start from the decision the research must support;
  primary sources first; synthesize through at least one outside
  discipline.
- *General tasks* — a six-item pre-flight checklist (outcome, hard
  target, instruments, outside judge, one outside-field method, what
  failure is allowed on).

## Contents

| File        | What it is                                              |
|-------------|---------------------------------------------------------|
| `SKILL.md`  | The full protocol: rules, the three axes, domain playbooks, worked examples |
| `README.md` | This file: origin, summary, and usage                    |
| `LICENSE`   | MIT                                                     |

## License

MIT. See [LICENSE](LICENSE). The underlying ideas are Felix Rieseberg's;
this adaptation is released under MIT for anyone to use and improve.

# Pitch Story

**The pitch story template — a successor to the pitch deck template, built for the AI era.**

In 2010, Sequoia published a pitch deck template, and a generation of founders filled in its slides: Company Purpose, Market Size, Competition, Team. It worked, because it was built for a world where building was expensive — so a credible *plan* was the scarce signal, and investors funded plans.

Building is cheap now. A competent founder can generate a full Sequoia-format deck in an afternoon, and investors know it. Plans became the most clonable artifact in the room. What can't be generated is a decision that already cost something, an eval built from years of real data, a refusal that loses deals every month, a customer quoting you unprompted.

**A good pitch shows decisions that cost something, not plans that promise everything.**

Pitch Story is not a deck template. It's a skill — a set of instructions any capable LLM can run — that interviews a founder, excavates what they've actually built, decided, and refused, and arranges it into a chaptered story an investor can retell without the founder in the room.

## Graph engineering, not loop engineering

Most AI pitch tools are loops: draft → critique → redraft. Loops converge on the average of every pitch the model has seen — polished, and identical to everyone else's.

This skill puts a graph at the center instead. Everything the founder provides becomes typed nodes (facts, decisions, beliefs, unlocks, customer voices, world-states) with typed edges (*caused*, *cost*, *proves*, *against*). The graph does the real work:

- A belief with no *proves* edge is a claim, and claims get cut or flagged.
- A decision with no *cost* edge is unverified judgment.
- The densest cluster picks which story leads.
- Chapters are cuts of the graph — and the same graph re-cuts for the hire pitch, the launch post, the Series A memo.

The one loop in the skill (draft → audit → fix) refines wording only. It is never allowed to add material. Only the founder can add nodes.

## The rule that makes it work

**The skill communicates; it never strategizes.** It presents what exists — it will not invent your GTM, your metrics, your moat, or your team's backstory. Every section has a Context Bar: if your material doesn't clear it, you get a specific, itemized Context Request instead of a plausible-sounding draft.

It will ask you for more context, repeatedly and without apology. That's not a limitation. A draft built on a thin dump flatters you in the room and fails in diligence.

## What's inside

```
SKILL.md          The skill: 6 principles, 7-phase workflow, audit checklist
RULES.md          Operating rules for any LLM running the skill (drop into
                  CLAUDE.md / AGENTS.md / your system prompt)
template.md       The Story Deck: 10 chapters, each point / proof / handoff
references/
  unlocks.md      The three unlocks every AI-era pitch rests on (research,
                  technical, market) and how to excavate them
  taste-ledger.md 12 components of a company's taste, with real-vs-fake
                  answer keys, routed into chapters
  story-graph.md  The graph, the spin, category canon research, four
                  narrative arcs, seven per-chapter story modes
  presentation.md How to present traction, competitors, demos, GTM, and
                  team; Context Bars; the memo spec; the final Story
                  Document (quiet narrative or interactive dossier)
examples/
  before-after.md Five before/after slides for a generic AI startup —
                  the old template's slide vs. what the skill produces
  sample-engagement.md  What a full engagement looks like
evals/
  evals.json      Test cases for the skill's behavior
dist/
  pitch-story.skill     Packaged skill, ready to install
```

## Quickstart

**Claude (claude.ai or Claude Code):** upload or install `dist/pitch-story.skill`, then say *"help me build my pitch"* and paste everything you have — deck text, memos, architecture docs, customer emails, benchmark results. The more raw material, the better the output. That's the design.

**Any other LLM:** paste `RULES.md`, then `SKILL.md`, into your system prompt or context, and attach the reference files when the skill asks for them (they're loaded per phase, not upfront).

**What you get back:** a three-sentence retell (the spec every chapter serves), a 60-second verbal pitch, a one-pager, a cold email, chaptered deck copy, a written memo, a technical appendix, a gap list of what you haven't lived yet — and a final Story Document as a single self-contained HTML file, print-ready for PDF.

## The six principles

1. **Excavate, never invent** — could every sentence survive a due-diligence call?
2. **First principles, not analogy** — strip the analogy; what remains is the pitch.
3. **Deeply technical is the style** — architecture, tradeoffs, evals. A proprietary eval is taste made measurable.
4. **Fingerprints over adjectives** — judgment is only visible in decisions that had a price.
5. **Retellability is the metric** — the pitch is judged at the partner meeting, without you.
6. **Communicate, don't strategize** — thin context gets a request, not a draft.

## Credits

The skill's format follows the behavioral-guideline structure popularized by Andrej Karpathy's coding guidelines. The per-chapter story modes adapt Kendall Haven's story-type research. The failure modes it targets were learned from reading a lot of decks.

**Created by Siddharth Ram** · [BoldCap](https://www.boldcap.com) · [X @siddharth_ram](https://x.com/siddharth_ram) · [LinkedIn](https://www.linkedin.com/in/siddharth-ram-8bb32132/) · siddharthr@boldcap.com

## License

MIT — use it, fork it, ship it. If it helps you raise, tell a founder about it.

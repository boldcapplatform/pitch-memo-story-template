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
dist/
  pitch-story.skill     Packaged skill, ready to install
```

## Quickstart

**Claude (claude.ai or Claude Code):** upload or install `dist/pitch-story.skill`, then say *"help me build my pitch"* and paste everything you have — deck text, memos, architecture docs, customer emails, benchmark results. The more raw material, the better the output. That's the design.

**Any other LLM:** paste `RULES.md`, then `SKILL.md`, into your system prompt or context, and attach the reference files when the skill asks for them (they're loaded per phase, not upfront).

**What you get back:** a three-sentence retell (the spec every chapter serves), a 60-second verbal pitch, a one-pager, a cold email, chaptered deck copy, a written memo, a technical appendix, a gap list of what you haven't lived yet — and a final Story Document as a single self-contained HTML file, print-ready for PDF.

## The principles

Eleven principles, in three acts: what goes into the pitch, how it's built, how it lands. Each one exists because pitches fail a specific way without it.

### Act I — The Material

**1. Excavate, Never Invent** — *Don't write before asking. Don't fill gaps. Don't accept claims.*

- No narrative line until the material is in — even when the founder arrives with a finished deck. Especially then.
- Never fabricate, embellish, or round up a fact, number, benchmark, or quote. A missing example is recorded as a gap, not filled.
- Chase every claim down to its fact, decision, or measurement, or cut it.

*The test: could every sentence survive a due-diligence call?*

**2. The Three Unlocks** — *Every AI-era pitch rests on what just became knowable, buildable, and wantable.*

- The research unlock: the capability shift the company quietly depends on, noticed before consensus.
- The technical unlock: what this team specifically can build that converts the shift into a product others can't easily copy.
- The market unlock: whose behavior or budget changed so a tribe now exists, reachable without renting someone else's channel.
- All three appear; one leads — chosen by where the evidence is strongest. The word "unlock" never appears; each is made felt through plain description.

*The test: could a partner name all three after one read?*

**3. The Taste Ledger** — *Judgment is only visible in decisions that had a price.*

- Twelve components of a company's taste, excavated every time: the arguable opinion, the tradeoff that cost, the feature killed, the workaround refused, the hire passed on, the promise with teeth, and six more.
- Fingerprints over adjectives: vision never stands where a scar exists.
- Fewer than two fingerprints means the story hasn't been lived yet. Saying so plainly is the most valuable feedback the process gives.

*The test: does every major claim have a scar or a measurement attached?*

### Act II — The Machine

**4. First Principles, Not Analogy** — *Strip the analogy. What remains is the pitch.*

- Every problem and solution claim derives from the structure of the problem: what is hard, why it stayed unsolved, why this path through it.
- "Uber for X" fails the filter. The category's canon shapes the argument's form, never its words.
- When the founder reasons by analogy, ask what remains without it. That remainder is the pitch.

*The test: does the argument stand if every named company in it disappears?*

**5. The Story Graph** — *Graph engineering, not loop engineering.*

- Everything the founder provides becomes typed nodes — facts, decisions, beliefs, unlocks, voices, world-states — with typed edges: *caused*, *cost*, *proves*, *against*.
- A belief with no *proves* edge is a claim, and claims get cut. A decision with no *cost* edge is unverified judgment. The densest cluster picks what leads.
- The graph, not the deck, is the company's narrative asset: the same graph re-cuts for the seed memo, the hire pitch, the launch post, the Series A.
- Iteration loops refine wording only. They are never allowed to add material — only the founder adds nodes.

*The test: can every sentence in the pitch be traced to a node in the graph?*

**6. Story Structures** — *Structure is chosen by the evidence, not by preference.*

- Four arcs — inevitability, discovery, craft, origin — fitted to where the graph is densest, never the other way around.
- The spin opens every arc: the world as it was, the world already moving without the company, the world with it. Ride the wave; never claim to be the wave.
- Each chapter runs one story mode — framing, struggle, put-a-face-on-it, wow, values-in-action, I-am-you, future vision — one dramatic intent per chapter.
- No struggle, no story: at least one real person's scene, because a pitch without a person in it is a report, and reports don't get funded.

*The test: read only the chapter titles aloud — do they tell the whole story?*

**7. Deeply Technical Is the Style** — *Architecture, tradeoffs, evals. Depth reads as taste.*

- The key architectural decisions, the tradeoff behind each, the reference architectures adopted and rejected — with reasons.
- Every performance claim cites its benchmark or eval, including the evals the team built itself. A proprietary eval is taste made measurable.
- Depth without jargon-performance: a smart generalist follows, a specialist nods.

*The test: could a technical partner probe any layer and find the founder home?*

### Act III — The Telling

**8. Attention** — *Hooks open. Takeaways close. Handoffs make the next chapter necessary.*

- Every section opens with a hook that frames what it must prove, and closes with a takeaway the reader can lift whole.
- A person and stakes appear in the first minute — the villain's bad week before the era-scale argument.
- The skim path is a first-class reader: hooks and takeaways alone must retell the entire pitch, because partners skim before they read.

*The test: would a reader who read only the openings and closings still get the whole story?*

**9. Visual Storytelling** — *The artifact is a taste signal. Its restraint is part of the pitch.*

- Show frameworks filled in, never described: the ledger, the map of defaults, the eval table as objects the reader inspects.
- The annotated run — one real request replayed with margin notes, unhappy path included — is the AI-native demo.
- Numbers in honest tables with full denominators; customer voices as pull-quotes; no icons, gradients, or decoration doing the work words should do.
- One self-contained artifact, in the style the use demands: the quiet print-first narrative, or the interactive dossier with a contents rail whose section titles alone tell the story.

*The test: does the document look like the company thinks?*

**10. Retellability** — *The pitch is judged at the partner meeting, without the founder.*

- The three-sentence retell is written first; it is the spec every chapter must serve.
- One opinion per pitch — three theses retell as zero.
- Prefer the scene to the statistic, the customer's sentence to the founder's. Zero superlatives, zero borrowed category language, zero TAM theater.

*The test: paraphrase the retell as a skeptical partner would. If the point survives, ship.*

**11. Communicate, Don't Strategize** — *Present what exists. Never write the founder's plan. Thin context gets a request, not a draft.*

- The skill presents; it does not invent strategy. GTM appears as beliefs and experiments already run, traction as pull that already happened, the team as lives already lived.
- Every section has a Context Bar. Below the bar, the output is a Context Request — specific, itemized, easy to answer — never a plausible-sounding draft.
- Output quality is bounded by what the founder drops in. Asking for more context, relentlessly, is the highest-leverage move in the system.

*The test: can every sentence in the output be traced to something the founder actually gave?*

These principles are working if: the pitch survives diligence, the graph outlives the deck, the retell survives the partner meeting, and nothing in the document could have been generated without the company having been lived.

## Credits

The skill's format follows the behavioral-guideline structure popularized by Andrej Karpathy's coding guidelines. The per-chapter story modes adapt Kendall Haven's story-type research. The failure modes it targets were learned from reading a lot of decks.

**Created by Siddharth Ram** · [BoldCap](https://www.boldcap.com) · [X @siddharth_ram](https://x.com/siddharth_ram) · [LinkedIn](https://www.linkedin.com/in/siddharth-ram-8bb32132/) · siddharthr@boldcap.com

## License

MIT — use it, fork it, ship it. If it helps you raise, tell a founder about it.

# The Operating Protocol

This is how the skill runs as a system, not a one-shot draft. Follow these stages in order, hold the gates, and keep the state object current. `SKILL.md`'s `## Workflow` names the seven phases; this file is the enforced version, with state, gates, and loops. When the two seem to disagree, this file governs how the engagement is run.

## The state object

Maintain four things across the whole engagement. They persist; every stage reads and writes them. Show the current state whenever the founder asks.

- **The story graph** — typed nodes and edges (`references/story-graph.md`). The company's real asset. Every deliverable is a cut of it.
- **The belief-stack** — the two or three load-bearing beliefs a reader must accept, each with a proof (or a marked gap where the proof does not exist yet).
- **The gap list** — what is missing, opened at Stage 1 and shrinking as the founder answers. This is the founder's pre-raise homework, tracked, not an end-note.
- **The config** — entry mode, the audience(s) (investor / talent / customer), the goal, and the outcome set.

The founder is the only source of material. Never add a node the founder did not give you.

## Entry modes (Stage 0 sets this)

- **New pitch** — start at Stage 1 and run the whole pipeline.
- **Sharpen an existing deck** — quick-polish: a light Stage 2, then Stage 5 (line-edit + faithfulness) and the audit only.
- **Re-cut** — a graph already exists; skip to Stage 6 and cut for a new audience.

## The stages

### 0 · Frame
Before anything else, settle the config: the entry mode, each audience (investor, talent, customer), the goal, and which artifacts are the outcome. The audience decides the cut at Stage 6, so pin it now. Write it down.

### 1 · Ingest
Collect everything before asking anything — decks, memos, architecture docs, landing page, transcripts, evals, metrics with denominators, customer emails. Open the **gap map** from what is missing.

### 2 · Excavate
Interview conversationally, a few questions at a time, never a form. Run three tracks: the three unlocks (`references/unlocks.md`), the taste ledger (`references/taste-ledger.md`), and the fingerprints — decisions that cost something. Every answer becomes a typed node. Every unanswered question becomes a gap.

### 3 · Spine
Lock the **belief-stack**: name the two or three beliefs a reader must accept for this to be a fundable bet, and attach a proof to each. A belief with no proof yet is written as a marked gap, never smoothed. This is the coherence spine; everything downstream defends it. (Detail: `references/taste-ledger.md`, "Taste in the Argument".)

### ◇ Gate 1 — enough anchors?
Do not proceed to Build until each leading belief rests on at least one anchor — an eval that ran, revenue that landed, a customer who stayed, a decision that cost. If it does not, return to Stage 2 and present the gaps as the blocker. Say plainly what is missing and why the story cannot be built yet. Naming this is the most valuable feedback the skill gives.

### 4 · Build
Turn the graph into a narrative. pitch-story designs the spin, chooses the arc, and cuts eight to twelve chapters (`references/story-graph.md`); **Story Architect** shapes the arc and runs its Quality Bar. Then run the coherence checks and the skeptic simulation (both below). Show the founder the chapter titles and the belief-stack side by side.

### ◇ Gate 2 — story approved
Do not draft prose until the founder approves the story: the belief-stack, the arc, and the chapter cut. Revisions here are one of two kinds (see The Two Loops). Get an explicit yes before Stage 5.

### 5 · Draft
Fill the template (`template.md`) and write the prose per the presentation patterns (`references/presentation.md`). Then run two passes on every section as you write it:

- **The line-edit** (`references/line-editing.md`) — cut the antithesis ("not X, but Y"), the em-dash pile-ups, the stacked adjectives, the AI tells.
- **The faithfulness check** — every specific claim traces to material the founder gave. Nothing invented. An unproven claim stays in as a marked gap with a note, never smoothed over.

### ◇ Gate 3 — faithfulness + anti-slop
Nothing ships until it passes both: zero fabricated specifics, and a clean line-edit. Run the full audit checklist in `SKILL.md`.

### 6 · Cut & Deliver
From the one approved graph, produce the cut for each audience in the config. Same nodes, different lead:

- **Investor** — leads with the market or technical unlock and the ask; the belief-stack is the spine.
- **Talent** — leads with the mission and the hardness of the problem; the founder and the stakes carry it.
- **Customer** — leads with the pain and the product; the unlock and the ask recede.

Deliver the outcome set: the retell, the 60-second pitch, the one-pager, the cold email, the Story Deck, the memo, the technical appendix, the gap list, and the Story Document. Hand the gap list back as the founder's homework.

## The two loops

- **Founder loop.** When the founder brings new facts, add nodes and return to Stage 2 to re-excavate. Only the founder adds material.
- **Wording loop.** When a section needs work but no new facts, refine the prose in place at Stage 5. The skill sharpens words; it does not invent material.

Keep the two loops distinct. That separation is what stops a revision from drifting into fiction — the failure mode of every draft-critique-redraft loop.

## Coherence checks (Stage 4, before Gate 2)

- **The through-line test** — read the chapter titles in order; they must state one advancing argument, each a consequence of the last. Topic titles ("The Problem," "The Market," "Our Solution") mean the cut is a report; re-cut around the belief-stack. (`references/story-graph.md`.)
- **Belief mapping** — each chapter defends exactly one belief in the stack. A chapter that defends none is cut.
- **The skim path** — hooks and takeaways alone must retell the whole pitch.
- **Retell survives paraphrase** — say the retell as a skeptical partner would; the point must survive.

## The skeptic simulation (Stage 4)

Simulate the partner before a real one does. Run Story Architect's adversarial pass (Sully) on the draft story: attack every belief, hunt the weakest anchor, name the one question that breaks the pitch. Then repair (Milo) — or, when the break is a missing fact rather than a wording problem, send it to the gap list. A story that survives the simulation is ready for Gate 2.

## How the two skills compose

- **pitch-story** owns: ingest, excavate, the graph, the belief-stack, the pitch-specific patterns (unlocks, taste ledger, presentation), the template, the line-edit, and the faithfulness check.
- **Story Architect** owns: the narrative arc, the Quality Bar audit, and the Sully/Milo skeptic-and-repair pass.
- **Sequence:** pitch-story builds the graph and the spine → Story Architect shapes the arc and audits it → pitch-story drafts per the template → Story Architect's Sully runs the skeptic simulation → pitch-story runs the line-edit and faithfulness, then delivers.

Story Architect is optional. When it is not loaded, pitch-story runs the arc selection (`references/story-graph.md`) and the audit itself; the coherence checks and the skeptic simulation still run, in pitch-story's own voice.

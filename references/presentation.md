# Presentation Patterns and the Final Deliverable

How to present the five sub-stories every pitch needs — from the founder's context dump, in ways that signal taste and read as native to the AI era. Load in Phase 5. Each section lists its minimum context (the Context Bar): if the dump doesn't clear the bar, output a Context Request for that section instead of a draft.

These patterns are not extra slides. Each one is *how a Story Deck chapter shows its proof*: Proof of Pull lives inside The Tribe, the Map of Defaults inside What Can't Be Cloned, the Annotated Run inside How It Feels, Distribution Beliefs inside The Engine, Fingerprint Bios inside The Character. The taste ledger routes into them (`taste-ledger.md`, "Where Each Component Lands").

## 1. Traction → "Proof of Pull"

Old way: an up-and-to-the-right chart with a truncated y-axis and a compound metric nobody can audit.

Present instead:
- **The pull ledger.** Each early customer as one row: how they found us, their words at signup (quoted), what they pay, whether they're still here. Ten honest rows beat any curve.
- **The number we watch.** One metric, with the reasoning for choosing it over the vanity alternative ("we track resolution rate, not deflection rate, because..."). The choice of metric is itself the taste signal.
- **Retention as scenes.** "Month 6: they turned off the human fallback" says more than a cohort chart. Pair scenes with the honest absolute numbers underneath.
- Always full denominators, zero-based axes, and the bad month left in. An honest dip presented calmly signals more confidence than a smoothed line.

Context Bar: raw numbers with denominators and dates; at least three customer quotes with sources; churn/retention truth including who left and why.

## 2. Competitors → "The Map of Defaults"

Old way: a 2x2 with the company alone in the top right.

Present instead:
- Frame competitors as **the defaults customers currently tolerate** — including spreadsheets, interns, and doing nothing, which are usually the real competition.
- **Say what each default gets right.** One generous, accurate sentence per competitor. Generosity reads as confidence; dismissal reads as fear.
- **The structural bet.** The one thing this company does that each default *structurally can't* — because of their architecture, their pricing, or their installed base — not merely doesn't yet.
- Never claim absence of competition. Claim a bet the incumbents are institutionally unable to copy, and say why.

Context Bar: the founder's honest read of each competitor's strength; at least one lost deal and the stated reason; the structural (not effort-based) reason each rival can't follow.

## 3. Demos and Test Runs → "Show the Unhappy Path"

Old way: a sizzle reel of the happy path, edited to hide latency and failure.

Present instead:
- **The annotated run.** One real request replayed end to end: input, the agent's decisions, the outcome — with the founder's margin notes on why each decision went that way. A trace told as a story is the AI-native demo artifact.
- **The unhappy path, handled.** Show the case where the system is unsure and what it does about it — the refusal, the escalation, the honest "I don't know." Trust is demonstrated at the edges, never on the happy path.
- **The eval beside the demo.** Every demo claim sits next to its eval number, the eval's provenance, and the current honest score. Invite the investor to bring their own test case.

Context Bar: at least one real run transcript or log; the eval suite's description and current numbers; one documented failure and the fix.

## 4. Go-to-Market → "Distribution Beliefs"

Old way: a funnel diagram, "land and expand," and pipeline math on customers who don't exist.

Present instead:
- **Two or three beliefs, not a strategy.** Opinionated bets about how this product travels ("support leads trust other support leads and nobody else; we grow inside their forums or not at all"), each with its reasoning.
- **One experiment per belief.** What was actually tried, what it cost, what happened — including the belief an experiment killed. A dead belief presented plainly is a taste signal no strategy slide can fake.
- **The GTM refusals.** What this company won't do for growth (cold spam, logo-chasing discounts, paid placement in the tribe's spaces) and what each refusal has cost so far.
- **Where the tribe already gathers.** Named places, not personas.

Context Bar: experiments actually run with outcomes; refusals with costs; named channels where real customers came from.

## 5. Team → "Fingerprint Bios"

Old way: headshots, logos, an advisor wall.

Present instead, per person, three lines:
- **What their life forced them to see** — the years or the wound that makes this company theirs.
- **One decision they own** — a call they made here, with its cost.
- **One refusal** — what they won't do, even under pressure.
Then, once for the team: the pass or the firing that proves the bar, and the two or three people they keep close whose presence is itself a filter.

Context Bar: real history per founder beyond titles; at least one owned decision each; the pass/firing story or an honest "hasn't happened yet" for the gap list.

## The Written Memo

The prose deliverable, for firms that circulate documents rather than sit through decks — increasingly the default at Series A. The memo's job is to do the partner's Monday work for them: it is the investment memo they would otherwise have to write, so every paragraph must survive being copy-pasted into their own doc.

Structure: the retell first, set apart, before anything else. Then the chapters as sections — same cut as the deck, same order, prose instead of slides. Then the technical appendix. Then the ask and the standard, last. Nothing before the retell, nothing after the ask.

Craft rules:
- **Headings are declarative sentences in the company's words**, never framework labels. "Power follows scarcity, and scarcity just moved" — a partner reading only the headings gets the whole argument. This is the chapter-titles test applied to prose.
- **Every section ends with a handoff line** that makes the next section necessary. A memo without handoffs is a stack of slides wearing prose.
- **Under 2,500 words** excluding tables. Partners skim; every section must also survive being read alone.
- Numbers live in simple tables with full denominators, never in paragraph-length number walls. Customer words appear as quotes, set apart. No adjective where a number exists.
- The villain scene goes early — the memo earns attention with one person's bad week before it argues an era.
- Where context is missing, the slot is visible and itemized (the Context Request, in-line), never smoothed over. A founder's memo with honest slots reads as more credible than a complete memo with hollow sections.
- The memo and the deck are two cuts of the same graph. They must never disagree on a number.

## The Final Deliverable: the Story Document

Assemble everything into **one self-contained HTML file** (all CSS inline, no external assets). The artifact itself is a taste signal — its restraint is part of the pitch.

**Ask the founder which outcome style before building** (or infer from how the document will be used), and offer PDF conversion after approval in either case:

- **The quiet narrative** (default) — a scrolling prose document that prints cleanly to PDF. Best when the document will be forwarded, printed, or read once, top to bottom. Spec below.
- **The interactive dossier** — a sectioned single-page app the reader navigates, for pitches with deep material that investors will return to and explore out of order. Anatomy:
  - A sticky contents rail (or tab bar) listing numbered sections — 01, 02, 03 — whose titles alone tell the whole story (the chapter-titles test, applied to navigation). Smooth-scroll or tab-switch; either way, every section must also survive being read alone.
  - A title block with badge chips stating what the document is and isn't (stage, confidentiality, any disclaimer), the one-line world, and who prepared it.
  - Every section opens with the same anatomy: the section number, a kicker line naming the move ("Step 3 · Building the narrative"), a declarative headline in the company's words, and a one-line hook that frames what the section must prove.
  - Every section closes with a takeaway the reader can lift whole — the section's point in one or two sentences, visually set apart. Hooks open, takeaways close; the skim path through hooks and takeaways alone must retell the pitch.
  - Frameworks are shown filled-in, never described — the ledger, the map of defaults, the eval table as artifacts the reader can inspect.
  - Sections cross-link where one claim is tested in another ("graded in 04 · Test It"), which is the story graph's edges made visible.
  - A verdict-style closing section (the ask and the standard), and optionally an appendix FAQ carrying the objections in Q&A form — allowed there because by then the story has already been told forward.
  - The dossier demands more material than the narrative: it exposes every framework filled-in, so thin sections are glaring. If more than two sections would carry Context Requests, build the quiet narrative instead and say why.

Structure: title + one-line world → the Retell (set apart, first) → the ten chapters in order, each with its point, proof, and any of the five section patterns above where they belong (Tribe carries Proof of Pull; What Can't Be Cloned carries the Map of Defaults; How It Feels carries the Annotated Run; Engine carries Distribution Beliefs; Character carries Fingerprint Bios) → Technical Appendix (the decisions/tradeoffs/evals table) → the ask and the standard. The Gap List is included only in the founder's copy, never the investor's.

Design rules: one serif for headings, one system sans for body; generous whitespace; black on off-white; customer voices as pull-quotes; numbers in simple tables with full denominators; no stock icons, no gradients, no logos-as-decoration, no emoji. If a page looks designed, quiet it down. Print CSS: page breaks before each chapter, A4 and Letter safe.

Offer PDF conversion after the HTML is approved, not before.

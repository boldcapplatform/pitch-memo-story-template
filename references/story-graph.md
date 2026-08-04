# The Story Graph

The mechanism underneath the pitch. Everything gathered in Phases 0–2 becomes a graph; the graph gets a spin and a structure; the structure gets cut into chapters. Build it explicitly — write it out for the founder to see — because the graph, not the deck, is the company's real narrative asset. It will be re-cut for every future audience: seed deck, hire pitch, launch post, Series A.

This is graph engineering applied to narrative, and it borrows that discipline's rigor on purpose: typed nodes under contract, edges that count only when real evidence passes along them, and anchors that cannot be argued with. The payoff is the same one that separates a graph from a linear chain of prompts — a pitch built this way is wide where the evidence is wide, honest where it is thin, and it survives the skeptical partner who leans on any single edge instead of collapsing like a straight line where one weak link stops everything.

## 1. Build the Graph

**Nodes**, typed:
- **Facts** — verifiable events, numbers, dates ("we shipped X in March," "eval score 84.2")
- **Decisions** — choices made, each with its cost attached (the fingerprints)
- **Beliefs** — the founder's opinions, each marked arguable or consensus
- **Unlocks** — the three from unlocks.md
- **Voices** — quoted words from customers, users, refusals
- **World-states** — snapshots of the market/technology at a moment in time

**Edges**, typed:
- **caused** (this shift caused that decision)
- **cost** (this decision cost that thing)
- **proves** (this eval proves that claim; this voice proves that pull)
- **against** (this decision was made against that default)

**Every node carries a contract** — one bounded claim, a stated type, and the evidence that fills it. A node whose content is a paragraph of prose is one only the founder can read; a node reduced to a single typed assertion with its proof attached is one the next node — and a skeptical partner — can consume without guessing. If you can't state a node as one claim plus its evidence, it isn't a node yet; it's a topic, and topics don't wire.

**Edges follow the real-edge test.** An edge counts only when something real passes along it. Before drawing *caused*, *cost*, *proves*, or *against* between two nodes, ask whether the second claim actually rests on the first, or whether they merely landed next to each other. An asserted connection that carries no load is a fake edge: it makes the argument look tighter than it is, and the first skeptic who leans on it finds air. Draw only the edges that carry weight — the pitch is only as strong as its real edges, never its drawn ones.

Rules: every Belief node must connect via *proves* to a Fact, Decision, or Voice — an unconnected belief is a claim, and claims get cut or flagged. Every Decision should carry a *cost* edge. Two proofs that trace back to the same source are one piece of evidence, not two — count the anchors, never the assertions; double-counted evidence is a hidden edge that inflates a chapter until diligence collapses it. The densest well-connected cluster in the graph is the pitch's natural center of gravity; note where it is before choosing a lead.

**The edge grammar.** Edges are typed *and* type-checked: each edge type is legal only between certain node types, which makes a bad connection catchable rather than merely wrong-feeling.

- **proves** may originate only at a **Fact, Voice, or eval** — never at another Belief. A belief that proves a belief is circular; only something from outside the argument can prove it.
- **cost** may originate only at a **Decision**. A cost with no decision behind it is a complaint, not a fingerprint.
- **caused** runs from a **World-state or Unlock** into a Decision or Belief — the world moved, and the company responded to it.
- **against** must target a **World-state** — a named default, incumbent, or reigning average, never a strawman.

Run the grammar as a check: any edge that breaks a type rule is either mislabeled or resting on a node that is not what it claims to be. Fix the node or cut the edge.

**Structure is separable from content.** The node set is the company's *material*; the chapter cut is the *structure* laid over it, and the two move independently. An editor holds the nodes fixed and changes only which cluster leads — producing the seed deck, the hire pitch, or the Series A memo from one graph, the way a compiled program stays fixed while its prompts are tuned. This is why the graph, not any single deck, is the asset: you re-cut the structure without rewriting the material, and no two cuts can contradict each other on a fact, because they read the same Fact node.

## 1b. Anchors — the Nodes That Cannot Be Argued With

A graph can be perfectly consistent and still be worthless. Wire enough beliefs to enough other beliefs and everything agrees with everything — an "audit" that checks the pitch's numbers against the pitch's own claims proves nothing. Internal consistency is not verification. This is the precise way a story fails diligence: green lights all the way down, and nothing actually anchored to the world.

The graph is only as honest as the nodes in it that refuse to move. Anchors are the claims a skeptic cannot argue with:

- **Measurements that happened** — the eval that actually ran on real data with an honest score, not "should reconcile."
- **Money that moved** — revenue that landed, a contract signed, a renewal, a deal walked away from.
- **People who stayed** — a named customer still on in month twelve, quoted in their own words.
- **Decisions that cost** — the hire passed on, the feature killed, the workaround refused. A price actually paid cannot be back-rationalized.

Every leading chapter must rest on at least one anchor. A cluster of beliefs with no anchor underneath is a mood, not an argument — send it to the gap list, not the deck.

**Freeze the load-bearing refusals.** Some nodes are kept off-limits precisely because they are the ones a founder under pressure would be tempted to bend to win the room — the promise with teeth, the refusal that costs deals. Mark them frozen: they do not get softened to make a chapter land easier. A pitch that will quietly weaken its own standard for one meeting has already spent the thing that made it credible.

**Verify like a fresh skeptic, never like the author.** The founder made the claims, so the founder cannot check them — a maker grading their own work only nods along in a different font. Interrogate every proof node from a clean context, and split the check three ways, because three lenses catch what one repeated question misses:

1. **Is it true?** Does the claim hold up to the fact, decision, or measurement underneath it?
2. **Is it current?** Is the proof still live, or a number from a version of the company that no longer exists?
3. **Would the source survive the pull?** If a partner called the customer, read the eval harness, or checked the bank — does it hold?

A proof that fails any lens returns to the gap list. Run this on the graph before a single chapter is drafted; it is the Audit's teeth applied early, while fixing a weak node still costs a question instead of a redraft.

Together these are the graph's **static checks** — the edge grammar, the real-edge test, the anchor requirement, and the three-lens verification. Run them over the artifact before it compiles into prose, the way a program is type-checked before it runs. A graph that passes them is not yet a good pitch, but a graph that fails them cannot become one.

## 1c. What This Graph Is Not

This is a modeling artifact, not an execution engine — and the distinction is worth stating, because "graph" now also names a different thing: the executable prompt and agent graphs that route model calls, run on a scheduler, and are optimized as programs (LangGraph, DSPy, and the like). The story graph borrows their rigor — typed nodes, checkable edges, a versioned artifact you can re-cut — but deliberately stops short of their defining property. It does not run.

- **It is authored, not generated.** Only the founder adds nodes; the skill never invents them. A graph the model fills in on its own is a different object, and a weaker one.
- **It has no runtime.** No scheduler, no state passed between nodes, no cycles executing. A chapter is a *reading* of the graph, not an execution of it.
- **Its output is a document, not a trace.** The artifact is the pitch and the reusable node set — something you version and re-cut by hand, not a pipeline that emits answers on demand.

If the day comes to run excavation, verification, and drafting as an actual agent pipeline — fan-out interviews, fresh-context verifier nodes, a synthesized retell — that is a *second* graph, an executable one, layered beneath this one. Keep the two separate: this graph decides what is true and what leads; that graph would decide how the work gets done.

## 2. Design the Spin

The spin is the arc of inevitability: the world's motion, with the company as its catalyst. Three world-state nodes, in order:

1. **The world as it was** — the old constraint, described concretely.
2. **The world as it's becoming** — evidence the motion already started *without* the company (the research and market unlocks live here). This is what makes the future credible: it is already happening.
3. **The world with this company** — the same motion, accelerated or catalyzed. Name what completes faster, and what the funding specifically accelerates.

The posture this creates: the founder is not asking the investor to believe in them. They are showing the investor a world already in motion and offering the fastest vehicle through it. Never claim to cause the wave; claim to be the one who saw it early and built for the water.

## 3. Consult the Category Canon

Before choosing structure, spend a research pass on the company's category: the two or three books its investors have all read, and the essays and Substacks currently shaping its discourse.

Use the canon two ways, and only two:
- **Borrow shapes, never language.** If the category's canonical book argues by inevitability-of-disruption, an inevitability arc will feel native to those investors. If its defining essays argue by bitter-lesson-style scaling logic, a compute-and-data arc will land. Match the argument's *form* to what the room already finds credible.
- **Position within the discourse.** Know what thesis these investors currently carry, and either ride it or argue with it explicitly. A pitch that seems unaware of its category's live debate reads as unread.

Any pitch that quotes the canon or borrows its vocabulary fails the first-principles filter. The canon shapes the skeleton; the founder's own material is every visible word.

## 4. Choose the Narrative Structure

Fit the structure to the graph, not the other way around:

- **Inevitability arc** (world-motion led) — when the spin nodes are the strongest cluster. Structure: was → becoming → with-us. Best default for market-led pitches.
- **Discovery arc** (research-led) — when the graph centers on the founder noticing a shift early. Structure: the anomaly noticed → what it implied → what we built to test it → what the evals showed → what it means at scale.
- **Craft arc** (technical-led) — when Decision nodes with heavy cost edges dominate. Structure: the default everyone accepts → our refusal → the price we paid → the measured property it bought → why that compounds.
- **Origin arc** (character-led) — when the founder-story material (Ch 09 Why Us) is unusually strong (rare; use only when the founder's history is itself the moat). Structure: the years that forced the seeing → the thing seen → the company as its inevitable expression.

Whichever structure is chosen, the taste ledger material gets distributed through it, never ghettoized into a "culture chapter."

## 4b. Story Modes Within Chapters

The arc is the macro-structure; each chapter then runs in a **mode** — a distinct dramatic intent, adapted for pitches from Kendall Haven's story-type research. Choose the mode per chapter, tell the founder which mode each chapter is running, and honor each mode's caution:

- **Framing** → *The Shift.* Set the frame and leave a question hanging that the rest of the pitch exists to answer. The arguable opinion is the frame.
- **Struggle** → *Why Us.* Focus on the struggle and the motive, never the triumph. The nobility is in the fight, not the founder. *Caution: a struggle that reads as self-serving reverses the message.*
- **Put-a-Face-on-It** → *Opposing Forces.* One representative person suffering the default, concrete enough to stand for the whole population. *Caution: one attackable detail discounts the entire argument — every detail must be real.*
- **Wow!** → *The Bets and the technical material.* Reveal the complexity, precision, and care insiders take for granted: the rejected architecture, the eval built from two years of tickets. Depth as drama. *Caution: the audience must be genuinely impressed; never overstate.*
- **Values-in-Action** → *The Moat and The Ask & the Standard.* A core value shown under pressure — the refusal that costs deals every month, the promise with teeth. The value must be decisive in the outcome, never decorative.
- **I-Am-You** → *The Pull.* The customers' own words proving "we know your issues because we live them." *Caution: never claim a mutuality the quotes don't establish; overstating alienates.*
- **Future Vision** → *the spin's third world-state and the closing horizon.* A concrete, vivid scene from the world if the company is right — what exists, what's gone, what nobody tolerates anymore (ledger #12). *Caution: one logically false detail lets the room discount the whole vision. Keep it modest and specific.*

Two standing rules across all modes: the founder is never the hero — the customer is, and the founder is the guide; and no chapter mixes modes — one dramatic intent per chapter, or the chapter blurs.

## 5. Cut Into Chapters

Chapters, not slides. Each chapter is one node-cluster from the graph, and carries exactly: a title in plain words, one point, one proof (fingerprint, eval, or voice), and a handoff line that makes the next chapter necessary. Eight to twelve chapters. If a chapter has a point but no proof, it returns to the gap list. If it has proof but doesn't advance the retell, it moves to the technical appendix.

Five chapters carry a presentation pattern from `presentation.md` — the pattern is how that chapter's proof gets shown:

| Chapter | Pattern | Ledger material it draws on |
| --- | --- | --- |
| 05 The Product | The Annotated Run | How It Feels, Workaround We Refused |
| 06 The Pull | Proof of Pull | (Voices nodes: exact customer words) |
| 07 The Moat | The Map of Defaults | Feature We Killed, Workaround We Refused, Our Promise |
| 08 The Growth Engine | Distribution Beliefs | The Opinion applied to distribution, GTM refusals |
| 09 Why Us | Fingerprint Bios | Hire We Passed On, People We Keep Close |

If a chapter's pattern has no material behind it, the chapter gets a Context Request, not filler.

The test of a good cut: read only the chapter titles aloud. They should tell the entire story on their own — the same property as a well-built essay's headings.

**The through-line test — coherence, not chapter quality.** A pitch can have ten strong chapters and still be incoherent, because coherence lives in the *sequence*, not the parts. Read the chapter titles in order and check one thing: do they state a single argument that advances, each title a consequence of the one before, all defending the retell? Generic titles that name topics rather than moves — "The Problem," "Our Solution," "The Market," "The Team" — are the symptom: they read as a table of contents, and a table of contents is a report, not a story. If the titles do not chain, the cut is wrong; find the one claim the whole pitch defends and re-cut so every chapter moves it one step forward.

This failure is most common — and most damaging — for **infrastructure and dev-tooling pitches**, where the product is a capability rather than a person's transformation and the draft drifts into narrating architecture. The fix is to anchor the through-line in one developer's changed workday; the presentation patterns for this are in `presentation.md` ("Technical and dev-tooling products").

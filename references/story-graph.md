# The Story Graph

The mechanism underneath the pitch. Everything gathered in Phases 0–2 becomes a graph; the graph gets a spin and a structure; the structure gets cut into chapters. Build it explicitly — write it out for the founder to see — because the graph, not the deck, is the company's real narrative asset. It will be re-cut for every future audience: seed deck, hire pitch, launch post, Series A.

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

Rules: every Belief node must connect via *proves* to a Fact, Decision, or Voice — an unconnected belief is a claim, and claims get cut or flagged. Every Decision should carry a *cost* edge. The densest well-connected cluster in the graph is the pitch's natural center of gravity; note where it is before choosing a lead.

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

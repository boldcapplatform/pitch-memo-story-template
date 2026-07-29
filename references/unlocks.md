# The Three Unlocks

Every serious AI-era company rests on three unlocks. The pitch must articulate all three — without ever using the word "unlock," which is investor jargon and reads as borrowed language. The founder's job is to make each unlock felt through plain description; this file is how to excavate them and decide which one leads.

## 1. The Research Unlock

What became *knowable* recently that wasn't before. A capability crossing a threshold: a model class that now reasons over long context, a technique out of a paper that now works at production scale, an emergent behavior the labs shipped without fully pricing in.

Excavation questions:
- What result, paper, or capability shift does this company quietly depend on? When did it happen?
- What did you personally notice about that shift before it was consensus? What did you build to test it?
- What would break in your product if that capability regressed? (If nothing breaks, there is no research unlock — say so.)

Articulation pattern: *"Two years ago, models could not X. Since [shift], they can — but only if you Y. Almost nobody has noticed the second half."* The second half is the company.

## 2. The Technical Unlock

What became *buildable* by this team specifically: the architecture, the data loop, the systems insight that converts the research shift into a working product others can't easily replicate.

Excavation questions:
- What was the hardest architectural decision, and what did you give up by making it?
- Which reference architectures did you adopt, and which did you reject after trying? Why?
- What do you measure that competitors don't? Which benchmarks do you run, which evals did you build yourselves, and what's the honest current number?
- Where does the cheap workaround live in your space, and why did you refuse it?

Articulation pattern: *"Everyone builds this as A. We built it as B, which cost us [price] and bought us [property]. Here is the eval that proves the property holds."* An architecture without a measurement is an opinion; with one, it is an unlock.

## 3. The Market Unlock

What became *wantable and reachable*: whose behavior or budget shifted so that a tribe now exists for this, and can be reached without renting someone else's channel. This is the future-narrative — told as the world's motion, never as TAM.

Excavation questions:
- Who changed their behavior in the last 18 months in a way that makes this company make sense? What do they do now that they didn't before?
- Who found you without being sold, and what were their exact words?
- What budget line does this come from — one that exists, one being created, or one being reallocated from humans to systems?

Articulation pattern: *"[Tribe] already does X the hard way, and started doing it recently. We are what X looks like when someone builds for it on purpose."*

## Choosing Which Unlock Leads

All three appear in every pitch; one carries the opening. Choose by where the company's real edge and evidence are strongest:

- **Research-led** — when the founder's edge is having noticed the capability shift early and having proof (experiments, evals) others lack. Leads with the shift; the room feels they're being let in on something. Requires genuine depth — this lead collapses fastest under a technical partner's probing if hollow.
- **Technical-led** — when the edge is the architecture and its measured properties. Leads with the contrarian build decision and its eval. The strongest lead for infra, dev tools, and anything sold to engineers.
- **Market-led** — when the edge is the tribe: unusual pull, vivid customer language, a budget shift the founder can prove. Leads with the world's motion and the people already living in the future. The right lead when research and technical depth are real but not differentiating.

If no unlock is strong enough to lead, tell the founder plainly. A pitch with three weak unlocks is a gap list, not a story yet.

## Where the Unlocks Land in the Chapters

The unlocks are not a chapter; they are distributed. The research and market unlocks live in the spin's world-state nodes and surface in **The Shift** and **Why Now**. The technical unlock surfaces in **The Bets** and the Technical Appendix, and its evals sit beside the demo in **The Product** (the Annotated Run pattern). The leading unlock must be unmistakable within the first two chapters — without the word "unlock."

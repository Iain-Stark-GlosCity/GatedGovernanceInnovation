# The Innovation Pipeline

## Explore, Reflect, Scope, Architect, Build, Review, Production, Observe

**Owner:** Iain Stark, Head of Transformation and Commissioning, Gloucester City Council
**Status:** Working draft — doctrine and operating model. A formal policy conversion (control table, decision rights, records and retention) is a separate, shorter document.
**Date:** 10 June 2026

-----

## The problem this solves

Two failures sit on either side of every council’s innovation work.

The first is under-governance: untested systems carrying statutory services, unknown code touching personal data, harm with named victims. Inquiries get written about this failure. Horizon is the standing example of what it costs.

The second is over-governance: production-grade scrutiny applied to a prototype, so the prototype never gets built and the knowledge it would have produced never exists. No inquiry is ever written about this failure. The harm is invisible because the missing thing was never seen.

Most organisations defend against the first failure by committing the second. The standard objection to AI-assisted development, “you don’t know the codebase, terrible things could happen”, is legitimate scrutiny aimed at the wrong target. It applies to production. It is corrosive when applied to exploration.

This pipeline separates the two so each gets the governance it actually needs. One process. Governance that scales with risk, both ways.

## The shape

Eight stages. A hard line between stage two and stage three.

```
EXPLORE → REFLECT ║ SCOPE → ARCHITECT → BUILD → REVIEW → PRODUCTION → OBSERVE
                  ║                                                      │
   the 90%        ║                  the 10%                             │
   scout's rules  ║                  settler's rules                     │
        ▲         ║                                                      │
        └─────────────────────────────────────────────────────────────--┘
```

Left of the line: cheap, fast, disposable, lightly governed. Right of the line: specified, assured, owned, recorded. Observe feeds the next explore. The pipeline is a loop, not a line, because innovation does not happen once.

Roughly 90% of innovation work happens left of the line. Delivery is the visible 10%. Any accounting that only counts delivery will conclude that the left side produces nothing. It produces the map that makes the right side fast.

|Stage     |Main question                       |Main output                 |
|----------|------------------------------------|----------------------------|
|Explore   |What is possible?                   |Findings and prototypes     |
|Reflect   |What did we learn?                  |Reusable knowledge          |
|Scope     |What are we actually delivering?    |Scope and gate record       |
|Architect |How will obligations be designed in?|Reviewable design           |
|Build     |Can we construct the designed thing?|Tested build                |
|Review    |Should this go live?                |Assurance decision          |
|Production|Can it operate responsibly?         |Live service                |
|Observe   |Did assurance hold?                 |Evidence and next candidates|

-----

## Stage 1: Explore

Walk paths that have not been walked. Find what tools do beyond their documentation, what combinations nobody has tried, where the real limits sit.

**Entry:** a lightweight exploration mandate, not a business case. Named lead, learning aim, cost cap, timebox, a first pass of the governance gates answered against the idea as conceived, and confirmation that the prohibitions below hold. The gate pass takes minutes, not meetings: each gate answered yes or no with a one-line rationale. Exploration that must justify its direction in advance is not exploration; exploration with no record of existing is not defensible.

The first gate pass does two jobs. It records the entry in the register with its risk profile visible from day one. And it acts as a design input: if the answers come back heavy before any work has started, that is the gates telling you the idea is framed heavier than it needs to be yet. See “Rescoping” below.

**Rules:**

- Off the production estate by default. Any proposed read-only, non-sensitive connection to a production system is not ordinary exploration and requires a recorded exception before work continues.
- Cost, time, data exposure and system exposure are capped. The learning question stays open.
- Infrastructure is disposable by default.

**Hard prohibitions before the line — Explore and Reflect:**

- No live personal data. No special category data. Pseudonymised personal data is still personal data.
- Test data is synthetic, genuinely anonymised, publicly available, or otherwise approved for exploration use. Pseudonymised personal data is not anonymised data.
- No production credentials.
- Staff, reviewers or invited testers may interact with prototypes where they understand they are testing a non-live artefact. No member of the public or service user may rely on the output as a service, decision, entitlement, instruction or advice.
- No public-facing service. No statutory decision-making. No automated action affecting a person.

These are absolute because their harm can occur before production. Everything else waits for the line.

**Containment:** if an exploration is found breaching a prohibition, it stops immediately and escalates to the named lead and the relevant control owner. This rule is what makes the left side safe to leave lightly governed.

**Output:** raw findings. Prototypes, dead ends, surprises.

**Failure mode:** there are two. Leaking into production, and never stopping.

## Stage 2: Reflect

Convert findings into assets. The prototype is scaffolding. The reflection is the deliverable.

Questions this stage answers in writing:

- What did this teach about architecture?
- What questions would I now ask a vendor in this category?
- Where are the cliffs?
- Honestly: would this hold weight?
- What would have to be true before this could safely carry weight?

The last question is the bridge. If the answer is ever needed at scope, it was written here first.

**Output:** notes, principles, question lists, mapped dead ends. Written down, not held in someone’s head.

**Exit:** one of three verdicts.

1. *Interesting, not now.* The most common verdict. File it.
1. *Wrong path.* Also a success. A mapped cliff stops the next person falling off it.
1. *This could carry a service.* Proceed to scope.

**Failure mode:** skipping this stage. Unreflected exploration produces anecdotes and a reputation for playing with toys. The reflection is what makes the 90% defensible.

-----

## The line

Crossing from reflect to scope is a decision. A named person makes it. It gets recorded. Nothing drifts across.

At the line, the governance gates are re-run against the production context, not the experiment. Audience, data and reliance all change at this boundary: a prototype that processed nothing personal may become a service that does; a tool only the builder relied on may become one residents rely on. The entry-pass answers are the starting point. Each is confirmed or revised against the service this would become. Promotion is a decision, not a drift.

The gates:

1. **Safeguarding, welfare and material harm**
1. **Statutory function and legal duty**
1. **Personal data, privacy and information rights** — sub-question: is DPIA screening required, and does screening require a full DPIA?
1. **Equality, accessibility and fairness** — sub-questions: EqIA; transparency recording, including ATRS where applicable, where algorithmic or AI-assisted decision support is involved
1. **Scale, users and public impact** — sub-question: transparency and public explanation
1. **Information security, cyber and supply chain** — sub-questions: security classification; dependency and supplier exposure; procurement route
1. **Operational criticality and live-service burden** — sub-question: what support, ownership and rollback will live operation demand?

Decision automation and AI influence is not a gate of its own. It is a named sub-question under gates 2, 3, 4, 5 and 7, because automation amplifies those risks rather than constituting a separate one.

**The gate design principle:** a gate earns its place only if a “no” is cheap to give and a “yes” changes behaviour downstream — the architecture, the review route, or the operating burden. Gates that everything answers “yes” to are decoration. Any future gate proposal is tested against this before it is added.

Every “yes” carries forward as an obligation through every remaining stage, discharged at named points: designed in at architect, evidenced at review, monitored at observe. A static careers site and a social care system enter the same pipeline. They leave scope with completely different loads.

**The proportionality duty — governance scales both ways:**

- Gate decisions are made within a defined period, scaled by risk. Low-risk work is not left in governance limbo.
- A control may only be required where it addresses a recorded gate answer. No control owner adds production-grade requirements to explore or reflect activity without recording which gate answer justifies it.
- Where assurance demands exceed the recorded gate profile, the project owner has a named escalation route.
- Where the high-risk gates all answer “no”, the project proceeds through a lightweight route by default.
- Periodic review of this framework examines both failure modes: incidents and near misses (under-governance), and explorations delayed, abandoned or never attempted because of process burden (over-governance). The second is recorded in the exploration mandate register, because invisible harm only becomes governable when it is counted.

-----

## Rescoping: generic first, specific later

The gates are a design input, not only a permission mechanism. Sometimes the entry pass on an idea comes back heavy before any work has started — a service concept that trips personal data, statute and information quality at once, where even the sandbox would carry significant governance. The wrong responses are to push through anyway or to drop the idea. The right response is to step back and rescope.

**The move:** park the idea as conceived, with its gate record intact, and open a generic version that learns the underlying technology and principles without the risk surface. A resident-facing benefits assistant becomes a generic governed-knowledge engine: no domain data, no personal data, synthetic content, nobody relying on it. The generic version’s gates come back clean. Sandbox, basic controls, go.

**The climb:** capability returns toward the specific in gated steps, each one a deliberate re-gate. Generic engine first. Then real but public domain content, which wakes the information quality gate: provenance, currency, a correction route. Then real users relying on it, which wakes personal data and scale. Then the statutory context. Each yes arrives one at a time with its obligations met as it arrives, instead of all of them landing on day one and crushing the idea before it can teach anything.

**Three rules keep this honest:**

1. *The descope is named.* The generic version’s record states explicitly what it will not do. “Generic knowledge engine” means nothing; “will not touch live personal data, will not serve residents, will not encode statutory decisions” is a descope.
1. *Scope watch.* The gates the parked original tripped are recorded as watched risks on the generic entry. A generic name does not descope the risk — a “generic resident query tool” that quietly processes personal data is gate 3 wearing a hat. The moment a watched capability appears, it is recorded as a yes and its obligations attach. The watch makes climbing cheap to do honestly and impossible to do silently.
1. *The original waits with its record.* The parked entry resumes when the generic groundwork has produced the map, re-entering with its gate answers standing. Rescoping defers the obligations; it never deletes them.

This is not gaming the gates. It is the same pattern as the architecture: the layering of the system is the layering of the risk. The LLM library is the standing example — the generic engine trips almost nothing, the domain content is where information quality starts to matter, and a resident-facing deployment is where everything else would. The governance gradient and the build gradient are the same shape, by design.

-----

## Stage 3: Scope

Define the delivery. For whom, under what statute, with what data, at what scale. Run the gates. Record the answers.

**Output:** a scope document with gate answers attached, a named owner, and an explicit statement of what the exploration taught that this delivery relies on.

**Failure mode:** scoping the prototype instead of the service. The prototype gets thrown away here. The route knowledge is what crosses.

## Stage 4: Architect

Design the production version using the map from reflect. Where the deterministic rules live. Where provenance attaches. What the contracts are at each boundary. What the model touches and what it is forbidden from touching.

Gate obligations from scope become architectural features here, not compliance paperwork bolted on later.

**Output:** a design reviewable by people who were not on the expedition. If the architecture only makes sense to the scout, it is not finished.

**Failure mode:** smuggling exploration into this stage. New ideas discovered during architect go back to explore. They do not ride into build.

## Stage 5: Build

Construct the designed thing. Boring on purpose.

This is where AI-assisted development is fastest and safest, because it is the second walk down a route already taken in the rough. The model fills in specified structure. It does not decide anything undocumented. Decisions live in the architecture. Dependencies live in the manifest: named, versioned, justified, owned.

AI assistance is strongest here on the meticulousness nobody previously funded: dependency manifests, boundary tests, documentation kept synchronised with the code as it changes. The assurance artifacts that were always supposed to exist become cheap to maintain.

**Rules:** provenance on the work, tests at the contracts, nothing load-bearing that is not inspectable.

**Build frameworks:** structured AI development methods exist for this stretch — typically role-based phases, each producing documents that constrain the next. Any of them can run scope through build under two conditions: the reflect output and gate obligations enter the method as inputs, and the method’s internal QA is not mistaken for stage six review. Internal QA is the build checking itself; review is the institution checking the build. The pipeline depends on no particular method, deliberately. Methods will churn; the road network should not.

**Failure mode:** velocity worship. Build speed is a consequence of good scouting, not a goal. Chasing it directly recreates vibe coding with extra steps.

## Stage 6: Review

Independent verification by someone who did not build it. Does the build meet the architecture? Does the architecture meet the scope? Were the gate obligations discharged?

**Independence has a floor:** the reviewer is not the build lead and is competent in the relevant risk class. Higher gate loads mean panel review, and specific gate answers name their reviewers: a personal data “yes” brings the DPO, a security “yes” brings cyber, a safeguarding “yes” brings the safeguarding lead. Without this, “independent” decays into a colleague in another team having a look.

**Three exits:** proceed, back to architect, kill.

A review that cannot kill is theatre, and everyone downstream knows it within a month.

**Output:** a recorded decision with reasons. This is the artefact that answers “who assured this” in any future inquiry.

**Failure mode:** rubber-stamping because the demo was magnificent. The demo is evidence. It is not assurance.

## Stage 7: Production

The service runs. Smallest possible footprint: only what passed review, only the components the scope required. The exploration estate stays outside.

**Rules:** named owner, support route, rollback path, accountability chain fully legible.

Production is a privilege the artefact earned at review, not a destination the project was entitled to.

**Failure mode:** scope creep in place. Quietly bolting unreviewed capability onto a reviewed service. New capability re-enters at scope.

## Stage 8: Observe

Two jobs.

First, verify the assurance held. Does live behaviour match what review approved? Did the gate obligations survive contact with reality?

Second, harvest. What does real usage reveal that no prototype could? What is the next impossible-at-human-cost task now visible? What failed in an interesting way?

**Re-gating:** the gates get re-run on material change. Triggers: new data type or new personal data use; new user group or increased scale; new integration, supplier or model; new statutory use or automated decision support; material architecture change; significant incident or near miss; any move from internal to public-facing use. New capability never accretes onto a reviewed service silently; it re-enters at scope.

**Output:** evidence for the governance record, and candidates for the next explore.

**Failure mode:** treating production as finished.

-----

## Worked examples

Two GCC projects and one high-gravity public service example. Same pipeline, different gravity.

### careers.gloucester.gov.uk — sprinted the loop

A schema-driven static site. At scope, nearly every gate answered “no”: no personal data, no user input, no statutory function, no authentication. Residual risk sat in the deployment pipeline and DNS, both secured. The worst case is a defaced or misleading careers page, reputational damage, or a compromised deployment route — serious, but not comparable to a statutory decisioning system touching vulnerable people or personal data. It went round the whole loop quickly because the gates said it could.

### The LLM library (council-tax-rebuild) — parked at reflect, deliberately

A three-layer governed knowledge architecture: deterministic rules, curated sourced pages, an RDF reasoning map. It will never enter production as built. That was never the product. The product is the map: rules must be deterministic and live in their own layer; sources are gated at ingestion, not filtered at retrieval; reasoning must be inspectable, not buried in embeddings. Plus the vendor question list that no glossy pitch deck can survive. The prototype is disposable. The knowledge is not.

### Adult social care gravity — would crawl, and should

Adult social care sits with the county, not the district, so this is a thought experiment in weight rather than a GCC project. A service of that gravity entering this pipeline answers “yes” at every gate and carries every obligation heavily. Same eight stages. The gravity is different because the risk is different. That is the pipeline working, not the pipeline failing.

-----

## What this answers

**“You don’t know the codebase.”** Left of the line, knowing the codebase is not the point; the codebase is disposable. Right of the line, every dependency is documented, every decision is recorded in the architecture, and review is independent. The question “where exactly could the terrible thing happen” gets a system-by-system answer.

**“AI code in production?”** Yes, in build, under the rules above. The model writes code. It does not make undocumented decisions. Human-written code has shipped vulnerable to production for decades behind QA that caught neither. The variable that predicts outcomes is the assurance process, not the author.

**“Why fund the 90%?”** Because the 10% is only fast and safe when it is a second walk. The exploration that looks like nothing on a quarterly report is what makes delivery look like magic. Success erases its own preconditions, so the scouting gets narrated as it happens. This document is part of that record.

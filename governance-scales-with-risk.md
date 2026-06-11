# Governance scales with risk

A proportionate model for deciding what governance a service needs — and giving everything else room to move.

**Owner:** Iain Stark, Head of Transformation and Commissioning, Gloucester City Council
**Status:** Working draft v3 — companion to The Innovation Pipeline (doctrine). The gates here are the gates that pipeline runs.
**Date:** 11 June 2026

-----

## The problem runs in both directions

Under-governance in high-risk services causes harm. The failure is visible: an incident, an inquiry, a report. It has a name and a date.

Over-governance in low-risk services causes harm too. The failure is usually invisible: the pilot that never happened, the idea that died in committee, the service that did not move while everything around it did. Nobody is accountable for it. It does not trigger an inquiry.

That asymmetry is why over-governance rarely gets challenged. Under-governance produces accountability; over-governance produces learned helplessness.

## The principle

Proportionality. A considered decision, per service, about which obligations apply — and a governance approach that matches them.

This is not removing governance. It is locating it.

## The gate model

Each gate asks one question, answered yes or no, recorded with a one-line rationale. A no means that layer does not apply. A yes means that layer applies for the life of the service: record the obligations it carries and meet them before that aspect of the service goes live.

|Gate                                   |Owner                     |Question                                                                      |A yes means                                                                                                                                                                                                                                                                  |
|---------------------------------------|--------------------------|------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|1 — Safeguarding and serious harm      |Safeguarding lead         |Could this cause serious harm to a person if it goes wrong?                   |Senior ownership, separate sign-off, and a materially higher bar throughout. Nothing else in this model dilutes that.                                                                                                                                                        |
|2 — Statutory function or formal policy|Legal / monitoring officer|Does this exercise a statutory function or implement formal council policy?   |Identify the specific provisions that bind the service and design within them. No discretion where statute does not permit it. A yes here is common and is not, by itself, heavyweight — it defines the constraint envelope, not the process burden.                         |
|3 — Personal or confidential data      |DPO                       |Does this process personal, special category, or otherwise confidential data? |Lawful basis, DPIA where required, data sharing agreements, access controls, and retention schedules — in place before any live data is touched. This includes data passed to third-party tools and AI services during development, not just data in the finished product.   |
|4 — Scale and material impact          |Service owner / SMT       |Does this reach many residents, or affect something material to how they live?|Scrutiny and sign-off at a level proportionate to reach — above the project team, not just within it.                                                                                                                                                                        |
|5 — Information quality                |Information governance    |Will people rely on information this service produces or reuses?              |Evidence of provenance, currency, and permission to reuse, plus a defined route for correcting errors. For AI-assisted or retrieval-based services this gate is load-bearing: outputs can look authoritative regardless of whether the source material is current or correct.|
|6 — Production                         |Independent reviewer      |Have all obligations accumulated through gates 1–5 been met?                  |No yeses: sandbox with basic controls. Yeses with unmet obligations: sandbox only. All obligations met: eligible for promotion to production.                                                                                                                                |

Each gate has a named owner. A disputed answer escalates the disputed gate — not the whole service — to that owner.

## When the gates run

The gates run twice in an entry’s life, and again on change.

**At entry.** Every entry into the register starts with a gate pass against the idea as conceived: six questions, six answers, one line of rationale each, a named owner, a review date. Minutes, not meetings. This records the risk profile from day one and determines the sandbox terms.

**At promotion.** A sandbox success does not slide into production; it is promoted through a deliberate step. Promotion means re-running the gates against the production context rather than the experiment — audience, data, and reliance all change at that boundary — and deciding whether the prototype becomes the product or serves as the specification for building it properly.

**On material change.** New data type, new user group, new integration, new supplier or model, new statutory use, a significant incident, or any move from internal to public-facing use. A service that gains a yes it did not previously carry must meet the new obligations before continuing in that form.

## The gates are a design input, not only a permission mechanism

Sometimes the entry pass comes back heavy before any work has started: a concept that trips personal data, statute and information quality at once, where even the sandbox would carry significant governance. The wrong responses are to push through anyway or to drop the idea. The right response is to rescope.

**Rescoping: generic first, specific later.** Park the idea as conceived, with its gate record intact, and open a generic version that learns the underlying technology and principles without the risk surface. A resident-facing benefits assistant becomes a generic governed-knowledge engine: no domain data, no personal data, synthetic content, nobody relying on it. The generic version’s gates come back clean. Sandbox, basic controls, go. Capability then climbs back toward the specific in gated steps — each new yes a deliberate re-gate, its obligations met as it arrives, instead of all of them landing on day one.

Three rules keep rescoping honest:

1. **The descope is named.** The generic version’s record states explicitly what it will not do. A descope without a “will not” statement is a rename, not a rescope.
1. **Scope watch.** The gates the parked original tripped are recorded as watched risks on the generic entry. A generic name does not descope the risk — a “generic resident query tool” that quietly processes personal data is gate 3 wearing a hat. The moment a watched capability appears, it is recorded as a yes and its obligations attach.
1. **The original waits with its record.** The parked entry resumes when the generic groundwork is done, re-entering with its gate answers standing. Rescoping defers obligations; it never deletes them.

## Baseline controls apply everywhere

The gates locate additional obligations. They do not switch off the basics. Every service, gated or not, sits on the organisation’s standard security posture: managed access, maintained dependencies, no exposed endpoints, no secrets in code. A service that trips no gates has no extra governance — it does not have no governance.

## Rules that keep the model honest

**Obligations inherit across boundaries.** A service that carries no yeses, but feeds into or integrates with one that does, takes on the relevant obligations at the point of integration. You cannot launder risk through a clean front end.

**Every assessment has a named owner.** The owner is accountable for revisiting the gates when the service changes — scope, audience, data use, operational context, or level of influence. Without a named owner, reassessment triggers belong to nobody and fire never.

**Every assessment lives in one register.** Per-service precision without portfolio visibility is just distributed paperwork. The register is the single view of what exists, what state it is in, and what obligations are outstanding — and it is the answer, on demand, to the question “what is the council building and on what basis?”

**Governance scales down as well as up.** Three controls protect the low-risk side:

- Gate decisions are timebound, scaled by risk. Low-risk work is not left in governance limbo.
- A control may only be required where it addresses a recorded gate answer. No control owner adds production-grade requirements to sandbox work without recording which gate answer justifies it.
- Where assurance demands exceed the recorded gate profile, the owner has a named escalation route.

Periodic review examines both failure modes: incidents and near misses, and explorations delayed, abandoned or never attempted because of process burden. Closure reasons are recorded in the register, because invisible harm only becomes governable when it is counted.

## Sandbox is not ungoverned

No yeses across gates 1–5 means sandbox with basic controls: no live personal data, no external publication, no implied formal advice, no operational decisions made on its outputs. Within those constraints, build and experiment without seeking permission you do not need. That is the point of the model — the default for ungated work is go, not wait.

Sandboxes expire. Every sandbox entry in the register carries a review date — set by its timebox, six months by default. At review the owner decides: promote, continue with a new date, or retire. Retired means switched off and access closed, not abandoned. Experiments that nobody owns and nobody remembers are a risk surface, not an asset.

## Promotion is a decision, not a drift

Promotion re-runs the gates against the production context (see “When the gates run”). Production also carries a continuity obligation: documentation sufficient for someone other than the builder to operate, maintain, and retire the service. If a service only works while one person remembers how, it is not ready for production, however well it runs.

## Running an assessment

The assessment should take minutes, not meetings: six questions, six answers, one line of rationale each, a named owner, a review date, an entry in the register. One page. If the answers are contested, escalate the disputed gate — not the whole service — to its named owner. The record is the audit trail: what was assessed, what obligations were identified, what changed, and when the classification was confirmed or revised.

That is not lighter governance. It is more precise governance.

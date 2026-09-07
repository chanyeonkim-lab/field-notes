# Enterprise AI doesn't fail one review. It fails four.

*Field note on the multi-executive gate that quietly decides most enterprise AI investments — and how a systematic methodology answers every seat at the table.*

---

## The moment AI investments actually die

Enterprise AI vendor pitches usually optimize for one executive. Sometimes it's the CFO — a big ROI number, dollar savings, months to payback. Sometimes it's the CIO — architecture diagram, security posture, integration story. Sometimes it's the CMO — customer experience uplift, brand differentiation.

The pitch lands with that one executive. The deal moves.

Then it hits the review gate. And the review gate — in every large enterprise I've worked with — is not one person. It's a committee of four or five, and each of them is reading a different column of the same business case:

- The **CFO** wants payback, downside scenario, and whether the number holds under attribution discounts.
- The **CIO** wants investment breakdown, operational burden, and whether the platform's total cost is being disclosed honestly.
- The **CRM / service leader** wants adoption rate, business-user impact, and evidence that peer companies actually got there.
- The **CMO** wants customer experience uplift and whether the retention story is defensible.
- The **HR / operations leader** wants headcount, onboarding time, and hours saved per employee.

A business case tuned to one column dies in another. That's the actual reason so many pilots don't clear production approval — not because the technology failed, but because the case only spoke to one seat at the table.

## What the case actually has to contain

Across ten-plus enterprise engagements running AI ROI simulations and business value cases, I've stopped trying to produce a single headline number. Instead, every case has to answer *categorically different* value types — because each executive at the review gate is looking for a different one:

- **Cost savings** — direct labor time reduction, automation-eligible volume, per-case processing cost. The CFO reads this hardest.
- **Revenue creation / protection** — retention driven by faster response, wallet share preserved, lead conversion uplifted. Paired with an explicit attribution boundary (which revenue stream is actually being touched, and which is excluded on purpose). Read by the CMO and the CRM leader.
- **Customer satisfaction** — response quality, first-contact resolution rate, self-service success. Measured, not asserted. Read by CMO and service leader.
- **Employee productivity** — handling time, after-call work, knowledge search speed. Compared to a live operational baseline, not an industry average. Read by the operations leader.
- **Working hours saved** — onboarding acceleration, ramp time, cognitive load reduction. Framed in FTE-equivalent terms. Read by HR and by any leader owning a large operational team.

Every one of those categories can be inflated. Every one of them will be inspected by the executive whose column it lives in. Which is why *the same guardrails* have to apply across all of them — or the whole case unravels when one thread gets pulled.

## The methodology I actually run

I run an internal Slackbot skill that produces Business Value Cases for enterprise AI deals — the document that goes into the multi-executive review. Every number it emits has to pass the same non-negotiable guardrails, applied uniformly regardless of which value type it belongs to:

- **Min/Max verification per driver.** Each calculated benefit is compared to a benchmark range. Falls outside → flagged with reason, not silently dropped.
- **Source hierarchy on every input.** Structured CRM data first, then internal discussions and notes, then peer benchmarks (median of 3+ same-industry cases, never a single anchor, individual customer names never exposed), then template defaults. Still unsourced → marked "requires customer input," never guessed.
- **Attribution factors to prevent double-counting.** When multiple AI capabilities touch the same operational minute, an attribution discount is applied to the overlapping driver before summing.
- **Ramp discipline.** Year 1 benefit conservatively de-rated (roughly 50–60%) for adoption ramp. Investment ramping applies only to consumption components, not to fixed licensing.
- **Strict revalidation order when payback is off.** Validate assumptions first, then value drivers, then investment. Never inflate benefits to hit a target.
- **High-ROI flag.** Anything above 300% ROI requires a conservative counterpart. Above 40% assumption-based inputs → stamped "directional only — not decision grade."
- **Downside/base/upside on every driver that has one.** Because the CFO always asks, and the CRM leader wants to know whether the base case survives slower adoption.

The point isn't that the skill is automated. Automation is easy. The point is that every value type — cost, revenue, CX, productivity, hours — gets treated with the same discipline, so no single reviewer can pull a thread and unravel the document.

## What this looks like on a real deal

On the AI call-center evaluation for a global enterprise's regional operation — the kind of engagement where the buying decision sat with a multi-executive steering committee, not with the operational team excited by the demo — the output was five value drivers, each written for a specific reader:

- Handling-time reduction — for the **operations leader**
- Case automation — for the **CFO's cost column**
- Onboarding acceleration — for the **HR leader**
- Customer retention through faster response — for the **CMO / service leader**
- First-contact resolution improvement — for the **customer service leader**

Every driver had an explicit formula, a stated assumption, an attribution boundary, downside/base/upside, and a live-data baseline. The four conservative adjustments were applied *before* presenting anything, not after pushback: attribution capped on the largest driver, revenue-protection restricted to a single defensible retention mechanism, Year 1 explicitly ramped down, automated-case volume removed from the human-processing base so the same minutes weren't counted twice.

Even the *downside* scenario cleared the finance column's acceptable payback window. The CIO could point at the investment breakdown line item. The CRM leader saw the peer benchmark citations. The CMO had a defensible retention number. Nobody had to trust a single vendor slide.

## Why I keep working on this

The single most consistent reason large-enterprise AI initiatives stall isn't that the model doesn't work. It's that the business case only speaks to one executive, and the deal has to clear four.

Vendors keep trying to solve that by making the number bigger. That's the wrong lever. The right lever is producing a case that every reviewer can walk through end-to-end, find their column, see the assumptions, and either accept them or challenge them on their own terms. Cost savings for the CFO. Adoption reality for the CRM leader. Experience uplift for the CMO. Hours saved for the operations leader. All in the same document, all held to the same standard of evidence.

That's what turns *"AI works"* into *"AI is funded in production."*

# The AI ROI number that survives a CFO

*Field note on why enterprise AI decisions stall at the finance-team review — and how a systematic, guardrailed methodology gets them unstuck.*

---

## The pattern I kept running into

Enterprise AI pilots almost always produce a headline number. "We'll save X million a year." "Payback in six months." "Ten-times ROI."

Almost none of those numbers survive contact with the customer's finance team.

Not because the technology doesn't work — it usually does. Not because the numbers are made up in bad faith. But because they're built the way vendor slideware has always been built: a single optimistic input, a linear extrapolation, no auditable source, no sensitivity, no explicit assumption ledger. A CFO sees that and correctly refuses to sign.

The deal doesn't die at the demo. It dies at the business case review.

That gap — between *"AI works"* and *"the finance team will fund it in production"* — is where I've spent a lot of my recent time. I've now run AI ROI simulations and business-value cases for more than ten enterprise customers, across industries. The pattern is consistent enough that it deserves writing down.

## What actually changed how I calculate it

I run an internal Slackbot skill that produces Business Value Cases for enterprise AI deals — the same document the customer's CFO eventually reviews. The point isn't that it's automated. Automation is easy. The point is that every number the skill produces has to pass a set of non-negotiable guardrails *before* it lands on the page:

- **Min/Max verification on every driver.** Each value driver's calculated benefit is compared to a benchmark range. If it falls outside, the skill doesn't quietly drop it — it flags the result and documents why. If the formula can't be evaluated at all, that gets flagged too.
- **Explicit source hierarchy on every input.** Structured CRM data first. Then account-channel discussions and internal notes. Then peer benchmarks (median of 3+ same-industry cases — never a single anchor, and individual customer names never exposed). Then template defaults. If a value still can't be sourced, it's marked *"requires customer input"* — never silently filled with a guess.
- **Strict revalidation order when payback is off.** Ideal window is roughly 6–12 months, acceptable 3–18. If a case falls outside, validate assumptions first, then value drivers, then investment. Never inflate benefits first to hit a target.
- **High-ROI flag.** Any case above 300% ROI is marked *"high sensitivity"* and must include a conservative counterpart. Any case where more than 40% of inputs are assumptions gets stamped *"directional only — not decision grade."*
- **Attribution factors to prevent double-counting.** When multiple AI capabilities touch the same operational minute (e.g., handling-time reduction and case automation both saving the same seconds), an attribution discount is applied to the overlapping driver — typically 30–35% off — before anything is summed.
- **Ramp discipline.** Year 1 benefit is conservatively de-rated (roughly 50–60%) to account for adoption ramp. Investment ramping applies only to consumption components, not to fixed licensing.

Those aren't cosmetic. They are the difference between a business case that survives finance-team review and one that comes back with red ink.

## What this looks like on a real deal

Across ten-plus enterprise engagements, one recent one is a good illustration: the AI call-center evaluation for a global enterprise's regional operation — the kind of engagement where the buying decision sits with a finance-and-IT steering committee, not with the operational team excited by the demo.

The output wasn't a single big number. It was five value drivers, each with an explicit formula, a stated assumption, an attribution factor for overlapping benefits, a three-year ramp with Year 1 de-rated, and downside/base/upside scenarios. Even the *downside* case paid back inside the finance team's acceptable window. That's the sentence a CFO actually cares about.

What made the case credible wasn't the size of the ROI number. It was the four conservative adjustments applied *before* presenting anything: attribution capped on the largest driver, revenue-protection benefit restricted to a single defensible retention mechanism (broader repurchase revenue excluded on purpose), Year 1 explicitly ramped down, and the automated-case volume removed from the human-processing base so the same minutes weren't counted twice.

That's what *"systematic"* means in practice. It's not a bigger spreadsheet. It's *fewer* places where a hostile reviewer can plant a flag.

## Why I keep working on this

The single most consistent reason large-enterprise AI initiatives stall is that the business case can't be defended by the customer's own finance team. Vendors keep trying to solve that with bigger numbers. That's the wrong lever.

The lever is trust — built through a methodology the reviewer can walk through end-to-end, see every assumption, and either accept or challenge on its merits. Every number cited. Every gap named, not hidden. Every optimistic input paired with a downside scenario.

Enterprise AI doesn't get funded by the biggest number in the deck. It gets funded by the number a CFO can defend to their board on a Monday morning.

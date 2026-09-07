# ISMS from both sides of the table

*Field note on Korea's government-mandated security certification — and why it quietly decides most enterprise AI adoption here.*

---

## What ISMS actually is (and why foreign vendors underestimate it)

ISMS — and its personal-data sibling ISMS-P — is Korea's government-mandated information-security certification, administered by KISA. If you process personal data at any meaningful scale in Korea, you can't skip it. It isn't a nice-to-have enterprise policy. It's regulatory.

Which means every foreign SaaS or AI vendor that wants to land at a Korean enterprise has to survive the customer's ISMS review, and every Korean enterprise buying that solution has to prove — on paper — that the vendor fits inside their certification boundary.

That review is where most enterprise AI adoption in Korea quietly dies. Not at the demo. Not at the pilot. Not at pricing. At ISMS.

## Two seats

I've sat on both sides of that table.

**Customer side, at adidas Korea.** As Digital Marketing Manager, I owned systems that touched real customer personal data — segmentation, campaigns, the outbound stack. When ISMS certification came around, *I* was the business person KISA's questions landed on. I had to answer, in writing and in interviews, exactly how personal data flowed through the systems I owned, who saw what, and why the controls were sufficient. That is a fundamentally different experience from reading a checklist. You learn what the auditor is actually trying to establish, what evidence looks like from the inside, and where legal and business trade-offs really get made.

**Vendor side, at Salesforce.** As a Solution Engineer, I've supported roughly twenty enterprise customers through their security-review and ISMS-response cycles — drafting the vendor's answers to the customer's questions, translating a global SaaS platform's architecture into terms a Korean security auditor recognizes as a valid answer, and working alongside specialized legal-review and security-consulting firms whose job is to find the gaps before KISA does.

Those two seats sound similar. They aren't. The customer-side person is trying to survive an audit. The vendor-side person is trying to not become the reason a customer fails one. If you've only done one, you're always translating in one direction. If you've done both, the translation mostly collapses — you already know what the other side needs before they ask for it.

## Why this is now an AI problem, not just a compliance one

Every new wave of enterprise technology hits the same wall in Korea, and AI is no exception. LLMs raise the exact same set of ISMS-shaped questions: where does the data physically live, who can access it, what training-data flows exist, how is model output audited, what's the retention policy, what's the opt-out.

Most vendor pitches ignore all of this — until the customer's security team drops a two-hundred-question spreadsheet on them. Then the deal stalls for six months while someone with no ISMS experience tries to answer questions written by someone with twenty years of it. That gap is why *"PoC succeeded, production got shelved"* is such a common Korean enterprise story. The model worked. The governance answers didn't.

## Why I keep working on this

I'm not a lawyer and I'm not a security consultant. But I've done enough of the drafting, sat through enough of the interviews, and worked alongside enough specialized legal and security-review firms that ISMS doesn't scare me. I can usually tell within a first conversation whether a new AI solution has a real path through it, or whether the deal will die at the review stage.

The bottleneck on enterprise AI in Korea is rarely the model. It's the translation between what the technology actually does and what a Korean auditor needs to hear to sign the certification. That translation layer is where I've spent a lot of years — and it's what I want to keep working on.

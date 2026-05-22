# Executive Investment Framework for Security and Infrastructure Programs

Getting investment approved for a security or infrastructure program is a different problem than getting investment approved for a product feature. Features have customers, revenue attribution, and adoption metrics. Security and infrastructure programs have risk reduction, compliance obligations, and technical debt - none of which show up on a revenue line.

This framework covers how to build the case, structure the ask, and present it in a way that gives executives what they need to say yes.

---

## The Core Problem

Executives approve investment based on expected return relative to cost and risk. For product features, that math is often visible: build this, get that many customers, generate this much revenue. For security programs, the math runs differently: invest now, avoid a loss that may or may not happen, satisfy a compliance requirement that exists whether we like it or not.

The investment case for a security or infrastructure program has to make that math legible. Not in technical terms - in business terms. What is the risk? What does it cost if it materializes? What does it cost to prevent it? What happens if we wait?

---

## Framework: The Five Questions

Every executive investment request for a security or infrastructure program should answer five questions. If you cannot answer all five clearly, you are not ready to make the ask.

### 1. What is the risk?

Be specific. Quantify where possible. Connect it to something the executive already cares about.

Not: "Our encryption coverage is insufficient."

Yes: "37% of our platform services are transmitting data without encryption in transit. Any of those services represents a potential data exposure path. In the last 18 months, three peer companies have reported breaches attributed to unencrypted internal traffic interception."

Risk has three components: what could happen, how likely it is, and what the impact would be. Give executives all three.

### 2. What does it cost if we do nothing?

This is the number most investment cases skip. Do not skip it.

Potential costs of inaction for security and infrastructure programs:

- **Regulatory penalties** - GDPR, HIPAA, PCI fines are quantifiable. Look them up and cite them.
- **Audit findings** - A finding that requires remediation after the fact almost always costs more than building it correctly the first time.
- **Breach costs** - IBM and Ponemon publish annual breach cost studies. Use them as benchmarks.
- **Technical debt** - The longer an infrastructure problem runs, the more expensive it becomes to fix. Quantify the compound cost.
- **Competitive risk** - Security posture is increasingly a customer evaluation criterion. Quantify what a trust incident would cost in customer terms.

### 3. What are we asking for?

Be specific and complete. Executive sponsors who get surprised by scope or cost mid-program do not stay sponsors.

The ask should include:
- Engineering headcount (named roles and allocations, not just FTEs)
- Timeline with key milestones
- Budget (tooling, licensing, vendor costs)
- What you are asking them to do personally (air cover, escalation authority, specific decisions)

### 4. What does success look like?

Define it with numbers. Vague objectives do not get funded and cannot be reported against.

Not: "Significantly improve our encryption posture."

Yes: "100% encryption in transit across all platform services by Q3. Measured by quarterly audit of service-to-service communication logs. Baseline today is 63%."

### 5. What is the risk of the program itself?

Every investment has execution risk. Acknowledge it and show you have a plan. Executives who feel like they are being sold a sure thing will be skeptical. Executives who feel like the TPM has thought through what could go wrong and has a plan will be more confident.

Typical program risks to address:
- Engineering team capacity and competing priorities
- Dependencies on other teams that are not yet committed
- Technical complexity or unknowns in the design
- Regulatory timeline constraints

---

## Structuring the Ask Document

A one-page investment case is better than a ten-page one if it answers the five questions clearly. Here is a structure that works.

```
PROGRAM INVESTMENT REQUEST

Program:        [Name]
Requesting:     [TPM name and executive sponsor]
Date:           [Date]
Decision Needed: [By when]

THE PROBLEM
[2-3 sentences. Specific. Quantified where possible.]

COST OF INACTION
[2-3 sentences. What happens if we do not address this and by when.]

THE INVESTMENT
[Table: headcount, timeline, budget]

WHAT SUCCESS LOOKS LIKE
[2-3 measurable outcomes with target dates]

PROGRAM RISKS AND MITIGATIONS
[2-3 bullet points. Each with a mitigation.]

ASK
[What you need from the executive specifically - budget approval,
headcount allocation, air cover for cross-org dependencies, etc.]
```

Keep it to one page if you can. Put supporting detail in an appendix.

---

## Compliance-Driven Programs

Compliance-driven programs have a different investment structure because the question is not whether to do it - it is how much to invest and how fast to move.

For compliance programs, lead with the regulatory obligation: what framework applies, what the specific requirement is, what the penalty exposure is, and what the timeline is. That frames the investment not as a choice but as a constraint.

Then give the executive two or three options with different cost and risk profiles:

| Option | Approach | Cost | Timeline | Risk |
|--------|---------|------|----------|------|
| Option A | Full compliance by deadline | Higher | Faster | Lower - meets requirement |
| Option B | Phased compliance with interim controls | Medium | Staged | Medium - some risk window |
| Option C | Minimum viable compliance | Lower | Slower | Higher - audit exposure |

Let the executive choose. Your job is to make sure the options are real and the risks are honest.

---

## Reporting Investment Progress to Executives

Once the investment is approved, executives need to see that it is being deployed effectively. They funded the program - they want to know it is working.

Executive investment reporting should show:

**Progress against the investment thesis.** If the investment case said we would achieve X% coverage by Y date, report against that metric. Not sprint velocity, not story points - the number that justified the investment.

**Risk trend.** Is the security risk declining as planned? Show it. A graph of vulnerability count over time, encryption coverage by quarter, or MFA adoption rate tells a story that bullet points cannot.

**Budget pacing.** Is spend tracking to forecast? Surprises here erode trust fast. Flag variances early with an explanation and a revised forecast.

**Decisions needed.** If the executive approved an investment, they have an obligation to clear blockers. Make it easy for them to do that by naming the specific decisions needed and by when.

---

## Common Mistakes in Security Investment Cases

**Starting with the technical problem.** Executives do not fund technical problems. They fund business outcomes and risk reduction. Lead with the business impact.

**Underestimating the ask.** Coming back for more budget mid-program is one of the fastest ways to lose an executive sponsor. Be thorough upfront even if the number is uncomfortable.

**Omitting the cost of inaction.** This is the most common gap. Without it, the investment looks like a cost with no alternative. With it, it looks like risk management.

**Vague success criteria.** "Improve our security posture" is not a success criterion. It cannot be measured, reported against, or celebrated when achieved. Make it specific.

**Burying the ask.** The executive needs to know what they are deciding. Put it at the top or the bottom - not in the middle.

**Not asking for what you actually need.** If you need the executive to personally call the VP of Engineering to unblock a dependency, say so. That is a legitimate ask. Hinting at it is not the same thing.

---

*Version 1.0. Propose changes via pull request.*

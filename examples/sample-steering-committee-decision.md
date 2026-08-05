# Sample Steering Committee Decision

A steering committee is a decision-making forum, not a status meeting. The test of a good decision item is simple: could the committee make the call in the room, with what you gave them, in the time they have? These examples show the difference between a decision the committee can actually make and an "update" that sends everyone back to email.

**Scenario (sanitized).** A platform-security program must close a compliance finding - TLS 1.0/1.1 still enabled on 12 services - before a contractual customer deadline. The remaining fix depends on the Identity Platform team, which does not report to the program and is fully committed to another release. Only the steering committee can reprioritize that team or approve an alternative.

---

## Weak

> "Encryption modernization is progressing well and most services are remediated. The Identity Platform dependency is a concern and may put the deadline at risk. We will need support from the committee and will keep you updated."

### Why This Fails

There is no decision here, only a status with a worry attached. The committee cannot act on it: no options, no recommendation, no dates or dollars, no statement of what "support" means or who would provide it. "May put the deadline at risk" hides the actual exposure. "We will keep you updated" tells nine busy executives they can disengage. This is the item that produces a follow-up meeting instead of a decision, and by the next session an option has usually expired.

---

## Better

> **Decision needed:** How to close the TLS 1.0/1.1 finding on the 12 remaining services before the March 31 contractual deadline.
>
> **Why this committee, why now:** The remaining fix depends on the Identity Platform team, which is outside the program's authority and fully committed to the SSO general-availability release. Only this committee can reprioritize them or fund an alternative. Identity's next sprint locks on February 13 - after that, the reprioritization option is gone and only the slower paths remain.
>
> **Options:**
>
> | # | Option | Hits Mar 31? | Cost / tradeoff |
> |---|--------|--------------|-----------------|
> | A | Reprioritize Identity Platform to deliver the integration | Yes | Slips SSO GA by about 3 weeks |
> | B | Scoped exemption plus compensating controls (WAF rule + monitoring), remediate by Q3 | Partial | Finding stays open through the Q2 audit; residual risk on exposed services |
> | C | Fund 2 contractors for 8 weeks to build in parallel | Yes, with risk | About $120K-$160K; onboarding and ramp risk |
>
> **Recommendation:** Option A for the 4 customer-facing services (real external exposure); Option B for the 8 internal-only services (low exposure, audit-acceptable with compensating controls). This concentrates the reprioritization cost where the risk actually is and avoids over-rotating the Identity team for internal services.
>
> **Cost of not deciding today:** Every week of delay past February 13 removes Option A. After that, only B (finding open through the audit) or C (higher cost, ramp risk) remain.

### Why This Works

The ask is one clear question. The reason it belongs at this level is explicit - a cross-organizational reprioritization no one below the committee can make. The options are bounded, and each carries an honest tradeoff, including the one the recommendation rejects. The recommendation is specific and reasoned - split by exposure rather than one-size-fits-all - which shows the committee the TPM has already done the thinking. And the cost of delay is not rhetorical: it names the date on which an option disappears, which is what turns "we will revisit next month" into a decision today.

---

## The Decision, Recorded

A decision that is not written down did not happen. Capture it in the room and read it back before the meeting ends:

> **Decision (Feb 6):** Approved Option A for the 4 customer-facing services; Option B (scoped exemption, remediate by Sep 30) for the 8 internal services. **Owner:** program lead. **Actions:** Identity reprioritization confirmed with the sponsoring VP by Feb 11; exemption and compensating controls filed with the audit team by Feb 20. **Revisit:** March steering, remediation status on the deferred 8.

This is what separates a committee that drives accountability from one that rubber-stamps: the decision, the owner, the action, and the date leave the room together.

---

## The Pattern That Works

A steering-committee decision the room can actually make answers five questions:

1. **What is the exact call?** One question, phrased so a choice is possible - not a status with a worry.
2. **Why here, why now?** Name the reason it needs this forum (a cross-org call no one below can make) and the date that forces it.
3. **What are the options?** Bounded, each with an honest tradeoff, including the cost of the one you are not recommending.
4. **What do you recommend, and why?** Do the thinking for them. A recommendation with reasoning is not a loss of neutrality, it is the job.
5. **What does waiting cost?** Name what specifically gets worse, ideally an option that expires on a date.

If the item cannot answer those five, it is an update, not a decision - and it belongs in the pre-read, not the committee's time.

---

## On the Instinct to Bring an Update Instead of a Decision

The most common steering-committee failure is not a bad decision. It is arriving with no decision - a polished status that lets everyone nod and move on. It feels safer: no one has to commit, and nothing can be pinned on the ask. But a program that never brings decisions trains its committee to disengage, and the calls that needed executive air cover get made too late, at the working level, without it. Bring the committee a real decision every time you have one. That is the only reason the forum exists, and it is the fastest way to earn the room's attention on the day a decision genuinely cannot wait.

---

*Part of the [program-reporting-frameworks](https://github.com/ChefPlex/program-reporting-frameworks) repo. See the [Steering Committee Deck Structure](../steering-committee-deck-structure.md) for the full model; this example fills Slide 5, Decisions Required. Dates, dollar figures, and team names are illustrative - sanitize to your context before use.*

*Version 1.0. Propose changes via pull request.*

# Steering Committee Deck Structure

A steering committee is not a status meeting. It is a decision-making forum. The deck exists to give decision-makers what they need to make good decisions - not to demonstrate program activity, not to prove the TPM is working hard, and not to give engineers an audience for technical deep dives.

If the steering committee ends without anyone having made a decision or taken an action, something went wrong. Either you did not bring them a real decision, or the deck buried the decision under so much status information that nobody got to it.

This guide covers how to structure a steering committee deck that actually serves its purpose.

---

## The Core Principle

Executives in a steering committee have limited time and high cognitive load. They are thinking about twenty things before your program and twenty things after it. Your job is to give them a clean signal - what is the current state, what decisions are needed, and what do they need to do - in a format they can process in 30 minutes.

Every slide should earn its place by answering a question an executive would actually ask. If you cannot articulate the question a slide answers, the slide does not belong in the deck.

---

## Recommended Structure

### Slide 1: Program Status at a Glance

The executive summary. This slide should be able to stand alone.

**Contents:**
- Program name and reporting period
- Overall status: Green / Yellow / Red with one-sentence explanation
- Top three things to know this period (each one sentence)
- One key decision needed from this committee (if any)

**Design principle:** If an executive reads only this slide, they should have enough to have an informed conversation about the program. Everything after this slide is supporting detail.

---

### Slide 2: Progress Against Objectives

Show movement against the Definition of Done. Not activity - outcomes.

**Contents:**
- Table of program objectives with current status and trend
- Key metrics with baseline, target, and current value
- Milestone status: what was planned this period, what was delivered

| Objective | Metric | Baseline | Target | Current | Trend |
|-----------|--------|---------|--------|---------|-------|
| [Objective 1] | | | | | Up / Flat / Down |

**Design principle:** The question this slide answers is "are we achieving what we said we would achieve?" If the answer is yes, this slide is reassuring. If the answer is no, this slide sets up the conversation about why and what to do about it.

---

### Slide 3: Schedule and Milestone Health

**Contents:**
- Current milestone status across workstreams
- What was completed since last steering committee
- What is planned for the next period
- Any milestone slippage with explanation

| Milestone | Owner | Planned Date | Current Forecast | Status |
|-----------|-------|-------------|-----------------|--------|
| | | | | Green / Yellow / Red |

**Design principle:** Show the dates, show the current forecast, show the status. Do not hide slippage - it will come out eventually and it is better to present it with context and a plan than to have it surface as a surprise.

---

### Slide 4: Risks and Issues

The slide most executives want to spend the most time on - and the one most TPMs under-invest in.

**Contents:**
- Top 3-5 active risks with probability, impact, and mitigation status
- Active issues requiring steering committee awareness or decision
- Risks that were closed since last steering committee

| Risk / Issue | Type | Rating | Status | Mitigation | Owner | Escalation Needed? |
|-------------|------|--------|--------|-----------|-------|-------------------|
| | | | | | | Yes / No |

**Design principle:** The steering committee should see risks before they become issues. If a risk only shows up on this slide after it has materialized into a problem, the reporting was too slow. Yellow and Red risks belong here while they are still manageable.

---

### Slide 5: Decisions Required

The reason the steering committee exists. Be explicit.

**For each decision needed:**
- What the decision is
- Why it needs to be made at this level
- What options the committee is choosing between
- The recommendation (if you have one) and the reasoning
- The consequence of not deciding

| Decision | Options | Recommendation | Why Now | Owner |
|---------|---------|---------------|---------|-------|
| | | | | |

**Design principle:** Never walk into a steering committee without knowing what decisions you need. If there are no decisions this period, say so explicitly - "no decisions required this period" is valid and gives the committee time to ask questions rather than manufacture decisions.

---

### Slide 6: Dependencies and Cross-Functional Items

**Contents:**
- Dependencies at risk and what support is needed from steering committee members
- Cross-organizational issues that require executive intervention
- Items where the committee can clear blockers by making a call, sending an email, or assigning resources

**Design principle:** This slide converts steering committee participation from passive reception to active support. Executives often have the ability to clear blockers in five minutes that have been stuck for weeks at the working level. Give them the specific ask.

---

### Slide 7: Budget and Resources

**Contents:**
- Budget status: approved, spent, forecast
- Resource status: planned vs. actual headcount, any gaps
- Any budget variance with explanation and reforecast

| Category | Approved | Spent to Date | Remaining | Forecast | Variance |
|----------|---------|--------------|-----------|---------|---------|
| Engineering | | | | | |
| Tooling | | | | | |
| Vendor | | | | | |
| Total | | | | | |

**Design principle:** Keep this brief unless there is a variance to explain. If the program is tracking to budget, this slide should take 60 seconds to cover. If there is a variance, explain it clearly and present a reforecast.

---

### Slide 8: Next Period Preview

**Contents:**
- Top 3 priorities for the next reporting period
- Upcoming milestones and target dates
- Decisions needed in the next period (so the committee can be thinking about them)
- When the next steering committee is

**Design principle:** Ending with a forward look leaves the committee oriented and prepared rather than just updated.

---

## What Does Not Belong in a Steering Committee Deck

**Sprint velocity and story points.** Executives do not know what these mean and do not need to. Convert to milestone progress or outcome metrics.

**Engineering architecture diagrams.** If the committee needs to understand a technical decision, describe it in business terms. The architecture diagram belongs in the working-level design review.

**Complete RAID log.** Include a summary of top risks. Link to the full RAID log in an appendix.

**Meeting notes or action item trackers.** These go in the distributed program materials, not the deck.

**More than 10 slides.** If the deck is longer than 10 slides, something is being covered that belongs in a pre-read or a working session, not a steering committee.

---

## Before the Meeting

**Distribute the deck 24-48 hours in advance.** Steering committee members should come prepared, not be reading the deck for the first time on the call. A pre-read note identifying the key decisions for the session helps them prioritize.

**Know what you are asking for.** Every steering committee should have a clear ask. Even if the ask is "no decisions needed this session, we are here to update you and answer questions," know that going in.

**Prepare for the hard questions.** If your program is Yellow or Red, know what the executive is going to ask and have a direct answer ready. "We are working on it" is not an answer.

---

## In the Meeting

**Do not read the slides.** The committee has the deck. Walk them through the highlights and spend the time on discussion, not narration.

**Lead with the status and the decisions.** Do not save the important things for the end of the meeting. Put the key decisions and any Yellow or Red status first.

**Capture decisions and actions in real time.** Have someone taking notes. Before the meeting ends, read back the decisions made and the actions assigned. Confirm owners and due dates out loud.

**Respect the time.** End on time or early. Steering committees that run long become steering committees people stop attending.

---

## After the Meeting

- Circulate notes within 24 hours
- Enter actions in the tracker
- Update the RAID log with any new risks or issues surfaced
- Follow up on any decisions that need to be communicated to the broader team

---

*Version 1.0. Propose changes via pull request.*

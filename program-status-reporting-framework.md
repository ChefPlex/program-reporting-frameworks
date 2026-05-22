# Program Status Reporting Framework

A status report has one job: give the right people the right information at the right time so they can make decisions. Everything else is overhead.

The mistake most TPMs make is writing status reports for themselves - detailed, comprehensive, technically accurate. The mistake after that is writing them for the auditors - process-heavy, formatted to prove effort rather than communicate state. Neither serves the people who actually need to act on the information.

This framework defines a two-tier approach: a short version for async consumption and quick triage, and a long version that gives decision-makers full context. Both are built around the same core content - you write the long version once and the short version falls out of it.

---

## The Two-Tier Model

### Short Version

Designed to be read in 30 seconds. Works in Slack, email, a dashboard cell, or a spreadsheet column. The reader should be able to tell at a glance whether they need to pay attention to this program this week.

```
[PROGRAM NAME] | [REPORTING PERIOD] | Status: 🟡 At Risk

Highlights:
• [Workstream A] — [one-line status + ETA if relevant]
• [Workstream B] — [one-line status + ETA if relevant]
• [Workstream C] — [one-line status + ETA if relevant]

Risks / Blockers: [one line or "None"]
Leadership Ask: [one line or "None"]
```

**Rules:**
- Max 5 highlight bullets; each bullet 15 words or fewer
- Status emoji per bullet: 🟢 on track / 🟡 at risk / 🔴 off track / 🔵 complete
- If any workstream is 🟡 or 🔴, the header status matches the worst color
- Leadership Ask is never omitted - "None" is a valid answer and a useful signal

---

### Long Version

Designed to give a full-context picture for executive briefings, steering committees, or async review. Also serves as the source document for anyone who needs to understand the program in depth without asking you questions.

```markdown
# [PROGRAM NAME] -- [STATUS PERIOD] | [DATE]

**Program Status:** 🟡 At Risk | **Reporting Period:** [dates]

---

## Highlights
* 🟢 [Workstream A] -- [1-2 sentences: what happened, what is next, ETA]
* 🟡 [Workstream B] -- [1-2 sentences + why it is at risk + path-to-green with owner and date]
* 🔴 [Workstream C] -- [1-2 sentences + revised plan and timeline]

---

## Workstream Health

| Workstream | Owner | Status | ETA | Notes |
|-----------|-------|--------|-----|-------|
| [A] | [name] | 🟢 On Track | [date] | [brief] |
| [B] | [name] | 🟡 At Risk | [date] | [path-to-green] |
| [C] | [name] | 🔴 Off Track | [date] | [revised plan] |

---

## Critical Issues / Risks
* [Issue] -- [impact] -- [mitigation in progress]

---

## Leadership Ask
* [Specific ask with owner and deadline] OR N/A

---

## Reference Docs
* [Link to RAID log, project tracker, design docs, etc.]

---
*For questions: [#channel]. cc: [stakeholder list]*
```

**Rules:**
- Any 🟡 or 🔴 workstream MUST include: why it is off track + path-to-green + owner + resolution date
- Leadership Ask is always present - N/A is fine, omitting it is not
- The long version links to source docs rather than repeating raw work item lists inline
- If chronologically stacking updates, newest entry goes at the top

---

## Status Color Definitions

The color means something specific. Use it that way.

| Color | Definition | What the reader should expect |
|-------|-----------|-------------------------------|
| 🟢 Green | On track. No action needed. | Nothing to do here this week |
| 🟡 Yellow | At risk. Specific issue identified, mitigation in progress. May need support. | Read the notes, may need to engage |
| 🔴 Red | Off track. Leadership attention required. | Needs a decision or intervention now |
| 🔵 Blue | Complete. Workstream or milestone finished. | Informational - no action needed |

**The Yellow requirement:** Any Yellow or Red status must include a path-to-green with a named owner and a target date. "Working on it" is not a path-to-green. "Engineering Lead completing the dependency mapping by [date], which unblocks the implementation team to start by [date]" is a path-to-green.

**Never go from Green to Red without a Yellow.** If a program goes from Green to Red in a single reporting cycle without a Yellow in between, the reporting was wrong, not the program. That is a trust issue with your stakeholders that is harder to fix than the program problem itself.

---

## Reporting Cadence

Match the cadence to the program velocity and stakeholder needs. There is no universal right answer, but there are wrong ones.

| Program Type | Recommended Cadence | Notes |
|-------------|--------------------|----|
| Fast-moving / high-risk | Weekly | Anything with a near-term deadline or active escalations |
| Standard delivery | Bi-weekly | Most programs in steady-state execution |
| Slow-moving / monitoring phase | Monthly | Programs in performance and control phase with no active issues |
| Crisis / incident response | Daily or as-needed | Frequency matches the rate of meaningful change |

The cadence should reflect the rate at which the program state meaningfully changes. A weekly report that says the same thing every week is noise. A bi-weekly report that misses a critical status change is a problem.

---

## Executive vs. Operational Reporting

The same program needs two different reporting modes for two different audiences.

### Executive audience

Infrequent, high-signal, outcome-focused. Executives need to know three things:
1. Are we on track to achieve the objective by the committed date?
2. What is the current risk exposure and how is it trending?
3. Is there anything that requires a decision or escalation at their level?

Lead with the status and the bottom line. Put the detail in an appendix or a linked doc. An executive update that buries the status on page three is not serving its audience.

### Operational / team audience

Frequent, specific, action-oriented. Engineering teams and cross-functional partners need to know what is blocked, what decisions have been made, what is due next week, and what you need from them. The RAID log drives this conversation - the status report summarizes it.

---

## Mapping to Spreadsheets and Dashboards

If your organization tracks program status in a spreadsheet or portfolio dashboard, the short version maps cleanly to standard columns:

| Column | Maps to |
|--------|--------|
| Program | Header program name |
| Status | Header emoji + label |
| Period | Reporting period |
| Summary | Highlights bullets (semicolon-separated or one per cell) |
| Risk | Risks / Blockers line |
| Ask | Leadership Ask line |
| Updated | Date in header |

The short version is intentionally plain text so it survives a paste into any tool without breaking formatting.

---

## Common Mistakes

**Writing for yourself, not your audience.** A status report is not a journal entry or a project log. Every sentence should serve the reader's ability to understand state and take action.

**Burying the status.** The color and the one-line summary go at the top. Every time.

**Omitting the Leadership Ask.** If you need something from leadership, say so explicitly. Hints do not get acted on. A named ask with a deadline does.

**Reporting Yellow or Red without a path-to-green.** Telling leadership a program is at risk without telling them what is being done about it and by when is not useful. Come with the problem and the plan.

**Inconsistent color standards.** If Yellow means something different from week to week or TPM to TPM, the color stops being a signal. Define what the colors mean for your program at the start and apply them consistently.

**Late status reports.** A status report that comes out after the meeting it was meant to inform is a status report for the record, not for the decision. Get it out before people need it.

---

*Version 1.0. Propose changes via pull request.*

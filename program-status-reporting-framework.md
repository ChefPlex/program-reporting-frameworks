# Program Status Reporting Framework

A status report has one job: give the right people the right information at the right time so they can make decisions. Everything else is overhead.

The mistake most TPMs make is writing status reports for themselves - detailed, comprehensive, technically accurate. The mistake after that's writing them for the auditors - process-heavy, formatted to prove effort rather than communicate state. Neither serves the people who actually need to act on the information.

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
- Any 🟡 or 🔴 workstream MUST include: why it's off track + path-to-green + owner + resolution date
- Leadership Ask is always present - N/A is fine, omitting it's not
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

**Never go from Green to Red without a Yellow.** If a program goes from Green to Red in a single reporting cycle without a Yellow in between, the reporting was wrong, not the program. That's a trust issue with your stakeholders that's harder to fix than the program problem itself. The exception is an external event nobody could have seen in the previous cycle - a vendor failure, a new regulatory ruling, an incident. When that happens, say so in the report: name the event and when it occurred, so the jump reads as news rather than as a reporting failure.

**Silence from a dependency owner is not a Green status.** If you have not heard back, that is the information. Either it's fine and they forgot to tell you, or it's not fine and they're hoping you won't notice. Neither of those is Green. Chase it before the report goes out, and if you can't get an answer in time, report the silence rather than the assumption you made in its place.

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

Lead with the status and the bottom line. Put the detail in an appendix or a linked doc. An executive update that buries the status on page three isn't serving its audience.

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

**Writing for yourself, not your audience.** A status report isn't a journal entry or a project log. Every sentence should serve the reader's ability to understand state and take action.

**Burying the status.** The color and the one-line summary go at the top. Every time.

**Omitting the Leadership Ask.** If you need something from leadership, say so explicitly. Hints do not get acted on. A named ask with a deadline does.

**Reporting Yellow or Red without a path-to-green.** Telling leadership a program is at risk without telling them what is being done about it and by when isn't useful. Come with the problem and the plan.

**Inconsistent color standards.** If Yellow means something different from week to week or TPM to TPM, the color stops being a signal. Define what the colors mean for your program at the start and apply them consistently.

**Late status reports.** A status report that comes out after the meeting it was meant to inform is a status report for the record, not for the decision. Get it out before people need it.

**Adjectives where numbers belong.** "Encryption coverage increased significantly" tells the reader nothing they can act on. "Coverage increased from 67% to 78% this month, on track for 90% by end of quarter" gives them the rate, the remaining gap, and grounds to decide whether to worry. Numbers beat adjectives everywhere, and a status report is where the substitution costs the most.

**Numbers with no source.** A number is only as good as the reader's ability to check it. Every number in a status report carries three things: its **source** (the system it came from), an **as-of time**, and the **method** (what was counted and how). "78% of services encrypted (source: fleet scanner, as of Monday 09:00 UTC, services with all listeners on TLS 1.2+ out of all services in the inventory)" can be checked. "78%" cannot. Derive the number from the system of record each time rather than copying it forward from last week's report, because a restated number goes stale silently and nobody notices until two reports disagree.

---

## Reporting an AI Workstream

AI work breaks some of the usual reporting habits. Three adjustments:

- **Report reuse, not usage.** Logins and prompt counts rise under any mandate, whether or not the work changed. Report how many people came back to the same workflow and what it replaced.
- **Report the spread, not one run.** The same AI task run twice gives different results. An accuracy or quality figure from a single run is an anecdote. Run it several times and report the range alongside the average.
- **An AI-drafted status must say what it did not read.** If a model summarized channels, tickets or documents into the report, state its coverage: which sources it read, which it skipped or truncated, and the time window. A confident summary of half the inputs reads exactly like a summary of all of them.

*The reasoning behind several of these is in [TPM craft notes](https://github.com/ChefPlex/learning-notes/blob/main/tpm-craft-notes.md).*

---

*Version 1.0. Propose changes via pull request.*

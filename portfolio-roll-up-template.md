# Portfolio Roll-Up: Reporting Across Programs

A portfolio roll-up has one reader and one question. The reader is the leader who owns several programs. The question is: **where should I spend my attention this week?**

Everything on the page should help answer that. A roll-up that tells the leader "mostly fine" has answered nothing, because "mostly fine" is true of almost every portfolio right up to the week it is not.

This document sits on top of the [Program Status Reporting Framework](https://github.com/ChefPlex/program-reporting-frameworks/blob/main/program-status-reporting-framework.md). It does not replace it. Each program still writes its own report, with its own color, path-to-green and leadership ask. The roll-up is a disciplined **reading** of those reports, put on one page. It is not a portfolio-management system, it does not decide what gets funded, and it says nothing about how to staff or design a PMO [Program Management Office]. It is reporting, across programs.

One sentence to keep in mind the whole way through: **the roll-up is only as honest as the weakest program report under it.**

---

## Before You Roll Anything Up

Three things have to be true first. If they are not, the roll-up will compare things that do not mean the same thing, and the page will look precise while being wrong.

| Prerequisite | What it means | Why it matters |
|:---|:---|:---|
| **One set of color definitions** | Every program uses the Green / Yellow / Red / Blue definitions in the Status Reporting Framework. | If Yellow means "a bit behind" in one program and "needs a decision" in another, counting Yellows tells the reader nothing. |
| **One as-of date** | Every program report in the roll-up is cut at the same point, or carries its own date so staleness is visible. | A Green from three weeks ago and a Red from yesterday are not the same kind of fact. |
| **One set of thresholds** | Schedule slip and budget variance use the same bands for every program. | A 15% overrun cannot be Yellow in one program and Green in the next. Pick the bands once and apply them to all. |

For the thresholds, a public precedent exists. The US federal IT Dashboard rates cost and schedule variance with fixed bands: "a variance greater than or equal to 30 percent is red, a variance greater than or equal 10 percent and less than 30 percent is yellow, and a variance less than 10 percent is green" ([GAO-27-108416](https://files.gao.gov/reports/GAO-27-108416/index.html), October 7, 2026). You do not have to use those numbers. You do have to use one set.

---

## The Roll-Up Rules

These are practice, not a standard. No published standard reviewed for this document gives an authoritative formula for combining program colors into a portfolio view. Each rule below is here because breaking it hides a Red.

### 1. Never average colors

Four Greens, one Yellow and one Red do not average to Green. They are four Greens, one Yellow and one Red.

Averaging is attractive because it produces one tidy answer. It is also the single fastest way to make the Red program disappear. The leader who most needs to see the Red is the one reading the averaged color.

Even an auditor who does average has to override the average for serious risk. When the US GAO [Government Accountability Office] rated 53 federal IT investments itself in 2026, it scored each risk's exposure, "created a weighted average of the investment's risk exposure scores," and then "adjusted ratings if serious risks to an investment were discussed in" audit reports or executive briefings ([GAO-27-108416](https://files.gao.gov/reports/GAO-27-108416/index.html), October 7, 2026). The average alone was not trusted to show a serious risk. A portfolio color averaged from program colors has no such override, which is why this template does not average at all.

### 2. Show the distribution, not a portfolio color

A portfolio does not have a color of its own. It has a **count by color** and a **named list of the programs that are not Green.**

If you have budget or headcount numbers you trust, show the share by color as well as the count. One small Red program and one Red program that holds half the budget are different conversations. A public example of a distribution done well: the UK IPA [Infrastructure and Projects Authority] shows the count of major projects at each rating, department by department, never one color per department ([IPA Annual Report on Major Projects 2015-16](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/535243/ipa_annual_report_on_major_projects_2015_2016.pdf), Figure 17; the data in it is from 2015).

**If someone insists on one headline color,** use worst-of and say so: "Portfolio headline: Red (worst-of rule; one program Red)." That matches the single-program rule that the header matches the worst workstream. Never present a headline color without saying how it was derived.

### 3. Report status and delivery confidence as two separate fields

They answer different questions.

- **Status** is about today: is the program on its plan right now? It is mostly computed. Dates hit or missed, variance inside or outside the bands.
- **Delivery confidence** is about the commitment: will the program deliver what it promised, when it promised? It is a judgment by the program owner.

The UK IPA rates projects on delivery confidence, not status, and its definitions read as forecasts. Green: "Successful delivery of the project on time, budget and quality appears highly likely and there are no major outstanding issues that at this stage appear to threaten delivery significantly." Red: "Successful delivery of the project appears to be unachievable." ([IPA Annual Report 2015-16](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/535243/ipa_annual_report_on_major_projects_2015_2016.pdf), Annex: Definitions, page 25.) The US IT Dashboard keeps judgment and measurement apart too: cost and schedule colors are computed from variance, and, "Unlike the cost and schedule ratings, the Dashboard's CIO rating is determined by the agency CIO" ([GAO-27-108416](https://files.gao.gov/reports/GAO-27-108416/index.html)).

The two fields matter most when they disagree. **Status Green, confidence Low is the early-warning case.** Every milestone so far has landed, and the owner can already see the one that will not. A single color throws that information away.

### 4. Show trend only with the prior value

An arrow means nothing without the number it moved from. "Trend: worse" is a claim. "Yellow, was Green last report" is a fact the reader can check.

Show the prior color next to the current one, every time. If there is no prior report, write "New" and leave the trend empty. Do not draw an up arrow for a program that has only reported once.

The IPA report does this at portfolio level: each department's ratings for three consecutive annual reports, stacked side by side, so movement is visible as a change in the mix rather than claimed with an arrow (IPA Annual Report 2015-16, Figure 17). At your scale, a two-column table of prior color against current color, per program, does the same job.

### 5. A stale or missing report is never Green

Freshness is a field on the page, not a footnote.

- **Stale:** the program's latest report is older than its agreed cadence.
- **No report:** nothing arrived this period.

Count both separately from the colors. Never fold them into Green. This is the portfolio version of a rule in the Status Reporting Framework: silence from a dependency owner is not a Green status. Silence from a whole program is not Green either.

This is a failure the public record documents. In its 2026 review of federal IT investment ratings, the GAO found that "21 of the 53 CIO ratings were not updated in a timely manner, as required by agency processes" ([GAO-27-108416](https://files.gao.gov/reports/GAO-27-108416/index.html), October 7, 2026). Stale ratings are not an edge case. They are the default if nobody counts them.

### 6. Do not re-score a program's own call. Flag the disagreement instead

The program owner sets the program's color. They have read the detail and they are accountable for it. The person assembling the roll-up has not, and is not.

That does not mean the roll-up accepts every color. If you think a program is wrong, **challenge it with the owner before the page goes out.** If you still disagree, show both: "Owner: Yellow. Roll-up read: Red. Reason: ..." The leader then sees the program's call, your concern, and the evidence for each.

What you never do is quietly change the color. A roll-up that re-scores programs becomes a second, unaccountable status system, and the program owners stop trusting the first one.

The GAO-versus-CIO record shows why the disagreement is worth showing. In 2026, of "53 investments assessed, GAO's assessments matched the CIO ratings 27 times, showed more risk 24 times, and showed less risk two times." The same report recalls its 2016 review: of 95 investments, "our assessments matched the CIO ratings 22 times, showed more risk 60 times, and showed less risk 13 times" ([GAO-27-108416](https://files.gao.gov/reports/GAO-27-108416/index.html)). Ten years apart, an independent read found more risk than the self-rating far more often than less. Hiding that read helps no one. Overwriting the self-rating with it hides who owns the call.

### 7. State the roll-up's coverage

Every roll-up ends with a coverage line: which programs reported on time, which were stale, which did not report, and which reports you did not read in full. A reader will assume anything not mentioned was covered.

If a model drafted any part of the roll-up, it follows the [Status Contract](https://github.com/ChefPlex/tpm-toolbox/blob/main/STATUS-CONTRACT.md): the draft carries its coverage, and a person sets every color.

---

## Status, Confidence, Trend and Freshness at a Glance

| Field | Question it answers | Who sets it | Values |
|:---|:---|:---|:---|
| **Status** | Is it on plan today? | Program owner, from data | 🟢 🟡 🔴 🔵, per the Status Reporting Framework |
| **Confidence** | Will it deliver the commitment? | Program owner, by judgment | High / Medium / Low |
| **Trend** | What changed since last report? | Derived | Prior color shown beside current; "New" if no prior |
| **Freshness** | Is this report current? | Derived from the report date and cadence | Current / Stale / No report |
| **Roll-up read** | Does the assembler agree? | Portfolio TPM [Technical Program Manager] | Blank if agreed; a color and a reason if not |

---

## What Belongs at Portfolio Level

The roll-up is not six program reports stapled together. Most of what a program reports stays in the program report. The test for the portfolio page: **does this need action or attention from someone above the programs?**

| Belongs on the portfolio page | Stays in the program report |
|:---|:---|
| Count by color, with movement since last period | Workstream-by-workstream detail |
| The non-Green programs: why, path-to-green, owner, ask | Task burn-down and sprint metrics |
| Committed external dates missed or at risk in the next 90 days | Internal milestones with slack |
| Budget variance as a percent of plan, against the shared bands | Line-item spend and vendor detail |
| Cross-program dependencies at risk, with both owners named | Dependencies inside one program |
| Shared-capacity conflicts: one team or environment in two plans | Individual staffing changes |
| The top three risks across the portfolio, by exposure | Every risk on every log |
| Open leadership asks and how long each has been open | Asks already answered |
| Report freshness and coverage | Test counts, defect counts, tickets |

On risk, keep the portfolio view to the few highest-exposure risks across all programs, not a count of risks. "We have 140 open risks" tells a leader nothing. "These three risks, in these two programs, are the ones that would move a committed date" tells them where to look. The probability-times-impact rating in the [RAID log guide](https://github.com/ChefPlex/tpm-templates/blob/main/raid-log-guide.md) gives you the exposure to rank by.

If the page is growing past one screen, cut from the right-hand column of this table, not the left.

---

## Cross-Program Dependencies and Shared Capacity

This is the part of the roll-up no single program report can produce. It is often the most useful thing on the page.

Two kinds of item belong here:

1. **A dependency between programs.** Program A cannot finish until Program B delivers something specific. Each program may report its side as Yellow and reasonable. Nobody reports the connection.
2. **A shared-capacity conflict.** Two programs both plan on the same team, the same environment or the same change window in the same month. Each plan is fine on its own. Together they are impossible.

For each one, write one line with four parts: **what is needed, by when, the owner on each side, and what happens if it slips.**

**Weak:** "Some dependency concerns between Identity and Encryption."

**Better:** "Identity Migration and Encryption Coverage both plan on the platform networking team for the whole of March. The team can support one. Owners: Sarah (Identity), Priya (Encryption). If unresolved by March 13, one program loses its April date. Ask: sponsor to pick the order."

The weak line is true and useless. The better line names the collision, the owners, the deadline and the decision, so the leader can settle it in one conversation.

These items feed directly into Slide 6, Dependencies and Cross-Functional Items, of the [Steering Committee Deck Structure](https://github.com/ChefPlex/program-reporting-frameworks/blob/main/steering-committee-deck-structure.md). The portfolio page is the input to a cross-program steering slide, not a substitute for one.

---

## Who Owns What

| Role | Owns | Does not |
|:---|:---|:---|
| **Program owner** | The program's color, confidence, path-to-green and ask. On time, at the agreed cadence. | Skip a period and expect to be counted Green. |
| **Portfolio TPM (the assembler)** | Collecting the reports, checking them against the prerequisites, chasing stale ones, writing the cross-program lines, challenging colors, stating coverage. | Change a program's color. Fill a gap with an assumption. |
| **Portfolio leader (the reader)** | Acting on the page: answering the asks, settling the conflicts, deciding the escalations. | Read the page and change nothing. If that keeps happening, see Where This Breaks. |

---

## The Roll-Up Page

Copy this block. Fill one row per non-Green program; Green programs appear only in the counts and the coverage line unless something about them needs saying (such as Green with Low confidence).

```markdown
# [PORTFOLIO NAME] Roll-Up | As of [DATE] | Cadence: [weekly / bi-weekly / monthly]

## Distribution
| | Green | Yellow | Red | Blue | Stale | No report | Total |
|:---|:---|:---|:---|:---|:---|:---|:---|
| This period | [n] | [n] | [n] | [n] | [n] | [n] | [n] |
| Last period | [n] | [n] | [n] | [n] | [n] | [n] | [n] |
| Share of budget (optional) | [%] | [%] | [%] | [%] | [%] | [%] | 100% |

Headline (only if required): [worst color] (worst-of rule; [program] is [color])
Moved since last period: [program: prior -> current], ...

## Programs needing attention
| Program | Owner | Status (was) | Confidence | Why | Path-to-green (owner, date) | Ask | Roll-up read |
|:---|:---|:---|:---|:---|:---|:---|:---|
| [name] | [name] | [color] ([prior]) | [H/M/L] | [specific fact] | [action, owner, date] | [ask + deadline, or None] | [blank, or color + reason] |

## Committed dates at risk (next 90 days)
- [Program] - [milestone] - [committed date] - [at risk / missed] - [new date or "unknown"]

## Cross-program dependencies and capacity conflicts
- [What is needed] - [by when] - [owner A] / [owner B] - [impact if it slips] - [ask]

## Top risks across the portfolio (by exposure)
1. [Risk] - [program(s)] - [exposure] - [owner] - [mitigation]

## Open leadership asks
| Ask | Program | Raised | Days open | Decision needed by |
|:---|:---|:---|:---|:---|
| [ask] | [program] | [date] | [n] | [date] |

## Coverage
Reported on time: [list]. Stale: [list, with last report date]. No report: [list].
Not read in full: [list or "none"]. Drafted with AI assistance: [yes / no; if yes, coverage per the Status Contract].
Thresholds: schedule and budget bands [state them]. Colors per the Program Status Reporting Framework.
```

---

## Worked Example

*Everything in this example is invented: the company, the portfolio, the programs, the people and the figures.*

Fernhollow Systems, a fictional mid-size software company, runs a Platform Reliability portfolio of six programs: Identity Migration, Logging Consolidation, Vendor Exit, Encryption Coverage, Access Review Automation and Data Retention. All six report bi-weekly. The portfolio TPM assembles the roll-up for the VP of Platform every other Friday.

### Weak

> **Platform Reliability: Overall Green.** The portfolio is mostly on track. Four programs are Green, one is Yellow and one is Red, which averages out to Green. There are a few dependency concerns we are watching. Vendor Exit has had some challenges. More detail in the program reports.

### Why This Fails

- **The average hid the Red.** The one program that needs the VP this week is described as "some challenges."
- **No program is named** except in passing, and no owner, date or ask appears anywhere.
- **No trend.** The reader cannot tell that Vendor Exit was Yellow two weeks ago and is now Red.
- **No freshness.** One of the "Green" programs has not reported in three weeks. It was counted Green anyway.
- **The cross-program problem is invisible.** "A few dependency concerns" is the shared-capacity conflict that will cost a date in April.
- **No coverage.** The reader assumes all six reports were current and read. They were not.

### Better

```markdown
# Platform Reliability Roll-Up | As of Friday, March 6 | Cadence: bi-weekly

## Distribution
| | Green | Yellow | Red | Blue | Stale | No report | Total |
|:---|:---|:---|:---|:---|:---|:---|:---|
| This period | 2 | 2 | 1 | 0 | 1 | 0 | 6 |
| Last period | 4 | 2 | 0 | 0 | 0 | 0 | 6 |

Moved: Vendor Exit Yellow -> Red. Access Review Automation Green -> Yellow.
Data Retention Green -> Stale (last report February 13; counted as Stale, not Green).

## Programs needing attention
| Program | Owner | Status (was) | Confidence | Why | Path-to-green | Ask | Roll-up read |
|:---|:---|:---|:---|:---|:---|:---|:---|
| Vendor Exit | Marcus | 🔴 (🟡) | Low | Data export from the outgoing vendor is 40% complete; contract ends April 30 | Marcus and vendor agree a daily export schedule by March 11 | VP to approve a 60-day contract extension as fallback, decision by March 13 | |
| Encryption Coverage | Priya | 🟡 (🟡) | Medium | Coverage 71% against 80% plan; platform networking team not yet scheduled | Priya to confirm networking slot by March 13 | See capacity conflict below | 🔴: April date depends on the conflict below, which is unresolved |
| Access Review Automation | Lena | 🟡 (🟢) | Medium | Two of five source systems have no export API | Lena and Dev to agree a manual interim feed by March 18 | None | |
| Identity Migration | Sarah | 🟢 (🟢) | **Low** | All milestones met to date; April cutover needs the networking team in March | Resolve capacity conflict below | See below | |

## Committed dates at risk (next 90 days)
- Vendor Exit - vendor fully off - April 30 - at risk - new date unknown until March 11
- Identity Migration - cutover - April 20 - at risk - holds only if networking team is assigned

## Cross-program dependencies and capacity conflicts
- Identity Migration and Encryption Coverage both plan on the platform networking team for all of March; the team can support one.
  Owners: Sarah / Priya. If unresolved by March 13, one program loses its April date. Ask: VP to set the order.
- Vendor Exit needs Logging Consolidation's new pipeline live before the vendor's log service is switched off.
  Owners: Marcus / Tomas. Logging reports Green for April 1; no action needed this period.

## Open leadership asks
| Ask | Program | Raised | Days open | Decision needed by |
|:---|:---|:---|:---|:---|
| Order of networking team work | Identity / Encryption | Feb 27 | 8 | March 13 |
| Approve fallback contract extension | Vendor Exit | March 6 | 0 | March 13 |

## Coverage
Reported on time: Identity Migration, Logging Consolidation, Vendor Exit, Encryption Coverage, Access Review Automation.
Stale: Data Retention (last report February 13; Tomas chasing, owner on leave until March 9).
Not read in full: none. Drafted with AI assistance: no.
Thresholds: schedule slip 10% / 30%, budget variance 10% / 30%. Colors per the Program Status Reporting Framework.
```

### Why This Works

The [Sample Red / Yellow / Green Status](https://github.com/ChefPlex/program-reporting-frameworks/blob/main/examples/sample-red-yellow-green-status.md) sets five questions every program update must answer: what is the status, why, what is being done, what the reader needs to do, and when the status changes. Each row in the Better table answers all five. The portfolio page adds four things a single program report cannot:

1. **Movement.** The VP sees what changed since the last page, with the prior color shown, not an arrow.
2. **Freshness.** Data Retention is counted as Stale. It is not hiding inside the Greens, and the page says who is chasing it.
3. **The early warning.** Identity Migration is Green with Low confidence. Its owner can see the problem coming, and the page shows it a month before it would turn Yellow.
4. **The cross-program item.** The networking conflict appears in neither program's Red. It is the one decision on the page that only the VP can make, and it has a date.

Note also what the roll-up did with Encryption Coverage. Priya reports Yellow. The portfolio TPM reads it as Red because its date depends on an unresolved conflict. The page shows both and the reason, and Priya's color stands.

---

## Common Mistakes

**Averaging, or any arithmetic on colors.** Covered above. It is listed again because it is the mistake people make most and notice least.

**One color for the whole portfolio, with no derivation.** If a headline is required, it is worst-of, and the page says so.

**Counting "no report" as Green.** The program that went quiet is the one most likely to have a problem.

**Trend arrows with no prior value.** An arrow the reader cannot check is decoration.

**Too many measures.** If every program metric is on the portfolio page, nothing on it stands out. Use the table above and cut from the right.

**Re-scoring programs.** The assembler's opinion is useful. Silently overwriting the owner's color with it is not.

**Reporting every program every period at the same length.** Green programs with High confidence and current reports get one line in the counts. The space goes to the programs that need it.

---

## Where This Breaks

**The page is read and nothing changes.** If the same asks sit open period after period, the roll-up has become a record rather than a decision tool. Show "days open" on every ask, and when one passes a limit you agree in advance, it moves to the steering committee agenda by default.

**Programs learn to game the definitions.** Once the roll-up is visible, some owners will keep a program Green for as long as the definitions allow. The confidence field and the roll-up read are the counterweight, but only if the assembler actually uses them. A confidence rating that is always High is as useless as a color that is always Green.

**Self-ratings lean optimistic.** This is documented, not a theory. In the 2026 review, the CIO ratings that showed less risk than GAO's "minimized the potential severity and impact of high-risk scores" ([GAO-27-108416](https://files.gao.gov/reports/GAO-27-108416/index.html)), and the 2016 review found the same direction of error. An occasional independent read of a few programs, done by someone outside them, is the check.

**The same color in every period.** A program that has been Yellow for six periods with the same path-to-green is not Yellow. It is a program whose plan no longer describes reality. The movement row will show "Yellow -> Yellow" every time. Treat a long run of no movement as a question, not as stability.

**Different programs read the same definitions differently.** The GAO found exactly this across federal agencies: the selected agencies used the same suggested rating factors, but "their interpretation of these factors varies significantly" ([GAO-27-108416](https://files.gao.gov/reports/GAO-27-108416/index.html)). The fix is the prerequisites table at the top. Calibrate the colors with the program owners once, with real examples, before the first roll-up.

**The roll-up arrives after the meeting it was for.** Then it is a record, not an input. Set the as-of date early enough that the page reaches the leader before they need it, and accept a Stale line over a late page.

---

## Sources

All as of October 2026.

- US GAO, *IT Dashboard: Selected Agencies' Investment Ratings Fail to Fully Consider Risks*, GAO-27-108416, October 7, 2026. https://files.gao.gov/reports/GAO-27-108416/index.html. Source of every GAO figure and quote in this template, including its summary of the 2016 review (*IT Dashboard: Agencies Need to Fully Consider Risks When Rating Their Major Investments*, GAO-16-494, June 2, 2016).
- UK Infrastructure and Projects Authority, *Annual Report on Major Projects 2015-16*. https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/535243/ipa_annual_report_on_major_projects_2015_2016.pdf
- For portfolio management as a discipline (selection, funding, balancing), see PMI, *The Standard for Portfolio Management*, Fourth Edition. It is out of scope here; this document covers reporting only.

---

## Related

- [Program Status Reporting Framework](https://github.com/ChefPlex/program-reporting-frameworks/blob/main/program-status-reporting-framework.md): the color definitions, path-to-green and source rules every program report in the roll-up inherits.
- [Sample Red / Yellow / Green Status](https://github.com/ChefPlex/program-reporting-frameworks/blob/main/examples/sample-red-yellow-green-status.md): the single-program counterpart to the worked example above.
- [Steering Committee Deck Structure](https://github.com/ChefPlex/program-reporting-frameworks/blob/main/steering-committee-deck-structure.md): Slides 1 and 6 take the roll-up as input.
- [RAID Log Guide](https://github.com/ChefPlex/tpm-templates/blob/main/raid-log-guide.md): the exposure rating used to rank portfolio-level risks.
- [Status Contract](https://github.com/ChefPlex/tpm-toolbox/blob/main/STATUS-CONTRACT.md): the rules for any AI-assisted draft of this page.

---

*Part of the [ChefPlex TPM portfolio](https://github.com/ChefPlex/tpm-templates/blob/main/PORTFOLIO-GUIDE.md). Maintained by [Eric White](https://www.linkedin.com/in/edwhite). Licensed under [CC BY 4.0](LICENSE).*

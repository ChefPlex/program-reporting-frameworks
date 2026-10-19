# Steering Committee Deck Structure

A steering committee exists to close decisions. If nobody had to decide anything, it should have been an email. The deck's job is to get people to the decision, which means most of what you want to put in it doesn't belong: the activity summary, the proof you've been busy, the deep dive an engineer wants to give.

The table below is the whole steering committee, in the order the work happens: before the meeting, the deck slide by slide, the meeting itself, and the follow-up. Each row says what happens, what it produces, who owns it and how much it matters. What each slide should contain is in [Reference](#slide-by-slide). When you want the deck outline with its tables ready to paste, use the [alternate style](#alternate-style-the-deck-outline-on-one-page) at the bottom of this page.

---

## Steering Committee - [Program Name], [Date]

| What happens | Artifact / outcome | Owner | Level | Status | Notes |
|:---|:---|:---|:---|:---|:---|
| **Before the meeting** | | | | | |
| Name the decisions you need from this committee | List of decisions, or "no decisions this session" | TPM | Must | | Know what you're asking for, even if the ask is only to update and answer questions |
| Prepare for the hard questions | Direct answers ready | TPM | Must | | If the program is Yellow or Red, know what the executive will ask. "We are working on it" is not an answer |
| Send the deck 24-48 hours ahead, with a pre-read note naming the key decisions | Deck and pre-read sent | TPM | Must | | Members should come prepared, not read it for the first time on the call |
| **The deck** | | | | | |
| Slide 1: Program status at a glance | Status slide | TPM | Must | | It should stand alone. One decision needed, if any, goes here too |
| Slide 2: Decisions required | Decision table | TPM + product / program owner | Must | | Right after the status, because it is why the committee exists |
| Slide 3: Progress against objectives | Objectives and metrics table | TPM | Should | | Outcomes, not activity |
| Slide 4: Schedule and milestone health | Milestone table | TPM | Should | | Show the planned date, the forecast and the status. Don't hide slippage |
| Slide 5: Risks and issues | Top 3-5 risks and active issues | TPM | Must | | Risks belong here while still manageable, not after they land |
| Slide 6: Dependencies and asks | Specific asks of committee members | TPM | Should | | Executives can often clear in five minutes what has been stuck for weeks |
| Slide 7: Budget and resources | Budget table | TPM + finance | Should | | 60 seconds if on budget; a clear explanation and reforecast if not |
| Slide 8: Next period preview | Priorities, milestones, upcoming decisions, next meeting date | TPM | Should | | Ends the meeting looking forward |
| Appendix: link to the full RAID log | Link | TPM | As needed | | The deck carries the top risks only |
| **In the meeting** | | | | | |
| Lead with the status and the decisions | Decisions discussed first | TPM | Must | | Don't save the important things for the end |
| Walk the highlights; do not read the slides | Time spent on discussion | TPM | Should | | The committee has the deck |
| Capture decisions and actions in real time, and read them back before the end | Decisions and actions, with owners and due dates | Notes owner | Must | | Confirm owners and due dates out loud |
| End on time or early | | TPM | Should | | Steering committees that run long become steering committees people stop attending |
| **After the meeting** | | | | | |
| Circulate notes | Notes sent within 24 hours | TPM | Must | | |
| Enter the actions in the tracker | Actions tracked | TPM | Must | | |
| Update the RAID log with new risks or issues | RAID log updated | TPM | Must | | |
| Tell the broader team about decisions that affect them | Decisions communicated | TPM | Should | | |

### What goes in each column

- **What happens:** the activity, in the order it happens. Bold rows mark before, the deck, during and after.
- **Artifact / outcome:** what exists when it is done.
- **Owner:** the person who does it. Write a name once you know it.
- **Level:** **Must** - nearly every steering committee needs it. **Should** - the right practice for most. **As needed** - add it when the program calls for it.
- **Status:** done, in progress, not started, or skipped.
- **Notes:** a link, what is still open, or why it was skipped.

---

## How to Fill It In

**Start from the decisions.** Executives in a steering committee have limited time and high cognitive load. They're thinking about twenty things before your program and twenty things after it. Your job is to give them a clean signal - what is the current state, what decisions are needed, and what do they need to do - in a format they can process in 30 minutes.

**Make every slide earn its place.** Every slide should answer a question an executive would actually ask. If you can't articulate the question a slide answers, the slide doesn't belong in the deck.

**Say so when there is nothing to decide.** "No decisions required this period" is valid and gives the committee time to ask questions rather than manufacture decisions.

---

## What to Learn From

### Unknown vs Actionable

The same row on the Decisions Required slide, written two ways:

| | Decision | Options | Recommendation | Why Now | Owner |
|:---|:---|:---|:---|:---|:---|
| **Unknown** | Budget | TBD | | | TPM |
| **Actionable** | Approve [amount] for additional HSM capacity in both regions, so wave two can cut over | A) Approve now. B) Defer to next quarter; wave two slips about six weeks, and wave three with it | A - wave two holds its Apr 30 date | The platform team's capacity review is on the 22nd. After that, the slot goes to another program | [Sponsor name] decides; [TPM name] brings it |

The actionable row answers who decides, what they are deciding, when it has to be decided and why, where it lands (waves two and three), and how each option plays out. The unknown row asks the committee to do the TPM's thinking.

### Where This Breaks

- **Nobody decided anything.** If the meeting ends and nobody decided anything or took an action, something went wrong. Either you didn't bring them a real decision, or the deck buried it under so much status that nobody got there.
- **Sprint velocity and story points.** Executives don't know what these mean and don't need to. Convert to milestone progress or outcome metrics.
- **Engineering architecture diagrams.** If the committee needs to understand a technical decision, describe it in business terms. The architecture diagram belongs in the working-level design review.
- **The complete RAID log.** Include a summary of top risks. Link to the full RAID log in an appendix.
- **Meeting notes or action item trackers.** These go in the distributed program materials, not the deck.
- **More than 10 slides.** If the deck is longer than 10 slides, something is being covered that belongs in a pre-read or a working session, not a steering committee.
- **Risks that show up only after they land.** If a risk only shows up on the slide after it has materialized into a problem, the reporting was too slow.

---

## Reference

### Slide by Slide

**Slide 1: Program Status at a Glance.** The executive summary. Program name and reporting period · overall status, Green / Yellow / Red, with a one-sentence explanation · top three things to know this period, one sentence each · one key decision needed from this committee, if any. *If an executive reads only this slide, they should have enough to have an informed conversation about the program. Everything after this slide is supporting detail.*

**Slide 2: Decisions Required.** For each decision: what the decision is · why it needs to be made at this level · what options the committee is choosing between · the recommendation, if you have one, and the reasoning · the consequence of not deciding. *Never walk into a steering committee without knowing what decisions you need.*

**Slide 3: Progress Against Objectives.** Show movement against the Definition of Done. Not activity - outcomes. Program objectives with current status and trend · key metrics with baseline, target and current value · milestones planned this period and what was delivered. *The question this slide answers is "are we achieving what we said we would achieve?" If the answer is yes, this slide is reassuring. If the answer is no, this slide sets up the conversation about why and what to do about it.*

**Slide 4: Schedule and Milestone Health.** Current milestone status across workstreams · what was completed since the last steering committee · what is planned for the next period · any slippage, with the explanation. *Don't hide slippage - it will come out eventually, and it's better to present it with context and a plan than to have it surface as a surprise.*

**Slide 5: Risks and Issues.** The slide most executives want to spend the most time on - and the one most TPMs under-invest in. Top 3-5 active risks with probability, impact and mitigation status · active issues needing the committee's awareness or decision · risks closed since the last meeting. *The steering committee should see risks before they become issues. Yellow and Red risks belong here while they are still manageable.*

**Slide 6: Dependencies and Cross-Functional Items.** Dependencies at risk and what support is needed from committee members · cross-organizational issues that need executive intervention · items the committee can clear by making a call, sending an email, or assigning resources. *This slide converts steering committee participation from passive reception to active support. Give them the specific ask.*

**Slide 7: Budget and Resources.** Budget: approved, spent, forecast · resources: planned vs. actual headcount, any gaps · any variance, with the explanation and the reforecast. *Keep this brief unless there's a variance to explain.*

**Slide 8: Next Period Preview.** Top 3 priorities for the next period · upcoming milestones and target dates · decisions needed next period, so the committee can be thinking about them · when the next steering committee is. *Ending with a forward look leaves the committee oriented and prepared rather than just updated.*

---

## Alternate Style: The Deck Outline on One Page

Use this when you want the deck outline with its tables ready to paste into slides. Copy the block into the program folder.

```markdown
# Steering Committee: [Program Name] - [Date]

## Slide 1: Program Status at a Glance
- Program name and reporting period:
- Overall status (Green / Yellow / Red) and one-sentence explanation:
- Top three things to know this period:
  1.
  2.
  3.
- Key decision needed from this committee (if any):

## Slide 2: Decisions Required
| Decision | Options | Recommendation | Why Now | Owner |
|:---|:---|:---|:---|:---|
| | | | | |

## Slide 3: Progress Against Objectives
| Objective | Metric | Baseline | Target | Current | Trend |
|:---|:---|:---|:---|:---|:---|
| [Objective 1] | | | | | Up / Flat / Down |

## Slide 4: Schedule and Milestone Health
| Milestone | Owner | Planned Date | Current Forecast | Status |
|:---|:---|:---|:---|:---|
| | | | | Green / Yellow / Red |

## Slide 5: Risks and Issues
| Risk / Issue | Type | Probability / Impact | Status | Mitigation | Owner | Escalation Needed? |
|:---|:---|:---|:---|:---|:---|:---|
| | | | | | | Yes / No |

## Slide 6: Dependencies and Cross-Functional Items
- Dependencies at risk, and the support needed:
- Cross-organizational issues needing executive intervention:
- Asks the committee can clear:

## Slide 7: Budget and Resources
| Category | Approved | Spent to Date | Remaining | Forecast | Variance |
|:---|:---|:---|:---|:---|:---|
| Engineering | | | | | |
| Tooling | | | | | |
| Vendor | | | | | |
| Total | | | | | |

## Slide 8: Next Period Preview
- Top 3 priorities:
- Upcoming milestones and target dates:
- Decisions needed next period:
- Next steering committee:

## Appendix
- Link to the full RAID log:
```

---

*Version 1.1. Propose changes via pull request.*

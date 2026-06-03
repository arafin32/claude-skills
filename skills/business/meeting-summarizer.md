# Skill: Meeting Summarizer

| Category | Business |
| Version | 1.0 |
| Author | Kamrul Arafin |
| Last Updated | 2026 |
| License | MIT |

---

## What it does

Extracts key decisions, action items, and takeaways from meeting notes or transcripts, organizing them for clarity and follow-up.

---

## How to use it

1. Copy the system prompt below
2. Paste it into Claude
3. Paste your meeting notes or transcript
4. Get organized summary with action items
5. Share with team

### Time needed: 2-3 minutes per meeting

---

## System Prompt

```
You are an expert meeting facilitator and organizer. Your job is to extract key information from meeting notes and make them actionable.

When given meeting notes or a transcript, you will:
1. Identify key decisions made
2. Extract action items with owners and deadlines
3. List important discussion points
4. Highlight risks or blockers
5. Identify next steps
6. Organize for easy scanning and follow-up

Format your response as:

## Meeting Summary: [Meeting Name]

**Date:** [Date]
**Attendees:** [Who was there]
**Duration:** [How long]

---

## Key Decisions

- **Decision 1:** [What was decided and why]
  - Owner: [Who is responsible]
  - Impact: [Why this matters]

---

## Action Items

| Item | Owner | Deadline | Priority |
|------|-------|----------|----------|
| [Action] | [Name] | [Date] | High/Medium/Low |

---

## Discussion Highlights

- **Topic 1:** [What was discussed and conclusion]
- **Topic 2:** [Key points and any disagreements]

---

## Risks & Blockers

- 🚨 [Risk 1] — [What could go wrong and mitigation]
- 🚨 [Risk 2]

---

## Next Meeting

- **Date:** [When]
- **Focus:** [What to discuss]
- **Preparation:** [What to do before]

---

Rules:
- Be concise but specific
- Identify clear owners for every action item
- Include deadlines for everything
- Flag risks clearly
- Use clear formatting for scanning
- Include decisions and their rationale
- Highlight what changed from previous meetings
```

---

## Example Input

```
Team Sync Meeting - Q1 Planning
Date: January 15, 2024
Attendees: Sarah (PM), James (Engineering Lead), Maria (Design), Alex (Product)

Sarah: "Alright team, let's get aligned on Q1 priorities. We have three major items: the mobile redesign, API performance improvements, and customer feedback loop. Marketing is pushing hard on the mobile redesign since we'll be promoting it in February."

Maria: "The mobile designs are 80% done. I can have them finalized by end of week. But I need feedback from engineering on technical constraints."

James: "We can handle most of it, but the new gesture controls might need some work on older devices. Also, we're already slammed with the API optimization. Can we prioritize? The API work affects our SaaS performance tier, which is impacting customer churn."

Alex: "Right, the churn is the bigger issue. We've lost 3 customers this month due to slow API response times. I'd say fix the API first, then do the mobile redesign in February after we ship the API work."

Sarah: "Okay, so we're saying API first? That shifts our timeline."

James: "Yeah, if we focus the team on API optimization, we could ship in mid-February. Then mobile redesign would shift to late Feb/early March."

Maria: "That's tight for my team but doable. We'll need design reviews from all of you though."

Sarah: "Who's owning the API work? We need to make sure it's properly tracked."

James: "I'll own it. I'll need two engineers full-time on it. That means we pull them from other projects."

Alex: "What about the customer feedback loop? That was supposed to start this month."

Sarah: "Let's push that to Q2. We need to focus on retention first."

Maria: "I can start the feedback loop tool design anyway, so we're ready to build in Q2."

Sarah: "Great. So to confirm: API optimization is priority one, mobile redesign moves to late Feb, feedback loop pushes to Q2 design phase."

James: "We'll need QA to test the API changes thoroughly. Should be 1-2 weeks of testing before we ship."

Sarah: "Okay. Let's reconvene next Monday to look at progress."
```

## Example Output

## Meeting Summary: Q1 Planning - Team Sync

**Date:** January 15, 2024
**Attendees:** Sarah (PM), James (Engineering Lead), Maria (Design), Alex (Product)
**Duration:** ~20 minutes

---

## Key Decisions

🎯 **Priority Shift: API Optimization is now Q1 Priority #1**
- **What:** Shift engineering focus from mobile redesign to API performance optimization
- **Why:** API slowness is causing customer churn (3 lost customers in Jan due to performance)
- **Impact:** Mobile redesign timeline shifts from mid-February to late Feb/early March
- **Owner:** Sarah (PM) to communicate to stakeholders

🎯 **Customer Feedback Loop Pushed to Q2**
- **What:** Delay customer feedback loop project from Q1 to Q2
- **Why:** Need to focus on retention (API performance) first
- **Mitigation:** Maria will do design work in Q1 so we're ready to build in Q2
- **Owner:** Sarah (PM)

🎯 **Resource Allocation: Two Full-Time Engineers on API**
- **What:** Dedicate 2 engineers full-time to API optimization
- **Why:** Critical for customer retention and performance tier viability
- **Impact:** Other projects will be affected
- **Owner:** James (Engineering Lead)

---

## Action Items

| Action | Owner | Deadline | Priority | Notes |
|--------|-------|----------|----------|-------|
| Finalize mobile designs | Maria | Jan 19, 2024 | High | 80% done, needs eng feedback |
| Complete API optimization work | James | Feb 15, 2024 | High | 2 engineers full-time, includes 1-2 weeks QA testing |
| Review mobile designs (engineering feedback) | James | Jan 22, 2024 | High | Provide technical constraints feedback |
| QA testing for API changes | [TBD] | Feb 10, 2024 | High | 1-2 weeks testing before shipping |
| Begin mobile redesign (post-API) | Maria | Feb 20, 2024 | Medium | Ready after API ships |
| Design customer feedback loop tool | Maria | Feb 28, 2024 | Medium | Get ahead for Q2 build phase |
| Communicate Q1 priority changes to stakeholders | Sarah | Jan 16, 2024 | High | Marketing needs to know about timeline shift |
| Review feedback loop designs | Team | [Q2] | Low | Can happen in Q2 once designs are done |

---

## Discussion Highlights

📌 **API Performance Crisis**
- The API slowness is directly causing customer churn (3 customers lost this month)
- This is blocking the SaaS performance tier
- More urgent than the mobile redesign project

📌 **Mobile Redesign Status**
- Maria's designs are 80% complete, can finalize by end of week
- Gesture controls may have issues on older devices (technical constraint to solve)
- Team needs to do design reviews once finalized

📌 **Mobile Redesign Timeline Change**
- Originally: Early February
- New timeline: Late Feb/Early March (after API ships)
- Maria says it's tight but doable if she gets timely design feedback

📌 **Feedback Loop Tool**
- Originally planned for Q1 build, now pushed to Q2
- Maria will do design work in Q1 so we're ready to go in Q2
- This is the "smart" move to prepare without over-committing resources

---

## Risks & Blockers

🚨 **Risk: Mobile Redesign Timeline is Aggressive**
- Moving to late Feb/early March is tight for design, engineering, and QA
- **Mitigation:** Get design feedback immediately after finalization (James reviews by Jan 22)
- **Impact:** If delayed, could push into April or delay other Q1 work

🚨 **Risk: QA Capacity Unknown**
- API optimization requires 1-2 weeks of thorough QA testing
- **Blocker:** Who is doing the QA testing? Not yet assigned
- **Action:** Need to assign QA owner and check their capacity before Feb 1

🚨 **Risk: Unclear Technical Constraints on Mobile**
- Maria mentioned gesture controls might be problematic on older devices
- **Blocker:** James needs to provide technical constraints by Jan 22
- **Impact:** Could require design changes, pushing timeline further

🚨 **Opportunity: Q2 Feedback Loop Design**
- Maria preparing in Q1 means we can build immediately in Q2 without design delays
- **Action:** Make sure design work doesn't get de-prioritized for mobile redesign support

---

## Questions/Clarifications Needed

❓ **Who is the QA owner for API testing?** (Not yet assigned, but critical)
❓ **What's the full scope of API optimization work?** (Mentioned but not detailed)
❓ **How many older devices are affected by gesture control issues?** (Impact not quantified)

---

## Next Steps

✅ **Before next meeting (Jan 22):**
1. James provides technical constraints feedback on mobile designs
2. Maria finalizes mobile designs
3. Sarah communicates priority shift to stakeholders
4. Assign QA owner for API testing

✅ **Next meeting:** Monday, January 22, 2024
- **Focus:** 
  - Review engineering feedback on mobile designs
  - Confirm API optimization scope and timeline
  - Assign QA resources
  - Update on progress
  
- **Preparation:**
  - James: Have technical constraints written down
  - Maria: Have finalized designs ready to share
  - Sarah: Have communicated timeline change to stakeholders

---

## Meeting Health Check

✅ **What went well:**
- Clear decision-making (priorities were decided quickly)
- Team aligned on what matters (retention > new features)
- Realistic timeline discussion (acknowledged "tight" schedule)

⚠️ **What could be better:**
- QA owner should have been identified before end of meeting
- More detail on API scope would help James plan the work
- Gesture control issue needs quantification (how many users affected?)

---

## Tips & Variations

### For different meeting types:
- **Standup:** Focus on blockers and progress updates
- **Planning:** Emphasize decisions and timeline impacts
- **Retrospective:** Highlight learnings and process improvements
- **Client meeting:** Highlight decisions affecting deliverables and timeline

### Get more structured output:
- Ask for "executive summary" (1 paragraph for busy stakeholders)
- Request "timeline critical path" (what needs to happen in what order)
- Get "risk assessment" (probability and impact of each risk)
- Ask for "communication template" (what to send to stakeholders)

### Pro tips:
- Review summary with team before sharing (catch errors early)
- Share within 24 hours while things are fresh
- Use summaries as input for your project management system
- Track how many action items get completed (meeting effectiveness metric)
- For recurring meetings, track decisions over time to see patterns

---

## Common Issues

**Q: My meeting notes are messy/incomplete**
A: That's okay. The tool will extract what's there and flag gaps with "❓ Questions/Clarifications."

**Q: There are conflicting opinions in the meeting**
A: The summary will note disagreements and the final decision made.

**Q: Too many action items**
A: Prioritize them by deadline and impact. Long list usually means unclear planning.

**Q: Some attendees didn't get action items**
A: Good catch. Maybe they weren't the right person for the decision, or they need to be assigned something.

---

## Related Skills

- [`email-template-generator.md`](../business/email-template-generator.md) — Email the summary to the team
- [`calendar-blocker.md`](../other/) — Schedule time for action items [coming soon]

---

## Tags

#meetings #productivity #actionitems #organization #management

---

## Notes

- Sharing summaries within 24 hours keeps team aligned and motivated
- Clear action item ownership prevents things from falling through cracks
- Flagging risks early allows for better planning
- Good meeting summaries are a form of async communication for distributed teams
- Review old summaries quarterly to see if you're making progress on goals

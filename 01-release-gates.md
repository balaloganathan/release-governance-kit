# Release Gates

A gate is a short list of conditions that must be true before a change moves forward. Keep each gate small enough to check in five minutes.

Timings assume a twice-weekly CAB and a weekly release window. Adjust them to your cadence.

## Gate 1: Ready for release planning (T-10 business days)
- [ ] Change is linked to an approved story, defect or risk item
- [ ] Release type agreed: major, medium, minor or hotfix
- [ ] Dependencies identified: other teams, shared environments, enterprise release calendar
- [ ] Target release window booked

## Gate 2: Ready for CAB (T-5 business days)
- [ ] Testing complete in non-production, with evidence attached
- [ ] Implementation plan written step by step, with owners and timings
- [ ] Rollback plan written **and tested**
- [ ] Business production verification test (PVT) planned: who checks what, and when
- [ ] Required sign-offs collected (product owner, QA, security if applicable)
- [ ] Change record complete (see [04-change-record-template.md](04-change-record-template.md))

## Gate 3: Go/no-go (T-1 business day)
- [ ] CAB approval received
- [ ] No open critical defects
- [ ] Deployment team, approvers and on-call support confirmed for the window
- [ ] Go/no-go checklist completed (see [03-go-no-go-checklist.md](03-go-no-go-checklist.md))

## Gate 4: Release complete (T+1 business day)
- [ ] Post-implementation verification (PIV) done by the technical team
- [ ] Business PVT passed and confirmed by the business
- [ ] Change record closed with outcome
- [ ] Incidents, if any, logged and linked

## Hotfix and emergency path
Emergencies skip the timings, **not the gates**. Compress Gates 2 and 3 into one call, get the minimum approvals your policy allows, and always complete Gate 4. Review every emergency release in the next post-implementation review. Fewer emergencies over time is the goal.

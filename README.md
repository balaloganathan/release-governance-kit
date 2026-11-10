# Release Governance Kit

A lightweight set of templates for teams that need **more releases, fewer emergency releases and near-zero rollbacks** without slowing down.

It comes from leading a release-process redesign for a cash management business inside a large bank. That business had several value streams, shared engineers, limited non-production environments, a change advisory board (CAB) twice a week, and regulators paying attention. The templates are generic, and no client data or internal documents are included.

## Who this is for
- Release managers, Release Train Engineers and Scrum Masters
- Delivery leads who own production releases but don't control every team involved
- Teams moving from ad hoc releases to a predictable cadence

## What's in the kit
| File | Use it to… |
|---|---|
| [01-release-gates.md](01-release-gates.md) | Define what must be true before a change moves to the next stage |
| [02-release-raci.md](02-release-raci.md) | Make it clear who does what before, during and after a release |
| [03-go-no-go-checklist.md](03-go-no-go-checklist.md) | Run a short, honest go/no-go decision |
| [04-change-record-template.md](04-change-record-template.md) | Write a change record a CAB can approve on the first pass |
| [05-post-implementation-review.md](05-post-implementation-review.md) | Learn from each release without a blame session |

## How to adopt it
1. **Start with the gates.** Agree them with your SRE or operations team and your product owners, and adjust the timings to your release cadence.
2. **Fill in the RACI** with real names, not just roles. Gaps show up quickly.
3. **Use the change record template** for one release cycle, then trim whatever your CAB doesn't need.
4. **Hold a post-implementation review** after every major release, and after any release with an incident or rollback.
5. **Track four numbers monthly:** total releases, emergency releases, rollbacks, and releases deployed in business hours.

## What changed when we used this approach
Over six months: more releases overall, fewer emergency releases, deployments moved into business hours and weeknights, and near-zero rollbacks.

## Notes
- Written by Bala Loganathan, drafted with AI assistance and reviewed against real practice.
- Free to use and adapt. A link back is appreciated.

# Release RACI

**R** = Responsible (does the work) · **A** = Accountable (one person, owns the outcome) · **C** = Consulted · **I** = Informed

Replace roles with real names before you use it.

## Pre-release
| Activity | Release Manager / RTE | Product Owner | Dev Lead | QA Lead | SRE / Ops | Change / CAB | Business |
|---|---|---|---|---|---|---|---|
| Book release window and check the enterprise calendar | **A/R** | I | C | I | C | I | I |
| Map dependencies and resolve conflicts | **A/R** | C | R | I | C | C | I |
| Complete testing and attach evidence | C | I | R | **A/R** | I | I | I |
| Write implementation and rollback plans | C | I | **A/R** | C | R | I | I |
| Test the rollback | C | I | R | C | **A/R** | I | I |
| Plan business PVT | R | **A** | I | C | I | I | R |
| Prepare and submit the change record | **A/R** | I | C | C | C | I | I |
| Present at CAB | **A/R** | C | C | I | C | R | I |

## Release
| Activity | Release Manager / RTE | Product Owner | Dev Lead | QA Lead | SRE / Ops | Change / CAB | Business |
|---|---|---|---|---|---|---|---|
| Go/no-go decision | **A/R** | C | C | C | C | I | C |
| Execute deployment | I | I | R | I | **A/R** | I | I |
| Post-implementation verification (PIV) | I | I | R | C | **A/R** | I | I |
| Business PVT | I | **A** | I | C | I | I | R |
| Rollback decision, if needed | **A** | C | R | C | R | I | C |

## Post-release
| Activity | Release Manager / RTE | Product Owner | Dev Lead | QA Lead | SRE / Ops | Change / CAB | Business |
|---|---|---|---|---|---|---|---|
| Close the change record | **A/R** | I | I | I | C | I | I |
| Handle incidents from the deployment | **A** | C | R | C | R | I | I |
| Post-implementation review | **A/R** | C | C | C | C | I | C |
| Update monthly release metrics | **A/R** | I | I | I | I | I | I |

**Rule of thumb:** if a row has two A's or no A, fix it before the next release.

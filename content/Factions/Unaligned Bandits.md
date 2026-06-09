---
name: Unaligned Bandits
type: faction
disposition: hostile
status: active
first_encountered:
last_encountered:
sessions: []
locations: []
known_ranks: []
known_members: []
tags:
  - faction
---

# 

> [!infobox]
> # Unaligned Bandits
> ![[Art Assets/Portraits/Unaligned Bandits.png]]
> ###### Details
> | | |
> |---|---|
> | **Disposition** | `= this.disposition` |
> | **Status** | `= this.status` |
> | **First Encountered** | `= this.first_encountered` |
> | **Last Encountered** | `= this.last_encountered` |

## Overview
*What do we know about this faction? Goals, territory, reputation.*

## Known ranks
```dataview
TABLE disposition AS "Disposition", threat_level AS "Threat Level", times_encountered AS "Encountered"
FROM "path/to/your/notes"
WHERE type = "faction-rank" AND faction = [[Unaligned Bandits]]
SORT times_encountered DESC
```

## Known members
```dataview
TABLE rank AS "Rank", status AS "Status", known AS "IdentityKnown"
FROM "path/to/your/notes"
WHERE type = "npc" AND faction = [[Unaligned Bandits]]
SORT known DESC
```

## Encounter log
| Session | Location | Notes |
|---------|----------|-------|
| | | |

## Theories & rumours
*Things we've heard, things we suspect, things we're not sure about.*

## DM / Player notes
*Running thoughts, questions to follow up, connections to other factions.*
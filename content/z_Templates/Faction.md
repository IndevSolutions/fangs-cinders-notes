---
name: <% tp.file.title %>
type: faction
disposition: unknown
status: active
first_encountered: 
last_encountered: 
sessions: []
locations: []
known_ranks: []
known_members: []
tags: [faction]
---

---

> [!infobox]
> # <% tp.file.title %>
> ![[Art Assets/Sigils/<% tp.file.title %>.png]]
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
TABLE WITHOUT ID file.link AS "Rank", disposition AS "Disposition", threat_level AS "Threat Level", times_encountered AS "Encountered"
FROM "path/to/your/notes"
WHERE type = "faction-rank" AND faction = [[<% tp.file.title %>]]
SORT times_encountered DESC
```

## Known members
```dataview
TABLE WITHOUT ID file.link AS "Name", rank AS "Rank", status AS "Status", known AS "Identity Known"
FROM "path/to/your/notes"
WHERE type = "npc" AND faction = [[<% tp.file.title %>]]
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
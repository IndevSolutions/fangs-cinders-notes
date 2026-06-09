---
name: <% tp.file.title %>
type: faction-rank
faction: 
disposition: unknown
threat_level: unknown
times_encountered: 0
first_encountered: 
last_encountered: 
sessions: []
locations: []
tags: [faction-rank]
---

# 

> [!infobox]
> # <% tp.file.title %>
> ###### Details
> | | |
> |---|---|
> | **Faction** | `= this.faction` |
> | **Disposition** | `= this.disposition` |
> | **Threat Level** | `= this.threat_level` |
> | **Times Encountered** | `= this.times_encountered` |
> | **First Encountered** | `= this.first_encountered` |
> | **Last Encountered** | `= this.last_encountered` |

## Overview
*What is this rank/role within the faction? What do they do, what are they capable of?*

## Observed capabilities
*Abilities, tactics, equipment we've seen them use. Build this up over multiple encounters.*

## Known individuals
```dataview
TABLE status AS "Status", known AS "Identity Known", last_encountered AS "Last Seen"
FROM ""
WHERE type = "npc" AND rank = [[<% tp.file.title %>]]
SORT known DESC
```

## Encounter log
| Session | Location | Notes |
|---------|----------|-------|
| | | |

## Notes & theories
*Anything worth remembering about encounters with this rank.*
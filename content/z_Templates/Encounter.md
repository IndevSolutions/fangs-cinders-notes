---
name: <% tp.file.title %>
type: encounter
session: 
location: 
date: 
outcome: victory/defeat/fled/ongoing
ranks: []
npcs: []
tags: [encounter]
---

---

> [!infobox|block center]
> # <% tp.file.title %>
> ###### Details
> | | |
> |---|---|
> | **Session** | `= this.session` |
> | **Location** | `= this.location` |
> | **Date** | `= this.date` |
> | **Outcome** | `= this.outcome` |

## Ranks involved
```dataview
TABLE WITHOUT ID file.link AS "Rank", faction AS "Faction", disposition AS "Disposition", threat_level AS "Threat", times_encountered AS "Total Encounters"
FROM ""
WHERE type = "faction-rank" AND contains(this.ranks, file.link)
```

## NPCs involved
```dataview
TABLE faction AS "Faction", rank AS "Rank", status AS "Status", known AS "Identity Known"
FROM ""
WHERE type = "npc" AND contains(this.npcs, file.link)
```

## What happened
*Narrative summary of the encounter. What led to it, how it unfolded, how it ended.*

## Tactics observed
*Anything notable about how they fought, coordinated, or behaved.*

## Loot & consequences
*What we gained, what we lost, what changed.*

## Outstanding questions
*Things this encounter raised that we don't have answers to yet.*

---

```meta-bind-button
label: "⚔ Log Encounter — Update All Ranks"
id: log-encounter
style: primary
actions:
  - type: js
    file: "DM Layer/Scripts/logEncounter.js"
```
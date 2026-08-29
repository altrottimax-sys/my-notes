---
title: Recap of Sessions 5-10
draft: false
tags:
  -
---
<style>
.ms-page {
  color-scheme: light;
  --paper: #f3ead2;
  --paper-edge: #e2d3ab;
  --ink: #2b2013;
  --ink-dim: #5c5138;
  --link: #0645ad;
  --border: #b8a473;
  --header-bar: #a9824c;
  --header-bar-dark: #8a6a3c;
  --table-head: #e6d7ae;
  --accent: #7a2626;
  --accent-bright: #9c3a3a;
  --note-bg: #ede0bb;

  background: var(--paper) !important;
  color: var(--ink) !important;
  border: 1px solid var(--border);
  padding: 28px 32px 22px;
  font-family: 'Georgia', 'Cormorant Garamond', serif;
  line-height: 1.55;
  box-shadow: 0 2px 10px rgba(0,0,0,0.12);
}

.ms-page, .ms-page * {
  color: var(--ink) !important;
}

.ms-page a { color: var(--link) !important; text-decoration: none; border-bottom: 1px dotted var(--link); }
.ms-page a:hover { text-decoration: none; border-bottom-style: solid; }

.ms-page h2 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.25rem;
  letter-spacing: 1px;
  color: var(--accent) !important;
  border-bottom: 2px solid var(--border);
  padding-bottom: 4px;
  margin-top: 30px;
}

.ms-page h3 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1rem;
  letter-spacing: .5px;
  color: var(--ink-dim) !important;
  border-bottom: 1px solid var(--border);
  padding-bottom: 2px;
  margin-top: 22px;
}

.ms-page table {
  border-collapse: collapse;
  width: 100%;
  margin: 10px 0 18px;
  font-size: .95rem;
}
.ms-page th {
  background: var(--table-head) !important;
  border: 1px solid var(--border);
  padding: 5px 9px;
  text-align: left;
  font-family: 'Cinzel', serif;
  font-size: .72rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
}
.ms-page td {
  border: 1px solid var(--border);
  padding: 5px 9px;
}
.ms-page tr:nth-child(even) td { background: rgba(184,164,115,0.12) !important; }

.ms-page blockquote {
  border-left: 3px solid var(--accent);
  background: rgba(122,38,38,0.05) !important;
  margin: 12px 0;
  padding: 6px 16px;
  font-style: italic;
  color: var(--ink-dim) !important;
}

.ms-page ul, .ms-page ol { padding-left: 22px; }

.ms-page hr {
  border: none;
  border-top: 1px solid var(--border);
  margin: 26px 0;
}

.ms-notice {
  background: var(--note-bg) !important;
  border: 1px solid var(--border);
  border-left: 4px solid var(--header-bar);
  padding: 8px 14px;
  font-size: .85rem;
  color: var(--ink-dim) !important;
  margin-bottom: 20px;
}

/* ===== Session header plate ===== */
.session-plate {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  border-bottom: 1px solid var(--border);
  padding-bottom: 16px;
  margin-bottom: 24px;
}
.session-plate .sp-title h1 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.7rem;
  letter-spacing: 2px;
  margin: 0 0 4px;
  color: var(--accent) !important;
}
.session-plate .sp-sub {
  font-family: 'Cinzel', serif;
  font-size: .68rem;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
}
.session-plate .sp-number {
  font-family: 'Cinzel', serif;
  font-size: 2.2rem;
  color: var(--header-bar) !important;
  border: 2px solid var(--border);
  border-radius: 50%;
  width: 64px;
  height: 64px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  background: var(--table-head) !important;
}

/* ===== Session metadata bar ===== */
.session-meta {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1px;
  background: var(--border) !important;
  border: 1px solid var(--border);
  border-radius: 3px;
  overflow: hidden;
  margin-bottom: 22px;
}
.session-meta .meta-cell {
  background: #fbf5e3 !important;
  padding: 8px 10px;
  text-align: center;
}
.session-meta .meta-cell .m-label {
  font-family: 'Cinzel', serif;
  font-size: .55rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  display: block;
  margin-bottom: 2px;
}
.session-meta .meta-cell .m-value {
  font-size: .92rem;
  color: var(--ink) !important;
}

/* ===== Callout boxes (reused) ===== */
.ms-page blockquote.callout {
  border: 1px solid var(--border);
  border-left: 4px solid var(--header-bar-dark);
  background: #fbf5e3 !important;
  border-radius: 2px;
  padding: 0;
  margin: 14px 0 20px;
  font-style: normal;
  box-shadow: 0 1px 4px rgba(0,0,0,0.1);
}
.ms-page blockquote.callout .callout-title {
  display: flex;
  align-items: center;
  gap: 8px;
  background: linear-gradient(180deg, var(--table-head), var(--border)) !important;
  padding: 8px 14px;
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: .85rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  cursor: pointer;
}
.ms-page blockquote.callout .callout-title .callout-icon svg,
.ms-page blockquote.callout .callout-title .fold-callout-icon svg {
  fill: var(--accent) !important;
  stroke: var(--accent) !important;
  color: var(--accent) !important;
}
.ms-page blockquote.callout .callout-content {
  padding: 14px 16px 4px;
}
.ms-page blockquote.callout .callout-content table {
  margin: 0 0 10px;
}
.ms-page blockquote.callout p {
  font-style: normal;
}

/* GM-only callout — visually flagged as private */
.ms-page blockquote.callout[data-callout="warning"] {
  --color: #7a2626;
  --border: #7a2626;
  --bg: #f3e0e0;
  border-left-color: var(--accent) !important;
}
.ms-page blockquote.callout[data-callout="warning"] .callout-title {
  background: linear-gradient(180deg, var(--accent-bright), var(--accent)) !important;
  color: #fbf5e3 !important;
}

/* ===== Key Events timeline ===== */
.ms-timeline {
  position: relative;
  margin: 14px 0 22px;
  padding-left: 26px;
  border-left: 2px solid var(--border);
}
.timeline-entry {
  position: relative;
  margin-bottom: 16px;
}
.timeline-entry::before {
  content: "";
  position: absolute;
  left: -32px;
  top: 4px;
  width: 11px;
  height: 11px;
  border-radius: 50%;
  background: var(--header-bar) !important;
  border: 2px solid var(--paper);
  box-shadow: 0 0 0 1px var(--header-bar-dark);
}
.timeline-entry .te-title {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: .95rem;
  color: var(--accent) !important;
  margin-bottom: 2px;
}
.timeline-entry .te-body {
  font-size: .92rem;
  color: var(--ink) !important;
}

.ms-cat-footer {
  margin-top: 30px;
  padding-top: 10px;
  border-top: 1px solid var(--border);
  font-size: .78rem;
  color: var(--ink-dim) !important;
  background: var(--note-bg) !important;
}

@media (max-width: 700px) {
  .session-meta { grid-template-columns: 1fr; }
}
</style>

<div class="ms-page">

<div class="session-plate">
  <div class="sp-title">
    <h1>Title</h1>
    <div class="sp-sub">A Chronicle of The Tyranny of Dragons</div>
  </div>
  <div class="sp-number">1-5</div>
</div>

<div class="session-meta">
  <div class="meta-cell"><span class="m-label">In-Game Date</span><span class="m-value">—</span></div>
  <div class="meta-cell"><span class="m-label">Real-World Date</span><span class="m-value">—</span></div>
  <div class="meta-cell"><span class="m-label">Location</span><span class="m-value">—</span></div>
</div>

## Recap

Our group of adventurers started off by meeting in the Stonehill Inn in Phandalin, where they were promptly thrown out for causing a stir. These adventurers decided to move past their differences and form a group of their own and start completing the work assigned to the town notice board. 

The townmaster, Harbin Wester, set this adventuring group on quests to inform locals about the dragon that had recently moved into the region. At their first location they fought off a Manticore (after Petitearena was downed a few times and Elsaangra watched the whole thing) and secured a stable flow of healing potions from Adabra Gwynn.

The girls then set off to inform two dwarves about the dragon, and as they approached the excavation site, the dragon swooped in; but Zaenerys was able to convince it to leave by feeding it a rabbit. The girls helped out the dwarves clear the excavation site of slimes (petitearena again was reduced to 0hp a couple of times). That night while the girls slept, a group of assassins attempted to attack them, but they were able to fight them off. The head Assassin looked towards the group and mentioned "We will come back to get you"; but they couldn't distinguish who he had meant. 

The girls arrived back at Phandalin the next day and saw more notices were placed on the notice board; more quests. Before they set off again they checked out the local shrine of Phandalin, a shrine of luck. However, the priest was away on a trip so the girls investigated the priests house and found out she was a secret Harper who went to report back to HQ in the city of Neverwinter. 

The girls decided now was the time to take Don-Jon Raskin out to his Gold Mine, which they found was littered with bodies and some new tenants... Wererats!!!......... but they didn't really care or pick up on that so the Wererats sent them on a quest to clear out their old home, which was invaded by a local orc tribe! So the girls set out for the Shrine of the god of Divination, Savras. Cuntita tried to peacefully convince the Orcs to raid and inhibit the local innocent town of Conyberry, however relations quickly soured when the girls realised that this might not be for the good of the realm. Once the orcs were defeated, Zaenerys touched the altar and had a prophetic dream and the altar didn't work again that day, has this prophetic power been used up or may there be a way again to utilise it?!

When the girls returned to the Gold Mine, the wererats still wouldn't budge, so the girls did what they do best; They murdered all the men, women and children with improvised explosives. However, they saw that two little wererat children had run off into the wilds, and were not seen again. The girls then found their way to Butterskull ranch, where they would attempt to free Big Al Kalazorn from the hands of the Orc tribe. After a big long fight they completed their quest! Returning his prized cow Petunia as well!

Continuing on their journey, they came to Falcon's hunting lodge. He was the most charming, most beautiful man they had ever laid eyes on. He swooned and charmed them all night, thanks to that bottle of wine they brought. Here it was that the girls learned about the Neverwinter Civil War that had occurred years earlier. Just when things were winding down for the night, Elsaangra noticed clerics arriving from her home town of Saang, maybe their names would be El and Ra? Or Elsaang and Saangra? Either way they didn't seem to recognise Saang, and so luckily conflict was avoided. 

The girls then found themselves at the Loggers camp, which was suspiciously devoid of any and all loggers. They were soon beset upon by Ankhegs! and a boar that was actually an orc follower of Talos! again by fighting them all off they were able to secure the area and save Tibor Wester, brother of the Phandalin Townsmaster. The girls promptly left in the direction of Phandalin but ran into a walking piece of armour, which seemed to try and mimic their movements! They all saved a woman from a kobold and veeeeeery subtly demanded payment (they did the finger rubbing gesture). 

When the girls arrived back in Phandalin, they see it is surrounded in new camps of refugees and the displaced. Phandalin seems to be the last refuge for the area, and is teetering on the edge of destruction. Will the girls be able to save it? To be continued...

---

## Key Events

<div class="ms-timeline">

<div class="timeline-entry">
  <div class="te-title">Arrival at Greenest</div>
  <div class="te-body">The party crests the hill overlooking Greenest to find it under attack — a blue dragon circling overhead and raiders moving through the streets below.</div>
</div>

<div class="timeline-entry">
  <div class="te-title">The Mill</div>
  <div class="te-body">The party investigates the burning mill and rescues several townsfolk trapped inside before it collapses.</div>
</div>

<div class="timeline-entry">
  <div class="te-title">Reaching the Keep</div>
  <div class="te-body">Fighting through raiders in the streets, the party reaches Greenest Keep and reports to Governor Nighthill.</div>
</div>

<div class="timeline-entry">
  <div class="te-title">A Captive's Warning</div>
  <div class="te-body">A captured cultist reveals the raid is a diversion tied to something larger — the Cult of the Dragon is searching for something beneath the town.</div>
</div>

</div>

## NPCs Encountered

| Name | Role | Disposition | Notes |
|---|---|---|---|
| [[Governor Nighthill]] | Town Governor | Ally | Sheltering in the keep |
| [[Leosin Erlanthar]] | Harper Agent | Ally (captive) | Held by cultists, not yet rescued |
| — | Cult Raider | Hostile | Captured for questioning |

> [!note]- Loot &amp; Rewards
> | Item | Found By | Notes |
> |---|---|---|
> | | | |
> | | | |
>
> **Gold:** —

## Memorable Quotes

> "Insert a memorable line said at the table this session."
> — Character Name

> "Another one, if the table produced one."
> — Character Name

## Cliffhanger / Next Session

*Where the session ended and what the party is heading into next.*

## Trivia

- —

</div>
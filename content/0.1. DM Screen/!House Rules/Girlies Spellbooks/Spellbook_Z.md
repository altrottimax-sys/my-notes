---
title: Zaenerys' Spellbook
tags:
description:
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
  font-size: .92rem;
}
.ms-page th {
  background: var(--table-head) !important;
  border: 1px solid var(--border);
  padding: 5px 9px;
  text-align: left;
  font-family: 'Cinzel', serif;
  font-size: .68rem;
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

.ms-page ul { padding-left: 22px; }

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

/* ===== Spellbook header plate ===== */
.spell-plate {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  border-bottom: 1px solid var(--border);
  padding-bottom: 16px;
  margin-bottom: 22px;
}
.spell-plate .sp-title h1 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.7rem;
  letter-spacing: 2px;
  margin: 0 0 4px;
  color: var(--accent) !important;
}
.spell-plate .sp-sub {
  font-family: 'Cinzel', serif;
  font-size: .68rem;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
}
.spell-plate .sp-sigil {
  width: 58px; height: 58px;
  border-radius: 50%;
  flex-shrink: 0;
  background: radial-gradient(circle at 40% 35%, var(--header-bar), var(--header-bar-dark) 70%);
  box-shadow: 0 0 0 3px var(--paper), 0 0 0 4px var(--border);
  display: flex; align-items: center; justify-content: center;
  color: #fbf5e3 !important;
  font-size: 1.4rem;
}

/* ===== Caster stat bar ===== */
.caster-meta {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1px;
  background: var(--border) !important;
  border: 1px solid var(--border);
  border-radius: 3px;
  overflow: hidden;
  margin-bottom: 22px;
}
.caster-meta .meta-cell {
  background: #fbf5e3 !important;
  padding: 8px 10px;
  text-align: center;
}
.caster-meta .meta-cell .m-label {
  font-family: 'Cinzel', serif;
  font-size: .55rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  display: block;
  margin-bottom: 2px;
}
.caster-meta .meta-cell .m-value {
  font-family: 'Cinzel', serif;
  font-size: 1.05rem;
  color: var(--accent) !important;
}

/* ===== Spell Slot Tracker — 2-row grid: level/total header row, pips row below.
   Each pip-cell is its own 2-column mini-grid so pips wrap after every 2 —
   this is an inline break WITHIN the pip row, not a new tracker row. ===== */
.slot-grid {
  display: grid;
  grid-template-columns: repeat(9, 1fr);
  gap: 1px;
  background: var(--border) !important;
  border: 1px solid var(--border);
  border-radius: 3px;
  overflow: hidden;
  margin-bottom: 22px;
}
.slot-head-cell {
  background: var(--table-head) !important;
  text-align: center;
  padding: 6px 2px 5px;
}
.slot-head-cell .lvl {
  font-family: 'Cinzel', serif;
  font-size: .58rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
  display: block;
}
.slot-head-cell .tot {
  font-family: 'Cinzel', serif;
  font-size: .95rem;
  color: var(--accent) !important;
}
.slot-pip-cell {
  background: #fbf5e3 !important;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-content: center;
  gap: 5px 6px;
  padding: 8px 6px;
}
/* Pips beyond this level's current slot total — greyed and inert until leveled up */
.ms-page .prep-check.unused {
  opacity: .25;
  pointer-events: none;
  border-style: dashed;
}
/* Whole column dimmed when 0 slots at this level yet */
.slot-head-cell.inactive .lvl,
.slot-head-cell.inactive .tot {
  color: var(--ink-dim) !important;
  opacity: .5;
}
.slot-pip-cell.inactive { opacity: .4; }

/* ===== Callout boxes (Spell List summary tables) ===== */
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

/* Prepared checkbox column in level tables (also reused by the Spell Slot tracker) */
.ms-page .prep-check {
  position: static !important;
  margin: 0 !important;
  left: auto !important;
  top: auto !important;
  appearance: none;
  -webkit-appearance: none;
  width: 14px; height: 14px;
  border: 1.5px solid var(--header-bar-dark);
  border-radius: 50%;
  background: rgba(255,255,255,0.4);
  cursor: pointer;
}
.ms-page .prep-check:checked {
  background: var(--accent) !important;
  border-color: var(--accent) !important;
}

/* ===== Spell Details — native <details>/<summary> tiers =====
   Styled to match the gold callouts, with an explicit hint badge and
   hover feedback so the element clearly reads as clickable/expandable. */
.detail-tier {
  border: 1px solid var(--border);
  border-left: 4px solid var(--header-bar-dark);
  background: #fbf5e3 !important;
  border-radius: 2px;
  margin: 14px 0 20px;
  box-shadow: 0 1px 4px rgba(0,0,0,0.1);
  overflow: hidden;
}
.detail-tier summary {
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
  list-style: none;
  transition: background .12s ease;
}
.detail-tier summary::-webkit-details-marker { display: none; }
.detail-tier summary::before {
  content: "▸";
  color: var(--accent) !important;
  transition: transform .15s ease;
  flex-shrink: 0;
}
.detail-tier[open] summary::before { transform: rotate(90deg); }
.detail-tier summary:hover {
  background: linear-gradient(180deg, var(--border), var(--header-bar)) !important;
}
/* Explicit "clickable" affordance badge, right-aligned in the summary bar */
.detail-tier summary .tier-hint {
  margin-left: auto;
  font-family: 'Georgia', serif;
  font-size: .68rem;
  font-style: italic;
  letter-spacing: 0;
  text-transform: none;
  color: var(--ink-dim) !important;
  opacity: .8;
  white-space: nowrap;
}
.detail-tier summary .tier-hint::before { content: "click to "; }
.detail-tier[open] summary .tier-hint::before { content: "click to "; }
.detail-tier[open] summary .tier-hint::after { content: ""; }
.detail-tier:not([open]) summary .tier-hint::after { content: "expand"; }
.detail-tier[open] summary .tier-hint::after { content: "collapse"; }
.detail-tier .tier-content {
  padding: 14px 16px 4px;
}

/* ===== Individual spell detail card ===== */
.spell-card {
  border: 1px solid var(--border);
  border-radius: 3px;
  background: var(--paper) !important;
  margin-bottom: 16px;
  overflow: hidden;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}
.spell-card:last-child { margin-bottom: 4px; }
.spell-card .sc-head {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 10px;
  background: linear-gradient(180deg, var(--header-bar), var(--header-bar-dark)) !important;
  padding: 7px 14px;
}
.spell-card .sc-name {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1rem;
  color: #fbf5e3 !important;
}
.spell-card .sc-tag {
  font-size: .74rem;
  font-style: italic;
  color: #f1e3c0 !important;
}
.spell-card .sc-body {
  padding: 10px 16px 14px;
  font-size: .9rem;
}
.spell-card .sc-stats {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 6px;
  margin-bottom: 10px;
}
.spell-card .sc-stats .stat-box {
  text-align: center;
  border: 1px solid var(--border);
  border-radius: 3px;
  background: var(--table-head) !important;
  padding: 4px 3px;
}
.spell-card .sc-stats .stat-label {
  font-family: 'Cinzel', serif;
  font-size: .52rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  display: block;
}
.spell-card .sc-stats .stat-value {
  font-size: .8rem;
  color: var(--ink) !important;
}
.spell-card .sc-desc { margin-bottom: 6px; }
.spell-card .sc-higher {
  font-size: .85rem;
  font-style: italic;
  color: var(--ink-dim) !important;
  border-top: 1px dotted var(--border);
  padding-top: 6px;
  margin-top: 8px;
}

.ms-cat-footer {
  margin-top: 30px;
  padding-top: 10px;
  border-top: 1px solid var(--border);
  font-size: .78rem;
  color: var(--ink-dim) !important;
  background: var(--note-bg) !important;
}

@media (max-width: 900px) {
  .slot-grid { grid-template-columns: repeat(5, 1fr); }
}
@media (max-width: 560px) {
  .slot-grid { grid-template-columns: repeat(3, 1fr); }
}
@media (max-width: 700px) {
  .caster-meta { grid-template-columns: 1fr 1fr; }
  .spell-card .sc-stats { grid-template-columns: 1fr 1fr; }
  .detail-tier summary .tier-hint { display: none; }
}
</style>

<div class="ms-page">

<div class="spell-plate">
  <div class="sp-title">
    <h1>Zaenerys's Spellbook</h1>
    <div class="sp-sub">As the Dragonkin Curse corrupts and transforms her blood, Zaenerys' magical prowess grows.</div>
  </div>
  <div class="sp-sigil">ཐི༏ཋྀ</div>
</div>

<div class="caster-meta">
  <div class="meta-cell"><span class="m-label">Spellcasting Ability</span><span class="m-value">Wisdom</span></div>
  <div class="meta-cell"><span class="m-label">Spell Save DC</span><span class="m-value">14</span></div>
  <div class="meta-cell"><span class="m-label">Spell Attack Bonus</span><span class="m-value">+6</span></div>
  <div class="meta-cell"><span class="m-label">X</span><span class="m-value">X</span></div>
</div>

<div class="ms-notice">
Prepared spells are marked below with a filled circle. Spell slot totals and current expenditure are tracked in the panel below.
</div>

<div class="slot-grid">

  <div class="slot-head-cell"><span class="lvl">1st</span></div>
  <div class="slot-head-cell"><span class="lvl">2nd</span></div>
  <div class="slot-head-cell"><span class="lvl">3rd</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">4th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">5th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">6th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">7th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">8th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">9th</span></div>

  <div class="slot-pip-cell">
    <input type="checkbox" class="prep-check">
    <input type="checkbox" class="prep-check">
    <input type="checkbox" class="prep-check">
    <input type="checkbox" class="prep-check">
  </div>
  <div class="slot-pip-cell">
    <input type="checkbox" class="prep-check">
    <input type="checkbox" class="prep-check">
    <input type="checkbox" class="prep-check unused" disabled>
  </div>
  <div class="slot-pip-cell inactive">
    <input type="checkbox" class="prep-check unused" disabled>
    <input type="checkbox" class="prep-check unused" disabled>
    <input type="checkbox" class="prep-check unused" disabled>
  </div>
  <div class="slot-pip-cell inactive">
    <input type="checkbox" class="prep-check unused" disabled>
    <input type="checkbox" class="prep-check unused" disabled>
    <input type="checkbox" class="prep-check unused" disabled>
  </div>
  <div class="slot-pip-cell inactive">
    <input type="checkbox" class="prep-check unused" disabled>
    <input type="checkbox" class="prep-check unused" disabled>
    <input type="checkbox" class="prep-check unused" disabled>
  </div>
  <div class="slot-pip-cell inactive">
    <input type="checkbox" class="prep-check unused" disabled>
    <input type="checkbox" class="prep-check unused" disabled>
  </div>
  <div class="slot-pip-cell inactive">
    <input type="checkbox" class="prep-check unused" disabled>
    <input type="checkbox" class="prep-check unused" disabled>
  </div>
  <div class="slot-pip-cell inactive">
    <input type="checkbox" class="prep-check unused" disabled>
  </div>
  <div class="slot-pip-cell inactive">
    <input type="checkbox" class="prep-check unused" disabled>
  </div>

</div>

## Spell List

> [!note]- 1st Rank
> | Source | Spell | School | Casting Time | Range |
> |:---:|---|---|:---:|:---:|
> | Ranger | Hunter's Mark | Divination | 1 action | 24sq |
> | Ranger | Cure Wounds | Evocation | 1 action | 6sq |
> | Primal Awareness | Speak with Animals | Divination | 1 action or ritual | Self |


> [!note]- 2nd Rank
> | Source | Spell | School | Casting Time | Range |
> |:---:|---|---|:---:|:---:|
> | Ranger | Silence | Evocation | 1 action | 20sq |
> | Ranger | Pass Without Trace | Abjuration | 1 action | Self |
> | Primal Awareness | Beast Sense | Divination | 1 action or ritual | Touch |


## Spell Details

<details class="detail-tier">
<summary>1st Rank<span class="tier-hint"></span></summary>
<div class="tier-content">

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Hunter's Mark</div>
    <div class="sc-tag">1st-Rank Divination</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action, Alongside a Weapon Attack</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">24sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous, 10 Turns</span></div>
  </div>

  <div class="sc-desc">Choose an enemy you can see within range and mystically mark it as your quarry. Until the spell ends, you deal an extra 1d6 damage to the target whenever you hit it with a weapon attack. If the target drops to 0 hit points before the spell ends, you can use a bonus action on a subsequent turn of yours to mark a new enemy (the duration does not reset). Additionally you have advantage on any Perception or Survival checks you make to track your quarry for up to 2 hours. </div>

  <div class="sc-higher">When you cast this spell using a spell rank above 3rd-rank, you can maintain the duration for an additional 5 turns and tracking for 8 hours; when you cast this spell using a spell slot above 5th-rank you can maintain another additional 5 turns and tracking for 24 hours.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Cure Wounds</div>
    <div class="sc-tag">1st-Rank Evocation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">1 hour</span></div>
  </div>

  <div class="sc-desc">A creature you touch regains a number of hitpoints equal to 1d8+Wisdom Mod. This spell has no effect on undead or constructs.</div>

  <div class="sc-higher">When you cast this spell using a spell slot rank above 1st, the healing increases by 1d8 for each additional rank.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Speal With Animals</div>
    <div class="sc-tag">1st-Rank Divination (Ritual)</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">10 minutes</span></div>
  </div>

  <div class="sc-desc">You gain the ability to comprehend and verbally communicate with beasts for the duration. The knowledge and awareness of many beasts is limited by their intelligence, but at minimum, beasts can give you information about nearby locations and monsters, including whatever they have perceived within the past day. You might be able to persuade a small favour for you at the DM's Discretion.</div>

  </div>
</div>

</details>

<details class="detail-tier">
<summary>2nd Rank<span class="tier-hint"></span></summary>
<div class="tier-content">

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Silence</div>
    <div class="sc-tag">2nd-Rank Illusion (Ritual)</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">20sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 10 minutes</span></div>
  </div>

  <div class="sc-desc">For the duration, no sound can be created within or pass through a 4-square-radius sphere centred on a point you choose within range. Any creature or enemy entirely inside the sphere is immune to thunder damage, and creatures inside are deafened while entirely inside it. Casting a spell includes a verbal component is impossible inside the sphere.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Pass Without Trace</div>
    <div class="sc-tag">2nd-Rank Abjuration</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 1 hour</span></div>
  </div>

  <div class="sc-desc">A veil of shadows and silence radiates from you, masking you and your companions from detection. For the duration, each creature you choose within 6 squares of you (including you) has a +10 bonus to Stealth checks  and can't be tracked except by magical means. A creature that receives this bonus leaves behind no tracks or other traces of its passage.</div>
  
  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Beast Sense</div>
    <div class="sc-tag">2nd-Rank Divination</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 1 hour</span></div>
  </div>

  <div class="sc-desc">You touch willing beast. For the duration of the spell, you can use your action to see through the beast's eyes and hear what it hears, and continue to do so until you use your action to return to your normal senses.</div>

  </div>
</div>

</details>

## Spellcasting Focus

- **Spell Casting Focus:** Zaenerys' Scaley Hand

## Notes

*Homebrew rulings, spell combos discovered in play, or DM-approved variants specific to this character.*

## Trivia

- 

</div>


<div class="ms-cat-footer"> 
Categories: [[Characters]] · [[Spellbook]] · [[Tyranny of Dragons Campaign]]
</div>
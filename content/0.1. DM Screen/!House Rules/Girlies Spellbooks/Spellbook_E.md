---
title: Elsaangra's Spellbook
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
    <h1>Elsaangras's Spellbook</h1>
    <div class="sp-sub">As Elsaangra's devotion to Sehanine waxes, she feels imbued with the power of her holy magic. As it wanes her rogueish skills improve.</div>
  </div>
  <div class="sp-sigil">⏾</div>
</div>

<div class="caster-meta">
  <div class="meta-cell"><span class="m-label">Spellcasting Ability</span><span class="m-value">Charisma</span></div>
  <div class="meta-cell"><span class="m-label">Spell Save DC</span><span class="m-value">13</span></div>
  <div class="meta-cell"><span class="m-label">Spell Attack Bonus</span><span class="m-value">+5</span></div>
  <div class="meta-cell"><span class="m-label">Devotion Level</span><span class="m-value">Moonward Acolyte</span></div>
</div>

<div class="ms-notice">
Prepared spells are marked below with a filled circle. Spell slot totals and current expenditure are tracked in the panel below.
</div>

<div class="slot-grid">

  <div class="slot-head-cell inactive"><span class="lvl">1st</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">2nd</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">3rd</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">4th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">5th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">6th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">7th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">8th</span></div>
  <div class="slot-head-cell inactive"><span class="lvl">9th</span></div>

  <div class="slot-pip-cell">
    <input type="checkbox" class="prep-check">
    <input type="checkbox" class="prep-check">
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

> [!note]- Cantrips
> | Source | Spell | School | Casting Time | Range |
> |:---:|---|---|:---:|:---:|
> | High-Elf (Moon)| Ray of Frost | Evocation | 1 action | 12sq |
> | Moonward Acolyte | Guidance | X | 1 action | Touch |
> | Moonward Acolyte | Spare the Dying | Necromancy | 1 action | Touch |


> [!note]- 1st Level
> | Source | Spell | School | Casting Time | Range |
> |:---:|---|---|:---:|:---:|
> | Moonward Acolyte | Bane | Evocation | 1 action | 6sq |

## Spell Details

*Full descriptions for every spell in the Spell List above, organized by the same tiers. Click any tier bar to expand it.*

<details class="detail-tier">
<summary>Cantrips<span class="tier-hint"></span></summary>
<div class="tier-content">

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Ray of Frost</div>
    <div class="sc-tag">Evocation Cantrip</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">12sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">1 round</span></div>
  </div>

  <div class="sc-desc">A frigid beam of white-blue light streams toward an enemy. On a hit it takes 2d8 cold damage and its speed is reduced by 2sq until the start of your next turn.</div>

  <div class="sc-higher">This spell's damage increases by 1d8 when you reach 11th level (3d8), and 17th level (4d8).</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Guidance</div>
    <div class="sc-tag">Divination Cantrip</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, 1 minute</span></div>
  </div>

  <div class="sc-desc">You touch one willing creature. Once before the spell ends, the target can roll a d4 and add the number rolled to one ability check of its choice. It can only roll the dice before making the skill check, the spell then ends.</div>

  <div class="sc-higher">This spell cannot be use reactively (e.g. during a perception check to see a trap).</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Spare the Dying</div>
    <div class="sc-tag">Necromancy Cantrip</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">You touch a living creature that has 0 hit points. The creature becomes stable and can regain 2d4hp. This spell has no effect on undead or constructs.</div>

  <div class="sc-higher">This spell's healing increases by 1d4 when you reach 11th level (3d4), and 17th level (4d4).</div>

  </div>
</div>

</div>
</details>

<details class="detail-tier">
<summary>1st Level<span class="tier-hint"></span></summary>
<div class="tier-content">

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Bane</div>
    <div class="sc-tag">1st-Level Enchantment</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">6sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, 1 Minute</span></div>
  </div>

  <div class="sc-desc">Up to three enemies of your choice that you can see within range must make a Charisma saving throw. While under the effects of this spell, any target that  makes an attack roll or a saving throw will receive a -1d4 malus to their end result.</div>

  <div class="sc-higher">When you cast this spell using a spell slot above 1st, you may target one additional enemy for each additional level.</div>

  </div>
</div>

</details>


## Spellcasting Focus

- **Spell Casting Focus:** Religious Vestments of Sehanine 


## Notes

*Homebrew rulings, spell combos discovered in play, or DM-approved variants specific to this character.*

## Trivia

- 

</div>


<div class="ms-cat-footer"> 
Categories: [[Characters]] · [[Spellbook]] · [[Tyranny of Dragons Campaign]]
</div>
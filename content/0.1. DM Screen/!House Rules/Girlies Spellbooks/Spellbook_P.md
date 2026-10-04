---
title: Petitearena's Spellbook
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
    <h1>Petitearena's Spellbook</h1>
    <div class="sp-sub">The only legible writings found within the Oghma Infinium, pencilled by the wizard Petitearena Genesis herself.</div>
  </div>
  <div class="sp-sigil">🕮</div>
</div>

<div class="caster-meta">
  <div class="meta-cell"><span class="m-label">Spellcasting Ability</span><span class="m-value">Intelligence</span></div>
  <div class="meta-cell"><span class="m-label">Spell Save DC</span><span class="m-value">14</span></div>
  <div class="meta-cell"><span class="m-label">Spell Attack Bonus</span><span class="m-value">+6</span></div>
  <div class="meta-cell"><span class="m-label">Spells Preparation Limit</span><span class="m-value">8</span></div>
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
> | Prepared | Spell | School | Casting Time | Range |
> |:---:|---|---|:---:|:---:|
> | <input type="checkbox" class="prep-check" checked> | Chill Touch | Necromancy | 1 action | 24sq |
> | <input type="checkbox" class="prep-check" checked> | Mage Hand | Conjuration | 1 action | 6sq |
> | <input type="checkbox" class="prep-check" checked> | Shocking Grasp | Evocation | 1 action | Touch |
> | <input type="checkbox" class="prep-check" checked> | Thunderclap | Evocation | 1 action | 20sq |

> [!note]- 1st Rank
> | Prepared | Spell | School | Casting Time | Range |
> |:---:|---|---|:---:|:---:|
> | <input type="checkbox" class="prep-check" checked> | Burning Hands | Evocation | 1 action | Self (3-sq cone) |
> | <input type="checkbox" class="prep-check"> | Charm Person | Enchantment | 1 action | 6sq |
> | <input type="checkbox" class="prep-check"> | Comprehend Languages | Divination | 1 action | Self |
> | <input type="checkbox" class="prep-check" checked> | Detect Magic | Divination | 1 action | Self |
> | <input type="checkbox" class="prep-check"> | Identify | Divination | 1 minute | Touch |
> | <input type="checkbox" class="prep-check" checked> | Mage Armor | Abjuration | 1 action | Touch |
> | <input type="checkbox" class="prep-check" checked> | Magic Missile | Evocation | 1 action | 24sq ft |
> | <input type="checkbox" class="prep-check"> | Shield | Abjuration | 1 reaction | Self |
> | <input type="checkbox" class="prep-check" checked> | Sleep | Enchantment | 1 action | 18sq |

> [!note]- 2nd Rank
> | Prepared | Spell | School | Casting Time | Range |
> |:---:|---|---|:---:|:---:|
> | <input type="checkbox" class="prep-check"> | Blur | Illusion | 1 action | Self |
> | <input type="checkbox" class="prep-check" checked> | Hold Person | Enchantment | 1 action | 12sq |
> | <input type="checkbox" class="prep-check" checked> | Magic Weapon | Transmutation | 1 bonus action | Touch |
> | <input type="checkbox" class="prep-check"> | Spider Climb | Transmutation | 1 action | Touch |

> [!note]- 3rd Rank
> | Prepared | Spell | School | Casting Time | Range |
> |:---:|---|---|:---:|:---:|
> | <input type="checkbox" class="prep-check" checked> | Fireball | Evocation | 1 action | 30sq |
> | <input type="checkbox" class="prep-check"> | Lightning Bolt | Evocation | 1 action | Self (20sq line) |
> | <input type="checkbox" class="prep-check"> | Slow | Transmutation | 1 action | 24sq |
> | <input type="checkbox" class="prep-check"> | Tiny Servant | Transmutation | 1 minute | Touch |

---

## Spell Details

*Full descriptions for every spell in the Spell List above, organized by the same tiers. Click any tier bar to expand it.*

<details class="detail-tier">
<summary>Cantrips<span class="tier-hint"></span></summary>
<div class="tier-content">

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Chill Touch</div>
    <div class="sc-tag">Necromancy Cantrip</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">18sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">1 round</span></div>
  </div>

  <div class="sc-desc">You create a ghostly, skeletal hand in the space of a creature within range. Make a ranged spell attack against the creature to assail it with the chill of the grave. On a hit, the target takes 2d8 necrotic damage, and it can't regain hit points until the start of your next turn. If you hit an undead target, it also has disadvantage on attack rolls against you until the end of your next turn.</div>

  <div class="sc-higher">This spell's damage increases by 1d8 when you reach 11th level (3d8), and 17th level (4d8).</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Mage Hand</div>
    <div class="sc-tag">Conjuration Cantrip</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">6sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">1 minute</span></div>
  </div>

  <div class="sc-desc">A spectral, floating hand appears at a point you choose within range. It can manipulate an object, open an unlocked door or container, stow or retrieve an item, or pour the contents of a vial. You can move the hand up to 6sq each time you use it. The hand can't attack, activate magic items, or carry more than 10 units/brambleplinths.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Shocking Grasp</div>
    <div class="sc-tag">Evocation Cantrip</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">Lightning springs from your hand to deliver a shock to a creature you try to touch. Make a melee spell attack against the target — you have advantage if the target is wearing armour made of metal. On a hit, the target takes 2d8 lightning damage and can't take reactions until the start of its next turn.</div>

  <div class="sc-higher">This spell's damage increases by 1d8 when you reach 11th level (3d8), and 17th level (4d8).</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Thunderclap</div>
    <div class="sc-tag">Evocation Cantrip</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self (20sq cube)</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">You create a burst of thunderous sound, which can be heard 20 squares away. Each creature within range, other than you, must make a Constitution saving throw or take 2d6 thunder damage..</div>

  <div class="sc-higher">This spell's damage increases by 1d6 when you reach 11th level (3d6), and 17th level (4d6).</div>

  </div>
</div>

</div>
</details>

<details class="detail-tier">
<summary>1st Rank<span class="tier-hint"></span></summary>
<div class="tier-content">

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Burning Hands</div>
    <div class="sc-tag">1st-Rank Evocation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self (3sq cone)</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">A thin sheet of flame shoots forth from your outstretched fingertips. Each creature in a 3-square cone must make a Dexterity saving throw, taking 3d6 fire damage on a failed save, or half as much on a success. The fire ignites any flammable objects in the area not being worn or carried.</div>

  <div class="sc-higher">When you cast this spell using a spell slot above 1st, the damage increases by 1d6 for each additional slot rank.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Charm Person</div>
    <div class="sc-tag">1st-Rank Enchantment</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">6sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">1 hour</span></div>
  </div>

  <div class="sc-desc">You attempt to charm a humanoid you can see within range. It must make a Wisdom saving throw, and does so with advantage if you or your companions are fighting it. On a failed save, it is charmed by you until the spell ends or until you or your companions do anything harmful to it. When the spell ends, the creature knows it was charmed.</div>

  <div class="sc-higher">When you cast this spell using a spell slot rank above 1st, you can target one additional creature for each additional slot rank, as long as the targets are within 6 squares of each other.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Comprehend Languages</div>
    <div class="sc-tag">1st-Rank Divination (Ritual)</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">1 hour</span></div>
  </div>

  <div class="sc-desc">For the duration, you understand the literal meaning of any spoken language you hear, and any written language you see, though you must be touching the surface it's written on. This doesn't decode secret messages, and it doesn't grant a general understanding of context or subtext.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Detect Magic</div>
    <div class="sc-tag">1st-Rank Divination (Ritual)</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 10 minutes</span></div>
  </div>

  <div class="sc-desc">For the duration, you sense the presence of magic within 6 squares. If you sense magic, you can use your action to see a faint aura around any visible creature or object that bears it, revealing its school of magic if it's not blocked by lead or a thick wall of wood or dirt.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Identify</div>
    <div class="sc-tag">1st-Rank Divination (Ritual)</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 minute</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">You choose one object you touch throughout the casting. If it's a magic item, you learn its properties, how to use them, whether it requires attunement, and how many charges it has. You learn whether any spells are affecting the item, and if it was created by a spell, which one.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Mage Armor</div>
    <div class="sc-tag">1st-Rank Abjuration</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">8 hours</span></div>
  </div>

  <div class="sc-desc">You touch a willing creature who isn't wearing armor, and a protective magical force surrounds it until the spell ends. The target's base AC becomes 13 + its Dexterity modifier. The spell ends early if the target dons armor or if you dismiss it as an action.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Magic Missile (Bang Bang)</div>
    <div class="sc-tag">1st-Rank Evocation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">18sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">You create three glowing darts of magical force. Each dart hits a creature of your choice that you can see within range. A dart deals 1d4+1 force damage to its target. The darts all strike simultaneously, and you can direct them to hit one creature or several.</div>

  <div class="sc-higher">When you cast this spell using a spell slot rank above 1st, the spell creates one more dart for each additional slot rank.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Shield</div>
    <div class="sc-tag">1st-Rank Abjuration</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 reaction</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">1 round</span></div>
  </div>

  <div class="sc-desc">An invisible barrier of magical force appears and protects you. Until the start of your next turn, you have a +5 bonus to AC, including against the triggering attack, and you take no damage from Magic Missile.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Sleep</div>
    <div class="sc-tag">1st-Rank Enchantment</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">18sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">1 minute</span></div>
  </div>

  <div class="sc-desc">This spell sends creatures into a magical slumber. Roll 5d8; the total is how many hit points of creatures this spell can affect. Creatures within a 4-square-radius sphere are affected in ascending order of current hit points, starting with the lowest. Affected creatures fall unconscious until the spell ends, they take damage, or someone uses an action to shake or slap them awake.</div>

  <div class="sc-higher">When you cast this spell using a spell slot rank above 1st, roll an additional 2d8 for each additional slot rank.</div>

  </div>
</div>

</div>
</details>

<details class="detail-tier">
<summary>2nd Rank<span class="tier-hint"></span></summary>
<div class="tier-content">

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Blur</div>
    <div class="sc-tag">2nd-Rank Illusion</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 1 minute</span></div>
  </div>

  <div class="sc-desc">Your body becomes blurred, shifting and wavering to all who can see you. For the duration, any creature attacking you has disadvantage on its attack roll. An attacker is immune if it doesn't rely on sight or can see through illusions.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Hold Person</div>
    <div class="sc-tag">2nd-Rank Enchantment</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">12sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 1 minute</span></div>
  </div>

  <div class="sc-desc">Choose a humanoid you can see within range. The target must succeed on a Wisdom saving throw or be paralyzed for the duration. At the end of each of its turns, the target can repeat the saving throw, ending the effect on itself on a success.</div>

  <div class="sc-higher">When you cast this spell using a spell slot rank above 2nd, you can target one additional humanoid for each additional slot rank, as long as the targets are within 6 squares of each other.</div>
  
  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Magic Weapon</div>
    <div class="sc-tag">2nd-Rank Transmutation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 bonus action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 1 hour</span></div>
  </div>

  <div class="sc-desc">You touch a nonmagical weapon. Until the spell ends, that weapon becomes a magic weapon with a +1 bonus to attack and damage rolls.</div>

  <div class="sc-higher">When you cast this spell using a spell slot rank of 4th or higher, the bonus increases to +2. Using a spell slot rank of 6th or higher, the bonus increases to +3.</div> 

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Spider Climb</div>
    <div class="sc-tag">2nd-Rank Transmutation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 1 hour</span></div>
  </div>

  <div class="sc-desc">Until the spell ends, one willing creature you touch gains the ability to move up, down, and across vertical surfaces and upside down along ceilings, leaving its hands free. The target also gains a climbing speed equal to its walking speed.</div>

  </div>
</div>

</div>
</details>

<details class="detail-tier">
<summary>3rd Rank<span class="tier-hint"></span></summary>
<div class="tier-content">

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Fireball</div>
    <div class="sc-tag">3rd-Rank Evocation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">30sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">A bright streak flashes to a point you choose within range, then blossoms with a low roar into an explosion of flame. Each creature in a 4 square-radius sphere must make a Dexterity saving throw, taking 8d6 fire damage on a failed save, or half as much on a success. Flammable objects in the area that aren't being worn or carried begin burning.</div>

  <div class="sc-higher">When you cast this spell using a spell slot rank above 3rd, the damage increases by 1d6 for each slot.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Lightning Bolt</div>
    <div class="sc-tag">3rd-Rank Evocation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Self (20sq line)</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">A stroke of lightning forming a line 20 squares long and 1 square wide blasts out from you in a direction you choose. Each creature in the line must make a Dexterity saving throw, taking 8d6 lightning damage on a failed save, or half as much on a success. The lightning ignites flammable objects in the area not being worn or carried.</div>

  <div class="sc-higher">When you cast this spell using a spell slot rank above 3rd, the damage increases by 1d6 for each slot.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Slow</div>
    <div class="sc-tag">3rd-Rank Transmutation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">24sq</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Concentration, up to 1 minute</span></div>
  </div>

  <div class="sc-desc">You alter time around up to six creatures of your choice in a 8 square cube within range. Each target must make a Wisdom saving throw. On a failed save, a target's speed is halved, it takes a -2 penalty to AC and Dexterity saves, and it can't use reactions, and on its turn it can take either an action or a bonus action, not both. At the end of each of its turns, an affected target can repeat the save, ending the effect on itself on a success.</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Tiny Servant</div>
    <div class="sc-tag">3rd-Rank Transmutation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 minute</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">Touch</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S, M</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">8 hours</span></div>
  </div>

  <div class="sc-desc">You animate up to two tiny, nonmagical objects, transforming each into a tiny servant that obeys your spoken commands. The servant moves as you direct it, can perform simple tasks (fetching, opening unstuck doors, carrying small items), and has statistics matching an ordinary tiny animated object, but can't attack.</div>

  <div class="sc-higher">You can animate one additional object for every 2 spell slot ranks above 3rd.</div>

  </div>
</div>

</div>
</details>

## Spellcasting Focus &amp; Materials

- **Spell Casting Focus:** Petitarena's Quarterstaff &amp; the Oghma Infinium
- **Material Components Pouch:** 5x Silver Dust | 1x Diamond Crystals | 1x Sulfur | 

## Notes

*Homebrew rulings, spell combos discovered in play, or DM-approved variants specific to this character.*

## Trivia

- She loves to use finger guns for her Magic Missiles

</div>


<div class="ms-cat-footer"> 
Categories: [[Characters]] · [[Spellbook]] · [[Tyranny of Dragons Campaign]]
</div>
---
title: Petitearena's — Spellbook
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

/* ===== Callout boxes (reused base, one per spell level) ===== */
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

/* ===== Individual spell detail card ===== */
.spell-card {
  border: 1px solid var(--border);
  border-radius: 3px;
  background: #fbf5e3 !important;
  margin-bottom: 16px;
  overflow: hidden;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
}
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

/* Prepared checkbox column in level tables */
.ms-page .prep-check {
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

.ms-cat-footer {
  margin-top: 30px;
  padding-top: 10px;
  border-top: 1px solid var(--border);
  font-size: .78rem;
  color: var(--ink-dim) !important;
  background: var(--note-bg) !important;
}

@media (max-width: 700px) {
  .caster-meta { grid-template-columns: 1fr 1fr; }
  .spell-card .sc-stats { grid-template-columns: 1fr 1fr; }
}
</style>

<div class="ms-page">

<div class="spell-plate">
  <div class="sp-title">
    <h1>Character Name's Spellbook</h1>
    <div class="sp-sub">A Record of Arcane &amp; Divine Workings</div>
  </div>
  <div class="sp-sigil">✦</div>
</div>

<div class="caster-meta">
  <div class="meta-cell"><span class="m-label">Class</span><span class="m-value">Wizard</span></div>
  <div class="meta-cell"><span class="m-label">Spellcasting Ability</span><span class="m-value">Intelligence</span></div>
  <div class="meta-cell"><span class="m-label">Spell Save DC</span><span class="m-value">13</span></div>
  <div class="meta-cell"><span class="m-label">Spell Attack Bonus</span><span class="m-value">+5</span></div>
</div>

<div class="ms-notice">
Prepared spells are marked below with a filled circle. Spell slot totals and current expenditure are tracked on the [[Character Sheet]].
</div>

## Spell List

> [!note]- Cantrips (At-Will)
> | Prepared | Spell | School | Casting Time | Range | Duration |
> |:---:|---|---|:---:|:---:|:---:|
> | <input type="checkbox" class="prep-check" checked> | Fire Bolt | Evocation | 1 action | 120 ft | Instantaneous |
> | <input type="checkbox" class="prep-check" checked> | Mage Hand | Conjuration | 1 action | 30 ft | 1 minute |
> | <input type="checkbox" class="prep-check"> | Prestidigitation | Transmutation | 1 action | 10 ft | Up to 1 hour |

> [!note]- 1st Level
> | Prepared | Spell | School | Casting Time | Range | Duration |
> |:---:|---|---|:---:|:---:|:---:|
> | <input type="checkbox" class="prep-check" checked> | Magic Missile | Evocation | 1 action | 120 ft | Instantaneous |
> | <input type="checkbox" class="prep-check" checked> | Shield | Abjuration | 1 reaction | Self | 1 round |
> | <input type="checkbox" class="prep-check"> | Detect Magic | Divination | 1 action | Self | Concentration, up to 10 minutes |

> [!note]- 2nd Level
> | Prepared | Spell | School | Casting Time | Range | Duration |
> |:---:|---|---|:---:|:---:|:---:|
> | <input type="checkbox" class="prep-check"> | Misty Step | Conjuration | 1 bonus action | Self | Instantaneous |
> | <input type="checkbox" class="prep-check"> | Scorching Ray | Evocation | 1 action | 120 ft | Instantaneous |

> [!note]- 3rd Level
> | Prepared | Spell | School | Casting Time | Range | Duration |
> |:---:|---|---|:---:|:---:|:---:|
> | <input type="checkbox" class="prep-check"> | Fireball | Evocation | 1 action | 150 ft | Instantaneous |
> | <input type="checkbox" class="prep-check"> | Counterspell | Abjuration | 1 reaction | 60 ft | Instantaneous |

---

## Spell Details

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Fire Bolt</div>
    <div class="sc-tag">Evocation Cantrip</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">120 ft</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">You hurl a mote of fire at a creature or object within range. Make a ranged spell attack against the target. On a hit, the target takes 1d10 fire damage. A flammable object hit by this spell ignites if it isn't being worn or carried.</div>

  <div class="sc-higher">This spell's damage increases by 1d10 when you reach 5th level (2d10), 11th level (3d10), and 17th level (4d10).</div>

  </div>
</div>

<div class="spell-card">
  <div class="sc-head">
    <div class="sc-name">Magic Missile</div>
    <div class="sc-tag">1st-Level Evocation</div>
  </div>
  <div class="sc-body">

  <div class="sc-stats">
    <div class="stat-box"><span class="stat-label">Casting Time</span><span class="stat-value">1 action</span></div>
    <div class="stat-box"><span class="stat-label">Range</span><span class="stat-value">120 ft</span></div>
    <div class="stat-box"><span class="stat-label">Components</span><span class="stat-value">V, S</span></div>
    <div class="stat-box"><span class="stat-label">Duration</span><span class="stat-value">Instantaneous</span></div>
  </div>

  <div class="sc-desc">You create three glowing darts of magical force. Each dart hits a creature of your choice that you can see within range. A dart deals 1d4+1 force damage to its target. The darts all strike simultaneously, and you can direct them to hit one creature or several.</div>

  <div class="sc-higher">When you cast this spell using a spell slot of 2nd level or higher, the spell creates one more dart for each slot level above 1st.</div>

  </div>
</div>

## Spellcasting Focus &amp; Materials

- **Spell Casting Focus:** Petitarena's Quarterstaff &amp; the Oghma Infinium
- **Material Components Pouch:** 5x Silver Dust | 1x Diamond Dust |

## Notes

*Homebrew rulings, spell combos discovered in play, or DM-approved variants specific to this character.*

## Trivia

- She loves to use finger guns for her Magic Missiles

</div>

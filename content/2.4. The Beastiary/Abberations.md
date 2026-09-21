---
title: Abberations
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

/* ===== Bestiary scroll gallery ===== */
.ms-bestiary {
  display: flex;
  flex-direction: column;
  gap: 26px;
  margin: 20px 0;
}

/* ===== Individual stat-block card ===== */
.ms-statblock {
  border: 1px solid var(--border);
  border-radius: 4px;
  background: #fbf5e3 !important;
  box-shadow: 0 3px 10px rgba(0,0,0,0.18);
  overflow: hidden;
}

.sb-header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 14px;
  background: linear-gradient(180deg, var(--header-bar), var(--header-bar-dark)) !important;
  padding: 10px 18px;
}
.sb-header .sb-name {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.15rem;
  letter-spacing: 1px;
  color: #fbf5e3 !important;
  margin: 0;
}
.sb-header .sb-type {
  font-size: .8rem;
  font-style: italic;
  color: #f1e3c0 !important;
}
.sb-header .sb-badges {
  display: flex;
  gap: 8px;
  flex-shrink: 0;
}
.sb-header .sb-cr,
.sb-header .sb-prof,
.sb-header .sb-perc {
  font-family: 'Cinzel', serif;
  font-size: .72rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: #fbf5e3 !important;
  border: 1px solid rgba(251,245,227,0.6);
  border-radius: 12px;
  padding: 3px 10px;
  white-space: nowrap;
}

.sb-body {
  padding: 14px 20px 18px;
  display: flex;
  gap: 18px;
  align-items: flex-start;
}

/* Left column: portrait + ability scores + senses/languages table, all locked to 240px */
.sb-portrait-col {
  flex-shrink: 0;
  width: 240px;
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.sb-main { flex: 1; min-width: 0; }

/* Portrait frame — fixed 240x240px, whatever the source image's native size */
.sb-portrait {
  width: 240px;
  height: 240px;
  border: 1px solid var(--border);
  border-radius: 3px;
  overflow: hidden;
  background: var(--ink);
  box-shadow: inset 0 0 0 1px rgba(251,245,227,0.3);
  line-height: 0;
}

.sb-portrait p {
  margin: 0;
  height: 100%;
}

.sb-portrait img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center center;
  margin: 0;
}

/* Empty-state placeholder shown when no <img> is present */
.sb-portrait:empty::after {
  content: "No Image";
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  font-family: 'Cinzel', serif;
  font-size: .7rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  background: var(--table-head) !important;
}

/* Ability scores — sit beneath the portrait, sized to its 240px column */
.sb-abilities {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 5px;
  width: 100%;
}
.sb-abilities .ab-box {
  border: 1px solid var(--border);
  border-radius: 3px;
  background: var(--table-head) !important;
  text-align: center;
  padding: 5px 2px;
}
.sb-abilities .ab-name {
  font-family: 'Cinzel', serif;
  font-size: .58rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  display: block;
}
.sb-abilities .ab-score {
  font-family: 'Cinzel', serif;
  font-size: .92rem;
  color: var(--ink) !important;
}
.sb-abilities .ab-mod {
  font-size: .72rem;
  color: var(--ink-dim) !important;
}

/* Senses/Languages mini-table — sits below the ability grid, same 240px width */
.sb-portrait-col table {
  width: 100%;
  margin: 0;
  font-size: .74rem;
  border: 1px solid var(--border);
  border-radius: 3px;
  overflow: hidden;
}
.sb-portrait-col th {
  width: 38%;
  font-size: .58rem;
  padding: 4px 6px;
  white-space: nowrap;
}
.sb-portrait-col td {
  padding: 4px 6px;
}

.sb-quickstats {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 8px;
  margin-bottom: 12px;
}
.sb-quickstats .qs-box {
  border: 1px solid var(--border);
  border-radius: 3px;
  background: var(--table-head) !important;
  text-align: center;
  padding: 6px 4px;
}
.sb-quickstats .qs-label {
  font-family: 'Cinzel', serif;
  font-size: .58rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  display: block;
}
.sb-quickstats .qs-value {
  font-family: 'Cinzel', serif;
  font-size: 1rem;
  color: var(--accent) !important;
}

.sb-main hr {
  border: none;
  border-top: 1px solid var(--border);
  margin: 12px 0;
}

/* Description — sits between Quick Stats and Features */
.sb-description {
  font-size: .92rem;
  font-style: italic;
  color: var(--ink-dim) !important;
  border-left: 3px solid var(--border);
  padding: 4px 12px;
  margin: 4px 0 14px;
}

.sb-section-title {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: .82rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--accent) !important;
  border-bottom: 1px solid var(--border);
  padding-bottom: 3px;
  margin: 14px 0 6px;
}

.sb-feature {
  margin-bottom: 8px;
  font-size: .92rem;
}
.sb-feature .feat-name {
  font-weight: 700;
  font-style: italic;
  color: var(--accent-bright) !important;
}

@media (max-width: 640px) {
  .sb-body { flex-direction: column; }
  .sb-portrait-col { width: 100%; }
  .sb-portrait { width: 100%; height: 240px; }
}

@media (max-width: 480px) {
  .sb-header { flex-wrap: wrap; }
  .sb-badges { flex-wrap: wrap; }
}
</style>

<div class="ms-page">

<div class="ms-notice">
This page catalogues enemy abberations encountered on the Sword Coast. Scroll down to browse further entries.
</div>

## Bestiary

<div class="ms-bestiary">

<div class="ms-statblock">
  <div class="sb-header">
    <div>
      <div class="sb-name">Badger</div>
      <div class="sb-type">Small beast</div>
    </div>
    <div class="sb-badges">
      <div class="sb-cr">CR 0</div>
      <div class="sb-prof">Proficiency +2</div>
      <div class="sb-perc">Perception 11</div>
    </div>
  </div>
  <div class="sb-body">

  <div class="sb-portrait-col">

  <div class="sb-portrait">
    <img src="badger.jpeg" alt="Badger">
  </div>

  <div class="sb-abilities">
    <div class="ab-box"><span class="ab-name">Str</span><span class="ab-score">4</span> <span class="ab-mod">(-3)</span></div>
    <div class="ab-box"><span class="ab-name">Dex</span><span class="ab-score">11</span> <span class="ab-mod">(+0)</span></div>
    <div class="ab-box"><span class="ab-name">Con</span><span class="ab-score">12</span> <span class="ab-mod">(+1)</span></div>
    <div class="ab-box"><span class="ab-name">Int</span><span class="ab-score">2</span> <span class="ab-mod">(-4)</span></div>
    <div class="ab-box"><span class="ab-name">Wis</span><span class="ab-score">12</span> <span class="ab-mod">(+1)</span></div>
    <div class="ab-box"><span class="ab-name">Cha</span><span class="ab-score">5</span> <span class="ab-mod">(-3)</span></div>
  </div>

  <table>
    <tr><th>Senses</th><td>Darkvision 6sq</td></tr>
    <tr><th>Languages</th><td>Animal</td></tr>
  </table>

  </div>

  <div class="sb-main">

  <div class="sb-quickstats">
    <div class="qs-box"><span class="qs-label">Armour Class</span><span class="qs-value">10</span></div>
    <div class="qs-box"><span class="qs-label">Hit Points</span><span class="qs-value">3 (1d4+1)</span></div>
    <div class="qs-box"><span class="qs-label">Speed</span><span class="qs-value">3sq, burrow 1sq</span></div>
    <div class="qs-box"><span class="qs-label">Initiative</span><span class="qs-value">+0</span></div>
  </div>

  <div class="sb-description">A stout, low-slung burrower with a striped face, more often heard snuffling through undergrowth than seen. Placid unless cornered, at which point its claws and temper are surprisingly sharp.</div>

  <div class="sb-section-title">Features</div>
  <div class="sb-feature"><span class="feat-name">Keen Smell:</span> The badger has advantage on Wisdom (Perception) checks that rely on scent.</div>

  <div class="sb-section-title">Actions</div>
  <div class="sb-feature"><span class="feat-name">Bite:</span> Melee Weapon Attack | +2 to hit, reach 5 ft, one target | Hit: 1 piercing damage.</div>

  </div>
  </div>
</div>

<div class="ms-statblock">
  <div class="sb-header">
    <div>
      <div class="sb-name">Boar</div>
      <div class="sb-type">Medium beast</div>
    </div>
    <div class="sb-badges">
      <div class="sb-cr">CR 1/4</div>
      <div class="sb-prof">Proficiency +2</div>
      <div class="sb-perc">Perception 9</div>
    </div>
  </div>
  <div class="sb-body">

  <div class="sb-portrait-col">

  <div class="sb-portrait">
    <img src="boar.jpeg" alt="Boar">
  </div>

  <div class="sb-abilities">
    <div class="ab-box"><span class="ab-name">Str</span><span class="ab-score">13</span> <span class="ab-mod">(+1)</span></div>
    <div class="ab-box"><span class="ab-name">Dex</span><span class="ab-score">11</span> <span class="ab-mod">(+0)</span></div>
    <div class="ab-box"><span class="ab-name">Con</span><span class="ab-score">12</span> <span class="ab-mod">(+1)</span></div>
    <div class="ab-box"><span class="ab-name">Int</span><span class="ab-score">2</span> <span class="ab-mod">(-4)</span></div>
    <div class="ab-box"><span class="ab-name">Wis</span><span class="ab-score">9</span> <span class="ab-mod">(-1)</span></div>
    <div class="ab-box"><span class="ab-name">Cha</span><span class="ab-score">5</span> <span class="ab-mod">(-3)</span></div>
  </div>

  <table>
    <tr><th>Senses</th><td>—</td></tr>
    <tr><th>Languages</th><td>Animal</td></tr>
  </table>

  </div>

  <div class="sb-main">

  <div class="sb-quickstats">
    <div class="qs-box"><span class="qs-label">Armour Class</span><span class="qs-value">11</span></div>
    <div class="qs-box"><span class="qs-label">Hit Points</span><span class="qs-value">11 (2d8+2)</span></div>
    <div class="qs-box"><span class="qs-label">Speed</span><span class="qs-value">8sq</span></div>
    <div class="qs-box"><span class="qs-label">Initiative</span><span class="qs-value">+0</span></div>
  </div>

  <div class="sb-description">A bristling, low-tempered tusker that roots through forest floor and farmland alike. Slow to provoke but relentless once charging — travelers know to give a lowered head a wide berth.</div>

  <div class="sb-section-title">Features</div>
  <div class="sb-feature"><span class="feat-name">Charge:</span> If the boar moves at least 10 feet straight toward a target and then hits it with a tusk attack on the same turn, the target takes an extra 3 (1d6) piercing damage. If the target is a creature, it must succeed on a DC 11 Strength saving throw or be knocked prone.</div>
  <div class="sb-feature"><span class="feat-name">Relentless (Recharges after a Short or Long Rest):</span> If the boar takes 7 damage or less that would reduce it to 0 hit points, it is instead reduced to 1 hit point.</div>

  <div class="sb-section-title">Actions</div>
  <div class="sb-feature"><span class="feat-name">Tusk:</span> Melee Weapon Attack | +3 to hit, reach 5 ft, one target | Hit: 4 (1d6+1) slashing damage.</div>

  </div>
  </div>
</div>

</div>

</div>
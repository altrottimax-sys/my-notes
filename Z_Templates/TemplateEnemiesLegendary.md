---
title: <%tp.file.title%>
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
.sb-header .sb-cr {
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

.sb-main { flex: 1; min-width: 0; }

/* Portrait frame — fixed 240x240px, whatever the source image's native size */
.sb-portrait {
  flex-shrink: 0;
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
  display: block; width: 100%; 
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

.sb-abilities {
  display: grid;
  grid-template-columns: repeat(6, 1fr);
  gap: 6px;
  margin-bottom: 12px;
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

.sb-meta {
  font-size: .85rem;
  margin-bottom: 4px;
}
.sb-meta .meta-label {
  font-family: 'Cinzel', serif;
  font-size: .68rem;
  letter-spacing: 1px;
  text-transform: uppercase;
  color: var(--accent) !important;
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
  .sb-portrait { width: 100%; height: 240px; }
}

/* ===== Legendary variant ===== */
.ms-statblock.legendary {
  border: 2px solid var(--accent);
  box-shadow: 0 0 0 1px var(--header-bar-dark), 0 4px 16px rgba(122,38,38,0.35);
}
.ms-statblock.legendary .sb-header {
  background: linear-gradient(180deg, var(--accent-bright), var(--accent)) !important;
}
.ms-statblock.legendary .sb-header .sb-type,
.ms-statblock.legendary .sb-header .sb-name { color: #fbf5e3 !important; }
.ms-statblock.legendary .sb-cr {
  background: rgba(0,0,0,0.2) !important;
  border-color: #fbf5e3 !important;
}
.ms-statblock.legendary .sb-portrait {
  width: 280px;
  height: 280px;
}
.ms-statblock.legendary .sb-section-title.legendary-title {
  color: var(--accent-bright) !important;
  border-bottom: 2px solid var(--accent);
}
.ms-statblock.legendary .legendary-tracker {
  display: flex;
  gap: 6px;
  align-items: center;
  margin: 4px 0 10px;
  font-size: .82rem;
}
.ms-statblock.legendary .legendary-tracker .pip {
  width: 14px; height: 14px;
  border: 1px solid var(--accent);
  border-radius: 50%;
  display: inline-block;
}

</style>

<div class="ms-page">

<div class="ms-notice">
This page catalogues enemy NPCs encountered on Vvardenfell. Scroll down to browse further entries.
</div>

## Bestiary

<div class="ms-bestiary">

<div class="ms-statblock legendary">
  <div class="sb-header">
    <div>
      <div class="sb-name">Ash Ghoul Matriarch</div>
      <div class="sb-type">Large undead, chaotic evil</div>
    </div>
    <div class="sb-cr">CR 9</div>
  </div>
  <div class="sb-body">

  <div class="sb-portrait"><img src="ash-ghoul-matriarch.png" alt="Ash Ghoul Matriarch"></div>

  <div class="sb-main">

  <div class="sb-quickstats">
    <div class="qs-box"><span class="qs-label">Armour Class</span><span class="qs-value">16</span></div>
    <div class="qs-box"><span class="qs-label">Hit Points</span><span class="qs-value">168 (16d10+80)</span></div>
    <div class="qs-box"><span class="qs-label">Speed</span><span class="qs-value">30 ft, climb 30 ft</span></div>
    <div class="qs-box"><span class="qs-label">Initiative</span><span class="qs-value">+3</span></div>
  </div>

  <div class="sb-abilities">
    <div class="ab-box"><span class="ab-name">Str</span><span class="ab-score">18</span> <span class="ab-mod">(+4)</span></div>
    <div class="ab-box"><span class="ab-name">Dex</span><span class="ab-score">16</span> <span class="ab-mod">(+3)</span></div>
    <div class="ab-box"><span class="ab-name">Con</span><span class="ab-score">20</span> <span class="ab-mod">(+5)</span></div>
    <div class="ab-box"><span class="ab-name">Int</span><span class="ab-score">11</span> <span class="ab-mod">(+0)</span></div>
    <div class="ab-box"><span class="ab-name">Wis</span><span class="ab-score">14</span> <span class="ab-mod">(+2)</span></div>
    <div class="ab-box"><span class="ab-name">Cha</span><span class="ab-score">17</span> <span class="ab-mod">(+3)</span></div>
  </div>

  <div class="sb-meta"><span class="meta-label">Saving Throws</span> — Con +9, Wis +6, Cha +7</div>
  <div class="sb-meta"><span class="meta-label">Damage Resistances</span> — necrotic; bludgeoning, piercing, slashing from nonmagical attacks</div>
  <div class="sb-meta"><span class="meta-label">Senses</span> — darkvision 60 ft, passive Perception 12</div>
  <div class="sb-meta"><span class="meta-label">Languages</span> — Dunmeris, understands Daedric but can't speak it</div>
  <div class="sb-meta"><span class="meta-label">Proficiency Bonus</span> — +4</div>
  <div class="sb-meta"><span class="meta-label">Legendary Resistance</span> — 3/Day (see Legendary Actions)</div>

  <div class="sb-section-title">Features</div>
  <div class="sb-feature"><span class="feat-name">Ash Shroud.</span> The matriarch is heavily obscured by drifting ash while stationary; creatures more than 10 feet away have disadvantage on attack rolls against her.</div>

  <div class="sb-section-title">Actions</div>
  <div class="sb-feature"><span class="feat-name">Multiattack.</span> The matriarch makes three claw attacks.</div>
  <div class="sb-feature"><span class="feat-name">Claw.</span> Melee Weapon Attack: +8 to hit, reach 10 ft, one target. Hit: 13 (2d8+4) slashing damage plus 7 (2d6) necrotic damage.</div>

  <div class="sb-section-title legendary-title">Legendary Actions</div>
  <div class="legendary-tracker"><span class="pip"></span><span class="pip"></span><span class="pip"></span> 3 per round, usable only at the end of another creature's turn</div>
  <div class="sb-feature"><span class="feat-name">Rend.</span> The matriarch makes one claw attack.</div>
  <div class="sb-feature"><span class="feat-name">Ash Step (Costs 2 Actions).</span> The matriarch teleports up to 30 feet to an unoccupied space she can see, leaving a cloud of ash behind.</div>

  <div class="sb-section-title legendary-title">Lair Actions</div>
  <div class="sb-feature">On initiative count 20 (losing ties), the matriarch takes a lair action to cause one of the following effects; she can't use the same effect two rounds in a row.</div>
  <div class="sb-feature">Choking ash fills a 20-foot-radius sphere centered on a point she can see within 60 feet, forcing creatures within to make a DC 15 Constitution save or be blinded until the end of their next turn.</div>

  </div>
  </div>
</div>

<div class="ms-statblock legendary">
  <div class="sb-header">
    <div>
      <div class="sb-name">Ash Ghoul Matriarch</div>
      <div class="sb-type">Large undead, chaotic evil</div>
    </div>
    <div class="sb-cr">CR 9</div>
  </div>
  <div class="sb-body">

  <div class="sb-portrait"><img src="ash-ghoul-matriarch.png" alt="Ash Ghoul Matriarch"></div>

  <div class="sb-main">

  <div class="sb-quickstats">
    <div class="qs-box"><span class="qs-label">Armour Class</span><span class="qs-value">16</span></div>
    <div class="qs-box"><span class="qs-label">Hit Points</span><span class="qs-value">168 (16d10+80)</span></div>
    <div class="qs-box"><span class="qs-label">Speed</span><span class="qs-value">30 ft, climb 30 ft</span></div>
    <div class="qs-box"><span class="qs-label">Initiative</span><span class="qs-value">+3</span></div>
  </div>

  <div class="sb-abilities">
    <div class="ab-box"><span class="ab-name">Str</span><span class="ab-score">18</span> <span class="ab-mod">(+4)</span></div>
    <div class="ab-box"><span class="ab-name">Dex</span><span class="ab-score">16</span> <span class="ab-mod">(+3)</span></div>
    <div class="ab-box"><span class="ab-name">Con</span><span class="ab-score">20</span> <span class="ab-mod">(+5)</span></div>
    <div class="ab-box"><span class="ab-name">Int</span><span class="ab-score">11</span> <span class="ab-mod">(+0)</span></div>
    <div class="ab-box"><span class="ab-name">Wis</span><span class="ab-score">14</span> <span class="ab-mod">(+2)</span></div>
    <div class="ab-box"><span class="ab-name">Cha</span><span class="ab-score">17</span> <span class="ab-mod">(+3)</span></div>
  </div>

  <div class="sb-meta"><span class="meta-label">Saving Throws</span> — Con +9, Wis +6, Cha +7</div>
  <div class="sb-meta"><span class="meta-label">Damage Resistances</span> — necrotic; bludgeoning, piercing, slashing from nonmagical attacks</div>
  <div class="sb-meta"><span class="meta-label">Senses</span> — darkvision 60 ft, passive Perception 12</div>
  <div class="sb-meta"><span class="meta-label">Languages</span> — Dunmeris, understands Daedric but can't speak it</div>
  <div class="sb-meta"><span class="meta-label">Proficiency Bonus</span> — +4</div>
  <div class="sb-meta"><span class="meta-label">Legendary Resistance</span> — 3/Day (see Legendary Actions)</div>

  <div class="sb-section-title">Features</div>
  <div class="sb-feature"><span class="feat-name">Ash Shroud.</span> The matriarch is heavily obscured by drifting ash while stationary; creatures more than 10 feet away have disadvantage on attack rolls against her.</div>

  <div class="sb-section-title">Actions</div>
  <div class="sb-feature"><span class="feat-name">Multiattack.</span> The matriarch makes three claw attacks.</div>
  <div class="sb-feature"><span class="feat-name">Claw.</span> Melee Weapon Attack: +8 to hit, reach 10 ft, one target. Hit: 13 (2d8+4) slashing damage plus 7 (2d6) necrotic damage.</div>

  <div class="sb-section-title legendary-title">Legendary Actions</div>
  <div class="legendary-tracker"><span class="pip"></span><span class="pip"></span><span class="pip"></span> 3 per round, usable only at the end of another creature's turn</div>
  <div class="sb-feature"><span class="feat-name">Rend.</span> The matriarch makes one claw attack.</div>
  <div class="sb-feature"><span class="feat-name">Ash Step (Costs 2 Actions).</span> The matriarch teleports up to 30 feet to an unoccupied space she can see, leaving a cloud of ash behind.</div>

  <div class="sb-section-title legendary-title">Lair Actions</div>
  <div class="sb-feature">On initiative count 20 (losing ties), the matriarch takes a lair action to cause one of the following effects; she can't use the same effect two rounds in a row.</div>
  <div class="sb-feature">Choking ash fills a 20-foot-radius sphere centered on a point she can see within 60 feet, forcing creatures within to make a DC 15 Constitution save or be blinded until the end of their next turn.</div>

  </div>
  </div>
</div>
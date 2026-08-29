---
title: The Tyranny of Dragons Campaign
draft: false
tags:

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

/* ===== Hero header ===== */
.ms-hero {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 22px;
  background: linear-gradient(180deg, #34302a, #211e19) !important;
  border: 1px solid var(--header-bar-dark);
  border-radius: 4px;
  padding: 22px 28px;
  margin-bottom: 24px;
  box-shadow: inset 0 1px 0 rgba(255,255,255,0.05), inset 0 -2px 4px rgba(0,0,0,0.5), 0 3px 10px rgba(0,0,0,0.3);
}
.ms-hero .hero-title h1 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-weight: 700;
  font-size: 2rem;
  letter-spacing: 3px;
  margin: 0;
  color: #e6d7ae !important;
  text-transform: uppercase;
  text-shadow: 0 0 14px rgba(230,215,174,0.25);
}
.ms-hero .hero-sub {
  font-size: .78rem;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: #c9a860 !important;
  margin-top: 6px;
}
.ms-hero .hero-sigil {
  width: 68px; height: 68px;
  border-radius: 50%;
  flex-shrink: 0;
  background:
    radial-gradient(circle at 50% 50%, #211e19 0 30%, transparent 31%),
    conic-gradient(from 0deg, #c9a860 0deg 8deg, transparent 8deg 45deg,
      #c9a860 45deg 53deg, transparent 53deg 90deg,
      #c9a860 90deg 98deg, transparent 98deg 135deg,
      #c9a860 135deg 143deg, transparent 143deg 180deg,
      #c9a860 180deg 188deg, transparent 188deg 225deg,
      #c9a860 225deg 233deg, transparent 233deg 270deg,
      #c9a860 270deg 278deg, transparent 278deg 315deg,
      #c9a860 315deg 323deg, transparent 323deg 360deg),
    radial-gradient(circle at 50% 50%, var(--accent) 0 45%, #211e19 46% 100%);
  box-shadow: 0 0 0 2px var(--header-bar-dark), 0 0 16px rgba(201,168,96,0.2);
  position: relative;
}
.ms-hero .hero-sigil::after {
  content: "\1F409"; /* dragon emoji as placeholder emblem */
  position: absolute; inset: 0;
  display: flex; align-items: center; justify-content: center;
  font-size: 1.5rem;
}

/* ===== Spotlight cards ===== */
.ms-spotlight-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 18px;
  margin: 16px 0 8px;
}
.spotlight-card {
  border: 1px solid var(--border);
  border-radius: 4px;
  background: #fbf5e3 !important;
  box-shadow: 0 2px 8px rgba(0,0,0,0.15);
  overflow: hidden;
  display: flex;
  flex-direction: column;
}
.spotlight-card .sc-image {
  width: 100%;
  height: 140px;
  overflow: hidden;
  background: var(--ink);
  line-height: 0;
}
.spotlight-card .sc-image p { margin: 0; height: 100%; }
.spotlight-card .sc-image img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  margin: 0;
}
.spotlight-card .sc-image:empty::after {
  content: "No Image";
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  font-family: 'Cinzel', serif;
  font-size: .65rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  background: var(--table-head) !important;
}
.spotlight-card .sc-tag {
  font-family: 'Cinzel', serif;
  font-size: .58rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--accent) !important;
  padding: 8px 14px 0;
}
.spotlight-card .sc-title {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.02rem;
  color: var(--ink) !important;
  padding: 3px 14px 0;
}
.spotlight-card .sc-blurb {
  font-size: .88rem;
  color: var(--ink-dim) !important;
  padding: 6px 14px 14px;
  flex: 1;
}
.spotlight-card .sc-link {
  border-top: 1px solid var(--border);
  padding: 8px 14px;
  font-family: 'Cinzel', serif;
  font-size: .7rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  background: var(--table-head) !important;
}

/* ===== Navigation index ===== */
.ms-index {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
  margin: 14px 0 10px;
}
.index-col {
  border: 1px solid var(--border);
  border-radius: 3px;
  background: #fbf5e3 !important;
  overflow: hidden;
}
.index-col .ic-head {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: .78rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: #fbf5e3 !important;
  background: linear-gradient(180deg, var(--header-bar), var(--header-bar-dark)) !important;
  padding: 7px 12px;
}
.index-col ul {
  list-style: none;
  margin: 0;
  padding: 8px 14px 12px;
  font-size: .88rem;
}
.index-col li { margin-bottom: 5px; }

.ms-cat-footer {
  margin-top: 30px;
  padding-top: 10px;
  border-top: 1px solid var(--border);
  font-size: .78rem;
  color: var(--ink-dim) !important;
  background: var(--note-bg) !important;
}

@media (max-width: 900px) {
  .ms-spotlight-grid { grid-template-columns: 1fr; }
  .ms-index { grid-template-columns: 1fr 1fr; }
}
@media (max-width: 560px) {
  .ms-index { grid-template-columns: 1fr; }
}
</style>

<div class="ms-page">

<div class="ms-hero">
  <div class="hero-title">
    <h1>The Tyranny of Dragons Campaign</h1>
    <div class="hero-sub">A Chronicle of the Cult of the Dragon &amp; the War Against Tiamat</div>
  </div>
  <div class="hero-sigil"></div>
</div>

<div class="ms-notice">
Welcome, traveler. This wiki tracks our ongoing campaign — player characters, notable NPCs, locations, session recaps, and house rules. Use the spotlight below for what's current, or the index further down to browse everything.
</div>

## Spotlight

<div class="ms-spotlight-grid">

<div class="spotlight-card">
  <div class="sc-image"></div>
  <div class="sc-tag">Latest Session</div>
  <div class="sc-title">Session 12 — The Fall of Greenest</div>
  <div class="sc-blurb">The party arrives too late to stop the raid, but not too late to make a difference. A recap of the battle, the choices made, and what was learned about the cult's plans.</div>
  <div class="sc-link"><a href="/sessions/session-12">Read the Recap →</a></div>
</div>

<div class="spotlight-card">
  <div class="sc-image"></div>
  <div class="sc-tag">Featured Location</div>
  <div class="sc-title">Greenest</div>
  <div class="sc-blurb">A small trading town on the Coast Way, now smoldering in the wake of a dragon raid. Home to Governor Nighthill and the keep that sheltered the survivors.</div>
  <div class="sc-link"><a href="/locations/greenest">Visit the Location →</a></div>
</div>

<div class="spotlight-card">
  <div class="sc-image"></div>
  <div class="sc-tag">Featured NPC</div>
  <div class="sc-title">Leosin Erlanthar</div>
  <div class="sc-blurb">A monk and member of the Harpers who has been tracking the Cult of the Dragon for months. Currently held captive by cultists near Greenest.</div>
  <div class="sc-link"><a href="/npcs/leosin-erlanthar">View NPC Entry →</a></div>
</div>

</div>

---

## Index

<div class="ms-index">

<div class="index-col">
  <div class="ic-head">Player Characters</div>
  <ul>
    <li><a href="/characters/">All Characters</a></li>
    <li><a href="/characters/party">The Party</a></li>
    <li><a href="/characters/relationships">Relationships</a></li>
  </ul>
</div>

<div class="index-col">
  <div class="ic-head">Bestiary &amp; NPCs</div>
  <ul>
    <li><a href="/bestiary/">Bestiary</a></li>
    <li><a href="/npcs/">Notable NPCs</a></li>
    <li><a href="/npcs/cult-of-the-dragon">Cult of the Dragon</a></li>
  </ul>
</div>

<div class="index-col">
  <div class="ic-head">World &amp; Locations</div>
  <ul>
    <li><a href="/locations/">All Locations</a></li>
    <li><a href="/locations/greenest">Greenest</a></li>
    <li><a href="/locations/map">World Map</a></li>
  </ul>
</div>

<div class="index-col">
  <div class="ic-head">Sessions &amp; Rules</div>
  <ul>
    <li><a href="/sessions/">Session Log</a></li>
    <li><a href="/rules/house-rules">House Rules</a></li>
    <li><a href="/rules/timeline">Campaign Timeline</a></li>
  </ul>
</div>

</div>

---

## Recently Updated

| Page | Type | Last Updated |
|---|---|:---:|
| [[Session 12 — The Fall of Greenest]] | Session Log | — |
| [[Leosin Erlanthar]] | NPC | — |
| [[Greenest]] | Location | — |
| [[House Rules]] | Reference | — |

</div>
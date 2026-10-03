---
title: World Map
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

/* ===== Map page header plate ===== */
.map-plate {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  border-bottom: 1px solid var(--border);
  padding-bottom: 16px;
  margin-bottom: 22px;
}
.map-plate .mp-title h1 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.7rem;
  letter-spacing: 2px;
  margin: 0 0 4px;
  color: var(--accent) !important;
}
.map-plate .mp-sub {
  font-family: 'Cinzel', serif;
  font-size: .68rem;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
}

/* ===== Full-width map frame =====
   line-height: 0 and the <p> reset below stop Markdown's auto-inserted
   <p> wrapper from adding a margin gap that reveals the dark background —
   same fix used for the bestiary portraits and infobox photo. */
.map-frame {
  border: 2px solid var(--border);
  border-radius: 4px;
  background: var(--ink);
  overflow: hidden;
  box-shadow: 0 4px 14px rgba(0,0,0,0.25), inset 0 0 0 1px rgba(251,245,227,0.15);
  margin-bottom: 8px;
  line-height: 0;
}
.map-frame p { margin: 0; }
.map-frame img {
  display: block;
  width: 100%;
  height: auto;
  margin: 0;
}
/* Empty-state placeholder if no image has been added yet */
.map-frame:empty::after {
  content: "No Map Uploaded";
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  min-height: 300px;
  font-family: 'Cinzel', serif;
  font-size: .8rem;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  background: var(--table-head) !important;
}
.map-caption {
  text-align: center;
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: .8rem;
  font-style: italic;
  color: var(--ink-dim) !important;
  margin-bottom: 24px;
}

/* ===== Legend table ===== */
.map-legend {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1px;
  background: var(--border) !important;
  border: 1px solid var(--border);
  border-radius: 3px;
  overflow: hidden;
  margin-bottom: 22px;
}
.map-legend .legend-item {
  background: #fbf5e3 !important;
  padding: 8px 12px;
  display: flex;
  align-items: center;
  gap: 10px;
  font-size: .92rem;
}
.map-legend .legend-marker {
  width: 18px;
  height: 18px;
  border-radius: 50%;
  flex-shrink: 0;
  border: 1.5px solid var(--header-bar-dark);
}
.map-legend .legend-marker.town { background: var(--header-bar) !important; }
.map-legend .legend-marker.danger { background: var(--accent) !important; }
.map-legend .legend-marker.poi { background: #5c5138 !important; }
.map-legend .legend-marker.unexplored {
  background: transparent !important;
  border-style: dashed;
}

.ms-cat-footer {
  margin-top: 30px;
  padding-top: 10px;
  border-top: 1px solid var(--border);
  font-size: .78rem;
  color: var(--ink-dim) !important;
  background: var(--note-bg) !important;
}

@media (max-width: 560px) {
  .map-legend { grid-template-columns: 1fr; }
}
</style>

<div class="ms-page">

<div class="map-plate">
  <div class="mp-title">
    <h1>The Sword Coast</h1>
    <div class="mp-sub">Campaign Map — Current Party Knowledge</div>
  </div>
</div>

<div class="ms-notice">
Unexplored regions and rumored locations are marked but not yet detailed.
</div>

<div class="map-frame">
<img src="/Z_Assets/Maps/Playable Area.png" alt="Map of Vvardenfell">
</div>
<div class="map-caption">North-West Faerun · The Sword Coast</div>

## Legend

<div class="map-legend">
  <div class="legend-item"><span class="legend-marker town"></span> Settlement</div>
  <div class="legend-item"><span class="legend-marker danger"></span> Known Danger</div>
  <div class="legend-item"><span class="legend-marker poi"></span> Point of Interest</div>
  <div class="legend-item"><span class="legend-marker unexplored"></span> Unexplored</div>
</div>

## Notable Locations

| Location | Region | Notes |
|---|---|---|
| Neverwinter | The Neverwinter Demense | A City of the Lord's Alliance |
| Silverymoon | Confederation of the Silver Marches | A City of the Lord's Alliance |
| Waterdeep | The Waterdhavian Open Districts | A City of the Lord's Alliance |
| Mirabar | Mirabar something | A City of the Lord's Alliance |
| Luskan | Luskan something | Pirate Republic |


## Notes

*Any ongoing discoveries, travel times, or map-related developments can be tracked here.*

</div>

<div class="ms-cat-footer">
Categories: [[World &amp; Locations]] · [[Map]] · [[Tyranny of Dragons Campaign]]
</div>
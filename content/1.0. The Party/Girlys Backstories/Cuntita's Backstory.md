---
title: Cuntita's Backstory
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

/* ===== Backstory header plate ===== */
.bio-plate {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  border-bottom: 1px solid var(--border);
  padding-bottom: 16px;
  margin-bottom: 24px;
}
.bio-plate .bp-title h1 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.7rem;
  letter-spacing: 2px;
  margin: 0 0 4px;
  color: var(--accent) !important;
}
.bio-plate .bp-sub {
  font-family: 'Cinzel', serif;
  font-size: .68rem;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
}

/* ===== Floating captioned image boxes ===== */
.bio-image {
  width: 260px;
  border: 1px solid var(--border);
  border-radius: 3px;
  background: #fbf5e3 !important;
  box-shadow: 0 2px 8px rgba(0,0,0,0.15);
  overflow: hidden;
  margin-bottom: 14px;
}
.bio-image.left {
  float: left;
  margin-right: 22px;
  margin-top: 4px;
}
.bio-image.right {
  float: right;
  margin-left: 22px;
  margin-top: 4px;
}
.bio-image .bi-frame {
  width: 100%;
  height: 220px;
  overflow: hidden;
  background: var(--ink);
  line-height: 0;
}
.bio-image .bi-frame p { margin: 0; height: 100%; }
.bio-image .bi-frame img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
  object-position: center top;
  margin: 0;
}
.bio-image .bi-frame:empty::after {
  content: "No Image";
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  font-family: 'Cinzel', serif;
  font-size: .68rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  background: var(--table-head) !important;
}
.bio-image .bi-caption {
  padding: 7px 12px;
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: .78rem;
  font-style: italic;
  text-align: center;
  color: var(--ink-dim) !important;
  border-top: 1px solid var(--border);
  background: var(--table-head) !important;
}

/* Clearfix so floated images don't bleed past a section into the next heading */
.bio-clear { clear: both; }

/* ===== Story Updates timeline (reused pattern) ===== */
.ms-timeline {
  position: relative;
  margin: 14px 0 22px;
  padding-left: 26px;
  border-left: 2px solid var(--border);
}
.timeline-entry {
  position: relative;
  margin-bottom: 18px;
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
.timeline-entry .te-date {
  font-family: 'Cinzel', serif;
  font-size: .62rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
  margin-bottom: 2px;
}
.timeline-entry .te-title {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: .98rem;
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

@media (max-width: 640px) {
  .bio-image.left, .bio-image.right {
    float: none;
    width: 100%;
    margin: 0 0 16px;
  }
}
</style>

<div class="ms-page">

<div class="bio-plate">
  <div class="bp-title">
    <h1>Cuntita the Criminal</h1>
    <div class="bp-sub">Origins &amp; Ongoing Story</div>
  </div>
</div>

<div class="ms-notice">
This page holds the backstory and ongoing narrative for Cuntita. It's a living document — expect it to grow as the campaign continues.
</div>

## Origins

<div class="bio-image left" style="width: auto;">
  <div class="bi-frame" style="height: 360px; width: auto;">
    <img src="Z_Assets/Girlies/Cuntita.jpeg" alt="description" style="width: auto; height: 100%; object-fit: initial;">
  </div>
  <div class="bi-caption">Character Name, before everything changed</div>
</div>

Cuntita the Criminal was born into a world that sang of betrayal and darkness. Raised in the back alleys of Baldur's Gate, a bustling port city notorious for its rampant corruption, she quickly learned that might made right. Her parents were lowly dockworkers who served as pawns in a larger game played by smugglers and pirates. 

When Cuntita was just ten years old, her family fell victim to an elaborate ploy orchestrated by one such pirate crew: they were framed for stealing cargo meant for the ruling Council of Four of Baldurs Gate. In one brutal stroke, both of her parents were imprisoned, leaving Cuntita to fend for herself on the unforgiving streets.

<div class="bio-clear"></div>

## The Turning Point

<div class="bio-image right" style="width: auto;">
  <div class="bi-frame" style="height: 360px; width: auto;">
    <img src="Z_Assets/Girlies/Cuntita.jpeg" alt="description" style="width: auto; height: 100%; object-fit: initial;">
  </div>
  <div class="bi-caption">The night that set them on this path</div>
</div>

Survival honed her skills; strength became her constant companion as she beat down those who would stand in her way. The Zhentarim, a cadre of self-serving thieves, spies, assassins and malevolent wizards, who for a time, were indentured by their leaders to serve the dark god Bane, took in Cuntita and nurtured her darker self.

They manufactured her desire and need for gold, viewing it as the only source of pleasure and power in this world. She quickly rose through the ranks and became privy to many illicit secrets. One day, Cuntita was working her usual job as Sergeant for the Zhentarim, and was playing with her dagger, when all of a sudden a child fell onto her dagger. 

She was immediately beset by guards, but broke free and went into hiding, with the child’s condition unknown; news spread quickly and Cuntita heard that the guards would execute the perpetrator of this attack on the child of a parent from the Council of Four. Knowing the Zhentarim would not protect her from an act so high-calibre and treasonous, she set out as a stowaway on a ship bound for Waterdeep.

From there Cuntita sought a cover for herself, an escape from her crimes (from her mistake), and set out to work as a mercenary in the developing town of Phandalin, where no-one would know her. From here she still seeks out justice for herself and her parents, whether it be in blood or pardons. Will she be able to release them and pay back their pain in kind?  Will enemies stand in her way… or gold blind her eyes yet again…

<div class="bio-clear"></div>

## Who They Are Now

*A shorter section summarizing the character as they exist at the start of the campaign — personality, goals, what they want, what they're avoiding.*

---

## Story Updates

<div class="ms-timeline">

<div class="timeline-entry">
  <div class="te-date">Session 1</div>
  <div class="te-title">First Steps</div>
  <div class="te-body">A short note on how the character entered the party's story and any first impressions worth remembering.</div>
</div>

<div class="timeline-entry">
  <div class="te-date">Session 5</div>
  <div class="te-title">An Old Face Resurfaces</div>
  <div class="te-body">Note a development tied to the character's backstory — someone or something from their past reappearing, a clue uncovered, a promise tested.</div>
</div>

</div>

> [!note]- Unresolved Threads
> - A backstory element still hanging over the character that hasn't paid off yet.
> - Another loose end to track for later.

## Trivia

- —

</div> 
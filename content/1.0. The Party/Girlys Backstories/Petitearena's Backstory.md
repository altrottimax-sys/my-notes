---
title: Petitearena's Backstory
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
    <h1>Petitearena Genesis</h1>
    <div class="bp-sub">Origins &amp; Ongoing Story</div>
  </div>
</div>

<div class="ms-notice">
This page holds the backstory and ongoing narrative for Petitearena. It's a living document — expect it to grow as the campaign continues.
</div>

## Origins

<div class="bio-image left" style="width: auto;">
  <div class="bi-frame" style="height: 360px; width: auto;">
    <img src="Petitearena.jpeg" alt="description" style="width: auto; height: 100%; object-fit: initial;">
  </div>
  <div class="bi-caption">Character Name, before everything changed</div>
</div>

Petitearena was born and raised in a quiet village, nestled between ancient woods and towering mountains. From a young age, she demonstrated a curiosity for the world around her. While other children played simple games, Petiterena immersed herself in dusty tomes at the local library, delighting in tales of arcane mysteries and celestial enigmas. Her studies took her to the elegant sorcerous city of Silverymoon. There she took her first steps to becoming a fully-fledged wizard. 

In the Grand Library of the Spellguard, Petitearena discovered an old tome, bound in a golden skin and inked with ominous symbols, a most intriguing book. When she opened this tome her mind could barely comprehend the vile shifting symbols on the page. As her mind burgeoned with untold secrets she was barely able to close the tome. She grew to be obsessed with this tome and also with unlocking its greatest potential… her greatest potential.

<div class="bio-clear"></div>

## The Turning Point

<div class="bio-image right" style="width: auto;">
  <div class="bi-frame" style="height: 360px; width: auto;">
    <img src="Petitearena.jpeg" alt="description" style="width: auto; height: 100%; object-fit: initial;">
  </div>
  <div class="bi-caption">The night that set them on this path</div>
</div>

Her goal now was to protect this tome from any that may threaten her or it. She quickly left Silverymoon, and continued to listen to this tome, which spoke to her whispers of forgotten sorcery. One such fragment of knowledge spoke out to Petitearena. “Dragon’s blood.”

From town to town she went, in secret, in hiding. Listening, waiting, what will the tome tell next, where shall she go. As Petitearena hid behind the stable by a rural inn, she heard her next whisper, not from the book, but from a passing traveller; “I was thinking of moving to Phandalin, help rebuild the town… but all these talks of a dragon are really freaking me out…”

Drawn by desperation mingled with ambition she set forth determinedly into the vast unknown landscape—armed not just by spells but fuelled by fervour born from an insatiable thirst for enlightenment. Questions still remain in her head, who wrote this tome? What does it contain? And what will Petitearena use this power for?

<div class="bio-clear"></div>

## Who They Are Now

*A shorter section summarizing the character as they exist at the start of the campaign — personality, goals, what they want, what they're avoiding.*

---

## Story Updates

*As the campaign progresses, log major character-relevant beats here — not a full session recap, just what matters to **this character's** ongoing story.*

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

---
title: Zaenerys' Backstory
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
    <h1>Zaenerys Alagondar</h1>
    <div class="bp-sub">Origins &amp; Ongoing Story</div>
  </div>
</div>

<div class="ms-notice">
This page holds the backstory and ongoing narrative for Zaenerys. It's a living document — expect it to grow as the campaign continues.
</div>

## Origins

<div class="bio-image left" style="width: auto;">
  <div class="bi-frame" style="height: 360px; width: auto;">
    <img src="Zaenaerys.jpeg" alt="description" style="width: auto; height: 100%; object-fit: initial;">
  </div>
  <div class="bi-caption">Character Name, before everything changed</div>
</div>

Zaenerys was born to the Alagondar Dynasty rulers of Neverwinter, a highborn family that was ashamed of their draconic ancestry. Her brother was 6 years older than her, and Zaenerys led a protected life as the second child, leaving her to spend most of her time alone in a giant castle, making friends with the bugs and animals that her family owned.  She was sweet by nature and spent a lot of time with her father who taught her how to rule, listen to the people's needs, and make the right choices. He also taught her their family’s history and language, telling her stories about how they are borne of the blood of dragons, and she was fascinated. Her mother was a wood elf from the Neverwinter forests, and saw beauty in all things, even dragons; but knew there was a darkness within them.

She didn’t care too much about her draconic secret as she didn’t feel a connection with them, having a human like appearance with long silver hair with fuck ass bangs. She was also a vegetarian cause she was besties with a baby cow and duckling.

Her parents did not speak much of the cadet branch of their royal lineage, but she knew there had been a rift between her father and his sister a while back. Her older brother often warned her about their aunt's devotion to draconic and demonic entities, she saw them as a caring familiar power rather than destruction.

<div class="bio-clear"></div>

## The Turning Point

<div class="bio-image right" style="width: auto;">
  <div class="bi-frame" style="height: 360px; width: auto;">
    <img src="Zaenaerys.jpeg" alt="description" style="width: auto; height: 100%; object-fit: initial;">
  </div>
  <div class="bi-caption">The night that set them on this path</div>
</div>

When she was 13 her brother had snuck out of the palace walls and was found in the room of their cousin with blood on his hands, holding a dagger. Their Aunt's only child was dead. Her aunt was furious and blamed Zaenerys' father for preventing her from creating a new lineage of Dragonborns in their family, that would be guided by the Draconic god of Vengeance, Tiamat. She had worked with magic rituals and curses to harvest the power of dragons and gain the favour of Tiamat so she could rule like their ancestors once did.

When Zaenerys was 15, the conflict culminated in a civil war between the family, with hundreds dead and almost all of the House Alagondar exterminated. Her Aunt had won. Zaenerys was in the Neverwinter keep with her mother, father, and a knight. The knight heard banging at the door and got his sword ready. However, the knight turned around, his eyes glowing with draconic magic, being commanded by Zaenerys' aunt who now entered easily.

Her aunt watched as the knight sliced at Zaenerys’ parents, shielding their daughter from all they could. As the last true born Alagondar alive, her Aunt found her new project, cursing Daenerys with a mark. As she would age, her features would change until she had no more humanity left in her. Just fire and rage. As her Aunt lost concentration on her spells, The knight broke free of her Aunt's control and knocked her tf out. He took Zaenerys to her Mother’s tribe in the Neverwinter woods where she would learn to be a skilled ranger.

On her 18th birthday she noticed her skin having a slight shimmer, that of a dragon. Her violet eyes became almost reptilian but changed back after a few seconds. She knew she had to leave the tribe and find a way to remove the curse. That night she snuck out, put on her lil fit, cut her hair, and became Zaenerys Dragonblood. Her search eventually led her to a little frontier town called 'Phandalin', jeopardised by a local roaming dragon.

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
---
title: "!Player Quest; Zaenaerys"
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
  --success: #4b6b3a;
  --success-bright: #5f8a4a;
  --success-bg: #e2e8d4;

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

.ms-page ul, .ms-page ol { padding-left: 22px; }

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

/* ===== Quest header plate ===== */
.quest-plate {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  border-bottom: 1px solid var(--border);
  padding-bottom: 16px;
  margin-bottom: 22px;
}
.quest-plate .qp-title h1 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.7rem;
  letter-spacing: 2px;
  margin: 0 0 4px;
  color: var(--accent) !important;
}
.quest-plate .qp-sub {
  font-family: 'Cinzel', serif;
  font-size: .68rem;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
}
.quest-plate .qp-status {
  font-family: 'Cinzel', serif;
  font-size: .7rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: #fbf5e3 !important;
  background: linear-gradient(180deg, var(--header-bar), var(--header-bar-dark)) !important;
  border-radius: 14px;
  padding: 5px 16px;
  white-space: nowrap;
  flex-shrink: 0;
}
.quest-plate .qp-status.complete {
  background: linear-gradient(180deg, var(--success-bright), var(--success)) !important;
}
.quest-plate .qp-status.failed {
  background: linear-gradient(180deg, var(--accent-bright), var(--accent)) !important;
}

/* ===== Quest metadata bar ===== */
.quest-meta {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1px;
  background: var(--border) !important;
  border: 1px solid var(--border);
  border-radius: 3px;
  overflow: hidden;
  margin-bottom: 20px;
}
.quest-meta .meta-cell {
  background: #fbf5e3 !important;
  padding: 8px 10px;
  text-align: center;
}
.quest-meta .meta-cell .m-label {
  font-family: 'Cinzel', serif;
  font-size: .55rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  display: block;
  margin-bottom: 2px;
}
.quest-meta .meta-cell .m-value {
  font-size: .92rem;
  color: var(--ink) !important;
}

/* ===== Blurb / description block — the part you keep editing ===== */
.quest-blurb {
  border: 1px solid var(--border);
  border-left: 4px solid var(--header-bar);
  background: #fbf5e3 !important;
  border-radius: 2px;
  padding: 14px 18px;
  margin-bottom: 22px;
  font-size: .98rem;
}
.quest-blurb .qb-label {
  font-family: 'Cinzel', serif;
  font-size: .6rem;
  letter-spacing: 2px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
  display: block;
  margin-bottom: 6px;
}

/* ===== Objectives checklist ===== */
.ms-page .quest-objectives {
  list-style: none;
  padding-left: 0;
  margin: 10px 0 20px;
}
.ms-page .quest-objectives li {
  display: flex;
  align-items: flex-start;
  gap: 10px;
  padding: 6px 4px;
  border-bottom: 1px dotted rgba(184,164,115,0.4);
  font-size: .96rem;
}
.ms-page .quest-objectives input[type="checkbox"] {
  appearance: none;
  -webkit-appearance: none;
  width: 16px;
  height: 16px;
  margin-top: 3px;
  flex-shrink: 0;
  border: 1.5px solid var(--header-bar-dark);
  border-radius: 3px;
  background: rgba(255,255,255,0.4);
  cursor: pointer;
  position: relative;
}
.ms-page .quest-objectives input[type="checkbox"]:checked {
  background: var(--success) !important;
  border-color: var(--success) !important;
}
.ms-page .quest-objectives input[type="checkbox"]:checked::after {
  content: "✓";
  position: absolute;
  top: -3px;
  left: 2px;
  font-size: .75rem;
  color: #fbf5e3 !important;
}
/* Failed objective — strike through in red instead of checking off */
.ms-page .quest-objectives li.failed span {
  text-decoration: line-through;
  text-decoration-color: var(--accent) !important;
  text-decoration-thickness: 2px;
  color: var(--accent-bright) !important;
  opacity: 0.85;
}
.ms-page .quest-objectives li.failed input[type="checkbox"] {
  border-color: var(--accent) !important;
  background: rgba(122,38,38,0.12) !important;
}
.ms-page .quest-objectives li.failed input[type="checkbox"]::after {
  content: "✕";
  position: absolute;
  top: -3px;
  left: 2px;
  font-size: .7rem;
  color: var(--accent) !important;
}

/* ===== Callout boxes (reused base) ===== */
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

/* Success callout — moss/laurel green, distinct from note (gold) and warning (red) */
.ms-page blockquote.callout[data-callout="success"] {
  --color: #4b6b3a;
  --border: #4b6b3a;
  --bg: #e2e8d4;
  border-left-color: var(--success) !important;
}
.ms-page blockquote.callout[data-callout="success"] .callout-title {
  background: linear-gradient(180deg, var(--success-bright), var(--success)) !important;
  color: #fbf5e3 !important;
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
  .quest-meta { grid-template-columns: 1fr; }
}
</style>

<div class="ms-page">

<div class="quest-plate">
  <div class="qp-title">
    <h1>Accursed Blood</h1>
    <div class="qp-sub">X</div>
  </div>
  <div class="qp-status">In Progress</div> 
<!-- qp-status complete | qp-status | qp-status failed -->
</div>

<div class="quest-meta">
  <div class="meta-cell"><span class="m-label">Quest Giver</span><span class="m-value">X</span></div>
  <div class="meta-cell"><span class="m-label">Location</span><span class="m-value">X</span></div>
  <div class="meta-cell"><span class="m-label">Started</span><span class="m-value">Session 1</span></div>
</div>

## Description

<div class="quest-blurb">
<span class="qb-label">Current Status</span>
X
</div>

## Objectives

<ul class="quest-objectives">
  <li><input type="checkbox"> X </li>


</ul>

---

> [!note]+ ***Quest Outcome***
> You haven't finished this quest yet.

## Notes

- —

</div>
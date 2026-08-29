---
title: Zaenerys Alagondar
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

/* Catch-all: force every descendant to use the parchment ink color,
   regardless of what Quartz's dark-mode stylesheet does to it */
.ms-page, .ms-page * {
  color: var(--ink) !important;
}

/* Re-apply specific accent colors on top of the catch-all */
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

.ms-infobox {
  float: right;
  width: 260px;
  margin: 0 0 16px 20px;
  border: 1px solid var(--border);
  background: #fbf5e3 !important;
  font-size: .85rem;
}
.ms-infobox .ib-header {
  background: linear-gradient(180deg, var(--header-bar), var(--header-bar-dark)) !important;
  color: #fbf5e3 !important;
  font-family: 'Cinzel', serif;
  font-size: .95rem;
  letter-spacing: 1px;
  text-align: center;
  padding: 8px 6px;
}

/* Portrait frame — locks to the infobox's 260px width and a fixed 300px height,
   whatever the source image's native size or aspect ratio */
.ms-infobox .ib-photo {
  width: 260px;
  height: 300px;
  overflow: hidden;
  border-top: 1px solid var(--border);
  border-bottom: 1px solid var(--border);
  background: var(--ink);
  line-height: 0;
}

.ms-infobox .ib-photo p { 
margin: 0; 
height: 100%; 
}

.ms-infobox .ib-photo img {
  display: block; 
  width: 100%; 
  height: 100%; 
  object-fit: cover; 
  object-position: center center; 
  margin: 0; 
  }

.ms-infobox .ib-sub {
  text-align: center;
  font-style: italic;
  color: var(--ink-dim) !important;
  padding: 6px 8px;
  border-bottom: 1px solid var(--border);
}
.ms-infobox table { width: 100%; margin: 0; font-size: .82rem; }
.ms-infobox th {
  background: transparent !important;
  border: none;
  border-top: 1px solid var(--border);
  text-align: left;
  width: 40%;
  font-size: .68rem;
  color: var(--ink-dim) !important;
  text-transform: none;
  letter-spacing: 0;
  vertical-align: top;
  padding: 5px 8px;
}
.ms-infobox td {
  border: none;
  border-top: 1px solid var(--border);
  padding: 5px 8px;
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
</style>

<div class="ms-page">

<div class="ms-infobox">
  <div class="ib-header">Zaenerys Alagondar</div>
  <div class="ib-photo">
    <img src="Z_Assets/Girlies/Zaenaerys.jpeg" alt="Portrait of Zaenerys">
  </div>
  <div class="ib-sub">Lost Princess of Neverwinter</div>
  <table>
    <tr><th>Race</th><td>Dragon-Cursed</td></tr>
    <tr><th>Class</th><td>Drakewarden Ranger</td></tr>
    <tr><th>Level</th><td>5</td></tr>
    <tr><th>Background</th><td>Noble Princess</td></tr>
    <tr><th>Proficiency Level</th><td>+3</td></tr>
    <tr><th>Passive Insight</th><td>13</td></tr>
    <tr><th>Passive Perception</th><td>16</td></tr>
    <tr><th>Armour Class</th><td>15</td></tr>
    <tr><th>Hit Points</th><td>42</td></tr>
  </table>
</div>

<div class="ms-notice">
This page documents Daenerys' journey. Some details may change as the story of Faerun unfolds.
</div>

## Character Overview

*A brief description of the character — appearance, bearing, and how they came to be.*

---
## Character Statistics
> [!note]- Attributes & Saving Throws
> | Ability | Score | Modifier | Save Proficient | Save Modifier |
> |---|:---:|:---:|:---:|:---:|
> | Strength | 10 | +0 | ✦ | +3 |
> | Dexterity | 16 | +3 | ✦ | +6 |
> | Constitution | 14 | +2 | ○ | +2 |
> | Intelligence | 8 | -1 | ○ | -1 |
> | Wisdom | 16 | +3 | ○ | +3 |
> | Charisma | 11 | +0 | ○ | +0 |

> [!note]- Skills & Proficiencies
> | Skill | Ability | Proficient | Modifier |
> |---|:---:|:---:|:---:|
> | Acrobatics | Dex | ○ | +3 |
> | Animal Handling | Wis | ✦ | +6 |
> | Arcana | Int | ○ | -1 |
> | Athletics | Str | ○ | +3 |
> | Deception | Cha | ○ | +0 |
> | History | Int | ✦ | +2 |
> | Insight | Wis | ○ | +3 |
> | Intimidation | Cha | ○ | +0 |
> | Investigation | Int | ○ | -1 |
> | Medicine | Wis | ○ | +3 |
> | Nature | Int | ○ | -1 |
> | Perception | Wis | ✦ | +3 |
> | Performance | Cha | ○ | +0 |
> | Persuasion | Cha | ✦ | +3 |
> | Religion | Int | ○ | -1 |
> | Sleight of Hand | Dex | ○ | +3 |
> | Stealth | Dex | ✦✦ | +9 |
> | Survival | Wis | ○ | +3 |

> [!note]- Class Traits and Abilities
> test

## Combat and Actions

> [!note]- Combat Statistics
> | Stat | Value |
> |---|:---:|
> | Initiative | +3 |
> | Speed | 6sq (9m) |
> | Armour Class | 15 |
> | Hit Point Maximum | 42 |
> | Temporary Hit Points | — |
> | Hit Dice | 5d10 |
> | Proficiency Bonus | +2 |

> [!note]- Attacks
> | Name | Attack Bonus | Damage / Type | Range |
> |---|:---:|---|:---:|
> | | | | |
> | | | | |
> | | | | |

> [!note]- Spell Slots 
> | Rank | Slot Total | Known Spells | 
>  |---|:---:|:---:| 
>  | Cantrips (Rank 0) | ∞✦ | |
>  | 1st | ✦✦✦✦ | |
> | 2nd | ✦✦ ○ | |
> | 3rd | ○ ○ ○ | |
> | 4th | ○ ○ ○ | |
> | 5th | ○ ○ | |
> | 6th | ○ | |
> | 7th | ○ | |
> | 8th | ○ | |
> | 9th | ○ | |

**<u>Ability</u>**: This is an ability.

## Equipment

- Leather or iron armour
- Weapon(s)
- Alchemy ingredients
- Coin purse (Gold/Platinum)

## Personality

> **Traits:** —
>
> **Ideals:** —
>
> **Bonds:** —
>
> **Flaws:** —

## Notes

*Anything unusual, ongoing plot threads, or GM-facing information can go here.*

## Trivia

- —

</div>

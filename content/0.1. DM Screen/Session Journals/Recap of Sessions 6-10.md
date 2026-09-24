---
title: Recap of Sessions 6-10
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

/* ===== Session header plate ===== */
.session-plate {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 20px;
  border-bottom: 1px solid var(--border);
  padding-bottom: 16px;
  margin-bottom: 24px;
}
.session-plate .sp-title h1 {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: 1.7rem;
  letter-spacing: 2px;
  margin: 0 0 4px;
  color: var(--accent) !important;
}
.session-plate .sp-sub {
  font-family: 'Cinzel', serif;
  font-size: .68rem;
  letter-spacing: 3px;
  text-transform: uppercase;
  color: var(--header-bar-dark) !important;
}
.session-plate .sp-number {
  font-family: 'Cinzel', serif;
  font-size: 2.2rem;
  color: var(--header-bar) !important;
  border: 2px solid var(--border);
  border-radius: 50%;
  width: 64px;
  height: 64px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  background: var(--table-head) !important;
}

/* ===== Session metadata bar ===== */
.session-meta {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1px;
  background: var(--border) !important;
  border: 1px solid var(--border);
  border-radius: 3px;
  overflow: hidden;
  margin-bottom: 22px;
}
.session-meta .meta-cell {
  background: #fbf5e3 !important;
  padding: 8px 10px;
  text-align: center;
}
.session-meta .meta-cell .m-label {
  font-family: 'Cinzel', serif;
  font-size: .55rem;
  letter-spacing: 1.5px;
  text-transform: uppercase;
  color: var(--ink-dim) !important;
  display: block;
  margin-bottom: 2px;
}
.session-meta .meta-cell .m-value {
  font-size: .92rem;
  color: var(--ink) !important;
}

/* ===== Callout boxes (reused) ===== */
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

/* ===== Key Events timeline ===== */
.ms-timeline {
  position: relative;
  margin: 14px 0 22px;
  padding-left: 26px;
  border-left: 2px solid var(--border);
}
.timeline-entry {
  position: relative;
  margin-bottom: 16px;
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
.timeline-entry .te-title {
  font-family: 'Cinzel', 'Georgia', serif;
  font-size: .95rem;
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

@media (max-width: 700px) {
  .session-meta { grid-template-columns: 1fr; }
}
</style>

<div class="ms-page">

<div class="session-plate">
  <div class="sp-title">
    <h1>Title</h1>
    <div class="sp-sub">A Chronicle of The Tyranny of Dragons</div>
  </div>
  <div class="sp-number">1-5</div>
</div>

<div class="session-meta">
  <div class="meta-cell"><span class="m-label">In-Game Date</span><span class="m-value">—</span></div>
  <div class="meta-cell"><span class="m-label">Real-World Date</span><span class="m-value">—</span></div>
  <div class="meta-cell"><span class="m-label">Location</span><span class="m-value">—</span></div>
</div>

## Recap

When the girls arrived back in Phandalin from the loggers camp, they quickly realised that things had gotten considerably worse. The town was now surrounded by camps of refugees and the displaced, with Phandalin seemingly becoming the last remaining refuge for the surrounding region. It was teetering on the edge of destruction.

Cryovain had attacked the town, destroying the home of a Goliath woman and killing her entire family.

Elsaangra, being the incredibly compassionate person she is, "investigated" the woman's house, only to be met with the bodies of the woman's family. Heh, Investigation complete without a scratch.

The girls decided that the best course of action was to rest, recover and resupply. While wandering through the hustle and bustle of Phandalin Town Square, Cuntita happened to bump into what appeared to be a Magistrate of the Lord's Alliance. Strangely, the man seemed to know who she was. Unfortunately, he was incredibly cryptic and vague about how or why he knew her, leaving the girlies with considerably more questions than answers.

The girls then heard rumours of the Tower of Storms and decided to head towards the coast to investigate.

When they arrived, they peered down from the cliffs and spotted a giant crab on the beach, they spoke to it. The giant crab could actually talk and offered them a reward if they could lay the ghost of his former captain friend to rest.

The girls agreed and found the ghost captain nearby and did something to that effect, gaining a new weapon in the process.

They continued along the coast, eventually crossing a narrow strip of land towards the lighthouse. Inside they discovered a corpse whose heart was still beating and extended all the way up to serve as the beacon of the lighthouse. After like 20 minutes of coaxing them into the building they discovered the corpse was still alive and turned out to be an Anchorite of Talos. 

They killed the Anchorite, and 2 of the girlies went upstairs to stare into the beacon-heart, blinding themselves temporarily in the process. But ducky gained a Charm of the Storm ability

The girls then travelled to the Dragon Barrow, where they discovered that the entire hill had been constructed over the skeleton of a massive three-headed dragon. The dragon was apparently an important symbol of the Alagondar Royal Family.

Inside the barrow they found a poem etched directly into bone, titled "Elegy for the First World."

They didn't really have time or want to sit around contemplating its meaning cause it is like way too long and is being edited atm to be nice and short, however, because by walking through an invisible wall they accidentally discovered a secret Dragon Cult base.

The girls proceeded to sneak through the Dragon Cult base, Mission Impossible style, silently taking out cultists one by one. One particular favourite method involved dunking Dragon Cultists into cauldrons filled with alchemically-altered dragon blood and watching them melt. They loved doing it so much they tried again at the end of this recap.

Deep within the base they discovered something considerably more personal: the coffin of Zaenerys' murdered cousin, Aegon. Although this coffin was empty.. except for the fresh Ducky poop that was dropped in.

Above the coffin was the motto of the House of Alagondar, although it had been strangely extended:

It read: "The Servitude of the Three-Headed Dragon; The One to be Murdered, the One to be a Monarch, and the One to be Mad."

The girls then overheard a sermon from one of the prominent priests within the Dragon Cult base. The priest spoke about the unexpected extinction of dragons and claimed that the only way to save the species was to bring Tiamat back from Avernus.

According to the priest, only then could the dragons be restored and the rightful rulers of the world endure.

The sermon was punctuated by monstrous cries from a nearby pit. After rescuing a  prisoner in the complex, they learned that his friends may have been taken and used as experimental subjects.

As they begun their measured retreat from the base they eventually the found the legendary Dragon Slayer sword within the barrow. Ducky then used some lightning charm powers and, somehow, became even more dragon-like and Zaenerys become a Drakewarden.

Petitearena also spent some more time investigating her forbidden tome and discovered that it belonged to Xarxes. Within the book she found a single mysterious word:

"Mantella."

Nobody knew what it meant. Naturally, it was written down and moved on from.

The girls then spent some time simply exploring the world, solving mysteries, and generally getting themselves involved in things.

Eventually they returned to Phandalin and began trying to piece together everything they had discovered. They made contact with the Harpers, who were able to provide information about what was happening in Neverwinter and directed the girls towards the town of Leilon.

They also learned more about the mysterious "Dark Spirit" that had attacked the Mere of Dead Men and caused devastation throughout the region during the Neverwinter Civil War.

The girls travelled to Leilon and immediately made their way to the library, where they began researching the Dragon Cult and everything else they had encountered.

There they found an image depicting a trifecta of Dragon Gods and also a nice recipe. They only knew the identities of two.

Petitearena also learned about her book was called the Oghma Infinium.

Then Cryovain attacked Leilon, and the girlies took the chance to test their mettle and fought it off, saving the town from destruction most likely.

Before they left the girls also learned about a mysterious Shaman living somewhere in the mountains who might know considerably more about everything that had been happening.

With yet another mystery added to the pile, the girls finally made their way towards Neverwinter.

Along the way they encountered the Flower Knight once again. Having previously crossed paths with this strange knight, the girls had already learned a little about it. 
It was hanging around a group of civilians moving towards Neverwinter.

Suddenly a group of tribal orcs emerged from the forest along the road.

It seemed that the Flower Knight had too learnt from the girlies; The girls and the Flower Knight immediately attacked them.

The tribal orcs were massacred.

These orcs were starving. They were emaciated and barely surviving, posing no threat and begging for some food. 

So the girlies moved on from that and took the newly dubbed "Rusty"  towards Neverwinter.

Eventually the girls arrived at the Sword Gate of Neverwinter, where they were stopped by the guards and informed that they would need to purchase a licence to enter the city. Surrounding the gate were prisoner carts waiting to enter Neverwinter, providing an ominous glimpse into the city's recently established prison trade. Following the Baldur's Gate Crisis, Neverwinter had begun taking prisoners and using them as labour to help rebuild the city from the Civil War and Eruption of Mount Hotenow, in preparation for any attacks from the Pirate Republic of Luskan. Refugees from Phandalin were also gathered outside the gates.

And then Cuntita spotted him. The Magistrate. The same mysterious man from Phandalin, entering the city and disppearing into a crowd again. As her eyes darted around they focused on something else nearby.

Down a hill, near a sewer entrance, stood an old friend. Dobby, A former companion from Cuntita's time in the Zhentarim. Dobby was apparently making deals with civilians, helping them enter the city using forged licences for only a third of the normal price.

When the girls approached him, Dobby was surprisingly friendly. He explained that he had effectively taken over Cuntita's old role within the Zhentarim and was now working in Neverwinter. He refused to say exactly what his current job was. All he would say was that whoever was paying him was paying **very** well.

After some negotiation, Dobby agreed to get all of the girls into the city for a total of thirty gold pieces.

Dobby then led them through the nearby sewer system. Unfortunately, they were ambushed by monsters. A massive battle broke out against a hulking abomination, and after a long fight the girls finally managed to bring the creature down.

When they inspected the bodies, they discovered something deeply disturbing. The creatures were Dragon Mutants. The influence of the Dragon Cult had reached Neverwinter.

Dobby explained that these beasts seemed to be becoming more and more common every day, although nobody seemed to know where they were coming from. The girls also discovered a note suggesting that a certain mage was working alongside the Dragon Cult to create these experiments; Another mystery.

Finally, the girls made it into Neverwinter proper. the first thing they did was find a tavern and get themselves some Aboba tea.

once they got the girls split up.

Two went back to loot the bodies (which they had forgotten), while the other two went shopping at the Pauper's Market. The looting expedition proved surprisingly fruitful. They found a strange ring, a dragon-shaped charm and a key. Zaenerys had a full-on Byakugan Naruto moment too.

Meanwhile, the shopping crew met Zaramush, the local blacksmith, who offered to create some new and exciting items and upgrade some of their existing equipment.

They also met a very flamboyant and funny gnome with a piercingly high voice that I cant remember how to do, but whatevs it will come back to me.

After all of that they head to the House of Knowledge... at closing time, and like try to semi-bully the Priest of Oghma right outside his place of work? Elsaangra is able to steal a couple of books while his back is turned because shes a thief thief thief. then they go home and go to sleep in their rented rooms that have been all very nicely personalised.

After waking up and heading downstairs they are ambushed... again! Kobolds start springing out of the floor boards, and two Zhentarim agents rush in with crossbows armed. a gnarly fight breaks out (mainly due to Cuntita putting her armour in for an upgrade.) Just as Cuntita is about to go down, a throwing knife flys past her head straight into the skull of a zhentarim agent. Inspecting the knife shows a rainy storm cloud etched into it, one of Dobby's favourite etchings.

Anyway the girlies then explore the holes that the Kobolds dug and follow it straight to another underground dragon cult base!! We do another mission impossible bit (because they are really really fun and cool to make as well). But then the girlies are spotted and have to fight their way out of the base! Elsaangra steals 5 chromatic vials found on a bench, and Petitearena uses her fireball necklace to immolate 3 dragon cultists all at one... just in time for Cuntita and Zaenerys to turn the corner, holding what could only be; George Miller (aka. Joji).

---

## Key Events

<div class="ms-timeline">

<div class="timeline-entry">
  <div class="te-title">Arrival at Greenest</div>
  <div class="te-body">The party crests the hill overlooking Greenest to find it under attack — a blue dragon circling overhead and raiders moving through the streets below.</div>
</div>

<div class="timeline-entry">
  <div class="te-title">The Mill</div>
  <div class="te-body">The party investigates the burning mill and rescues several townsfolk trapped inside before it collapses.</div>
</div>

<div class="timeline-entry">
  <div class="te-title">Reaching the Keep</div>
  <div class="te-body">Fighting through raiders in the streets, the party reaches Greenest Keep and reports to Governor Nighthill.</div>
</div>

<div class="timeline-entry">
  <div class="te-title">A Captive's Warning</div>
  <div class="te-body">A captured cultist reveals the raid is a diversion tied to something larger — the Cult of the Dragon is searching for something beneath the town.</div>
</div>

</div>

## NPCs Encountered

| Name | Role | Disposition | Notes |
|---|---|---|---|
| [[Governor Nighthill]] | Town Governor | Ally | Sheltering in the keep |
| [[Leosin Erlanthar]] | Harper Agent | Ally (captive) | Held by cultists, not yet rescued |
| — | Cult Raider | Hostile | Captured for questioning |

> [!note]- Loot &amp; Rewards
> | Item | Found By | Notes |
> |---|---|---|
> | | | |
> | | | |
>
> **Gold:** —

## Memorable Quotes

> "Insert a memorable line said at the table this session."
> — Character Name

> "Another one, if the table produced one."
> — Character Name

## Cliffhanger / Next Session

*Where the session ended and what the party is heading into next.*

## Trivia

- —

</div>
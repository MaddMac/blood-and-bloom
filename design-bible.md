# BLOOD AND BLOOM
### A Custom Magic: The Gathering Set — Design Bible v1.1

**Tagline:** *Two hungers. One world.*

**Elevator pitch:** Two factions wage war over the world's lifeblood. The **Lifeless Empire** practices **hemomancy** — blood magic that discounts its spells with life its enemies have already lost. The **Ironbloom Conservatory** is a veinless hive mind of plant and clockwork that **petrifies** what it touches, stunning creatures and lands into eternal stillness. New mechanics, new characters, new creature types, and a mirror-structure where every weapon has an answer.

**Status:** Wording-airtight (v1.1, September 2026). Batch-1 audit: 6 fixes across ~36 cards. Batch-2 audit: 6 fixes across 8 new cards, plus formal rust-counter and Husk-token definitions. Awaiting proxy playtesting.

---

## PART I — THE LORE

### The Lifeless Empire
A disciplined undead military power, commanded in the manner of old Rome. Its soldiers are not mindless — they are a legion, and they fight with doctrine. At its mythic root stands **Nekhros, the First Risen**, the progenitor from whom all hemomancy flows. Beneath him: **Tiberius, Grave-Legion Imperator**, the cold tactician whose very presence drains the living; **Lar'Otu**, the archon who treats entire planes as open veins; and **Mortach**, the titan of the lifeless.

The Empire does not conquer land. It harvests it. Every battle spills blood; every drop of spilled blood makes the next spell cheaper. To fight the Empire is to fuel it.

### The Ironbloom Conservatory
The opposition: beings **without veins**. A distributed plant-consciousness — the Bloom — running on bodies of grown clockwork and petrified root. No generals, no throne; every soldier a terminal, the forest the mind. Their fluid is **ichor**, golden sap that carries thought instead of oxygen.

The Bloom does not conquer either. It **reclaims**. Battlefields are overgrown, not occupied. Its doctrine, learned over a thousand simulated defeats:

- **Don't tap your creatures** — the weary are taken (Ironbloom Sapling).
- **Don't tap your lands** — the earth itself is listening (Enroot).
- **Don't attack** — attackers are fossilized (Terrasyl).
- **Don't die** — the fallen are worn as new bodies (Sylvos).

Where the Empire conquers, the Bloom *gardens*. Its cruelty is the cruelty of nature: patient, total, and utterly without malice.

### The War
Hemomancy needs blood. The Bloom has none to give — its life is insulated by **Rootbound**, and its bodies are wood, stone, and gear. So the Empire engineered the **Sanguine Membrane**: a living infection that seeps into veinless flesh and makes it *more* flammable than the living ever were. The Bloom answered with **petrification**: if the Empire will not stop moving, it will simply be stopped. Two infections, opposite directions. Two hungers, one world.

---

## PART II — MECHANICS REFERENCE

### New mechanics

**Siphon X** *(the signature mechanic)*
> *Siphon X (As you cast this spell, choose an opponent. It costs {1} less to cast for each 1 life that player has lost this turn from sources you controlled, up to X.)*

Hemomancy feeds on blood already spilled. Combat damage, drain effects, and direct life loss — anything *you* caused — banks a discount for your later spells. Design rulings:
- Only life lost **from sources you controlled** counts. Opponents' fetchlands, their combats, and their pain-lands bank you nothing.
- **Multiple instances stack.** Each Siphon counts the same life loss independently, each capped at its own X. (Printed Siphon 3 + granted Siphon 2 with 4 life lost = 5 off.)
- Each instance **chooses its own opponent** — they may be different opponents.
- Only **generic mana** is reduced. Colored pips are never discounted: no free spells, no mana-positive loops.
- **Choosing is not targeting.** Hexproof does nothing against Siphon. (Rootbound's "can't be chosen" does — different axis.)
- If every opponent has Rootbound, you choose no one and get no discount.

**Rootbound** *(the Bloom's insulation)*
> *You can't be chosen for Siphon abilities, and life you lose isn't counted for Siphon.*

Their blood cannot be spilled or spent. Note: Rootbound does **not** stop membrane counters from being placed — the membrane is the designed answer.

**Petrified** *(the Bloom's weapon — a rules-level status)*
> *A permanent with a petrification counter on it can't attack or block, and it doesn't untap during its controller's untap step.*

Works on creatures *and* lands. A petrified land can still be tapped **once more** — it simply never untaps afterward. Petrified creatures can still be sacrificed and still have static abilities; only attacking, blocking, and untapping are lost.

**Membrane counter** *(the Empire's answer to Rootbound)*
> *A player with one or more membrane counters ignores Rootbound. Life lost by a player with a membrane counter counts twice for Siphon abilities.*

The membrane doesn't just break immunity — it makes compromised bodies fuel Siphon **better** than living ones. Doubling applies **before** the Siphon cap: 3 life lost + membrane counter = counts as 6, so Siphon 5 discounts the full 5.

**Enroot** *(the Bloom's land weapon)*
> *Whenever an opponent taps a land for mana, put a petrification counter on that land.*

**Paradigm** *(blood magic's echo)*
> *When this spell resolves, exile it. At the beginning of your precombat main phase, you may cast a copy of this card from exile without paying its mana cost.*

The spell refuses to die — aggressively, unconditionally.

**Perennial** *(the Bloom's regrowth — Paradigm's mirror)*
> *When this spell resolves, exile it. At the beginning of your precombat main phase, if you control a Plant or Construct, you may cast a copy of this card from exile without paying its mana cost.*

The seed needs a tended garden. No Plants or Constructs, no regrowth. Same skeleton as Paradigm, opposite philosophy: not defiance of death, but the patience of spring.

### Tokens

**Blood token** (official): *Artifact token with "{1}, {T}, Discard a card, Sacrifice this artifact: Draw a card."*

**Ichor token**: *Artifact token with "{1}, {T}, Sacrifice this artifact: You gain 3 life."* Blood draws; ichor heals. Same skeleton, opposite philosophy.

**Rust counter** *(Vorthax's corrosion)*
> *Activated abilities of artifacts with rust counters on them cost {2} more to activate.*

Corrosion is inherent to the counter, not to Vorthax — the tax persists even if he leaves the battlefield. Multiple rust counters on one artifact still tax only {2} (one class-based static, not one instance per counter). As defined, the tax hits mana abilities too — a rusted Sol Ring is a paperweight. That's the submitted design and arguably the point of corrosion, but it's the strongest version: flagged as a playtest watch.

**Husk token** *(the Bloom's instantiation)*
> *A Husk token is a 1/1 colorless Husk creature token with "You may have this token enter the battlefield as a copy of any creature you control, except it isn't legendary and it's a Husk in addition to its other types."*

The Bloom doesn't travel — it instantiates. The copy choice is made as the token enters (a replacement effect; choosing isn't targeting, so hexproof is irrelevant), and the "isn't legendary" clause dodges the legend rule by design. Husk creation stays gated on the rootbound network — petrification, Plants/Constructs, host bodies — so it reads as Bloom machinery, not generic cloning.

### Returning mechanic

**Eminence** — *As long as [this] is in the command zone or on the battlefield, [effect].* Returns on Nekhros, the First Risen, in the tradition of the "Ur-" progenitor line.

---

## PART III — THE CARDS (FINAL WORDING)

### The Lifeless Empire

```
Nekhros, the First Risen — {4}{W}{U}{B}{R}{G}
Legendary Creature — Zombie Avatar                        Mythic
Eminence — As long as Nekhros is in the command zone or on
the battlefield, Zombie spells you cast cost {1} less.
Menace
Whenever one or more Zombies you control attack, each
opponent loses X life, where X is the number of attacking
Zombies. You gain life equal to the total life lost this way.
10/10
```
*The progenitor. The source of hemomancy itself. Your zombie discount is live from turn zero; every attack drains, gains, and banks Siphon fuel for post-combat spells.*

### The Aspects of Nekhros

Nekhros is the unknowable progenitor — "a god that hasn't finished arriving." The aspects are named manifestations: Nekhros wearing shapes. Each has its own name, so all five coexist with Nekhros himself under the legend rule — the intended "progenitor and aspect, together" Commander moment.

```
Veyla, Death-Knight of Nekhros — {3}{W}{B}
Legendary Creature — Zombie Knight                        Mythic
Vigilance
Other Zombie creatures you control get +1/+1.
At the beginning of combat on your turn, you may return target
Zombie card from your graveyard to the battlefield tapped and
attacking.
4/5
```
*The legion's general. Repeatable, cost-free, every-combat reanimation with no exile clause — the strongest effect in the batch-2 audit and the #1 playtest watch. (Reanimated Zombies were never declared as attackers, so they don't trigger Nekhros's attack drain — but their combat damage banks Siphon normally.)*

```
Umbriss, Shade of Nekhros — {2}{U}{B}
Legendary Creature — Zombie Shade                          Mythic
Umbriss can't be blocked.
{B}: Umbriss gets +1/+1 until end of turn.
Whenever Umbriss deals combat damage to a player, that player
discards a card.
3/3
```
*A formless walking eclipse, not a humanoid. Classic shade-pump plus saboteur discard — strong, fair mythic.*

```
Malachar, Lich of Nekhros — {3}{B}{B}
Legendary Creature — Lich                                   Mythic
Indestructible
When Malachar enters the battlefield, put a phylactery counter
on an artifact you control.
When you control no permanents with phylactery counters on
them, sacrifice Malachar.
{B}, Pay 2 life: Draw a card.
4/4
```
*The Phylactery Lich homage: indestructible until his vessel breaks — and indestructible doesn't stop the sacrifice. (Batch-2 critical fix: the dependency was written as a nonfunctional static "If"; corrected to the state trigger.)*

```
Ghorvath, Amalgam of Nekhros — {3}{B}{R}
Legendary Creature — Zombie                                 Mythic
Trample
When Ghorvath enters the battlefield, amass Zombies 3. (Put
three +1/+1 counters on an Army you control. If you don't
control one, create a 0/0 black Zombie Army creature token
first.)
Whenever another Zombie you control dies, amass Zombies 1.
5/5
```
*A walking battlefield of fused armor and banners. The Zombie Army is itself a Zombie — when it dies, it rebuilds from its own corpse. Self-sustaining, not infinite: each cycle needs an actual death.*

```
Vorthax, Caustic Haze of Nekhros — {2}{R}{G}
Legendary Creature — Zombie Elemental                       Mythic
Flying
Whenever a creature an opponent controls dies, put a -1/-1
counter on target creature.
At the beginning of your upkeep, put a rust counter on target
artifact an opponent controls.
4/4
```
*Caustic haze: a one-sided plague engine (the -1/-1 spread re-triggers off its own kills, terminating when the board is empty) plus the rust tax. Punishing against go-wide and artifact decks — playtest watch.*

```
Tiberius, Grave-Legion Imperator — {1}{W}{U}{B}
Legendary Creature — Zombie Soldier                        Mythic
At the beginning of your upkeep, each opponent loses 1 life.
Legio Mortis — Whenever you attack, you may sacrifice another
creature. When you do, choose one —
• Create two 2/2 black Zombie creature tokens that are tapped
  and attacking.
• Draw a card.
• The next spell you cast this turn has Siphon 3.
3/4
```
*Cold, empty, calculating. His upkeep drain is his gaze made mechanical — Siphon always has at least 1 banked before you've done anything. (A Mardu {1}{R}{W}{B} variant exists as an alternate.)*

```
// Front
Lar'Otu, Sanguine Archon — {3}{B}{B}
Legendary Creature — Zombie Wizard                         Mythic
Whenever an opponent loses life, you may look at the top card
of that player's library. You may exile it. You may cast it for
as long as it remains exiled, and you may spend mana as though
it were mana of any color to cast it.
At the beginning of your end step, if an opponent lost 5 or more
life this turn, transform Lar'Otu.
3/5

// Back
Lar'Otu, Lord and Ruler
Legendary Planeswalker — Lar'Otu [WUB]
Hexproof
[+2]: Each opponent loses 2 life and you gain 2 life. Create a
Blood token.
[-3]: Exile target instant or sorcery card from a graveyard. It
gains Paradigm.
[-7]: You get an emblem with "Whenever you gain life, each
opponent loses that much life."
Loyalty: 4
```
*Theft engine into ascension. The back face's abilities borrow from Kaya, Intangible Slayer (hexproof, mass-drain +2) and Professor Dellian Fel (the lifegain-to-drain emblem, with one word changed: "target" → "each"). The +2/emblem/Nekhros loop is verified loop-free.*

```
Mortach, Titan of the Lifeless — {4}{B}{B}
Legendary Creature — Zombie Giant                          Mythic
Deathtouch
When Mortach enters the battlefield, create two 2/2 black
Zombie creature tokens.
Whenever Mortach attacks, create two 2/2 black Zombie creature
tokens.
Zombie tokens you control have deathtouch.
6/6
```
*The legendary zombie Grave Titan players have asked for for years. One upgrade: his deathtouch extends to every zombie token.*

```
The Sanguine Crucible — {4}
Legendary Artifact                                        Mythic
Instant and sorcery spells you cast have Siphon 2.
{T}: Target opponent loses 1 life.
```
*The engine that spreads Siphon beyond its printed card pool. Stress-tested: only generic is reduced, only your sources count, tap is once-per-turn single-target. The dream curve (Crucible → 5 zombies connect → Awakening for {B}{B}{B}) is a three-piece setup that folds to removal — a payoff, not a break.*

```
Sanguine Membrane — {1}{B}{B}
Enchantment                                                 Rare
Whenever a Zombie you control deals combat damage to a player,
put a membrane counter on that player.
Players with membrane counters ignore Rootbound. Life lost by
a player with a membrane counter counts twice for Siphon
abilities.
```

```
Membranous Infestation — {2}{B}
Sorcery                                                     Rare
Siphon 2
Put a membrane counter on each opponent who lost life this
turn. Create a 2/2 black Zombie token.
```
*Only membranes opponents who've already bled — it obeys the spilled-blood rule.*

```
Exsanguinate the Fallen — {2}{B}{B}
Sorcery                                                   Uncommon
Siphon 3
Return target Zombie card from your graveyard to the
battlefield. Each opponent loses 2 life.
```
*The workhorse: reanimation plus a drain that banks your next Siphon.*

```
Awakening of the First Risen — {5}{B}{B}{B}
Sorcery                                                    Mythic
Siphon 5
Each opponent loses X life, where X is the number of Zombies
you control. Then return each Zombie card from your graveyard
to the battlefield.
```
*The capstone. Drain the table on the size of your army, then stand the entire graveyard back up.*

```
Cruor Vat of the Imperator — {2}{B}
Legendary Artifact                                          Rare
When Cruor Vat of the Imperator enters, target opponent
chooses one —
• You create a Blood token.
• That player loses 2 life.
{T}, Sacrifice a Blood token: Add {B}{B}.
{3}, Sacrifice three Blood tokens: Target Zombie or Vampire
gains indestructible and lifelink until end of turn.
```
*The entry choice now feeds Siphon (the 2 life is from your source). Blood becomes black mana; three blood buys near-immortality.*

```
Sanguine Exsanguination Seminar — {3}{W}{U}{B}
Sorcery — Lesson                                            Rare
Siphon 3
Each opponent loses X life, where X is the number of Zombies
you control. You gain life equal to the total life lost this way.
Create a 2/2 black Zombie token for each opponent who lost
life this way.
```

```
Covenant of the Lifeless Empire — {3}{W}{U}{B}
Sorcery                                                    Mythic
Siphon 4
Choose one —
• Create three 2/2 black Zombie tokens that are tapped and
  attacking.
• Exile target spell. You may cast it for as long as it remains
  exiled, and you may spend mana as though it were mana of
  any color to cast it.
If you control a permanent named Tiberius, Grave-Legion
Imperator and a permanent named Lar'Otu, Sanguine Archon or
Lar'Otu, Lord and Ruler, choose both instead.
```

```
Legion Sanguimancer — {2}{U}{B}
Creature — Zombie Wizard                                  Uncommon
Siphon 2
Whenever you sacrifice a Blood token, each opponent loses
1 life and you create a 2/2 black Zombie creature token.
3/2
```
*Every blood spent banks your next Siphon — the loop the deck wants.*

```
Drain the Defiant — {3}{B}
Sorcery                                                     Common
Siphon 3
Destroy target creature.

Tides of Cruor — {2}{U}
Sorcery                                                     Common
Siphon 2
Draw two cards.

Decree of the Lifeless — {3}{W}{B}
Sorcery                                                       Rare
Siphon 3
Each opponent sacrifices a creature. Create a 2/2 black Zombie
creature token for each creature sacrificed this way.
```

```
The Final Tally — {3}
Artifact                                                      Rare
Whenever a creature dies, put a tally counter on The Final
Tally.
{2}, {T}: Double the number of tally counters on The Final
Tally.
When there are twenty or more tally counters on The Final
Tally, each opponent loses 10 life and you create ten 2/2
black Zombie creature tokens.
```
*The Millennium Calendar, rebuilt for zombie arithmetic. Every death — tokens included, yours included — feeds the count; the doubler turns a grind into a countdown. Corner case for the diary: at twenty-plus counters with a "can't lose" effect on board, the payoff becomes a mandatory loop and the game is a draw.*

```
Edict of Stillness — {4}{W}{W}
Sorcery                                                     Mythic
Until your next turn, creatures can't attack you unless their
controller pays {2} for each creature they control that's
attacking you.
Paradigm (When this spell resolves, exile it. At the beginning
of your precombat main phase, you may cast a copy of this
card from exile without paying its mana cost.)
```
*The Chronomantic Escape rework, Empire-flavored. The hard lock was rejected — a free, recurring, exile-based lock is effectively a permanent, uninteractable creature-lock, and raising only the initial cost doesn't fix the play pattern. The approved version is a recurring Ghostly Prison: {4}{W}{W} once, then a standing attack tax every precombat main phase. Strong, staple-worthy, not a lock.*

### The Ironbloom Conservatory

```
Terrasyl, Voice of the Bloom — {2}{W}{B}{G}
Legendary Creature — Plant Construct                       Mythic
Rootbound — You can't be chosen for Siphon abilities, and life
you lose isn't counted for Siphon.
Construct and Plant creatures you control get +1/+1.
Whenever a creature an opponent controls deals combat damage
to you, put a petrification counter on it.
4/5
```
*The Bloom's defense: its controller is insulated, its tribe is anthemed, and attackers are fossilized. (Petrified attackers stay tapped forever under the final rules.)*

```
Sylvos, Bloom Egregore — {3}{W}{B}{G}
Legendary Creature — Plant Construct                       Mythic
Whenever a Plant or Construct you control deals combat damage
to a player, put a petrification counter on up to one target
creature that player controls.
Whenever a creature with a petrification counter on it dies, you
may return it to the battlefield under your control. If you do,
it becomes a Plant Construct in addition to its other types.
4/6
```
*Egregore: a collective psychic entity. The Bloom's advance — petrify what you hit, then wear their bodies. Your zombies don't just die against the Bloom; they come back wrong.*

```
Calcifex, Bloom Titan — {5}{G}{G}
Creature — Plant Construct                                 Mythic
Trample
Enroot
Whenever a land with a petrification counter on it becomes
tapped, create an Ichor token.
7/7
```
*The filed-off Vorinclex homage: same weight class, but instead of doubling your mana it drinks theirs — every land they tap sleeps forever and pays you an ichor on the way down.*

```
Ironbloom Warden — {3}{W}
Creature — Construct                                      Uncommon
Vigilance
Whenever a creature with a petrification counter on it dies,
create an Ichor token.
3/4
```
*The harvester: your statues are rendered down into ichor. Reclamation made literal.*

```
Petrified Rebuke — {1}{W}
Instant                                                     Common
Counter target spell with Siphon. Create an Ichor token.
```

```
Rootbound Tithe — {2}{W}
Enchantment                                               Uncommon
Spells with Siphon cost {2} more to cast.
```
*The tax applies before Siphon's reduction — it really bites.*

```
The Great Petrification — {5}{W}{G}
Sorcery                                                    Mythic
Put a petrification counter on each creature target player
controls. Create an Ichor token for each of those creatures.
```
*The Bloom's answer to Awakening of the First Risen: it doesn't destroy the legion, it gardens it — and every statue becomes fuel.*

```
Ironbloom Sapling — {1}{G}
Creature — Plant                                            Common
{T}: Put a petrification counter on target tapped creature.
1/2
```
*The Bloom takes the weary. Tapped-out is vulnerable — permanently.*

```
Ironbloom Deep-Rooter — {3}{G}
Creature — Plant                                          Uncommon
Enroot
3/4
```

```
Petrify the Leylines — {4}{G}{G}
Sorcery                                                     Rare
Put a petrification counter on each land target player controls.
```
*The nuclear option. Permanent land-stun is the least forgiving thing in Commander — playtest will tell whether it creates grudges or stories.*

```
Ironbloom Flakvine — {2}{G}
Creature — Plant                                          Uncommon
Reach
{T}, Sacrifice a creature with a petrification counter on it:
Ironbloom Flakvine deals 3 damage to target creature with
flying.
2/3
```
*Anti-air artillery: it hurls your own statues. Every Sylvos assimilation doubles as reloading.*

```
Drag Them Down — {2}{G}
Instant                                                     Common
Target creature with flying loses flying until end of turn. Put
a petrification counter on it.
```
*The vine-whip: grabbed mid-air, petrified, crashed — permanently grounded, permanently tapped.*

```
Uprising of the Bloom — {2}{G}
Enchantment                                                 Rare
When Uprising of the Bloom enters, if you control a creature
with power 4 or greater, draw a card.
Creatures you control with power 4 or greater have trample
and reach.
Whenever a creature with power 4 or greater enters the
battlefield under your control, draw a card.
```
*Garruk's Uprising with one added word: reach. The Bloom's giants swat.*

```
The Thousand Roots — {7}
Legendary Artifact                                        Mythic
Your maximum hand size is ten.
At the beginning of your end step, if you have fewer than ten
cards in hand, draw cards equal to the difference.
{2}, {T}: Put a petrification counter on target tapped creature.
```
*The Ten Rings, Bloom-flavored: the refill engine stapled to the grasp of the forest.*

```
Deep Roots Reclaim — {3}{G}
Sorcery                                                   Uncommon
Perennial
Put a petrification counter on target creature. Create an
Ichor token.
```
*It keeps coming back every turn the garden stands.*

**The Bloom cycle** — *The Bloom ___* enchantments, the faction's signature line:

```
The Bloom Remembers — {1}{G} — At the beginning of your upkeep, scry 1.
The Bloom Listens — {2}{G} — Whenever an opponent taps a land for mana,
  you may draw a card unless that player pays {1}. (Rhystic Study, with roots —
  renamed from "Bloom Study" to avoid the contention.)
The Bloom Hungers — {1}{B}{G} — At the beginning of your upkeep, each opponent
  loses 1 life for each petrification counter on creatures they control.
  (Corrected from permanents — lands as fuel was unanswerable.)
The Bloom Dreams — {2}{G} — At the beginning of your upkeep, choose one —
  Scry 2; create an Ichor token; or put a petrification counter on target
  tapped creature.
The Bloom Composts — {1}{G} — Whenever an opponent casts a spell from exile,
  create an Ichor token. (Their Paradigm echoes fertilize you. The Bloom doesn't
  counter their magic — it mulches it.)
```

### Cross-faction

```
Harvest of the Fallen — {3}{B}{G}
Enchantment                                                   Rare
At the beginning of your end step, if three or more creatures
died this turn or a player lost the game this turn, you may
sacrifice Harvest of the Fallen. If you do, search your library
for up to two creature cards, put them onto the battlefield,
then shuffle.
```
*The Defense of the Heart variant. The trigger moved from upkeep to end step at the designer's insistence — "this turn" has almost no deaths to count before upkeep. Note: "this turn" at your end step counts only your turn's deaths (Vorthax kills on opponents' turns don't count); the card is self-enabling through your own wipes, combat, and sac outlets. One-shot, gated, strong in multiplayer — fair.*

---

## PART IV — DESIGN DIARY (what changed and why)

- **Siphon 1.0 → 2.0.** The original made an opponent lose life *and* converted it to mana — two benefits, no setup cost. The reframe: Siphon now discounts off life *already lost this turn*. Hemomancy feeds on spilled blood; combat and drains become the setup.
- **Caster's sources only.** Early wording counted any life loss. Restricting to the caster's own sources pulls the reins: no profiting off fetchlands or opponents' combats.
- **Tiberius: Mardu → Esper.** Red had low value in the deck's direction; Esper made him cold, empty, calculating — his upkeep drain is his gaze made mechanical. The Mardu original is preserved as an alternate variant.
- **Lar'Otu's promotion.** The inherited planeswalker netted +5 loyalty on its +2. Rebuilt as a Liliana-style double-faced card: theft-engine creature into an ascended walker, borrowing hexproof and the mass-drain +2 from Kaya, Intangible Slayer and the lifegain-emblem from Professor Dellian Fel (one word changed: "target" → "each").
- **The Bloom's identity.** Started as "veinless phytomancers." The Destiny's-Vex parallel (fluid minds piloting machine bodies, collective consciousness, world-conversion) was recognized and filed off: no names copied, all flavor rebuilt as the Bloom.
- **Petrified, revised.** Originally only stopped attacking/blocking. Gaining "doesn't untap" unified creatures and lands under one status and enabled Enroot.
- **Bloom Study → The Bloom Listens.** "Study" tread too close to Rhystic Study; the Bloom doesn't study, it listens. This founded *The Bloom ___* cycle.
- **The Bloom Hungers, corrected.** Counted petrification counters on all permanents — with Enroot stunning lands, that was 5–10 unanswerable drain per turn. Now creatures only.
- **Covenant naming fix.** "Control both Tiberius and Lar'Otu" fails under real rules for double-faced cards; now names all three faces.
- **The five aspects (batch 2).** Nekhros stays the unknowable five-color progenitor; the aspects are named shapes he wears — one per color identity (W, U, B, BR, RG) — so all six can share a battlefield under the legend rule. Veyla answers the set's male-skewed face cards as the legion's general: lore-organic, not tokenistic.
- **Malachar's critical fix.** The phylactery dependency was written as a static "If you control no…" — nonfunctional, since static abilities can't perform sacrifices. Corrected to Phylactery Lich's state trigger ("When you control no…"). The batch-2 audit's most important catch.
- **Rust counters, defined.** Vorthax's tax moved into the counter definition per the petrification/membrane precedent — future rust cards inherit it automatically. Applies to mana abilities as written; playtest will judge whether that's corrosion or cruelty.
- **Husk tokens, formalized.** The Bloom's copy-hosts: a replacement effect, so "any creature" not "target creature." Gated on the rootbound network by design.
- **Edict of Stillness: lock rejected, tax chosen.** A free recurring exile-based hard lock is effectively a permanent, uninteractable creature-lock; cost alone can't fix the pattern. Option B — a recurring Ghostly Prison tax — approved as the white-staple path.
- **The Final Tally's draw loop.** Twenty-plus counters plus a "can't lose" effect = mandatory non-terminating loop, game is a draw. Corner case, diary-noted, not a design flaw.
- **Lar'Otu emblem corrected to −7.** The v1.0 card list printed −8; the design intent was always −7.

## PART V — RULINGS FAQ

1. **All my opponents have Rootbound. What does my Siphon spell do?** You choose no one and get no discount. That's the intended hose — bring the Membrane.
2. **My spell has Siphon 3 and the Crucible grants Siphon 2. Opponent lost 4 life. Total discount?** 5. Each instance counts the same 4 life independently (3 + 2), each capped at its own X. The instances may even choose different opponents.
3. **Opponent lost 3 life and has a membrane counter. My Siphon 5 spell?** The 3 counts as 6 (doubling before the cap), so Siphon 5 discounts the full 5.
4. **Does my opponent cracking a fetchland bank my Siphon?** No — only life lost from sources *you* controlled.
5. **Wound Reflection doubles their life loss at end of turn. Does Siphon see it?** Next turn's Siphon spells do — the extra loss came from your enchantment.
6. **Tiberius grants "the next spell has Siphon 3" to a spell that already has Siphon 2?** They stack (see #2). The grant is consumed on cast.
7. **Does hexproof stop Siphon choosing?** No — choosing isn't targeting. Rootbound's "can't be chosen" does stop it. Different axes.
8. **Sylvos returns my opponent's petrified creature. What is it?** It enters with no counters (counters vanish on zone change), under your control, a Plant Construct in addition to its other types, indefinitely.
9. **Can a petrified land ever tap again?** Once more — then it never untaps.
10. **Lar'Otu's -3 grants Paradigm to an opponent's graveyard spell. Who casts the free copies?** You do — "you" is Lar'Otu's controller. The original stays exiled; copies recur every precombat main phase.
11. **Veyla reanimates a Zombie tapped and attacking. Does Nekhros's attack trigger see it?** No — it was never declared as an attacker. It still deals combat damage, which banks Siphon normally.
12. **Malachar enters with no artifacts out. What happens?** The ETB does nothing, then the state trigger sacrifices him — identical to Phylactery Lich. Indestructible doesn't save him.
13. **Do rust counters fall off when Vorthax leaves?** No — the tax is inherent to the counter. Multiple rust counters on one artifact still tax only {2}.
14. **How do Husk tokens work?** As the token enters, you may have it enter as a copy of any creature you control — except it isn't legendary, and it's a Husk in addition to its other types. Decline and it's a 1/1 colorless Husk.
15. **The Final Tally hits twenty counters while someone can't lose the game?** The payoff re-fires as long as the condition is true — with no way to end it, the game is a draw. Corner case; remove the Tally first.
16. **Harvest of the Fallen — whose deaths count?** Only deaths during your turn, checked at your end step. It's meant to be self-enabled: your wipe, your combat, your sac outlets.

## PART VI — FOR THE COMMUNITY

This set is a starting point, not a finished product. It's built for proxies, playtesters, and tinkerers.

**Try to break it.** The interactions we most want tested:
- Siphon against the eternal card pool (Wound Reflection, Furnace of Rath, Exquisite Blood effects).
- Whether the Crucible's global Siphon grant has a line we missed.
- Whether Enroot/permanent land-stun (Calcifex, Petrify the Leylines) creates stories or grudges at real tables.
- The Nekhros/Lar'Otu/Tiberius engine pieces in real Commander games.
- Veyla's cost-free every-combat reanimation — the audit's #1 playtest watch.
- Vorthax's rust tax, especially against mana rocks — corrosion or cruelty?
- Paradigm recursion lines (Edict of Stillness every turn; Lar'Otu's -3 on real cards).
- Harvest of the Fallen self-enable combos in multiplayer.

**Play it.** A 100-card Nekhros Commander pre-con (`decklist-nekhros-commander.md`) and a step-by-step playtest manual (`playtest-manual.md`) ship with the set — download, proxy, and report back.

**Build on it.** Open design space, deliberately left fertile:
- More Siphon spells in every color (white's tax-counterspell space is barely touched).
- More "should-be-legendary" upgrades (the Mortach treatment for other iconic non-legendaries).
- *The Bloom ___* cycle wants a sixth and seventh verse.
- Draft archetypes for a real limited format.
- **Set two:** two new factions are sketched — the **Starborne** (cosmic elves; ally to one faction, existential threat to the other) and a **nomadic insectoid hunter-pack** species (the Bloom owns "hive mind," so these are individualist packs — same tree, opposite philosophy). Names and designs open.

**Ground rules for contributors:** preserve each faction's core fantasy (hemomancy *must* feed on the opponent's spilled life; the Bloom *must* remain veinless and patient). Fix balance problems around the fantasy, never by replacing it.

**Reimagine the art.** Every piece so far is first-pass proxy art, generated as direction — not canon. Submit original reimaginings of any card; the strongest takes get curated into the set's gallery. Per-card art briefs (mood, palette, composition notes) live in the repo's art folder.

*Designed by Anthony MacDuff, with design counsel. v1.1 — September 2026.*

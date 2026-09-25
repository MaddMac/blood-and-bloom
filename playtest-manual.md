# BLOOD AND BLOOM — Playtest Manual v1.1
### *Two hungers. One world.*

This manual gets a playtest table from zero to breaking the set as fast as possible. Read the faction primer for whatever you're playing, skim the Siphon worked example once, then shuffle up.

**In this packet:** the design bible (`blood-and-bloom-design-bible.md` — every card, every ruling), the Nekhros Commander pre-con (`decklist-nekhros-commander.md` — 100 cards, importable), and this manual.

---

## 1. Proxying the pre-con

The decklist is 94 real cards + 6 custom cards (the commander Nekhros, the First Risen, plus the five aspects: Veyla, Umbriss, Malachar, Ghorvath, Vorthax). Proxy the six customs as printouts in sleeves over bulk cards. Everything else is a real, purchasable Magic card — check the decklist for exact names.

For set-vs-set testing (Empire vs. Bloom constructed decks), proxy from the bible's card list. There is no curated Bloom pre-con yet — building one from the bible's Bloom section is itself useful playtest data.

---

## 2. Faction primers

### The Lifeless Empire — hemomancy

**The core loop:** hurt them first, then cast cheap. Siphon discounts your spells based on life *that opponent* has lost *this turn* from *sources you controlled*.

**Worked example.** Turn 5. You attack with three Zombies; all connect. Each opponent loses 3 life (Nekhros isn't even out — this is just combat). Post-combat, you cast **Exsanguinate the Fallen** ({2}{B}{B}, Siphon 3): choose the opponent who lost the 3 life → it costs {1} less per life lost, up to 3 → you pay {B}{B}. Net: a 5-mana reanimate-and-drain for 2 mana, because you spilled blood first. Then its own "each opponent loses 2 life" banks fuel for your *next* spell.

**Rules that trip people up:**
- Choosing the opponent for Siphon is **not targeting** — hexproof does nothing. (Rootbound's "can't be chosen" does.)
- Only **generic mana** is discounted. Colored pips are never reduced.
- Each Siphon instance counts the same life loss **independently**, each capped at its own X.
- Tiberius's upkeep drain means you *always* have at least 1 banked before doing anything.

**What the Empire wants:** go wide early, connect, then chain discounted spells post-combat. Your life total is a resource — the drains refill it.

### The Ironbloom Conservatory — petrification

**The core loop:** punish everything the opponent does. The Bloom's doctrine, learned over a thousand simulated defeats:

- **Don't tap your creatures** — the weary are taken (Ironbloom Sapling).
- **Don't tap your lands** — the earth is listening (Enroot: tapping a land for mana puts a petrification counter on it).
- **Don't attack** — attackers are fossilized (Terrasyl).
- **Don't die** — the fallen are worn as new bodies (Sylvos).

**What "petrified" means:** a permanent with a petrification counter can't attack or block and doesn't untap during its controller's untap step. Works on creatures *and* lands. A petrified land taps **once more**, then sleeps forever.

**What Rootbound means:** you can't be chosen for Siphon, and your life loss doesn't count for it. The Empire's answer is the **Sanguine Membrane** — membrane counters ignore Rootbound and make that player's life count *double* for Siphon.

**What the Bloom wants:** patience. Every petrification counter is permanent. You don't win fast — you win when the opponent has nothing left that untaps.

### The five aspects (Nekhros Commander)

Nekhros himself usually stays in the command zone — his eminence discounts every Zombie from turn zero. The aspects are the on-board threats: **Veyla** (reanimates a Zombie tapped and attacking every combat — note: these were never *declared* as attackers, so they don't trigger Nekhros's drain, but their damage banks Siphon), **Umbriss** (unblockable saboteur), **Malachar** (indestructible card draw while his phylactery artifact survives), **Ghorvath** (the self-rebuilding Zombie Army), **Vorthax** (plague-spread plus rust counters that tax artifact activations, *including mana abilities*).

---

## 3. Running a session

**Minimum useful session:** 3 games with the same decks, rotating who plays what at least once. Commander multiplayer (4 players) is the primary target; 1v1 is secondary data.

**Record per game:**
- Turns taken, winner, and how they won (combat / drain / combo / concession).
- **MVP card** (overperformed) and **most confusing card** (rules questions, misplays).
- Any turn where a player couldn't meaningfully act for 2+ consecutive turns (non-game flag).
- Siphon gut-check each game: did discounts feel *earned* (set up by combat/drains) or *free*?

**Then answer these five questions** (this is the feedback form — copy, answer, send back):

1. Did Siphon ever discount a spell to a cost that felt wrong? Which spell, what board state?
2. Did any single card create a non-game? Which one, and could the table have answered it?
3. Did petrification feel oppressive or fair? Did Enroot change how anyone played their lands?
4. Which aspect over- or underperformed? (Veyla is our #1 watch — was she?)
5. Would you play this set again as-is? What one change would you make first?

---

## 4. Break bounties

Named targets. Break one, report exactly how, and you did the set a service:

- **Break Siphon.** Find a line — with real, printed Magic cards — that turns the discount into something the cost can't justify. (Wound Reflection, damage doublers, and lifegain-conversion loops are the known suspects; surprise us.)
- **Break Paradigm.** Edict of Stillness recurs every precombat main phase; Lar'Otu's −3 grants Paradigm to real cards. Find the copy that shouldn't exist.
- **Break Harvest of the Fallen.** Self-enable it faster or more reliably than intended in multiplayer.
- **Break Vorthax.** The rust tax hits mana abilities — is there a lock? Is it miserable?
- **Break the Final Tally.** Race it, double it, or force the can't-lose draw loop on purpose.

**Ground rule for all demolition:** report the *exact* sequence (cards, board state, turn order). "It's broken" is noise; "turn 6 with X, Y, Z on board does this" is data.

---

## 5. Reporting back

File break reports, confusion reports, and art submissions as issues on the repo (link in the Reddit post). Include: set version (v1.1), format played, the five answers above, and any break-bounty sequences.

*Two hungers. One world. Get your hands dirty.*

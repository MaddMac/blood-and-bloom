# Blood and Bloom — Airtight Consistency Pass
**Date:** 2026-09-23 | **Auditor:** subagent audit (not new design)
**Method:** Every card checked against the FINAL mechanic definitions supplied in the task. Verdicts: CLEAN (no change), MINOR (polish), FIX NEEDED (must change). All proposed fixes are minimal wording adjustments only.

---

## 1. CARD-BY-CARD WORDING CHECK

### Lifeless Empire

**1. Nekhros, the First Risen** — MINOR (polish)
Eminence matches the real template (Ur-Dragon/Ur-Sphinx). Attack trigger is understandable but the double "X life" sentence is clumsy. Corrected:
> Whenever one or more Zombies you control attack, each opponent loses X life, where X is the number of attacking Zombies. You gain life equal to the total life lost this way.
(The life loss is from Nekhros's ability — a source you control — so it banks Siphon. Intended.)

**2. Tiberius, Grave-Legion Imperator (Esper)** — CLEAN
Upkeep drain and Legio Mortis are templated correctly. Note: "The next spell you cast this turn has Siphon 3" — recommend including Siphon's reminder text on the card at least once in the final file, since it's a grant (not strictly required by rules, but players need it). The grant is consumed when the spell is cast, stacks with printed Siphon per the stacking ruling.

**3. Lar'Otu, Sanguine Archon (front)** — CLEAN
Theft trigger and transform condition ("if an opponent lost 5 or more life this turn, transform Lar'Otu") match DFC conventions.

**4. Lar'Otu, Lord and Ruler (back)** — CLEAN
Hexproof static is fine. [+2] and [-7] are clean. [-3] ("Exile target instant or sorcery card from a graveyard. It gains Paradigm.") functions: see R7.

**5. Mortach, Titan of the Lifeless** — MINOR (template)
> When Mortach enters the battlefield, create two 2/2 black Zombie creature tokens.
("enters the battlefield" — the shortened form isn't used on real cards.)

**6. The Sanguine Crucible** — CLEAN
"Instant and sorcery spells you cast have Siphon 2" is a legal grant; the granted instance stacks with printed Siphon per the stacking ruling.

**7. Sanguine Membrane** — CLEAN (text fine; interaction needs the R3 ruling, not a text change)
"Players with membrane counters ignore Rootbound" cleanly overrides both Rootbound clauses.

**8. Membranous Infestation** — CLEAN
Note: "each opponent who lost life this turn" deliberately counts life lost from ANY source for counter placement (only the Siphon *discount* is restricted to your sources). Working as designed.

**9. Exsanguinate the Fallen** — CLEAN

**10. Awakening of the First Risen** — CLEAN

**11. Cruor Vat of the Imperator** — CLEAN
The ETB "target opponent chooses one" is legal; the 2-life option is life loss from a source you control, so it banks Siphon. Intended.

**12. Sanguine Exsanguination Seminar** — MINOR (ambiguity)
"You gain life equal to the life lost this way" is ambiguous if different opponents lose different amounts (replacement effects). Corrected:
> Each opponent loses X life, where X is the number of Zombies you control. You gain life equal to the total life lost this way. Create a 2/2 black Zombie token for each opponent who lost life this way.

**13. Covenant of the Lifeless Empire** — FIX NEEDED (name reference)
"If you control both Tiberius and Lar'Otu" doesn't work under real rules: cards are referenced by full name, and Lar'Otu is double-faced (front "Lar'Otu, Sanguine Archon", back "Lar'Otu, Lord and Ruler"). Corrected:
> If you control a permanent named Tiberius, Grave-Legion Imperator and a permanent named Lar'Otu, Sanguine Archon or Lar'Otu, Lord and Ruler, choose both instead.

**14. Legion Sanguimancer** — CLEAN
Siphon on a creature spell functions on the stack. The Blood-sac trigger works with any Blood sacrifice (including the Vat's).

**15. Drain the Defiant** — CLEAN
**16. Tides of Cruor** — CLEAN
**17. Decree of the Lifeless** — CLEAN

### Ironbloom Conservatory

**18. Terrasyl, Voice of the Bloom** — CLEAN
Rootbound as printed matches the final definition. (If the only opponent can't be chosen for Siphon, the spell gets no discount — see R1/FAQ.)

**19. Sylvos, Bloom Egregore** — MINOR (redundant clause)
"Remove all petrification counters from it" is dead text: counters cease to exist when a card changes zones (CR 122.2), so the returned card never has any. Corrected:
> Whenever a creature with a petrification counter on it dies, you may return it to the battlefield under your control. If you do, it becomes a Plant Construct in addition to its other types.
(Keep "If you do" — without it, the type-change would apply to the card in the graveyard when you decline.) The type change has no duration, so it's indefinite while it remains on the battlefield.

**20. Calcifex, Bloom Titan** — CLEAN
**21. Ironbloom Warden** — CLEAN
**22. Petrified Rebuke** — CLEAN ("target spell with Siphon" is checkable on the stack)
**23. Rootbound Tithe** — CLEAN (cost increasers apply before reducers per CR 601.2f — see R5)
**24. The Bloom Remembers** — CLEAN
**25. Ironbloom Sapling** — CLEAN
**26. Ironbloom Deep-Rooter** — CLEAN
**27. Petrify the Leylines** — CLEAN (wording; balance-flagged in §3)
**28. Ironbloom Flakvine** — CLEAN ("{T}, Sacrifice a creature with a petrification counter on it:" is a legal compound cost)
**29. Drag Them Down** — CLEAN (the "loses flying" is near-redundant next to the counter, but harmless and flavorful — the crash)
**30. The Bloom Listens** — CLEAN (Rhystic template, correctly adapted)
**31. Uprising of the Bloom** — CLEAN
**32. The Thousand Roots** — CLEAN
**33. The Bloom Hungers** — CLEAN (wording; SEVERE balance flag in §3)
**34. The Bloom Dreams** — CLEAN
**35. The Bloom Composts** — CLEAN (opponents only — your own Paradigm/Perennial recasts don't trigger it, as worded)
**36. Deep Roots Reclaim** — CLEAN

**Tally:** 30 CLEAN, 5 MINOR, 1 FIX NEEDED (Covenant naming).

---

## 2. RULES ISSUES

**R1. Siphon with no legal choice.** "As you cast this spell, choose an opponent." If every opponent can't be chosen (Rootbound in 1v1), there is no legal choice — you choose no one and get no discount. (Choices with an empty legal set simply aren't made.) This is the intended hose; it must be in the FAQ, not on the card.

**R2. Separate choices per Siphon instance.** A spell with two Siphon instances (printed + granted) makes the "choose an opponent" choice separately for each instance — they may be different opponents, and each instance's discount is computed from its own chosen opponent's life loss.

**R3. Membrane doubling happens before the X cap.** "Counts twice for Siphon" doubles the life-loss *count*, then each Siphon instance caps at its own X. Example: opponent with a membrane counter lost 3 life from your sources → counts as 6 → Siphon 5 reduces {5}, and a stacked Siphon 2 reduces {2} (each instance sees the doubled 6, capped independently). This is the single most confusing interaction in the set — FAQ-mandatory.

**R4. Costs are locked at casting.** Total cost is determined once during casting (CR 601.2f–h). Life lost *after* you've finished casting doesn't retroactively increase the discount.

**R5. Increases before reductions.** Rootbound Tithe's +{2} is applied before Siphon's reduction (CR 601.2f order: base → increases → reductions). E.g. {3}{B} with Siphon 3 vs. Tithe: {3}{B} → {5}{B} → Siphon removes up to {3} → {2}{B} (with enough banked life).

**R6. Tiberius's granted Siphon.** "The next spell you cast this turn has Siphon 3" is a continuous effect consumed the moment you cast a spell (even if countered). It stacks with printed Siphon on that spell. It does nothing if the spell has no generic mana in its cost.

**R7. Lar'Otu's -3 granting Paradigm.** Functions. "You" on the granted ability = Lar'Otu's controller (the controller of the granting effect). Paradigm's "when this spell resolves, exile it" clause is inert (the card is already exiled, never resolves as a spell). Each precombat main phase, the controller may cast a *copy* from exile without paying; the original stays exiled, so it recurs indefinitely. The copy ceasing to exist on resolution doesn't stop the original.

**R8. Sylvos's return.** See card 19: zone change clears counters (the removed clause was redundant). The "Plant Construct in addition" change is indefinite.

**R9. Covenant naming.** See card 13 — FIX NEEDED, corrected text supplied.

**R10. Petrified as a status.** "A permanent with a petrification counter on it can't attack or block, and it doesn't untap during its controller's untap step" works as a rule-level status (like "monstrous") — no layer interactions. Note: nothing stops a petrified land from being tapped *once more* for mana; it simply never untaps afterward.

**R11. Enroot timing.** The trigger watches the tap event; mana is already added before the trigger resolves. The punishment is forward-looking (the land won't untap), which matches the design.

**R12. Choosing is not targeting — but "can't be chosen" is absolute.** Hexproof does nothing against Siphon's choice. Rootbound's "can't be chosen" does. These are different axes; no contradiction.

**R13. Known infinite (acknowledged, not new).** Lar'Otu's emblem ("whenever you gain life, each opponent loses that much life") + Exquisite Blood ("whenever an opponent loses life, you gain that much life") is the classic Exquisite Blood/Sanguine Bond infinite. The set enables it natively via the emblem — same as real Magic has for years. Not a rules problem; noted for honesty in the guide.

---

## 3. BALANCE FLAGS

**SEVERE**
- **The Bloom Hungers + Enroot'd lands.** Enroot permanently counters lands; Hungers drains 1 life per counter on permanents each upkeep with no interaction point (counters are nearly unremovable, the trigger is unstoppable except by enchantment removal). By mid-game this is 5–10 unanswerable life per opponent per turn. **Recommended minimal fix:** "for each petrification counter on *creatures* they control" — keeps the creature-petrification synergy, removes the land-lock drain.

**MODERATE**
- **The Sanguine Crucible + stacking.** Global Siphon 2 turns every Siphon spell's discount up by 2. Safeties hold (generic-only, your-sources-only), but it's the highest-leverage card in the set — watch in playtest.
- **Tiberius's upkeep drain.** Unconditional 1-life bank every turn for all Siphon spells, plus it enables every "opponent lost life" rider (Infestation, Lar'Otu's flip). Slow but free; probably fine, verify in playtest.
- **Lar'Otu emblem + Nekhros.** Attack with 5 Zombies: opponents lose 5, you gain 5, emblem drains 5 more = 10/opponent plus 10 banked. Two-mythic, 9-mana setup — acceptable finisher, but confirm it ends games rather than just winning them.
- **The Thousand Roots.** Draw-to-ten every end step at {7} plus repeatable petrify — strictly better than The Ten Rings ({8}, no upside). The tapped-creature condition is real but thin. Consider {8}.
- **Calcifex, Bloom Titan.** 7/7 trample Enroot that ichors per land tapped. Warps any game it lands in; the social-contract concern from design stands.
- **Sylvos assimilation.** Permanently stealing dead petrified creatures is very strong, but requires the full petrify→kill pipeline. Verify it doesn't make Terrasyl obsolete as the Bloom commander.
- **Wound Reflection / Furnace of Rath + Siphon.** Existing cards double your banked life loss (Reflection's extra loss is from your source). Legal synergy, but it means Siphon's ceiling in eternal formats is ~2x what in-set testing shows.
- **Petrify the Leylines.** 6-mana one-player permanent land lock. Answerable (sorcery, telegraphed), but maximum feel-bad in casual Commander — the exact card that makes tables groan.
- **Membrane double-count + stacking.** 3 life → counts as 6 → Siphon 5 + Siphon 2 = 7 off. Fair as a multi-card payoff; the *rules clarity* (R3) matters more than the power.

**MINOR**
- **The Bloom Listens.** Rhystic Study is famously annoying; the land-tap trigger fires even more often. It's the homage — keep, but expect complaints.
- **Nekhros eminence.** Turn-1 zombie discount + Siphon = fast starts. Standard eminence strength; acceptable for the flagship.

---

## 4. CROSS-CARD CONTRADICTIONS

Checked all interacting pairs. **No hard contradictions found.** Notable verifications:
- **Membrane vs. Rootbound:** the membrane's "ignore Rootbound" explicitly overrides; the double-count then applies cleanly. No conflict.
- **Sylvos vs. Ironbloom Warden:** both trigger on the same death; controller orders them; Warden's ichor is still created even if Sylvos returns the creature. No conflict.
- **Terrasyl's Rootbound vs. membrane counters:** Rootbound doesn't prevent membrane counters (they're not Siphon choices) — intended, since the membrane is the *answer* to Rootbound.
- **The Bloom Composts vs. your own Paradigm/Perennial:** "opponent" excludes your recasts. No conflict.
- **Calcifex vs. petrified lands:** each land triggers the ichor ability exactly once (it never untaps). No conflict.
- **Enroot + The Bloom Listens:** both trigger on the same land tap; no conflict, order as applicable.
- **Nekhros + Lar'Otu emblem:** verified NO infinite loop — the emblem triggers on your *gain*; the opponents' resulting loss causes no further gain. Terminates.
- **Covenant naming (R9)** is the only text-level conflict, fixed in §1.

---

## 5. FAQ (players will ask these)

**Q1. My only opponent controls Terrasyl (Rootbound — can't be chosen for Siphon). I cast a Siphon spell. What happens?**
There's no legal opponent to choose, so you choose no one and get no discount. That's the hose working as intended — bring membrane counters.

**Q2. My spell has Siphon 3 printed and the Crucible grants Siphon 2. Opponent lost 4 life from my sources. Discount?**
Choose an opponent separately for each instance (they may differ). Each instance counts the same 4 life, capped at its own X: 3 + 2 = **5 off** generic mana.

**Q3. Opponent has a membrane counter and lost 3 life from my sources. My spell has Siphon 5. Discount?**
The 3 counts twice = 6, capped at 5 → **{5} off**. The doubling applies before the cap, and every stacked instance sees the doubled number.

**Q4. Does life my opponent lost to someone else's creatures, or their own fetchland, count for my Siphon?**
No. Only life lost **from sources you controlled**.

**Q5. I control Wound Reflection. Opponent lost 3 to my attack; Reflection makes them lose 3 more at end step. Siphon count?**
6 — the extra loss is from a source you control. Note it happens at end step, so it banks for *next* turn's spells.

**Q6. Tiberius gives my next spell Siphon 3 and it already has Siphon 2. Stack?**
Yes — two instances, each capped separately (see Q2).

**Q7. Does hexproof stop Siphon's "choose an opponent"?**
No — choosing isn't targeting. (Rootbound's "can't be chosen" does stop it; that's a different rule.)

**Q8. Sylvos returns my petrified creature. Does it keep the counters? What is it?**
No — counters vanish on zone change. It enters under Sylvos's controller's control as its normal self **plus** the Plant and Construct types, indefinitely (until it leaves the battlefield).

**Q9. My land has a petrification counter. Can I still use it?**
Once. Nothing stops you tapping it for mana one more time — but a petrified permanent **never untaps**, so that was its last activation.

**Q10. Lar'Otu's -3 gives an opponent's graveyard card Paradigm. Who casts the free copies?**
Lar'Otu's controller — "you" refers to the player who controls Lar'Otu. The original stays exiled; you cast a free copy from exile each precombat main phase for the rest of the game (unless the exile pile is disrupted).

---

## Summary for the user
- **30 of 36 cards are clean.** 5 need minor polish (Nekhros, Mortach, Seminar, Sylvos, plus reminder-text recommendation on Tiberius/Crucible). **1 needs a real fix:** Covenant's "Tiberius and Lar'Otu" name reference (corrected text supplied).
- **No rules-breaking designs.** The trickiest correct readings (membrane doubling order, separate Siphon choices, Lar'Otu's granted Paradigm) are documented in §2/§5.
- **One SEVERE balance flag:** The Bloom Hungers counting counters on *lands* (recommended: creatures only). Everything else is MODERATE-or-lower "watch in playtest."
- **No cross-card contradictions.** The Nekhros+emblem pairing was verified loop-free; the known Exquisite Blood infinite is pre-existing Magic, not a new break.
- Set is **wording-airtight pending the 6 small fixes above**. True airtightness still needs what the transcript already concluded: sleeved proxies and real games.

---
pdf_options:
  displayHeaderFooter: true
  headerTemplate: |-
    <div style="font-size: 8px; width: 100%; text-align: center; color: #b91c1c; font-family: 'Cinzel', serif; font-weight: 700; letter-spacing: 1px; padding-bottom: 5px;">
      NANO DUNGEON ENGINE v1.5
    </div>
  footerTemplate: |-
    <div style="font-size: 8px; width: 100%; display: flex; justify-content: space-between; padding: 0 20px; color: #78716c; font-family: 'Cinzel', serif;">
      <span>Nano Dungeon Engine</span>
      <span>Page <span class="pageNumber"></span> of <span class="totalPages"></span></span>
    </div>
  margin:
    top: "20mm"
    bottom: "20mm"
    left: "20mm"
    right: "20mm"
generated_at: "2026-01-16T08:50:46.439Z"
---


<style>
    body > h1:first-of-type, .markdown-body > h1:first-of-type { 
        text-align: center; 
        font-size: 2.5em; 
        border-bottom: 2px solid #b91c1c; 
        padding-bottom: 0.5em;
        margin-bottom: 2em;
    }
</style>

<style>
    h1 { color: #1c1917; }
    
    /* Dice & Tokens */
    .rpg-token {
        display: inline-block;
        padding: 0 0.3em;
        border-radius: 0.25em;
        font-weight: bold;
        font-family: 'Courier New', Courier, monospace;
        white-space: nowrap;
        font-size: 0.9em;
    }
    .token-d4 { background-color: #fef08a; color: #854d0e; border: 1px solid #eab308; }
    .token-d6 { background-color: #e2e8f0; color: #1e293b; border: 1px solid #94a3b8; }
    .token-d8 { background-color: #bfdbfe; color: #1e40af; border: 1px solid #60a5fa; }
    .token-d10 { background-color: #d8b4fe; color: #6b21a8; border: 1px solid #c084fc; }
    .token-d12 { background-color: #fbcfe8; color: #9d174d; border: 1px solid #f472b6; }
    .token-d20 { background-color: #bbf7d0; color: #166534; border: 1px solid #4ade80; }
    .token-tn { background-color: #451a03; color: #ea580c; border: 1px solid #9a3412; }
    .token-luck { background-color: #fef08a; color: #854d0e; border: 1px solid #eab308; }
    .token-power { background-color: #e9d5ff; color: #6b21a8; border: 1px solid #c084fc; }
    .token-heart { background-color: #fecaca; color: #991b1b; border: 1px solid #ef4444; }
    .token-stat { background-color: #451a03; color: #ea580c; border: 1px solid #9a3412; }
    .token-math { background-color: #1e293b; color: #38bdf8; border: 1px solid #0f172a; }
    
    /* Footer Styling */
    .pdf-footer {
        font-family: 'System-ui', sans-serif;
        font-size: 9px;
        color: #78716c;
        width: 100%;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 0 20px;
        border-top: 1px solid #e7e5e4;
        padding-top: 8px;
    }
    .footer-logo { height: 16px; vertical-align: middle; opacity: 0.6; margin-left: 10px; }
    
    /* Density Adjustments */
    h1, h2, h3, h4 { margin-top: 1em; margin-bottom: 0.5em; }
    p, ul, ol, blockquote { margin-bottom: 0.6em; }
    hr { margin: 1.5em 0; border: 0; border-top: 1px solid #e7e5e4; }
</style>
# Monster Book



---



---

### What is this Book for

This book is a set of **tools** for creating opponents and threats in NDE:
- quickly (in 2-5 minutes),
- without calculating stats,
- in a manner consistent with the rules from **Basic Rules** and **MG's Book**.

**The most important assumption of NDE:** *only players roll dice.*
Opponents do not 'attack with a roll' — they attack through **pressure in fiction**: setting obstacles, forcing tests, creating threats and consequences.



---

### 0. Glossary (terms in this book)

**Defense**: the threshold for hitting/bypassing an opponent in battle. The player rolls and compares the result to Defense.,**Difficulty (D)**: the threshold for tests against the environment, phenomenon, special move, or an enemy's 'trick'.,**Hearts**: how much damage a creature can withstand in this scene.,**Minion / Elite / Boss**: three levels of 'importance' of an opponent in the scene.,**Advantage / Disadvantage**: changing the player's dice size by 1 degree (**<span class="rpg-token token-d6">d6</span>→<span class="rpg-token token-d8">d8</span>→<span class="rpg-token token-d12">d12</span>→<span class="rpg-token token-d20">d20</span>** / downward).,**Special Move**: an enemy's active ability that changes the situation (often forces a player attribute check).,**Trait (passive)**: a permanent characteristic of an enemy (armor, flight, resistance, threat zone), which usually gives advantage/disadvantage or changes the stakes.



---

### 1. How the Opponent Works in NDE (in Brief)

In NDE, the opponent is simple but "alive" due to its behavior.

1) **Player acts → player rolls.**  
   - Melee attack: Strength (<span class="rpg-token token-stat">S</span>) vs the target's **Defense**.  
   - Ranged attack: Dexterity (D) vs the target's **Defense**.  
   - Powers: <span class="rpg-token token-power">Power</span> (<span class="rpg-token token-stat">P</span>) vs **Difficulty (D)** or vs Defense (if it's an attack/incapacitation).

2) **If the player misses/fails the check**, the scene continues: a cost or complication arises.  
   In combat, a cost might mean:
   - losing position,
   - losing time,
   - entering the range of a dangerous area,
   - or **losing a Heart**, if it makes sense (e.g., melee combat, crossfire, blast zone).

3) **Opponent "acts" without rolling:**  
   The GM describes what the enemy does, and if it poses a real threat to the heroes, it:
   - forces a check (<span class="rpg-token token-stat">S</span>/D/<span class="rpg-token token-stat">P</span>) against **Difficulty (D)**,
   - or imposes a condition ("until you...", "when you enter...", "who is Close..."),
   - or changes the players' dice (advantage/disadvantage).

4) **Combat is understandable when the enemy has a one-sentence tactic.**  
   Every stat block should include: "what this enemy does in the first round" and "what it does when hit."



---

### 2. Statblock — Format and Fields

The minimal statblock has only what is needed in the scene.

> **Name — Class, Defense, Hearts, Role, Mobility, Abilities, Moves, Tactics**

### 2.1 Mandatory Fields

- **Class:** Minion | Elite | Boss  
- **Defense:** a number that needs to be overcome to hit/bypass the enemy.  
- **Hearts:** how many hits it can withstand (in NDE “hit” = 1 Heart by default).  
- **Role:** the kind of pressure it exerts in battle (see chapter 4).  
- **Mobility:** how it moves (described in zones; grid is optional).  
- **Abilities (passive):** 1–2 brief traits.  
- **Moves (active):** 1 move (Elite) or 2–3 moves (Boss).  
- **Tactics:** 1–3 sentences to help the GM run the enemy consistently.

### 2.2 Optional Fields (Good to Have if They Fit)

- **Range:** if the enemy is ranged (e.g., “Far”, “Very far”).  
- **Zone:** if the enemy creates a hazardous area (smoke, fire, force field).  
- **Weakness:** a clear “lever” for players (water, UV light, signal disruption).  
- **Reward / Clue:** what remains after defeat (loot, trail, information).  
- **Variants:** 1–2 quick swaps (e.g., “instead of flight has jump”; “instead of fire has acid”).

### 2.3 Example Statblock (Universal)

**Guard — Minion, Defense 5, Hearts 1, Brute, Mobility: Near→Close, Abilities: Shield, Moves: Push, Tactics: blocks passage and pushes out of cover.**

- **Shield (passive):** as long as it stands **Close** to cover or a shieldbearer, the attacker has **disadvantage** (dice step down by 1 level).  
- **Push (move):** if the Guard hits in melee (or if the player misses a melee attack against it), the GM may push the hero 1 zone (Close→Near) or 1–2 tiles in grid variant.  
- **Tactics:** engages with the weakest target, guards the corridor, does not flee.



---

### 3. Enemy Classes: Minion, Elite, Boss

In NDE, an opponent's 'difficulty' consists of two things:
- **how hard they are to hit** (Defense),
- **how much they can withstand** (Hearts),
- and **the pressure they exert** (role + moves).

### 3.1 Minion

- **Defense:** typically **5** (easier: 4, harder: 6).
- **Hearts:** **1** (falls after being hit).
- **Moves:** usually 0–1 (simple, predictable).
- **Purpose:** provides pace, context, and a sense of "fighting with a group."
- **How to run:** appears in numbers of 3–8, dies quickly, but makes noise and occupies space.

> A good rule: a minion primarily has *position* (cover, numerical advantage, high ground), not “complex mechanics.”

### 3.2 Elite

- **Defense:** usually **6** (easier elite: 5, "tough elite": 8).
- **Hearts:** **2**.
- **Moves:** 1 distinctive move + 1 passive trait.
- **Purpose:** serves as a "mini-boss" in a scene, forces adaptation.

> The elite should do *one thing distinctly*: "break barriers," "set up zones," "jump off walls," "heal minions."

### 3.3 Boss

- **Defense:** usually **8** (legendary: 12).  
- **Hearts:** **3** (final: 5).  
- **Moves:** 2–3 moves + 1–2 passive traits.  
- **Purpose:** It serves as a scene in itself — it influences the terrain and pace.

**A boss without tricks is boring.** To make a boss "playable," give it at least one of the following: 
- a move that requires a test on multiple heroes, 
- a zone (terrain that needs managing), 
- or a "phase" mechanic (changes behavior after losing 1 Heart).

### 3.4 “Legendary” (Optional Level)

If you need a campaign opponent: - **Defense 12**, **Hearts 5**, 3–4 moves, zones, and phases. This is the “final act boss” — do not use it randomly.



---

### 4. Roles of Adversaries (Clear Pressure)

Roles exist so that the GM immediately knows "how to play it." A role is not a statistic — it's a **style of threat**.

- **Brute (melee pressure):** comes in Close, pushes, topples, breaks the front.  
  *Question to players:* "who stands at the front and what do they risk?"

- **Skirmisher (mobile):** enters, does its thing, and escapes; punishes isolation.  
  *Question:* "who is separated from the team?"

- **Artillery (ranged):** shoots from cover; forces movement and position changes.  
  *Question:* "where is it safe, and where is the firing line?"

- **Controller (control):** zones, smoke, sticky terrain, traps, pressure on objectives.  
  *Question:* "how to avoid the zone instead of struggling within it?"

- **Support (support):** strengthens, heals, moves, provides shields.  
  *Question:* "who to eliminate first to simplify the fight?"

---



---

### 5. Simplifications/Complications in Monsters — GM Principle

In NDE **we do not complicate numbers**. 
Instead of: "+2 to hit, -1 to damage, AC bonus" — we implement:

- **simplification:** raise the player's die by 1 rank,
- **complication:** lower the player's die by 1 rank,
- **change of stakes:** success is possible, but requires a different approach (e.g., remove the cover first).

### 5.1 When to Change Defense and When to Change the Die

- **Most often change the player's die** (easier/harder).
- **Change defense rarely**, mainly when:
  - the enemy has 'armor/invisibility/force field' that *actually* makes them harder to hit,
  - or when it is a boss phase mechanic.

### 5.2 Examples of 'Pure' Disadvantages

- 'The enemy is in partial cover' → the attacker has a **disadvantage**.
- 'The enemy is stunned/bound' → the attacker has an **advantage**.
- 'The enemy is quick and jumping on walls' → the attacker has a **disadvantage** until they block them.



---

### 6. Passive Abilities (Traits) — Catalog for Attachment

Below you have traits that you can attach to a stat block. Choose **1–2** (boss: 2–3). Always describe them within the game world.

### 6.1 Protection and Toughness

- **Light Armor:** the first hit in this scene deals 1 Heart less (i.e., 0) *or* requires "clarification" (the success only deals Heart damage once the armor is bypassed).  
  *The simplest version:* "the first hit does not deal Heart damage".

- **Heavy Armor:** as long as you don't bypass the armor (flank, explosion, hook, magic), attacks have **disadvantage**.  
  *Note:* provide players with a clear path to bypass it.

- **Tough:** after losing 1 Heart, the enemy doesn't change positions (they can't be easily pushed over/knocked down).  
  Ideal for colossi and bosses.

### 6.2 Mobility

- **Quick:** once per round, you can change distance by an additional zone (e.g., Far→Near).
  In grid: +1–2 squares.

- **Jumper / Climber:** treats vertical obstacles as normal.
  Provides sensible 'shortcut entries' to the rear.

- **Flying:** ignores terrain obstacles but requires cover 'from above' or forces reaction tests (e.g., to avoid an airstrike).

### 6.3 Perception and Sneaking

- **Scout:** the first attempt to approach him by surprise has a **disadvantage**.
- **Sentinels:** if someone performs a loud action in the scene, the enemy immediately changes position to a better one (takes cover / calls for support).

### 6.4 Resistances and Weaknesses (Simple)

- **Resistance [type]:** the first time in a scene that an enemy would receive a specific effect (fire, ice, psychic, electricity), the effect is **weaker** (smaller area / shorter duration / no Heart loss).  
- **Weakness [type]:** the player gains an **advantage** against this type of attacks.  

> Transparency principle: resistances and weaknesses only make sense if players can discover and exploit them.

### 6.5 "Swarm" and the Pressure of Numbers

- **Swarm:** if at least two such creatures are Near a hero, the hero has a **disadvantage** on movement/escape tests until they change zones.



---

### 7. Active Moves — How to Write and How to Lead

An active move should answer 3 questions:
1) **What does it do in the fiction?** (description)
2) **Who does it concern and when?** (trigger)
3) **How is it resolved mechanically?** (test / effect / cost)

### 7.1 Simple Move Format

- **Name of the move:** a one-sentence description.
- **Trigger:** when it happens (e.g., "when the hero is Close," "when someone shoots from cover").
- **Test:** which attribute and what Difficulty.
- **Consequence of failure:** what you lose, what changes.
- **Consequence of success:** usually you avoid the consequence or gain an advantage.

### 7.2 How to Determine the Difficulty of an Enemy Move (Without Tables)

If the move is 'attacking' and involves a single target:
- set **T of the move = Enemy Defense** (this is consistent and easy to remember).

If the move is area-targeted or 'large':
- set T one threshold higher than the scene's standard (usually **T 6** or **T 8**).

### 7.3 Example Moves (Modules)

**Brute (Napór)**  
- **Description:** the enemy engages in close combat and pushes.  
- **Trigger:** when the enemy is Close to the hero.  
- **Test:** the hero performs a **<span class="rpg-token token-stat">S</span> or A** test against **T = Enemy's Defense**.  
- **Failure:** the hero loses 1 Heart *or* is pushed 1 zone (GM chooses what makes sense).  
- **Success:** you avoid damage and maintain your position.

**Artillery (Salwa)**  
- **Description:** a series of shots/shards in an area.  
- **Trigger:** when at least 2 heroes are in the same zone and not in cover.  
- **Test:** each target tests **A** against **T 6** (or T = Enemy's Defense if the enemy is elite).  
- **Failure:** −1 Heart and "you must move" (Close→Distant).  
- **Success:** you hide/do not get hit.

**Controller (Kotwica)**  
- **Description:** sticky terrain, force field, web, ice.  
- **Trigger:** the enemy has a moment to set up a zone.  
- **Test:** when you enter the zone, test **A or <span class="rpg-token token-stat">M</span>** against **T 5–6**.  
- **Failure:** you lose movement this turn and are "in a bad position" (disadvantage on attacks).  
- **Success:** you pass through or neutralize the zone.

**Support (Wzmocnienie)**  
- **Description:** the enemy shields an ally/heals/gives an advantage.  
- **Trigger:** once per round when an ally is threatened.  
- **Effect:** a chosen ally receives a "shield" — attackers have **disadvantage** until the end of the round, or the ally regains 1 Heart (boss/elite).  
- **Player Counter:** disable the support or force them to choose (who to save).



---

### 8.1 Default: Distance Zones

In descriptive combat, use: **Close / Nearby / Far / Very Far**.

In the stat block, record mobility as:
- "**Mobility:** changes zone by 1 (standard)"
- or "**Mobility:** Fast (changes zone by 2)"
- or "**Mobility:** Flying (ignores obstacles, but requires tests during air raids)".

### 8.2 Option: Grid (if the table likes tactics)

If you are playing on a map:

- standard movement = **5 squares**,
- Fast = **6–7**, 
- Jump = 3 squares "vertically" or over obstacles.

**All descriptive abilities work the same** — the grid just "provides a measuring tape".



---

### 9. Building an Opponent in 2 Minutes (Procedure)

1) **Choose a class**: Minion / Elite / Boss.  
2) **Set Defense**: 5 / 6 / 8 (legendary: 12).  
3) **Set Hearts**: 1 / 2 / 3 (final: 5).  
4) **Choose a role**: Brute / Skirmisher / Artillery / Controller / Support.  
5) **Add 1–2 passive traits** (boss: 2–3).  
6) **Add moves**: Elite 1, Boss 2–3.  
7) **Write a strategy in 2 sentences** (first round + reaction to threat).  
8) (Optional) Add **weakness** and **reward**.

> Practical test: if you can run the enemy without looking at the table — the statblock is good.



---

### 10. Ready Templates (for Reskinning in Any World)

The following entries are intentionally 'colorless.' You change the name and description — the mechanics remain.

### 10.1 Minions

- **Guard — Minion, Defense 5, Hearts 1, Brute, Mobility: standard, Abilities: Shield, Moves: Press, Tactics: blocks and pushes.**
- **Scout — Minion, Defense 5, Hearts 1, Skirmisher, Mobility: Fast, Abilities: Scout, Moves: Escape, Tactics: approaches, marks targets, and vanishes.**
- **Shooter — Minion, Defense 5, Hearts 1, Artillery, Mobility: standard, Abilities: Cover, Moves: Barrage, Tactics: keeps Distance and forces to run.**
- **Controller — Minion, Defense 5, Hearts 1, Controller, Mobility: standard, Abilities: Zone, Moves: Anchor, Tactics: splits the team.**
- **Support — Minion, Defense 5, Hearts 1, Support, Mobility: standard, Abilities: Medic, Moves: Reinforcement, Tactics: protects the elite.**

**Quick moves for minions:**
- **Escape:** when hit (but not “out” in fiction, e.g. armor), retreats by 1 zone.
- **Barrage:** if someone is in the open, imposes a disadvantage for their next action (“bullets, shrapnel, fear”).
- **Zone:** once per scene places a small hindrance zone (smoke, oil, mud).

### 10.2 Elites

- **Tough Guy — Elite, Defense 6, Hearts 2, Brute, Mobility: standard, Abilities: Light Armor, Moves: Push, Tactics: closes in and holds the line.**
- **Assassin — Elite, Defense 6, Hearts 2, Skirmisher, Mobility: Fast + Jumper, Abilities: Scout, Moves: Flanking Slash, Tactics: strikes from behind and retreats.**
- **Sniper — Elite, Defense 6, Hearts 2, Artillery, Mobility: Far, Abilities: Cover, Moves: Precise Shot, Tactics: forces movement and punishes lack of cover.**
- **Terrain Manipulator — Elite, Defense 6, Hearts 2, Controller, Mobility: standard, Abilities: Zone (2×), Moves: Anchor, Tactics: cuts off escape routes.**
- **Commander — Elite, Defense 6, Hearts 2, Support, Mobility: standard, Abilities: Sensors, Moves: Reinforcement, Tactics: strengthens allies and positions them in cover.**

### 10.3 Bosses

- **Leader — Boss, Defense 8, Hearts 3, Support, Mobility: standard, Abilities: Sentries + Shield, Moves: Reinforce + Summon + Barrier, Tactics: maintains support and controls pace.**
- **Colossus — Boss, Defense 8, Hearts 3, Brute, Mobility: standard, Abilities: Tough + Heavy Armor, Moves: Shock + Assault, Tactics: breaks formation and forces tests.**
- **Hunter — Boss, Defense 8, Hearts 3, Skirmisher, Mobility: Fast + Jumper, Abilities: Scout, Moves: Ambush + Slice + Escape, Tactics: isolates and eliminates.**
- **Zone Architect — Boss, Defense 8, Hearts 3, Controller, Mobility: standard, Abilities: Zone (2×) + Resistance [type], Moves: Anchor + Volley + Shift, Tactics: divides the team and forces decisions.**



---

### 11. Environmental Hazards

Hazard is an 'opponent without a will' or a scene mechanism: turret, fire, avalanche, alarm.

**Format: Name — Difficulty (D), When it activates, Effect, How to disable/bypass**

### 11.1 Examples of Hazards (Universal)

**Turret / Defense Drone — D 6**
- **When it works:** at the end of the round, if someone is in line.
- **Effect:** test **C vs D 6**; failure: −1 Heart and you must take cover.
- **Deactivation:** test **<span class="rpg-token token-stat">M</span> or C vs D 6** at the panel / disruption / <span class="rpg-token token-power">power</span> cut.

**Latch / Mine / Trap — D 5**
- **When it works:** when you enter the zone.
- **Effect:** test **C vs D 5**; failure: −1 Heart or immobilization (lose movement).
- **Deactivation:** tools + test **C vs D 4–5**.

**Gas / Smoke / Contamination — D 5**
- **When it works:** at the beginning of the turn, if you are in the zone.
- **Effect:** test **F or <span class="rpg-token token-stat">M</span> vs D 5**; failure: −1 Heart or a penalty on tests to exit.
- **Deactivation:** ventilation, masks, sealing.

**Alarm / Timer — D (depending on scene)**
- **When it works:** when a complication occurs or someone makes noise.
- **Effect:** time pressure appears (next wave, door closing, reinforcements).
- **Deactivation:** test **<span class="rpg-token token-stat">M</span>** (hack/ritual) or "physically" **F/C** test.



---

### 12. Battle Scene Generator (Quick, Clear)

Choose one from each line (or roll a <span class="rpg-token token-<span class="rpg-token token-d6">d6</span>"><span class="rpg-token token-d6">d6</span></span>):

1) **Objective of the scene:** transition / retrieval / deactivation / escort / theft / defense  
2) **Terrain:** open / bottlenecks / multi-level / lots of cover / edges / fog-smoke  
3) **Opponents:** 6× minion / 4× minion + elite / 2× elite / boss / boss + 2× minion / elite + hazard  
4) **Enemy Advantage:** cover / height / mobility / countdown timer / ambush / long-range support  
5) **Players' Advantage:** surprise / tools / shortcut / neutral ally / terrain provides cover / information (they know who the enemy is)



---

### 13. Balance in Practice (Without Mathematics)

In NDE, balance is achieved through *pace* and *pressure*, not "CR."

### 13.1 Quick Rules for Setting Scene Difficulty

- **Easy Scene:** 4-6 minions or 1 elite.
- **Standard Scene:** 4 minions + 1 elite, or 2 elites.
- **Hard Scene:** boss + 2-4 minions, or boss + hazard.
- **Finale:** boss (5 Hearts) + elite + time pressure.

### 13.2 If the fight is too short

- Add a **wave of minions** (2-3 per round for 2 rounds).
- Increase environmental pressure: smoke zone, alarm, lack of cover.
- Change tactics: the enemy stops fighting "fair" (retreats, takes a hostage, blocks the exit).

### 13.3 If the Battle Drags On

- Give players a 'leverage': an exposed tank, panel, ritual, weakness.
- Allow **benefits for exceptional success**: breaking cover, disarming, dispersing support.
- Reduce the Boss's Hearts from 5 to 3 if this is not the final battle.



---

### 14. Reskin: How to Adapt One Enemy for Every Setting

You have the 'Scout' stat block. Now you just change the description:

- **Fantasy:** goblin archer scout (Scout + Volley).
- **Sci-fi:** reconnaissance drone (Scout + Sensors).
- **Cyberpunk:** gang scout on a skateboard (Quick + Escape).
- **Slavic:** a bies tracking by footprints (Weakness: iron; Immunity: fear).

The mechanics remain the same. This allows the community to add hundreds of entries without breaking the consistency of the core.

